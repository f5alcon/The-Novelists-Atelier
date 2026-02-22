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

## Version

1.0 Beta

## License

Apache License 2.0 - See LICENSE file for details
