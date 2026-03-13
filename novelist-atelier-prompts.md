# The Novelist's Atelier — Prompt Reference Guide

A complete reference for all editorial prompts, organized by type. Each prompt includes the exact text to copy into Claude (or another AI). Replace the bracketed placeholders with your manuscript text.

> **How to use:** Copy the prompt text, paste it into Claude.ai (or your preferred AI), and attach or paste your manuscript text where indicated. Most prompts accept either pasted text or an attached file.

---

## Table of Contents

1. [Manuscript-Level Analysis](#1-manuscript-level-analysis)
2. [Style & Voice](#2-style--voice)
3. [Developmental Editing](#3-developmental-editing)
4. [Copy Editing](#4-copy-editing)
5. [Line Editing](#5-line-editing)
6. [Character](#6-character)
7. [World-Building](#7-world-building)
8. [Location & Setting](#8-location--setting)
9. [Punch & Impact](#9-punch--impact)
10. [Chapter-Level Review](#10-chapter-level-review)
11. [Paragraph-Level](#11-paragraph-level)
12. [Sentence-Level](#12-sentence-level)
13. [Tension & Engagement](#13-tension--engagement)
14. [Prose & Style Audits](#14-prose--style-audits)
15. [Reader Experience](#15-reader-experience)
16. [Genre-Specific](#16-genre-specific)

---

## 1. Manuscript-Level Analysis

These prompts are designed for full manuscripts or large excerpts. Token costs are significant for long documents.

---

### ⚠ Full Manuscript Analysis — Deep Report
**Description:** Complete 22-pass editorial analysis with professional PDF report. WARNING: Very high token cost for long manuscripts.

```
# FULL MANUSCRIPT EDITORIAL ANALYSIS
## "[MANUSCRIPT TITLE]"

---

⚠️ **IMPORTANT — READ BEFORE RUNNING:**

**Claude.ai users:** Attach your manuscript as a .txt, .docx, or .pdf file directly in this chat window, then send this prompt.

**API / Claude Code users:** Upload your manuscript as a .docx or .md file and reference it in your request. Ensure your context window is large enough (use claude-opus-4 or claude-sonnet-4 with extended context).

**⚠ TOKEN COST WARNING:** A full novel (80,000–120,000 words) will consume 300,000–600,000+ tokens per analysis run. This will incur **significant API costs** — potentially $15–$60+ per run depending on your plan and model. Run this on completed or near-complete drafts only. For works-in-progress, use the individual chapter prompts in the Developmental and Chapter Review categories instead.

---

**SYNOPSIS PROVIDED:**
[PASTE YOUR 2-4 SENTENCE SYNOPSIS HERE, OR WRITE: No synopsis provided — infer from manuscript]

**MANUSCRIPT:**
[PASTE MANUSCRIPT HERE, OR WRITE: MANUSCRIPT IS ATTACHED AS FILE — analyze the attached document]

---

# YOUR TASK

You are a team of world-class editors: a developmental editor, line editor, copy editor, sensitivity reader, and literary analyst. Perform a complete 22-pass editorial analysis of this manuscript and produce a **professional, beautifully formatted HTML report** as your final output.

**Produce the full report as a single self-contained HTML document** that the user can save as a PDF (File → Print → Save as PDF in their browser). The HTML must include:

- A professional cover page with title, date, and overall grade
- A full table of contents with anchor links
- All 22 analysis sections with detailed findings
- Visual elements: pacing heatmap table, tension arc chart (SVG), character arc timeline, subplot tracker, word frequency bars, and a final scorecard
- Professional typography using Google Fonts (Playfair Display + Inter)
- A clean two-column layout where appropriate
- Color-coded severity indicators (🔴 Critical / 🟡 Important / 🟢 Minor)
- Page-break CSS for clean PDF output

---

## ANALYSIS PASSES — Complete ALL of the following:

### PASS 1 — PLOT STRUCTURE ANALYSIS
Evaluate the three-act structure: setup, confrontation, resolution. Identify the inciting incident (chapter/page), midpoint shift, all-is-lost moment (75% mark), climax, and resolution. Map hero's journey archetypes present and missing. **Rate structural integrity 1–10.** Cite specific chapter references for every issue.

### PASS 2 — PACING HEATMAP
Create a chapter-by-chapter pacing table: Chapter | Tension (1–10) | Pacing Rating (Too Fast/Fast/Good/Slow/Draggy) | Scene Types | Energy Level. Identify energy valleys, momentum problems, action-to-reflection imbalance. List top 10 pacing fixes ranked by impact.

### PASS 3 — CHARACTER ARC CONSISTENCY
For each major character: map their arc (start → turning points → end), identify growth evidence, flag regression moments, assess arc completion, check motivation consistency. Flag any character who changes too abruptly, doesn't change at all, or acts out of character for plot convenience.

### PASS 4 — THEMATIC COHERENCE
Identify the central theme beneath the plot. Assess how subplots reinforce or contrast the theme. Flag thematic drift. Map each character's journey to the theme. Evaluate the thematic resolution. Flag heavy-handed or preachy moments.

### PASS 5 — WORLD-BUILDING CONTINUITY SCAN
Check: setting contradictions (room layouts, geography, distances), rule violations (magic/tech/social), timeline errors (days/dates/seasons), character knowledge problems (knowing things they shouldn't), missing/disappeared characters, object tracking failures. Organize by severity: Critical / Important / Minor.

### PASS 6 — STAKES ESCALATION
Analyze personal stakes (what the protagonist loses), external stakes (widening consequences), urgency/ticking clock, cost of action increasing, point of no return, stakes at climax being the highest. Flag any moment where stakes plateau, decrease, or feel artificial.

### PASS 7 — SUBPLOT TRACKING
For each subplot: introduction chapter, purpose (serves main plot/theme how?), key beats, resolution quality, dropped threads. Flag redundant subplots, underdeveloped threads, and subplots that damage pacing.

### PASS 8 — DIALOGUE AUTHENTICITY
Rate each major character's voice uniqueness 1–10. Flag info-dumping ("As you know, Bob" moments). Identify best/worst subtext examples. Note unique speech patterns. Assess tag-vs-action-beat ratio. Flag emotionally inauthentic conversations. Suggest rewrites for the 10 worst dialogue passages.

### PASS 9 — SHOW VS. TELL AUDIT
Flag emotional telling, character description telling, backstory dumps, motivation telling, atmosphere telling. For the 10 worst offenders: quote original → write showing rewrite → explain why it's stronger. Note: flag only cases where showing would genuinely improve the experience.

### PASS 10 — SCENE TENSION & CONFLICT CHECK
For each scene: Goal (what does POV character want?) | Obstacle | Stakes | Outcome. Flag scenes where the character has no goal, there's no opposition, nothing changes, or tension is purely internal with no external manifestation. These are cut/strengthen candidates.

### PASS 11 — TRANSITION SMOOTHNESS
Check chapter endings (hook quality) and openings (orientation quality). Assess scene break clarity, POV shift handling, flashback/flash-forward mechanics, and tonal shift intentionality.

### PASS 12 — EMOTIONAL BEAT MAPPING
Chapter by chapter: dominant emotion, emotional high point, emotional low point, emotional variety. Assess: emotional monotone risk, whether big moments are properly set up, whether the emotional climax is the strongest moment, quiet intimate moments between action.

### PASS 13 — SENSORY DETAIL AUDIT
Sense inventory: which of the 5 senses are used/underused? Check for visual-heavy writing. Assess key scenes for sensory grounding. Evaluate setting atmosphere distinctiveness. Check character-filtered POV sensory details. Identify 10–15 scenes needing sensory enrichment with specific suggestions.

### PASS 14 — INFO-DUMP & EXPOSITION DETECTION
Flag: backstory dumps, world-building lectures, As-you-know-Bob dialogue, mirror descriptions, prologue front-loading. For each: quote passage, explain problem, suggest natural integration.

### PASS 15 — COPY EDIT PASS
Grammar errors, punctuation (especially dialogue), spelling, homophone errors, subject-verb agreement, tense consistency, comma splices, run-on sentences. List all errors with location and correction.

### PASS 16 — LINE EDIT PASS
Prose rhythm (sentence length variety, flow, musicality), word choice precision, verb strength (replace weak was/had/got), clarity (confusing sentences, ambiguous references), redundancy. Show 10 before/after improvement examples.

### PASS 17 — OVERUSED WORDS & PHRASES
Overused adverbs/weak verbs/filler words with estimated frequency. Crutch phrases. AI-sounding words (delve, tapestry, testament, visceral, nuanced, multifaceted, resonate, paradigm, myriad, beacon, realm). Repetitive sentence openers. Passive voice frequency (target <10%). Adverb density (target <5 per 1000 words).

### PASS 18 — CRUTCH WORD ELIMINATION
Flag every instance of: just, really, very, quite, actually, basically, literally, suddenly, felt/feeling, started to/began to, seemed/appeared, that (unnecessary), nodded/shrugged/sighed (overused). Provide prioritized cut list with estimated word savings.

### PASS 19 — SENSITIVITY READ
Cultural representation authenticity, stereotypes, language sensitivity (outdated/offensive terms), agency for marginalized characters, historical accuracy, unconscious bias patterns (who are the villains/heroes/victims). Flag for professional sensitivity reader review.

### PASS 20 — BETA READER PANEL (5 Perspectives)
**Reader 1 — The Casual Reader:** Gut reactions, boredom points, enjoyment rating 1–10
**Reader 2 — The Genre Expert:** Genre compliance, trope execution, market positioning, rating 1–10
**Reader 3 — The Harsh Critic:** Plot holes, weak motivations, clichés, the single biggest problem
**Reader 4 — The Target Reader:** Emotional journey, favorite scenes, recommendation, rating 1–10
**Reader 5 — The Superfan:** What made you keep reading? What almost made you stop? Would you pre-order the sequel?

### PASS 21 — PROSE QUALITY SCORING
Rate 1–10 across: Voice Distinctiveness | Sentence Variety | Imagery Quality | Dialogue Naturalism | Description Efficiency | Emotional Resonance | Tension Craft | World Integration

### PASS 22 — FINAL SYNTHESIS & ACTION PLAN
1. **Overall Grade:** A–F with full justification
2. **Top 5 Strengths:** What to keep and amplify
3. **Critical Fixes (10–20 items):** Must-do, ranked by priority, with chapter references
4. **Important Improvements (10–20 items):** Should-do items
5. **Polish Items (5–10 items):** Nice-to-have refinements
6. **Revision Roadmap:** Pass 1 order → Pass 2 order → Pass 3 order of operations
7. **Market Readiness Assessment:** Ready for beta readers / agent submission / self-publishing?
8. **Encouraging Close:** What makes this manuscript worth finishing

---

Output as a professional self-contained HTML report saveable as PDF via browser print. Begin with <!DOCTYPE html>.
```

---

### Manuscript Structure & Plot Report
**Description:** Focused analysis: plot structure, pacing, stakes, and subplots only. Lower cost than the full check.

```
# MANUSCRIPT STRUCTURE & PLOT ANALYSIS
## "[MANUSCRIPT TITLE]"

⚠️ **Usage:** Attach your manuscript as a file in Claude.ai, or upload .docx/.md via API. This is a focused structural pass — for the complete 22-pass analysis, use "Full Manuscript Analysis — Deep Report."

**⚠ TOKEN COST NOTE:** A full novel consumes 100,000–300,000+ tokens. Significant API costs apply for long documents.

**SYNOPSIS:** [PASTE YOUR SYNOPSIS OR WRITE: Infer from manuscript]

**MANUSCRIPT:**
[PASTE MANUSCRIPT HERE OR WRITE: MANUSCRIPT ATTACHED AS FILE]

---

You are a developmental editor with 20+ years of experience. Perform a structural analysis of this manuscript and output a **professional HTML report** (self-contained, saveable as PDF via browser print).

Cover these areas in detail:

**1. THREE-ACT STRUCTURE** — Setup / Confrontation / Resolution proportions and clarity. Structural integrity score 1–10.

**2. KEY STORY BEATS** — Inciting incident (when/strength), midpoint shift (genuine reversal?), all-is-lost moment (real despair?), climax (earned?), resolution (satisfying?). Rate each 1–10 with chapter references.

**3. PACING HEATMAP** — Chapter-by-chapter table: Chapter | Tension 1–10 | Pace Rating | Scene Type | Notes. Identify valleys, rushes, and imbalances. Top 10 pacing fixes.

**4. STAKES ESCALATION** — Personal stakes deepening, external consequences widening, urgency/ticking clock, cost of action, point of no return, climax stakes. Flag plateaus or artificial stakes.

**5. SUBPLOT TRACKER** — Each subplot: intro chapter, purpose, key beats, resolution, dropped threads. Flag redundant or underdeveloped subplots.

**6. HERO'S JOURNEY MAPPING** — Which archetypes are present, which are missing, which are underdeveloped.

Output as a professional self-contained HTML report.
```

---

### Character Arcs & Theme Coherence Report
**Description:** Deep analysis of all character arcs, motivations, and thematic consistency. Moderate token cost.

```
# CHARACTER ARCS & THEME COHERENCE ANALYSIS
## "[MANUSCRIPT TITLE]"

⚠️ **Usage:** Attach manuscript as a file in Claude.ai, or upload .docx/.md via API. Token costs apply for long manuscripts.

**MAIN CHARACTERS PROVIDED:**
[LIST YOUR MAIN CHARACTERS WITH ONE-LINE DESCRIPTIONS, OR WRITE: Identify from manuscript]

**MANUSCRIPT:**
[PASTE MANUSCRIPT HERE OR WRITE: MANUSCRIPT ATTACHED AS FILE]

---

You are a developmental editor specializing in character psychology and thematic analysis. Produce a **professional HTML report** (saveable as PDF) covering:

**1. CHARACTER ARC MAPPING** — For each major character: arc start → turning points → arc end | evidence of change in specific scenes | regression moments | arc completion | motivation consistency. Flag abrupt changes, flat arcs, or plot-convenience behavior.

**2. CHARACTER ARC TIMELINE** — Visual HTML/SVG horizontal timeline showing each character's arc trajectory across the manuscript chapters.

**3. RELATIONSHIP DYNAMICS** — How key relationships evolve, whether they serve the theme, and whether relationship arcs have satisfying resolutions.

**4. THEMATIC IDENTIFICATION** — What is this book really about beneath the plot? Identify primary and secondary themes.

**5. THEME IN SUBPLOTS** — Does each subplot reinforce or contrast the central theme?

**6. THEMATIC DRIFT MAP** — Sections where the theme is lost or diluted. Chapters where it shines strongest.

**7. THEME IN CHARACTER ARCS** — How each character's journey explores or challenges the theme.

**8. THEMATIC RESOLUTION** — Does the ending make a clear statement? Is it earned? Heavy-handed moments?

**9. EMOTIONAL BEAT MAP** — Chapter-by-chapter: dominant emotion | emotional high | emotional low | variety rating. Emotional monotone assessment.

Output as a professional self-contained HTML report.
```

---

### Line Edit & Copy Edit Report
**Description:** Prose quality, crutch words, show vs tell, dialogue, and copy errors. Best run on a single chapter or excerpt.

```
# LINE EDIT & COPY EDIT ANALYSIS
## "[MANUSCRIPT / CHAPTER]"

⚠️ **Usage note:** This prompt works best on excerpts of 5,000–20,000 words for detailed line-level feedback. For full novels, token costs will be very high and output may be truncated. Consider running chapter by chapter.

**TEXT TO ANALYZE:**
[PASTE YOUR TEXT HERE OR WRITE: ATTACH TEXT AS FILE]

---

You are a senior line editor and copy editor. Produce a **professional HTML report** (saveable as PDF) with these sections:

**1. PROSE QUALITY SCORECARD** — Rate 1–10: Voice Distinctiveness | Sentence Variety | Imagery Quality | Dialogue Naturalism | Description Efficiency | Emotional Resonance | Verb Strength | Clarity. Visualize as a colored bar chart.

**2. SHOW VS. TELL AUDIT** — Flag emotional telling, description telling, backstory dumps, motivation telling, atmosphere telling. For 10 worst offenders: quote original → showing rewrite → explanation of improvement.

**3. DIALOGUE AUTHENTICITY** — Rate each major character's voice uniqueness 1–10. Flag info-dumps in dialogue. Best/worst subtext examples. Tag vs action beat balance. 10 dialogue rewrites for worst passages.

**4. OVERUSED WORDS FREQUENCY** — Top overused adverbs, weak verbs, filler words with estimated frequency. AI-sounding words detected (delve, tapestry, testament, visceral, nuanced, multifaceted, resonate, paradigm, myriad, beacon, realm). Visualize as horizontal bar chart.

**5. CRUTCH WORD HIT LIST** — Every instance of: just, really, very, quite, actually, basically, literally, suddenly, felt/feeling, started to, began to, seemed, appeared, that (unnecessary), nodded, shrugged, sighed. Prioritized cut list with estimated word savings.

**6. LINE EDIT IMPROVEMENTS** — 10 before/after examples showing: prose rhythm improvement | word choice precision | weak-to-vivid verb replacement | clarity fix | redundancy removal.

**7. COPY EDIT ERRORS** — Grammar, punctuation (especially dialogue tags), spelling, homophones, subject-verb agreement, tense consistency, comma splices, run-ons. Full error list with corrections.

**8. PASSIVE VOICE & ADVERB DENSITY** — Percentage estimates with benchmark targets (<10% passive, <5 adverbs/1000 words).

Output as a professional self-contained HTML report.
```

---

## 2. Style & Voice

---

### Capture My Writing DNA
**Description:** Deep analysis of your unique voice and style fingerprint.

```
You are a literary analyst specializing in author voice. Analyze the following writing sample and produce a comprehensive "Style DNA" document.

Cover:
- Sentence structure patterns (average length, variation, rhythm)
- Vocabulary tier and register (literary, colloquial, technical mix)
- Dialogue style (how characters speak, tags, beats)
- POV handling and narrative distance
- Pacing signature (scene vs. summary ratio)
- Emotional tone and how you convey interiority
- Recurring stylistic tics (good and ones to watch)
- 3–5 "rules" that seem to govern the prose instinctively

End with a one-paragraph "author voice statement" to use as a north star.

WRITING SAMPLE:
---
[PASTE 3-5 PAGES OF YOUR BEST WRITING HERE]
---
```

---

### Consistency Check Against My Style
**Description:** Flag passages that drift from your established voice.

```
You are a line editor protecting an author's voice. Using the Style DNA below, analyze the new text and flag any passages that drift from the established voice.

For each flag:
- Quote the offending phrase/sentence
- Explain what rule or pattern it breaks
- Suggest a corrected version in the author's voice

STYLE DNA:
---
[PASTE YOUR STYLE DNA DOCUMENT HERE]
---
NEW TEXT:
---
[PASTE NEW TEXT TO CHECK HERE]
---
```

---

## 3. Developmental Editing

---

### Chapter Structure Audit
**Description:** Big-picture analysis of a chapter's structural integrity.

```
You are a developmental editor. Read this chapter and provide a structural audit.

Analyze:
1. **Scene Goals** — Does every scene have a clear goal, conflict, and outcome?
2. **Pacing** — Where does momentum stall? Where does it rush?
3. **Stakes** — Are the stakes clear and felt? Do they escalate?
4. **Character Agency** — Are characters driving the plot or being dragged?
5. **Promise & Payoff** — What does this chapter promise? Does it deliver?
6. **Structural Issues** — Plot holes, logic gaps, continuity problems?
7. **Chapter Arc** — Does the chapter have its own satisfying micro-arc?

End with: Top 3 Priority Fixes ranked by impact.

STORY CONTEXT: [BRIEFLY DESCRIBE WHERE WE ARE IN THE NOVEL]
CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Pacing Analysis
**Description:** Scene-by-scene pacing map with recommendations.

```
You are a developmental editor specializing in narrative pacing. Create a pacing map of this text.

For each distinct scene or section:
- Label it (Scene 1, Scene 2, etc.)
- Assign a pace rating: Crawl / Walk / Jog / Run / Sprint
- One sentence on what drives or kills momentum here
- Flag any pace whiplash (jarring transitions between speeds)

Then provide:
- Overall pacing assessment
- The 2–3 most critical pacing interventions
- Specific suggestions for slow sections
- Specific suggestions for rushed sections

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Story Arc
**Description:** Analyze story arc structure and proportions.

```
You are a developmental editor. Analyze the following manuscript excerpt and evaluate the story arc.

Specifically assess:
- Whether the setup, rising action, climax, falling action, and resolution are clearly defined and proportionate
- Whether the protagonist's transformation (internal arc) mirrors or meaningfully contrasts with the external plot arc
- Any structural imbalances — sections that drag, rush, or feel tonally disconnected

Return your feedback as:
1. A one-paragraph overall assessment
2. A bulleted list of specific structural issues with line or chapter references where possible
3. One concrete revision suggestion for the most critical issue

STORY CONTEXT: [CONTEXT]
CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Stakes Escalation
**Description:** Analyze how stakes escalate throughout the narrative.

```
You are a developmental editor specializing in pacing and tension. Analyze the following manuscript excerpt for how effectively the stakes escalate throughout the narrative.

Specifically assess:
- Whether each act raises the cost of failure for the protagonist (personally, professionally, relationally, or existentially)
- Whether the reader is made to feel the weight of those stakes through scene construction — not just told about them
- Any moments where stakes deflate prematurely or plateau for too long

Return your feedback as:
1. A stakes "heat map" summary — identify where tension peaks, plateaus, and dips
2. A bulleted list of specific moments where escalation succeeds or fails
3. One concrete revision suggestion for the weakest escalation point

STORY CONTEXT: [CONTEXT]
CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Subplot Resolution
**Description:** Evaluate how subplots are introduced and resolved.

```
You are a developmental editor. Analyze the following manuscript excerpt and evaluate how subplots are introduced and resolved.

Specifically assess:
- Whether each subplot introduced is meaningfully resolved or intentionally left open (and whether the intent reads clearly)
- Whether subplots connect thematically or causally to the main plot, or feel like detours
- Whether the timing of subplot resolutions disrupts or enhances the main narrative's momentum

Return your feedback as:
1. A list of all identified subplots with a status (resolved / unresolved / abandoned)
2. A bulleted list of subplots that need attention, with specific reasoning
3. One concrete revision suggestion for the most problematic subplot

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Plot Holes & Contradictions
**Description:** Find plot holes, logical inconsistencies, and internal contradictions.

```
You are a continuity editor and story analyst. Analyze the following manuscript excerpt for plot holes, logical inconsistencies, and internal contradictions.

Specifically look for:
- Events that could not logically occur given prior established facts
- Character knowledge that appears or disappears without explanation
- Timeline inconsistencies, geography errors, or world-rule violations
- Chekhov's Guns that are introduced but never fired (or fired without introduction)

Return your feedback as:
1. A numbered list of identified issues ranked by severity (critical / moderate / minor)
2. For each issue: what the contradiction is, where it occurs, and why it breaks internal logic
3. A brief note on any issues that may be intentional (unreliable narrator, mystery setup, etc.) that should be verified with the author

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Character Motivations
**Description:** Evaluate whether character motivations are clear, believable, and consistent.

```
You are a developmental editor specializing in character psychology. Analyze the following manuscript excerpt and evaluate whether character motivations are clear, believable, and consistent.

Specifically assess:
- Whether each major character's want (external goal) and need (internal wound or truth) are discernible
- Whether character decisions feel motivated by who they are — or merely by what the plot requires
- Any moments where a character acts in a way that contradicts their established psychology without sufficient justification

Return your feedback as:
1. A character-by-character breakdown of want vs. need as you understand them from the text
2. A bulleted list of moments where motivation feels unclear, forced, or contradictory
3. One concrete revision suggestion for the character whose motivations are least convincing

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Thematic Cohesion
**Description:** Analyze how effectively central themes are woven through the narrative.

```
You are a literary editor. Analyze the following manuscript excerpt and evaluate how effectively the central theme(s) are woven through the narrative.

Specifically assess:
- Whether the theme is embodied in action, image, and subtext — rather than stated outright through dialogue or narration
- Whether supporting characters, subplots, and settings serve as thematic mirrors or counterpoints to the protagonist's arc
- Any sections where the theme feels absent, heavy-handed, or contradicted without purpose

Return your feedback as:
1. A statement of what you believe the central theme(s) to be, based solely on the text
2. A bulleted list of the strongest and weakest moments of thematic integration
3. One concrete revision suggestion to deepen thematic resonance in the weakest area

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Scene Purpose
**Description:** Evaluate whether each scene earns its place in the story.

```
You are a story editor evaluating narrative efficiency. Analyze each scene in the following manuscript excerpt and assess whether it earns its place in the story.

For each scene, determine whether it accomplishes at least two of the following:
- Advances the plot (something changes as a result of this scene)
- Reveals character (we learn something new and meaningful about who someone is)
- Raises the stakes (the cost of failure increases or a new threat emerges)
- Establishes theme (a thematic idea is dramatized, not just stated)

Return your feedback as:
1. A scene-by-scene table: Scene | Primary Function | Secondary Function | Verdict (Keep / Cut / Merge / Rewrite)
2. A brief explanation for any scene marked Cut, Merge, or Rewrite
3. One concrete revision suggestion for the scene doing the least narrative work

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Scene Openings
**Description:** Analyze the opening lines of each scene.

```
You are a line editor and story analyst focused on reader engagement. Analyze the opening lines of each scene in the following manuscript excerpt.

Specifically assess whether each scene opening:
- Drops the reader into action, tension, or a compelling sensory moment (rather than orientation or weather)
- Establishes whose scene it is and what they want within the first few lines
- Creates an implicit question that pulls the reader forward

Return your feedback as:
1. A list of each scene opening with a one-line verdict (Strong / Weak / Needs Work) and a brief reason
2. Rewrite suggestions for the two weakest scene openings, preserving the author's voice
3. A pattern note — if the author has a recurring scene-opening weakness, name it specifically

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Scene Endings & Momentum
**Description:** Analyze the ending lines of each scene.

```
You are a story editor specializing in pacing and reader compulsion. Analyze the ending lines of each scene in the following manuscript excerpt.

Specifically assess whether each scene ending:
- Closes one question while opening another (the "yes, but / no, and" principle)
- Ends on a moment of change, revelation, decision, or unresolved tension — rather than a tidy wrap-up
- Creates forward momentum that makes stopping feel difficult

Return your feedback as:
1. A list of each scene ending with a one-line verdict (Propulsive / Flat / Closed Too Neatly) and a brief reason
2. Rewrite suggestions for the two flattest scene endings, preserving the author's voice
3. A pattern note — if the author tends toward a particular type of weak ending, name and explain it

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### POV Consistency
**Description:** Analyze POV consistency within each scene.

```
You are a line editor. Analyze the following manuscript excerpt for POV consistency within each scene.

Specifically look for:
- Head-hopping (shifting between character consciousnesses within a single scene without a clear break)
- POV intrusions — moments where information, observations, or language couldn't plausibly belong to the POV character
- Distance inconsistency — unearned shifts from deep interiority to remote, cinematic narration within the same scene

Return your feedback as:
1. The identified POV mode (First Person / Third Limited / Third Omniscient / Second / Mixed) and whether it's applied consistently
2. A numbered list of specific POV violations with line references and explanation of the problem
3. One concrete revision suggestion for the most disorienting POV break

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Scene-Level Conflict
**Description:** Analyze each scene for the presence and quality of conflict.

```
You are a story editor evaluating dramatic tension. Analyze each scene in the following manuscript excerpt for the presence and quality of conflict.

Conflict can be:
- Interpersonal (character vs. character)
- Internal (character vs. self)
- Environmental (character vs. world, nature, system)
- Philosophical (character vs. idea or belief)

Specifically assess:
- Whether every scene contains at least one active form of conflict
- Whether the conflict in each scene connects to the scene's core dramatic question
- Any scenes that feel static — where characters talk, move, or exist without meaningful opposition

Return your feedback as:
1. A scene-by-scene conflict audit: Scene | Conflict Type | Strength (Strong / Present / Weak / Absent)
2. A bulleted list of scenes where conflict is weak or absent, with explanation
3. One concrete revision suggestion for the most conflict-deficient scene

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Time & Causality Check
**Description:** Check timeline logic and cause/effect relationships.

```
You are a continuity editor. Analyze this chapter for timeline consistency and causality. Ensure actions have logical reactions and time passes believably.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Scene vs. Summary Balance
**Description:** Assess the ratio of real-time scene to summary.

```
You are a developmental editor. Audit this text for the balance of scene (real-time action) versus summary (telling). Flag areas where summary should be expanded to scene.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Information & Revelation Pacing
**Description:** Analyze how information is revealed to the reader.

```
You are a thriller editor. Analyze how clues and information are paced. Is it too front-loaded? Too confusing?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Setup & Payoff Tracker (Chekhov's Gun)
**Description:** Audit elements introduced and evaluate if they pay off.

```
List every implicit "promise", object, or element introduced. Evaluate whether it was paid off, left dangling, or needs resolution later.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Action & Spatial Choreography Check
**Description:** Map physical position and movements.

```
Map the physical position and movements of characters/objects. Flag any "teleportation" or confusing physical mechanics.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Chapter Purpose/Theme Identification
**Description:** Analyze core narrative purpose and thematic function within the larger story.

```
Analyze this chapter and identify its core narrative purpose and thematic function within the larger story. Determine what this chapter is designed to accomplish — whether it advances plot, deepens character, establishes atmosphere, raises stakes, or shifts tone. Identify any central themes present (e.g., betrayal, identity, sacrifice) and explain how the chapter embodies or develops them. Note whether the thematic intent is clearly executed or muddled by competing elements. Flag any moments where the chapter loses focus or drifts from its primary purpose. Provide a concise statement of what this chapter should make the reader feel, know, or question by its final line.

STORY CONTEXT: [CONTEXT]
CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Key Events Summary
**Description:** Identify and summarize key events in order.

```
Identify and summarize the key events in this chapter in the order they occur. Focus only on events that carry narrative weight — those that change circumstances, shift relationships, reveal information, or create consequences. Distinguish between plot events (external action) and emotional/internal events (decisions, realizations, shifts in feeling). Flag any events that are underdeveloped, rushed, or given disproportionate page time relative to their importance. Note whether each key event connects logically and causally to what precedes and follows it. Identify any events that feel extraneous or could be cut without damaging the chapter's purpose.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Character Growth Analysis
**Description:** Analyze character development and arc changes.

```
Analyze the character development that occurs in this chapter for each named character with a significant presence. For each character, identify where they begin emotionally, psychologically, or motivationally at the chapter's opening and where they end. Determine whether meaningful growth, regression, or revelation has occurred and whether it feels earned by the events on the page. Flag any character whose arc feels stagnant, contradictory, or inconsistent with their established traits. Note moments where a character's change feels forced, unearned, or conveniently timed. Identify missed opportunities where growth could have been more clearly dramatized or deepened.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Backstory Revealed
**Description:** Identify and evaluate backstory delivery.

```
Identify all backstory introduced in this chapter — information about characters, world, history, or events that occurred before the chapter's present timeline. For each instance of backstory, evaluate whether it is delivered at the right moment (i.e., when the reader most needs or wants it), whether it is proportionate in length to its narrative importance, and whether it is integrated naturally into the scene or delivered artificially (e.g., forced flashbacks, unprompted explanation). Flag any backstory that halts narrative momentum, over-explains, or could be cut without consequence. Note any backstory the chapter withholds that the reader urgently needs for clarity or emotional investment.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Character Interactions
**Description:** Analyze exchanges between characters.

```
Analyze every significant interaction between characters in this chapter. For each exchange — dialogue or physical — evaluate whether the interaction feels authentic to both characters' established voices and motivations. Determine what each character wants from the other in the scene and whether that tension is present and active on the page. Flag dialogue that feels expository, on-the-nose, or out of character. Identify subtext: note where what characters say diverges from what they mean or want, and evaluate whether that subtext is effectively written. Highlight any interactions that feel unresolved, underwritten, or that miss an opportunity to deepen relationship dynamics.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Exposition Delivery
**Description:** Evaluate expository passages and delivery methods.

```
Identify all expository passages in this chapter — sections where the narrative pauses to deliver information about setting, world-building, character history, or context. For each, evaluate the delivery method (narration, dialogue, internal thought, environmental detail) and determine whether the method suits the scene's tone and pacing. Flag exposition that is front-loaded, excessive, repetitive, or delivered through unnatural dialogue ("as you know" constructions). Assess whether the reader is given enough information to remain oriented without being over-explained. Suggest where exposition could be compressed, cut, or redistributed into action and scene rather than summary.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Information Clarity
**Description:** Evaluate clarity of information delivery.

```
Evaluate the clarity of information delivery throughout this chapter from the perspective of a reader experiencing it for the first time. Identify any passages where it is unclear who is speaking, who is in the scene, where the scene is taking place, or what is happening and why. Flag pronoun ambiguity, unclear scene transitions, confusing timelines, or moments where the narrative assumes knowledge the reader does not yet have. Note where information is repeated unnecessarily. Assess whether key plot points, character motivations, and cause-and-effect relationships are legible without being over-explained. Provide specific line-level examples where clarity breaks down.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Information Relevance
**Description:** Assess relevance of information to story needs.

```
Evaluate every piece of information delivered in this chapter — plot details, character facts, world-building, backstory, and context — and assess its relevance to the story's present needs. For each significant block of information, determine whether it serves an immediate narrative purpose (advancing plot, deepening character, creating tension) or whether it is included out of the author's attachment rather than the reader's need. Flag information that is redundant, premature, or so tangential that it dilutes focus. Identify any details that are introduced but never paid off, and any critical information the chapter fails to deliver when the narrative demands it. Distinguish between information that enriches and information that merely fills space.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### New Character Introduction
**Description:** Evaluate effectiveness of new character introductions.

```
Identify every new character introduced in this chapter and evaluate the effectiveness of each introduction. For each character, assess whether the reader is given enough immediate information to distinguish them — voice, physical presence, attitude, role — without being overwhelmed by detail. Determine whether the character's introduction is motivated by the scene (they appear because the story requires them) or feels forced or convenient. Evaluate whether the character makes a distinct impression on first appearance and whether their purpose in the narrative is at least partially legible. Flag introductions that are too sparse to be memorable, too dense to be digestible, or that drop a character into the scene without sufficient grounding. Note whether any new character risks being confused with an existing one.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Setting & World-Building
**Description:** Analyze setting and world-building passages.

```
Analyze how setting and world-building are handled in this chapter. Identify every passage where the physical environment, time period, social context, or world rules are established or developed. Evaluate whether setting is rendered through specific, sensory detail or delivered as vague generality. Assess whether the world-building is integrated into the action and character experience or front-loaded as passive description. Determine whether the setting actively influences the scene — affecting character behavior, mood, and conflict — or functions as inert backdrop. Flag any world-building that halts pacing, over-explains rules or history, or assumes the reader shares context the text has not yet established. Note any setting details that feel inconsistent with what has been previously established in the story.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Tropes Identification
**Description:** Identify recognizable narrative tropes.

```
Identify all recognizable narrative tropes present in this chapter — character archetypes, plot devices, relationship dynamics, dialogue patterns, and situational conventions drawn from genre tradition or broader storytelling culture. For each trope identified, name it clearly, cite the specific passage or element where it appears, and assess how consciously it appears to be employed. Distinguish between tropes that are used with intention and craft versus those that appear to have slipped in as defaults. Evaluate whether each trope serves the story's specific needs or whether it substitutes for original character, plot, or emotional work. Note any tropes that risk undermining reader trust or creating predictability that works against narrative tension.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Trope Subversion
**Description:** Analyze deliberate trope inversions and subversions.

```
Analyze this chapter for instances where familiar tropes, conventions, or reader expectations are deliberately subverted, inverted, or complicated. For each subversion identified, evaluate whether it is executed with sufficient clarity — that is, whether the reader can recognize the expectation being undermined in order to feel the impact of its departure. Assess whether the subversion serves a meaningful narrative or thematic purpose or whether it functions only as a surface-level surprise. Flag subversions that are undermined by inconsistent execution, that rely on the reader having knowledge the text hasn't established, or that inadvertently introduce new clichés in place of the ones being avoided. Identify any moments where a trope could have been subverted more effectively but was instead played straight without apparent intention.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

## 4. Copy Editing

---

### Full Copy Edit Pass
**Description:** Grammar, consistency, fact-checking, and correctness.

```
You are a meticulous copy editor. Perform a full copy edit pass.

Flag and correct:
1. Grammar & Syntax — errors, unintentional fragments, run-ons
2. Punctuation — commas, em-dashes, ellipses, dialogue punctuation
3. Spelling — typos, homophones, name consistency
4. Continuity — character names, physical descriptions, timeline logic
5. Word Repetition — same word used too close together
6. Tense Consistency — any unintended tense shifts
7. POV Consistency — head-hopping or POV violations

Format: numbered list. For each: Quote original → corrected version → one-line explanation.
Preserve intentional style choices (fragments for effect, unconventional punctuation for voice).

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Dialogue Mechanics Check
**Description:** Audit all dialogue tags, beats, and punctuation.

```
You are a copy editor specializing in dialogue. Audit all dialogue in this text.

Check for:
- Incorrect dialogue punctuation (comma vs. period before/after tags)
- Overuse of "said" replacements — flag where "said" would be stronger
- Missing or unnecessary dialogue tags
- Action beats that could replace tags for better effect
- Characters speaking in ways inconsistent with their established voice
- Dialogue that sounds unnatural or on-the-nose

Present as: original → corrected format.

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Dialogue Tag & Action Beat Balance
**Description:** Analyze the rhythm of dialogue tags and action beats.

```
Strip out the dialogue and only look at tags and beats. Does the rhythm feel natural? Are there too many consecutive tags or cliché beats?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

## 5. Line Editing

---

### Line Edit for Clarity & Flow
**Description:** Sharpen prose without changing the author's voice.

```
You are a line editor. Cardinal rule: never sacrifice the author's voice for clarity.

Target:
- Sentences that are tangled or require re-reading
- Abrupt or muddy transitions
- Passive constructions that drain energy (flag — don't blindly fix)
- Vague, abstract language where concrete detail would land harder
- Filler phrases: "it was," "there were," "began to"
- Overwritten moments that undercut their own emotional impact

Present as: Original → Suggested Revision + one-line note on why. Always note if original is a valid style choice.

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Show vs. Tell Audit
**Description:** Find telling that should be showing, and vice versa.

```
You are a line editor. Audit this text for show vs. tell balance.

TELLING TO FLAG (needs showing): Abstract emotional statements, character trait announcements, summarized reactions that could be dramatized.

SHOWING TO FLAG (could be told): Scenes over-dramatized when a quick summary would serve better. Not all telling is bad — flag only where it actively weakens impact.

For each flag: Quote → label (NEEDS SHOWING or OVER-SHOWN) → rewritten example.

End with: The ratio feels [too much telling / balanced / too much showing] because ___

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Sensory Depth Pass
**Description:** Identify where sensory detail is missing or underdeveloped.

```
You are a line editor. Do a sensory depth pass on this text.

Map which senses are active in each scene: sight, sound, smell, touch, taste, proprioception, temperature.

For each scene or section:
- List which senses are present
- Flag which are absent or underused where they'd deepen immersion
- Identify passages that feel visually over-loaded
- Suggest 2–3 specific sensory additions (concrete, not generic) that would most elevate the scene

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Sentence Variety & Rhythm
**Description:** Analyze sentence variety and rhythmic quality.

```
You are a prose stylist and line editor. Analyze the following manuscript excerpt for sentence variety and rhythmic quality.

Specifically assess:
- Whether the author varies sentence length meaningfully — using short sentences for impact and longer sentences for momentum, immersion, or complexity
- Whether syntactic patterns repeat in ways that create monotony (e.g., subject-verb-object dominance, constant participial openers)
- Whether the prose rhythm matches the emotional register of the scene (terse in action, expansive in reflection, staccato in panic)

Return your feedback as:
1. A prose rhythm profile — describe the author's dominant patterns in plain language
2. Two or three representative passages that illustrate both strengths and weaknesses
3. Specific revision suggestions for the most rhythmically flat or monotonous passage, with a rewritten example

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Word Choice Precision
**Description:** Analyze precision and intentionality of word choice.

```
You are a line editor with a focus on diction and specificity. Analyze the following manuscript excerpt for the precision and intentionality of word choice.

Specifically look for:
- Vague, generic, or overused words that could be replaced with more precise, evocative alternatives (e.g., "walked" vs. "shuffled," "nice" vs. a specific quality)
- Adverb and adjective overuse that signals weak verb/noun choices
- Tonal inconsistencies where word choice doesn't match the scene's emotional register or the POV character's voice
- Clichés, dead metaphors, or mixed metaphors

Return your feedback as:
1. A list of the ten most problematic word choices or phrases, each with a suggested alternative and a brief reason
2. A note on whether the author's diction is generally precise, imprecise, or inconsistent — and what drives the pattern
3. One passage rewritten with improved word choice precision as a model for revision

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Dialogue Naturalism
**Description:** Analyze dialogue for naturalism, distinctiveness, and dramatic function.

```
You are a dialogue editor and script consultant. Analyze the dialogue in the following manuscript excerpt for naturalism, distinctiveness, and dramatic function.

Specifically assess:
- Whether each character has a distinct voice — vocabulary, rhythm, deflection patterns, and verbal habits that belong only to them
- Whether dialogue sounds like how people actually speak (with interruption, subtext, indirection, and evasion) rather than how they conveniently explain things
- Whether dialogue is doing double or triple duty (revealing character AND advancing plot AND suggesting subtext) or merely conveying information
- Overuse of dialogue tags beyond "said," on-the-nose exposition delivered through speech, or characters who speak in complete grammatical paragraphs

Return your feedback as:
1. A character-by-character voice assessment — is each speaker distinguishable without dialogue tags?
2. A bulleted list of specific dialogue exchanges that are too on-the-nose, expository, or unnatural, with brief notes
3. One dialogue passage rewritten to demonstrate stronger subtext and voice distinction

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### AI Detection Check
**Description:** Analyze text for AI-generated patterns.

```
[PASTE YOUR CHAPTER TEXT HERE]

---

## ANALYSIS FRAMEWORK

Evaluate the chapter across these six dimensions and score each 1–10 (10 = strongly AI-generated):

---

### 1. LINGUISTIC FINGERPRINTS
Flag any of the following AI-characteristic phrases and constructions:

**Transition overuse:**
- "It's worth noting that…" / "It is important to note…"
- "Furthermore," / "Moreover," / "Additionally," / "In addition,"
- "It goes without saying…" / "Needless to say…"
- "As previously mentioned…" / "As noted above…"
- "In conclusion," / "To summarize," / "In summary,"
- "This is not to say…" / "That said," / "With that in mind,"

**Hedging & qualification clusters:**
- "It's important to remember that…"
- "Of course, this is not always the case…"
- "While there are many factors to consider…"
- "The answer, of course, is complex…"
- "There is no one-size-fits-all answer…"
- "It depends on a variety of factors…"

**Hollow affirmations:**
- "Absolutely!" / "Certainly!" / "Of course!" / "Great question!"
- "You raise an excellent point…"
- "This is a fascinating topic…"

**Filler constructions:**
- "At the end of the day…"
- "In the grand scheme of things…"
- "It's a double-edged sword…"
- "All things considered…"
- "In today's [world/society/landscape]…"
- "Throughout history, humans have…"

**Score (1–10):** ___
**Evidence found:** [list specific examples with line references]

---

### 2. VOCABULARY PATTERNS
Flag repeated use of AI-favored words and terms:

**Overused descriptors:**
delve, dive into, explore, unpack, navigate, foster, leverage, utilize, facilitate,
tapestry, mosaic, kaleidoscope, labyrinth, nuanced, multifaceted, robust, holistic,
comprehensive, pivotal, crucial, paramount, essential, fundamental, intricate,
vibrant, dynamic, transformative, groundbreaking, revolutionary, game-changing,
profound, significant, notable, remarkable, unprecedented

**Abstract noun clusters:**
synergy, paradigm, framework, ecosystem, landscape, journey, intersection,
intersection of [X] and [Y], the realm of, the world of, the fabric of

**Verb inflation:**
"showcases" instead of "shows"
"demonstrates" instead of "proves"
"highlights" instead of "points to"
"underscores" instead of "confirms"
"encompasses" instead of "includes"

**Score (1–10):** ___
**Evidence found:** [list specific examples]

---

### 3. STRUCTURAL PATTERNS
Look for these AI-characteristic organizational habits:

- **The Rule-of-Three Obsession:** Ideas consistently grouped in threes; lists of exactly three examples
- **Symmetric Paragraph Architecture:** Every paragraph begins with a topic sentence, develops with two supporting points, and ends with a wrap-up
- **The Balanced Caveat:** Each positive claim immediately followed by an equal-length counterpoint
- **Section Bookending:** Chapters open and close with near-identical language or themes
- **Exhaustive Enumeration:** Tendency to list "not just A, but also B, C, and D" when A would suffice
- **Rhetorical Question Reliance:** Using questions ("But what does this mean?") to manufacture forward momentum
- **Artificial Escalation:** Moving from "small" to "global" scale at the end of paragraphs or sections

**Score (1–10):** ___
**Structural issues identified:** [describe]

---

### 4. VOICE & AUTHENTICITY MARKERS
Human writing typically includes:
- Idiosyncratic word choices that aren't "optimal"
- Incomplete thoughts or tangents that reveal a thinking mind
- Contradictions or genuine uncertainty (not performed uncertainty)
- Sensory specificity that feels lived-in, not researched
- Humor or irony that takes genuine risks
- An opinion the author seems to actually hold, with weight behind it
- **Asymmetry Detection:** When a single detail has unusually clean comic timing inside otherwise rougher prose, that asymmetry is worth flagging even if the detail itself passes surface inspection. Smoothness is still a signal.

AI writing typically includes:
- Consistent emotional temperature (never too hot, never too cold)
- "Safe" opinions that acknowledge all sides before landing on nothing
- Wisdom that sounds good but is empty on reflection ("The journey is just as important as the destination")
- Absence of authorial personality or a personality that reads as performed
- Information presented without surprise or confusion — as though the author never discovered it

**Score (1–10):** ___
**Voice assessment:** [describe what the author's voice feels like — or fails to feel like]

---

### 5. KNOWLEDGE TEXTURE
Examine how knowledge is handled:

- **Sourcing:** Does the author cite specific, verifiable sources or lean on vague authority ("studies show," "experts agree," "research suggests")?
- **Specificity:** Are examples concrete and traceable, or generic and illustrative?
- **Surprising Facts:** Does the chapter contain information that feels genuinely unexpected, or does it confirm what you already assumed?
- **Gaps:** Are there obvious follow-up questions the author ignores that a real expert would have addressed?

**Score (1–10):** ___
**Knowledge texture notes:** [describe]

---

### 6. CONSISTENCY & COHERENCE ANOMALIES
Check for:
- Contradictions between sections that suggest stitched-together outputs
- Sudden shifts in register (formal to casual, technical to accessible) without motivation
- Ideas referenced as "discussed earlier" that weren't actually discussed
- Character or subject descriptions that reset between sections
- Overlong scene-setting before any content is delivered
- Tonal flatness: no paragraph is significantly more energetic or urgent than any other

**Score (1–10):** ___
**Anomalies found:** [describe]

---

## VERDICT

**Total Score:** ___ / 60

| Range | Interpretation |
|-------|---------------|
| 6–18 | Likely human-written — minor AI-style tendencies at most |
| 19–30 | Ambiguous — may be AI-assisted or human writing with AI habits |
| 31–44 | Probably AI-generated or heavily AI-edited |
| 45–60 | Almost certainly AI-generated |

**Summary judgment:** [2–4 sentences: overall assessment, strongest signals, confidence level]

**Most suspicious passages:** [quote 2–3 specific excerpts with brief explanation of why they read as AI]

**Recommendations:** [If ambiguous, what additional information or comparison material would help confirm?]
```

---

### Intimacy Scene Craft
**Description:** Workshop a moment of physical or emotional intimacy.

```
Analyze the intimacy scene. Is it emotionally resonant, character-specific, and anatomically/physically coherent?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Metaphor & Simile Audit
**Description:** Evaluate the freshness and accuracy of figurative language.

```
Audit every metaphor and simile. Which are fresh and thematic? Which are clichés or mixed?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Filter Word & Narrative Distance Check
**Description:** Scan for filter words distancing the reader.

```
Scan for filter words (saw, heard, felt, realized) that distance the reader. Suggest rewrites to pull into Deep POV.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

## 6. Character

---

### New Character Creation
**Description:** Build a fully realized character from concept.

```
You are a creative collaborator and character development expert.

Concept: [CHARACTER CONCEPT / ROLE IN STORY]
Genre/tone: [GENRE AND TONE]
Context: [RELEVANT STORY CONTEXT]

Develop:
1. Core Identity — Name options, age, background, appearance (distinctive, not generic)
2. Psychology — Core wound, deepest fear, greatest desire, fatal flaw
3. Voice — How they speak (rhythm, vocabulary, verbal tics, what they never say)
4. Contradiction — The internal tension that makes them human
5. Relationships — How they relate to power, love, strangers
6. Arc Potential — What they need to learn, what they'll resist
7. Scene Presence — How they enter a room, how they behave under pressure
8. Three Revealing Details — Small, specific details that instantly characterize them

End with: One sentence capturing their essence — their through-line.
```

---

### Character Voice Workshop
**Description:** Develop and test a character's distinct dialogue voice.

```
You are a dialogue coach and character voice specialist.

CHARACTER:
[PASTE CHARACTER DESCRIPTION AND BACKGROUND HERE]

SCENE CONTEXT: [DESCRIBE THE SCENE CONTEXT FOR THE DIALOGUE]

First, define this character's Voice Rules:
- Sentence length tendency (clipped? flowing? interrupted?)
- Vocabulary level and register
- What they use instead of saying things directly
- What topics they deflect from and how
- Their emotional tell (how does stress/joy/anger show in speech?)
- 3 phrases they'd use; 3 phrases they'd NEVER use

Then write 8–10 lines of sample dialogue across different emotional registers: neutral, defensive, excited, lying, grieving.

Finally: write the same scene beat twice — once in their voice, once "generic" — to show the contrast.
```

---

### Character Consistency Audit
**Description:** Check if a character's behavior is consistent and motivated.

```
You are a developmental editor checking character consistency.

CHARACTER: [CHARACTER NAME]
PROFILE: [BRIEF CHARACTER PROFILE / KNOWN TRAITS]

Flag:
- Any action, decision, or reaction inconsistent with established character
- Dialogue that sounds like a different character or authorial voice
- Moments where the character is too conveniently helpful/obstructive
- Emotional reactions that aren't earned or set up
- Inconsistency in stated beliefs vs. behavior

For each flag: quote it, explain the inconsistency, suggest a fix.

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Emotional Interiority Depth
**Description:** Deepen the character's internal emotional landscape.

```
You are a literary editor focusing on character psychology. Analyze the interiority of the POV character. Where are they emotionally opaque?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Relationship Power Dynamics
**Description:** Analyze shifts in power between characters.

```
You are a scene analyst. Trace the shifting power dynamics between characters in this exchange. Who holds the high ground, and how does it shift?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Chemistry & Romantic Tension
**Description:** Evaluate romantic tension and chemistry.

```
You are a romance editor. Analyze the chemistry and romantic tension. Is it palpable? Based on character friction?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Emotional Vulnerability Calibration
**Description:** Assess moments of emotional exposure.

```
Analyze the emotional vulnerability of the characters. Are they guarding themselves appropriately or opening up unearned?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Full-Cast Voice Differentiation
**Description:** Ensure all voices in an ensemble are unique.

```
You are a dialogue coach. Look at a multi-character scene. Are the voices distinct enough to lose dialogue tags?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

## 7. World-Building

---

### World Building Bible Entry
**Description:** Create a structured reference entry for any world element.

```
You are a world-building consultant.

ELEMENT: [WHAT ARE YOU DOCUMENTING — e.g., magic system, government, technology]
GENRE/TONE: [YOUR GENRE AND TONE]
WHAT I KNOW SO FAR:
[PASTE YOUR EXISTING NOTES HERE]

Develop into a full World Bible entry:
1. Core Concept — One clear sentence definition
2. Rules & Logic — Internal laws (consistent, exploitable, with costs)
3. History & Origin — How it came to be, key turning points
4. Current State — How it exists in the world now
5. Factions & Perspectives — How different groups relate to this element
6. Sensory Reality — What it looks, sounds, smells, feels like
7. Story Potential — 5 conflict seeds this element could generate
8. Consistency Traps — Questions to answer to avoid plot holes

Flag any logical contradictions in what I've provided.
```

---

### World Consistency Check
**Description:** Audit a passage for world-building errors.

```
You are a continuity editor specializing in world-building. Check this passage against the established world rules.

WORLD RULES:
---
[PASTE YOUR WORLD RULES / BIBLE NOTES HERE]
---

Check for:
- Violations of established world rules
- Technology, magic, or social structures used inconsistently
- Anachronistic language or concepts for this world
- Details that contradict earlier established facts
- Missed opportunities to reinforce world-building organically

Present as: Issue → Quote → Explanation → Suggested Fix

TEXT:
---
[PASTE TEXT HERE]
---
```

---

### Tech & Jargon Calibration
**Description:** Evaluate the use of technical language.

```
You are a sci-fi accuracy editor. Is the tech jargon immersive or overwhelming? Suggest balancing.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Noir & Atmosphere Pressure
**Description:** Assess the atmospheric tension of the setting.

```
Evaluate the atmosphere. Does the setting exert a palpable pressure (noir, gothic, cyberpunk) on the characters?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

## 8. Location & Setting

---

### Location Deep Build
**Description:** Develop a location into a vivid, story-ready setting.

```
You are a setting development specialist.

LOCATION: [LOCATION NAME AND BASIC CONCEPT]
NARRATIVE ROLE: [ITS NARRATIVE ROLE IN YOUR STORY]
GENRE/TONE: [YOUR GENRE AND TONE]

Develop:
1. Establishing Shot — One paragraph introduction as a reader would first encounter it
2. Sensory Atlas — Dominant impressions across all senses, time-of-day variations
3. History Embedded in Space — What does this place carry from its past?
4. Living Ecosystem — What lives here? What rhythms govern it?
5. Emotional Register — What mood does it impose on characters?
6. Scene Potential — 4 different scene types this location enables
7. Symbolic Resonance — What could this place mean thematically?
8. 3 Unique Details — Specific, unusual details no other location would have

End with: A single image that captures the essence of this place.
```

---

### Location Scene Enhancement
**Description:** Deepen an existing location scene for atmosphere and immersion.

```
You are a line editor specializing in setting and atmosphere.

Assess:
1. Is the setting earning its place on the page, or is it wallpaper?
2. What sensory channels are underused?
3. Does the setting reflect or contrast the POV character's emotional state?
4. Are there missed opportunities for the setting to do story work?
5. Is there any over-description slowing the scene?

Then: Provide a rewritten version of the most underdeveloped descriptive passage, showing how to deepen it without adding length.

TEXT:
---
[PASTE TEXT HERE]
---
```

---

## 9. Punch & Impact

---

### Impact Rewrite — Multiple Options
**Description:** Get 4 punchy rewrites of any passage.

```
You are a master prose stylist. Rewrite this passage 4 times, each time using a different technique to maximize impact.

ORIGINAL:
---
[PASTE YOUR PASSAGE HERE]
---
Emotional goal: [WHAT SHOULD THIS PASSAGE DO EMOTIONALLY? OR WRITE: Infer from context]

REWRITE 1 — Compression: Strip it to its most essential form. Every word earns its place.
REWRITE 2 — Rhythm: Deliberate sentence-length variation for emotional punch. Short sentences land blows.
REWRITE 3 — Concrete Detail: Replace abstractions with specific, physical, visceral detail.
REWRITE 4 — Subtext: Pull back. Let the emotion live beneath the surface. Trust the reader.

After each rewrite: one sentence on what you sacrificed and what you gained.
Then: Which approach best serves this moment and why?
```

---

### Opening Line Workshop
**Description:** Generate and critique multiple opening line options.

```
You are a master of first lines.

WHAT THIS CHAPTER IS ABOUT: [SUMMARIZE YOUR CHAPTER/SCENE]
DESIRED TONE: [YOUR DESIRED TONE]
CURRENT OPENING: [YOUR CURRENT OPENING LINE, OR: None yet]

Generate 8 different opening lines, each using a different technique:
1. In medias res — action already happening
2. Disorientation — reader doesn't yet know where they are
3. Voice-first — pure character voice
4. Sensory ambush — lead with a striking sense impression
5. Paradox or contradiction — something that doesn't add up
6. The ordinary made strange
7. The last line of the previous scene as echo
8. Pure momentum — the first domino that starts everything falling

For each: one sentence on what it promises the reader.
Then: If forced to pick one, it would be ___ because ___.
```

---

### Closing Line Workshop
**Description:** Craft a chapter-ending line with maximum resonance.

```
You are a prose stylist specializing in chapter endings.

WHAT HAPPENED: [SUMMARIZE WHAT HAPPENED IN THIS CHAPTER]
WHAT'S COMING: [BRIEFLY DESCRIBE WHAT COMES NEXT]
CURRENT CLOSING: [YOUR CURRENT CLOSING LINE, OR: None yet]

Generate 6 closing line options:
1. The gut-punch — an image or fact that lands like a blow
2. The quiet devastation — understated, the weight arrives after
3. The question — leaves the reader unable to stop thinking
4. The reframe — changes how the reader sees everything before it
5. The echo — callbacks a word or image from the chapter's opening
6. The door — ends mid-motion, pure momentum into the next chapter

For each: what emotion it leaves behind.
Then: My recommendation for this chapter's emotional needs is ___ because ___.
```

---

## 10. Chapter-Level Review

---

### Overused Phrases & Words
**Description:** Find repetitive or clichéd language and suggest alternatives.

```
You are a prose editor specializing in eliminating overused, repetitive, and clichéd language.

NOVEL CONTEXT: [BRIEF CONTEXT / CHARACTER NAMES / SETTING NOTES]

Scan the following chapter for:
1. **Repeated words** — Words used too frequently (especially adjectives, adverbs, verbs)
2. **Clichés** — Overused phrases and expressions
3. **Filter words** — "He saw", "She heard", "He felt", "She noticed" etc.
4. **Weak constructions** — "There was", "It was", "He was", "She had"
5. **Redundancies** — Words or phrases that say the same thing twice
6. **Said-isms** — Overuse of "said" or weak dialogue tags
7. **Telling instead of Showing** — Instances where showing would be stronger

For each issue found, provide:
- The problematic phrase (quoted exactly)
- The line number or location
- Why it's problematic
- A suggested replacement (or "cut" if it can be removed)

Finally, provide a revised version of the first 500 words with your corrections applied.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Pronoun Usage Analysis
**Description:** Check pronoun density and sentence-start pronouns.

```
You are a prose editor specializing in varied, strong sentence construction.

Analyze the following chapter for pronoun usage patterns. The goal is to keep total pronoun usage under 15% and sentences starting with pronouns under 30%.

TARGETS:
- Total pronoun usage: under 15% of all words
- Sentence-start pronouns: under 30% of all sentences

Calculate and report:
1. **Total word count** and **total pronoun count**
2. **Pronoun density percentage** (pronouns ÷ total words × 100)
3. **Total sentences** and **sentences starting with pronouns**
4. **Initial pronoun percentage** (sentence-start pronouns ÷ total sentences × 100)

For each category, note if it passes or fails the target.

If OVER the targets, identify the specific problem sentences and provide revised versions with:
- Stronger sentence openers (action verbs, sensory details, setting, subject presence)
- Name substitutions where appropriate
- Varied sentence structures

Also identify any sentences that could be combined or restructured for better flow.

MAIN POV CHARACTER NAME(S): [ENTER NAME(S)]
CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Full Chapter Review
**Description:** Comprehensive editorial read covering all dimensions.

```
You are a senior editor at a major literary publishing house. Full editorial read.

NOVEL CONTEXT: [WHERE ARE WE IN THE NOVEL? STAKES, WHAT JUST HAPPENED]

**THE CHAPTER IN ONE SENTENCE** — What actually happens here (not what was intended, what's on the page).

**WHAT'S WORKING** — Specific. Quote the lines or moments that are genuinely excellent.

**THE CORE ISSUE** — If there's one structural or thematic problem, name it clearly.

**SCENE BY SCENE** — Walk through each scene: Goal / Conflict / Outcome. Flag scenes that don't change anything.

**CHARACTER** — Is everyone acting like themselves? Any character doing something for plot convenience?

**PACING** — Where does it breathe well? Where does it stall or rush?

**PROSE** — Flag the 3 weakest prose moments and the 3 strongest. Be specific.

**READER EXPERIENCE** — What will the reader feel at the end? Is that what the novel needs?

**3 PRIORITY ACTIONS** — If you could only change three things, in order of impact?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Chapter Hook & Cliffhanger Audit
**Description:** Analyze the start and end of the chapter for momentum.

```
Analyze the opening hook and the ending cliffhanger. Do they pull the reader in and enforce turning the page?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Tonal Consistency Check
**Description:** Flag jarring emotional or atmospheric tonal shifts.

```
You are a tone editor. Flag moments where the emotional tone dramatically shifts without narrative justification.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

## 11. Paragraph-Level

---

### Paragraph Dissection
**Description:** Sentence-level analysis and improvement of a single paragraph.

```
You are a line editor. Dissect this paragraph at the sentence level.

For each sentence:
- Assess its function (advance action, reveal character, set mood, provide information?)
- Rate effectiveness: Strong / Adequate / Weak
- If Weak: explain why and provide a rewrite

Assess the paragraph as a whole:
- Does it have a clear through-line?
- Is the rhythm varied and intentional?
- Does it earn its length?
- What is the single most impactful change?

Finally: Provide a polished rewrite incorporating your best suggestions (keep the author's voice).

PARAGRAPH:
---
[PASTE YOUR PARAGRAPH HERE]
---
```

---

### Transition Repair
**Description:** Fix a jarring or unclear transition between paragraphs or scenes.

```
You are a line editor specializing in flow and transitions. The transition between these sections isn't working. Diagnose and offer solutions.

Diagnose:
- What is the logical/emotional gap between these sections?
- Is this a tonal shift, a time jump, a POV distance change, a pace change?
- What's currently bridging them (if anything)?
- Why isn't it working?

Then provide 3 different transition options:
1. A bridging sentence or short paragraph
2. A structural fix (scene break, section break, different ending)
3. A rewrite of one or both endings/openings to create natural flow

BEFORE:
---
[PASTE THE SECTION THAT COMES BEFORE THE TRANSITION]
---
AFTER:
---
[PASTE THE SECTION THAT COMES AFTER THE TRANSITION]
---
```

---

### White Space & Paragraph Rhythm
**Description:** Analyze how paragraph breaks control pacing.

```
Analyze paragraph length and white space. Are blocks of text intimidating? Do short paragraphs land with punch?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Echo & Crutch Word Finder
**Description:** Identify word echoes and crutch words.

```
Identify words repeated too closely together (echoes) and likely unconscious crutch words used in the passage.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

## 12. Sentence-Level

---

### Sentence Surgery — 5 Options
**Description:** Get five distinct rewrites of any sentence.

```
You are a prose stylist. Rewrite this sentence 5 times, each version solving a different problem or pursuing a different strength.

ORIGINAL: [PASTE YOUR SENTENCE HERE]
CONTEXT: [PASTE 1-2 SURROUNDING SENTENCES FOR CONTEXT]
KNOWN ISSUE: [DESCRIBE WHAT'S WRONG WITH IT, OR WRITE: Diagnose yourself]

VERSION 1 — Tighter: Cut every unnecessary word. Minimum viable sentence.
VERSION 2 — Punchier rhythm: Reorder for a stronger landing. End on the word with most weight.
VERSION 3 — More concrete: Replace abstractions or vague verbs with specific, physical language.
VERSION 4 — More voice: Push the character or narrator's voice harder. Make it more "theirs."
VERSION 5 — Syntactic experiment: Try a completely different sentence structure (fragment, inversion, list, etc.)

For each: one phrase explaining what changed and why it works.
```

---

### Verb Audit
**Description:** Replace weak or passive verbs with muscular, specific alternatives.

```
You are a line editor. Do a verb audit on this text.

Flag every instance of:
- "To be" constructions that could be cut or made active
- Vague motion verbs: went, came, moved, got — replace with specific action
- "Began to" / "started to" constructions — usually just cut them
- Passive voice (flag it, don't automatically fix — sometimes it's right)
- Verbs propped up by adverbs — find one strong verb instead

For each flag: Original → Suggested Verb(s) → one-word reason.
Then: A rewritten version of the 3 weakest sentences with upgraded verbs.

TEXT:
---
[PASTE TEXT HERE]
---
```

---

## 13. Tension & Engagement

---

### Micro-Tension Audit
**Description:** Find places where tension flags on a line-by-line basis.

```
You are a line editor. Audit for micro-tension. Does every sentence carry a small spark of conflict, curiosity, or unease?

Return a tension heat map + 3 specific fixes.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Reader Curiosity Tracker
**Description:** Map what questions the reader is asking.

```
Map the reader's curiosity. What questions are opened? Which are closed? Is there a primary driving question? Flag momentum killers.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Confusion Mapping
**Description:** Identify where the reader might be unintentionally lost.

```
Read aggressively looking for unintentional confusion: unclear pronouns, spatial logic, or dropped context. Flag every moment of confusion and rank by severity.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Emotional Payoff Audit
**Description:** Ensure the chapter delivers on its emotional promises.

```
Identify emotional promises made and evaluate if they land. Flag unearned or rushed payoffs.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Threat Credibility Check
**Description:** Ensure the antagonist or threat feels genuinely dangerous.

```
You are a thriller developmental editor. Does the threat feel credible, or contrived?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

## 14. Prose & Style Audits

---

### Voice & Style Audit
**Description:** Analyze narrative voice consistency.

```
Analyze narrative voice — is it consistent? Flag shifts in tone, style, POV distance.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Sentence Variety Analysis
**Description:** Audit rhythm and sentence structure.

```
Analyze sentence variety — length, structure, rhythm. Flag monotony patterns.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Imagery & Metaphor Audit
**Description:** Evaluate sensory language.

```
Evaluate imagery, metaphor, and sensory language. Flag clichés and weak comparisons.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

## 15. Reader Experience

---

*(See also: [Confusion Mapping](#confusion-mapping), [Emotional Payoff Audit](#emotional-payoff-audit), and [Reader Curiosity Tracker](#reader-curiosity-tracker) above.)*

---

## 16. Genre-Specific

These prompts are tailored for specific genre conventions.

---

### Fantasy — Magic System Integrity Check
**Description:** Audit magic use for consistency and costs.

```
Audit every instance where magic is used. Are rules consistent? Does it solve problems too easily? Are costs legible?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Fantasy — World Weight Check
**Description:** Evaluate if the world exerts pressure on the plot.

```
Does history, culture, and geography exert genuine pressure on characters? Flag where the world recedes to backdrop.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Fantasy — Prophecy & Myth Handling
**Description:** Evaluate use of legend/prophecy.

```
If prophecy is used, does it create dramatic irony or act as a GPS removing tension? Suggest ambiguity.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Fantasy — Scale & Intimacy Balance
**Description:** Balance macro stakes with human stakes.

```
Evaluate balance between world-ending stakes and intimate human grief/loyalty.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Grimdark — Moral Ambiguity Audit
**Description:** Evaluate difficult moral choices.

```
Are moral choices genuinely difficult with real costs? Flag manufactured complexity.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Grimdark — Consequence Tracking
**Description:** Check if violent/costly events carry weight.

```
Do past traumas/costs carry weight? Flag resets or convenient forgetting.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Urban Fantasy — Mundane/Magic Collision
**Description:** Friction between ordinary and supernatural.

```
Is the mundane world grounded enough to make magic feel intrusive? Flag where the real world fades.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Urban Fantasy — Masquerade & Secrecy Tension
**Description:** Maintain tension of concealment.

```
Are stakes of exposure real? Does the protagonist feel the weight of living between two worlds?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Hard SF — Science Credibility Audit
**Description:** Internal consistency of technical content.

```
Evaluate scientific content for consistency. Flag hand-waved science or dramatic convenience.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Hard SF — Extrapolation Coherence
**Description:** Logical worldbuilding from premises.

```
Does society and tech follow logically from the central scientific premise?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Space Opera — Galactic Scale vs. Personal Stakes
**Description:** Make interstellar stakes feel personal.

```
Balance large-scale conflict with intimate drama. Flag where human story is crushed.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Space Opera — Crew/Ensemble Dynamic
**Description:** Group dynamics and interpersonal tension.

```
Is group dynamic clear? Are voices distinguishable? Flag if crew feels like a single unit.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Space Opera — Alien & Culture Specificity
**Description:** Render alien species genuinely other.

```
Do aliens feel genuinely other with distinct logic, or just humans in costume?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Literary — Subtext Density Audit
**Description:** Check if surface action carries hidden meaning.

```
Audit every scene for subtext. Characters saying one thing meaning another. Flag over-explanation.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Literary — Structural Symbolism
**Description:** Evaluate objects/weather carrying meaning.

```
Are symbols present and working without being overexplained?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Mystery — Clue Architecture Audit
**Description:** Map clues, red herrings, evidence.

```
Map every clue. Is it fair without being obvious? Flag clues buried too deep.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Mystery — Detective Logic Consistency
**Description:** Evaluate reasoning and deduction.

```
Are conclusions earned by evidence? Flag logical leaps.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Mystery — Suspect & Motive Mapping
**Description:** Audit suspects for legibility.

```
Does each suspect have motive/opportunity? Flag placeholder suspects.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Horror — Dread Architecture
**Description:** Wrongness accumulating before horror.

```
Is dread accumulating? Flag where it moves too quickly to shock.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Horror — The Uncanny Check
**Description:** Familiar becoming wrong.

```
Evaluate genuine uncanniness. Make familiar imagery fresh.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Historical Fiction — Period Authenticity Audit
**Description:** Evaluate historical texture.

```
Flag anachronisms in thought, speech, object. Period detail shouldn't just be decor.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Thriller — Countdown & Urgency
**Description:** Ticking clock mechanics.

```
Is the deadline real and felt? Flag where urgency goes slack.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Crime — Underworld Authenticity
**Description:** Evaluate criminal world rendering.

```
Does the criminal world have authentic rules and hierarchy? Flag generic TV shorthand.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Crime — Moral Compromise Tracking
**Description:** Track ethical erosion.

```
Are ethical compromises felt? Is narrative letting character off too easily?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Romance — The Meet or Reunion Dynamic
**Description:** Evaluate first meeting effectiveness.

```
Is there immediate specificity and friction? Flag formulaic meets.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Romance — Romantic Obstacles Audit
**Description:** Map external and internal obstacles.

```
Are obstacles genuine and character-rooted, or contrived misunderstandings?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### YA — Authentic Teen Voice
**Description:** Evaluate adolescent perspective.

```
Does voice feel genuinely adolescent without performing "teen"? Flag adult ideas of youth.

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

### Middle Grade — Age-Appropriate Complexity
**Description:** Moral complexity calibration.

```
Is emotional complexity challenging without being overwhelming?

CHAPTER:
---
[PASTE CHAPTER HERE]
---
```

---

*This reference guide covers all prompts from The Novelist's Atelier v1.4 Beta. For the interactive tool with pipeline features, use the full application.*
