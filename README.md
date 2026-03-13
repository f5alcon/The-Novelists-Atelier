# The Novelist's Atelier

AI-powered writing assistant for editing and world-building. Features multiple AI providers (Claude, GPT, Gemini), flexible context management at Series/Book/Chapter levels, and a privacy-first design with all data stored locally in your browser.

Version 1.4 Beta is feature complete. I do not expect to add more features to the tool, so unless more APIs or bug fixes are needed this should be the same as 1.0 Release. Going forward this single HTML version will stay free and open source. I am working on a more complete suite of tools that can go from idea to planning to writing to editing to marketing to publishing, but it will be a seperate project.  

## Disclaimer
Many traditional publishers require zero AI usage to be published, if you are persuing this distribution method you are using this tool at your own risk. For self publishing refer to your local laws and regulations. [Authors Guild stance on AI](https://authorsguild.org/resource/ai-best-practices-for-authors/)

## Tutorials
[Youtube Tutorial](https://youtu.be/watch?v=9akdLTKwpg0)
[Written Tutorial](https://github.com/f5alcon/The-Novelists-Atelier/blob/main/Tutorial/Tutorial.md)

## Features

![Settings](https://github.com/user-attachments/assets/59193865-7f38-4ee2-9af7-00998272d289)
![Home](https://github.com/user-attachments/assets/ae144c5e-be2c-4dbb-a1c5-7f8a5dc59627)

- **Multiple AI Providers**: OpenRouter, Anthropic Direct (Claude), OpenAI Direct (GPT), Google Direct (Gemini), and LM Studio (local models)
- **Flexible Context**: Add details at Series, Book, or Chapter level to customize AI prompts
- **AI-Powered Editing Tools**:
  - Character creation & motivations
  - World-building & locations
  - Copy editing
  - Line editing (sentence variety, word choice, dialogue naturalism)
  - Developmental editing:
    - Story arc structure
    - Stakes escalation
    - Subplot resolution
    - Plot holes & contradictions
    - Character motivations
    - Thematic cohesion
    - Scene purpose
    - Scene openings & endings
    - POV consistency
    - Scene-level conflict
  - And more...
- **Pipeline Mode**: Chain multiple prompts together for complex workflows
- **Local mode** — instant, no API call, parses markdown structure directly
- **AI Enhanced mode** — smarter extraction for complex or irregular outputs
- Works from both the Prompts output toolbar and the Compare tab
- Output opens in a new tab and can be saved, printed, or shared
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

- 1.35 Update
- Added full manuscript check option (This is a lot of tokens depending on the length of the manuscript, potentially very expensive on API usage, it is better to use a tool with a subscription to check)
- Also a prompt to take the output of that and create an html view of the report. Attach the report and put the prompt into the chat.
![Manuscript report](https://github.com/user-attachments/assets/9d61c946-a0c7-4c77-aa25-f5f8122a5320)
![Beta Reader feedback](https://github.com/user-attachments/assets/5c82c287-e585-43ed-b578-2363d23f9591)

-1.4 Update
- ### ⇄ Compare Tab

Run multiple different AI analyses on the same chapter, then cross-examine them automatically. The Compare tab finds **conflicts** (where two analyses give contradictory advice on the same passage) and **consensus** (where they independently flag the same problem), and reproduces every issue verbatim so nothing gets lost in synthesis.

**Why it matters:** A pacing audit and a show/tell audit will catch different things — but they'll also sometimes contradict each other. Knowing which flags are backed by both analyses tells you where to spend your revision time first.

- Add analyses from the Prompts tab with a single click, or paste in outputs from Claude.ai or any other session
- Run automated conflict detection via API, or copy the prompt to use in a chat interface
- Filter results by Conflicts only, Consensus only, or Full view
- Convert the comparison into a formatted **Visual Report** document

### 📄 Visual Report

Turn any AI analysis output into a formatted, printable HTML document — structured with a sidebar, section cards, and severity tags (Critical / Important / Minor).


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

1.4 Beta

## License

Apache License 2.0 - See LICENSE file for details
