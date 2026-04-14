# Security notes for `index.html`

This project is intentionally kept as a **single-file app**. The security work was implemented directly inside `index.html` without splitting code into external JS files.

## What was applied

### 1. Content Security Policy via meta tag
A CSP was added in `<head>`:

- `object-src 'none'`
- `frame-ancestors 'none'`
- `base-uri 'self'`
- `form-action 'self'`
- restricted `font-src`, `style-src`, `script-src`, `img-src`, `media-src`, `worker-src`, and `connect-src`

Why it helps:
- blocks plugin/object injection
- prevents embedding in hostile frames
- limits where scripts, styles, fonts, media, and network requests can come from

### 2. Referrer policy
Added:

```html
<meta name="referrer" content="no-referrer">
```

Why it helps:
- prevents the page URL from being sent as a referrer to external sites

### 3. Subresource Integrity for the external Mammoth script
The CDNJS Mammoth script now uses:

- `integrity="sha384-..."`
- `crossorigin="anonymous"`
- `referrerpolicy="no-referrer"`

Why it helps:
- ensures the downloaded third-party script matches the expected file
- reduces trust in the CDN alone

### 4. Runtime hardening for external links
A security helper was added that:

- finds all `a[target="_blank"]`
- adds `rel="noopener noreferrer"`
- normalizes/sanitizes `href` values
- blocks unsafe link protocols
- re-applies protection to dynamically inserted links using `MutationObserver`

Why it helps:
- prevents reverse-tabnabbing
- blocks `javascript:`-style link injection in dynamically rendered content

### 5. URL sanitization helper
A `sanitizeUrl()` helper was added.

It allows:
- relative URLs
- `http:`
- `https:`
- `mailto:`
- `tel:`
- `blob:`
- in controlled cases, `data:image/...`

It rejects unsafe schemes.

Why it helps:
- prevents malicious URLs from being inserted into generated links

### 6. Safer dynamic link generation in markdown-rendered output
Markdown link rendering inside the visual-report builders was updated to use safe URL handling before generating `<a>` tags.

Why it helps:
- protects generated report HTML from unsafe link injection

### 7. Safer escaping for dynamic HTML
Several dynamic rendering paths were hardened:

- search result type/title/snippet output is escaped
- find-all result highlighting now escapes snippet and match text before inserting markup
- project names and IDs are escaped before being written into HTML
- tooltip/help text is escaped before insertion
- error display output is escaped before rendering
- relationship modal values are escaped
- timeline modal values and IDs are escaped
- custom prompt template IDs passed into inline handlers are JS-escaped
- backup restore parameters are JS-escaped before insertion into inline handlers

Why it helps:
- reduces DOM XSS risk from imported data, model output, or user-created content

### 8. Safer JS string embedding
A `jsq()` helper was added for values interpolated into inline `onclick="..."` handlers.

Why it helps:
- prevents quote-breaking and script injection via embedded IDs/fields in inline handler strings

### 9. Additional font connection hardening
Added preconnect for:

- `fonts.googleapis.com`
- `fonts.gstatic.com` with `crossorigin`

This is mostly a correctness/performance improvement, but aligns with the CSP restrictions.

---

## Why the CSP still uses `'unsafe-inline'`
Because this app remains a **single HTML file** and still uses:

- inline `<script>` blocks
- inline `<style>` blocks
- inline `onclick="..."` handlers

`script-src 'unsafe-inline'` and `style-src 'unsafe-inline'` are still required to keep the app working as-is.

So the CSP is **meaningfully better than no CSP**, but it is **not as strong** as a nonce/hash-based CSP would be in a multi-file architecture.

---

## Remaining limitations
These are the main things that cannot be fully solved from HTML alone, or would require a much larger refactor:

### Header-based protections still need server/hosting config
These cannot be fully enforced from `index.html` alone:

- `Strict-Transport-Security`
- `X-Content-Type-Options: nosniff`
- `Permissions-Policy`
- `Cross-Origin-Opener-Policy`
- `Cross-Origin-Embedder-Policy`

### Inline handlers still exist
The app still contains many inline `onclick` handlers. They are functional, but they prevent a strict no-inline-script CSP.

### Not every `innerHTML` usage was removed
The app still uses string-based rendering in many places. The high-risk paths were hardened, but the architecture still relies heavily on dynamic HTML assembly.

---

## Best next step if the project stays single-file
If you want to harden it further **without splitting into multiple files**, the next best upgrade would be:

1. replace inline `onclick` handlers with delegated event listeners inside the same file
2. then switch CSP from `'unsafe-inline'` to hash-based or nonce-based script rules

That would keep the project single-file while allowing a much stronger CSP.

---

## Summary
The current `index.html` now includes:

- CSP meta protection
- referrer policy
- SRI for the third-party script
- automatic `noopener noreferrer` enforcement
- URL sanitization
- safer markdown link generation
- additional escaping in several dynamic rendering paths
- safer inline-handler string escaping

This significantly improves security while preserving the single-file design.