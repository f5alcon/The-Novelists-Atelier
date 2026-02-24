# The Novelist's Atelier

AI-powered writing assistant for editing and world-building. Features multiple AI providers (Claude, GPT, Gemini), flexible context management at Series/Book/Chapter levels, and a privacy-first design with all data stored locally in your browser.

## Features

- **Multiple AI Providers**: OpenRouter, Anthropic Direct (Claude), OpenAI Direct (GPT), Google Direct (Gemini), and LM Studio (local models)
- **Flexible Context**: Add details at Series, Book, or Chapter level to customize AI prompts
- **AI-Powered Editing Tools**:
  - Character creation
  - World-building & locations
  - Copy editing
  - Line editing
  - Developmental editing
  - And more...
- **Pipeline Mode**: Chain multiple prompts together for complex workflows
- **Auto-Save & Backups**:
  - Auto-save every 30 seconds
  - Visual save indicator in header
  - Last saved timestamp
  - Automatic hourly backups (24 per project)
  - Restore from any backup
- **Scene Navigator**: Quick access sidebar to jump to any chapter
- **Organization**: Tags/labels for characters and timeline events
- **Global Search**: Search across all chapters, characters, settings, timelines
- **Find & Replace**: Find Next, Replace, Replace All with regex support
- **Find All**: Find all occurrences across all chapters
- **Export**: Export to JSON or directly to Obsidian (Markdown/ZIP)
- **Style DNA**: Define your unique writing style and apply it to AI generations
- **Smart Context Auto-Toggling**: Automatically optimize context for each prompt
- **Local Text Analysis**: Analyze chapter text for word count, readability, sentiment
- **Token Breakdown**: See exactly how tokens are distributed in your prompts
- **Secure API Key Storage**: Password-encrypted (AES-256), Prompt Each Session, or Session Only options
- **Privacy-Focused**: All data stored locally in your browser

## Getting Started

1. Open `index.html` in your browser
2. Go to **Settings** to configure your API key
3. Add your project details in **Series**, **Book**, and **Chapter** tabs
4. Use **Prompts** to generate content and edit your writing

## API Setup

### Option 1: Cloud APIs (Recommended)

| Provider | Website | Notes |
|----------|---------|-------|
| OpenRouter | [openrouter.ai](https://openrouter.ai) | Multiple models, good pricing |
| Anthropic | [console.anthropic.com](https://console.anthropic.com) | Claude models |
| OpenAI | [platform.openai.com](https://platform.openai.com) | GPT models |
| Google | [aistudio.google.com](https://aistudio.google.com) | Gemini models |

### Option 2: Local Models (LM Studio)

1. Download [LM Studio](https://lmstudio.ai)
2. Load a model
3. Go to Developer tab, enable "Start Server"
4. In Settings, select "LM Studio (Local)" and click Test

## Inclusion Modes

Each section (Series Bible, Book Bible, Chapter Settings, etc.) has inclusion modes:

| Mode | Description |
|------|-------------|
| **Full** | Include all text |
| **Brief** | First ~450 words |
| **Extended** | First ~1000 words |
| **Custom** | Your word count |
| **Off** | Exclude from prompts |

Toggle sections On/Off in the Chapter tab to control what context the AI receives.

## Tips

- The more context you provide (Series → Book → Chapter), the better the AI can assist you
- Use "Brief" for long sections where you want a summary included
- Use Pipeline to chain multiple edits on the same text
- Local models via LM Studio work offline and keep your data private

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| Ctrl/Cmd + F | Open Search |
| Ctrl/Cmd + J | Open Scene Navigator |
| Ctrl/Cmd + S | Force save |
| Ctrl/Cmd + Enter | Run AI prompt |
| F1 | Open Help |

## Version

1.1 Beta

## License

Apache License 2.0 - See LICENSE file for details
