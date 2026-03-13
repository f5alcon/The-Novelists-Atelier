# The Novelist's Atelier - Complete Tutorial

Welcome to The Novelist's Atelier, a free AI-powered writing and editing tool designed for novelists and fiction writers. This comprehensive tutorial covers every feature across all tabs.

---

## Table of Contents

1. [Series Tab](#1-series-tab)
2. [Book Tab](#2-book-tab)
3. [Chapter Tab](#3-chapter-tab)
4. [Characters Tab](#4-characters-tab)
5. [Relationships Tab](#5-relationships-tab)
6. [World Tab](#6-world-tab)
7. [Prompts Tab](#7-prompts-tab)
8. [Pipeline Tab](#8-pipeline-tab)
9. [Settings Tab](#9-settings-tab)
10. [Timeline Tab](#10-timeline-tab)
11. [Analysis Tab](#11-analysis-tab)
12. [Find Tab](#12-find-tab)
13. [Stats Tab](#13-stats-tab)
14. [Branches Tab](#14-branches-tab)

---

## 1. Series Tab

# My Project


### Overview

The Series tab is your command center for managing multi-book series. It stores metadata and world-building content that applies across all books in your series.

### Key Features

| Feature | Description |
|---------|-------------|
| **Series Name** | The title of your book series |
| **Subtitle** | Optional series subtitle or tagline |
| **Series Bible** | Collection of world-building entries specific to the series |
| **Word Count** | Total word count of all series bible entries |
| **Export** | Export series data to Markdown format |

### Series Bible Entries

![Series Page](https://github.com/user-attachments/assets/c550681b-3915-41e3-9179-e558f5e95b59)


Each series bible entry contains:
- **Title** - Name of the entry (e.g., "Magic System," "Main Faction," "Historical Timeline")
- **Content** - Detailed description, rules, or information
- **Tags** - Optional categorization

### How to Use

1. **Set Series Name**: Click the Series Name field and type your series title
2. **Add Subtitle** (Optional): Click the Subtitle field to add a tagline
3. **Add Series Bible Entry**:
   - Click **+ Add Entry** button
   - Enter a title for the entry
   - Write detailed content in the editor
   - Click **Save** to persist
4. **Delete Entry**: Click the trash icon next to any entry
5. **Export Series**: Click **Export to Markdown** to download all series data

### Tips

- Use the Series Bible to document **magic systems**, **major factions**, **history**, and **rules** that apply to all books
- Reference series content in AI prompts by selecting it in the **Data Sources** section
- Keep entries **concise but comprehensive** - you'll be feeding this to AI tools

---

## 2. Book Tab

![Book](https://github.com/user-attachments/assets/da3a448e-cc45-419c-8401-43dcc2c7b1d6)


### Overview

The Book tab manages metadata for individual books within your series. Each book can have its own bible entries, characters, and settings.

### Key Features

| Feature | Description |
|---------|-------------|
| **Book Title** | Title of this specific book |
| **Book Number** | Position in series (#1, #2, etc.) |
| **Book Bible** | Book-specific world-building entries |
| **Word Count** | Total word count for this book's content |
| **Save** | Persist book metadata |

### Book Bible Entries

Similar to Series Bible but specific to this book:
- **Title** - Entry name (e.g., "This Book's Magic Rules," "Unique Locations")
- **Content** - Book-specific details
- **Inherits from Series** - Option to reference series bible entries

### How to Use

1. **Enter Book Title**: Click the title field and type your book name
2. **Set Book Number**: Enter the book number in the series
3. **Add Book Bible Entry**:
   - Click **+ Add Entry**
   - Write title and content
   - Click **Save**
4. **Save Book**: Click the **Save** button to persist all changes

### Tips

- Use Book Bible for **magic variations** specific to this book
- Document **unique locations** or **characters** that only appear in this book
- The book number helps AI tools understand **where you are in the series arc**

---

## 3. Chapter Tab

![Chapter](https://github.com/user-attachments/assets/78cf48dc-4088-4ccc-b568-5938c7adba18)


### Overview

The Chapter tab is your advanced editing workspace. It provides real-time prose analysis, entity tracking, and structured chapter goals.

### Key Features

#### Prose Pulse - Real-Time Analysis


| Metric | Description |
|--------|-------------|
| **Pacing Analysis** | Visual overlay showing fast (green) vs slow (red) sentences |
| **Dialogue %** | Percentage of dialogue in your chapter |
| **Sentiment/Mood** | Emotional trend tracking with visual indicators |

#### Entity Links


- Automatically links characters, locations, and world elements in your text
- Click any entity to see all its mentions
- Helps maintain consistency

#### Chapter Goals (S+C+R Framework)


| Field | Description | Example |
|-------|-------------|---------|
| **Setting** | Where and when | "Coffee shop, morning, rain outside" |
| **Conflict** | The problem or tension | "She must ask for help but fears rejection" |
| **Resolution** | How it's resolved | "She speaks up; he agrees to help" |

#### Documents List

- Shows all chapters/documents in your project
- Click to select which chapter to analyze
- Displays word count per document

### How to Use

1. **Select Chapter**: Click a document from the list to load it
2. **View Prose Pulse**: The analysis loads automatically as you type
3. **Set Chapter Goals**:
   - Fill in Setting, Conflict, Resolution
   - Use as a checklist while writing
4. **Track Entities**: Click entities in the text to see all mentions
5. **Review Sentiment**: Check the mood graph for emotional consistency

### Tips

- Use Prose Pulse to **balance pacing** - vary sentence lengths
- Keep dialogue between **20-40%** for engaging prose
- The S+C+R framework prevents **sagging middles**
- Review entity links to catch **continuity errors**

---

## 4. Characters Tab


### Overview

The Characters tab displays all characters from your Planning page and provides detailed character management.

### Key Features

| Feature | Description |
|---------|-------------|
| **Character List** | All characters in your project |
| **Role Display** | Protagonist, Antagonist, Mentor, etc. |
| **Description** | Character backstory and traits |
| **Goals & Conflicts** | Character motivations |
| **Edit Character** | Open full character editor |

### Character Fields


| Field | Description |
|-------|-------------|
| **Name** | Character's name |
| **Role** | Protagonist, Antagonist, Mentor, Ally, Deuteragonist, Supporting, Minor |
| **Age** | Character's age |
| **Description** | Physical appearance, personality |
| **Goals** | What the character wants |
| **Conflicts** | What opposes them |
| **Arc** | How they change through the story |
| **Inclusion** | Full, Partial, Mention Only |

### How to Use

1. **View Characters**: All characters display in a list with role badges
2. **Edit Character**: Click any character to open the full editor
3. **Add Character**: Click **+ Add Character** to create new
4. **Delete Character**: Use the trash icon (with confirmation)
5. **Include in Prompts**: Select characters to include in AI context

### Tips

- Use **detailed goals and conflicts** for better AI character development
- The **Inclusion** field helps AI focus on relevant characters
- Keep **character arcs** concise - one sentence per story beat

---

## 5. Relationships Tab


### Overview

The Relationships tab visualizes and manages character connections with a dynamic relationship map.

### Key Features

#### Relationship Types

| Type | Description |
|------|-------------|
| Related | Family/blood relations |
| Friend | Friendly associations |
| Family | Non-blood family |
| Romantic | Love interests |
| Rival | Competitive relationships |
| Enemy | Antagonistic relationships |
| Conflict | Characters in dispute |
| Mentor | Teacher/student dynamic |
| Ally | Cooperative partners |

#### Relationship Strength

- **1-10 Scale** - Visual bar showing relationship intensity
- **Dynamic Description** - Strength informs the relationship narrative

#### Relationship Map

[IMAGE: Relationship Map - Interactive node diagram]

- **Visual Node Graph** - Characters as nodes, relationships as lines
- **Color-Coded** - Different colors for each relationship type
- **Interactive** - Drag nodes to rearrange, click for details

### How to Use

1. **View Relationships**: See all character connections in list or map view
2. **Add Relationship**: Click **+ Add Relationship**, select two characters and type
3. **Set Strength**: Use the slider to rate 1-10
4. **Edit Description**: Add details about the relationship
5. **Explore Map**: Click nodes to see relationship details

### Tips

- Use the map to **spot relationship clusters** and isolated characters
- **Update strength** as relationships evolve through your story
- Reference relationships in prompts for **more authentic dialogue**

---

## 6. World Tab


### Overview

The World tab manages locations, settings, and world-building elements with rich sensory details.

### Key Features

#### Locations


| Field | Description |
|-------|-------------|
| **Name** | Location name |
| **Type** | City, Building, Region, World, Faction, Item |
| **Description** | Detailed location description |

#### Sensory Palette


| Sense | Description | Example |
|-------|-------------|---------|
| **Sight** | Visual elements | "Neon signs, fog, cobblestones" |
| **Sound** | Ambient noises | "Traffic, jazz from club, rain" |
| **Smell** | Scents | "Coffee, diesel, perfume" |
| **Touch** | Textures | "Cold metal, wet pavement" |
| **Taste** | Flavors | "Stale air, metallic tang" |

#### World Elements

- Factions, religions, technologies
- Custom world-building categories
- Can be referenced in AI prompts

### How to Use

1. **Add Location**: Click **+ Add Location**
2. **Fill Details**: Enter name, type, description
3. **Set Sensory Palette**: Fill in all five senses for immersive settings
4. **Add World Elements**: Create custom categories for factions, etc.
5. **Reference in Prompts**: Select locations/world elements for AI context

### Tips

- The **Sensory Palette** creates vivid settings - use all five senses
- Reference sensory details in **scene-setting prompts**
- Group related locations under **same-type categories**

---

## 7. Prompts Tab

![Prompts](https://github.com/user-attachments/assets/6540fad9-bb61-48a5-9ca6-9fa64d8cf21f)


### Overview

The Prompts tab is your AI-powered editing toolkit with 12+ prompt categories covering every stage of editing.

### Prompt Categories


| Category | Icon | Color | Purpose |
|----------|------|-------|---------|
| Character | ◑ | #e07070 | Character development and dialogue |
| World Building | ◒ | #70b0e0 | Magic systems, history, factions |
| Locations | ◓ | #70c0a0 | Setting development |
| Developmental | ◉ | #8fbc8f | Structure, pacing, plot holes |
| Copy Editor | ◎ | #87afc7 | Grammar, mechanics, consistency |
| Line Editor | ◐ | #c987c7 | Sentence-level improvements |
| Impact & Punch | ◆ | #e0b870 | Tightening weak prose |
| Paragraph | ¶ | #d8a098 | Paragraph flow and structure |
| Sentence | — | #98c8d8 | Sentence clarity and variety |
| Chapter Review | ❒ | #a098d8 | Full chapter analysis |
| Style Analysis | ◈ | #c9a96e | Voice and tone consistency |
| Custom | ✎ | #c8a660 | User-created prompts |

### Developmental Prompts (Examples)

| Prompt | Description |
|--------|-------------|
| **Chapter Structure** | Analyze act/scene structure |
| **Pacing Analysis** | Identify slow/fast sections |
| **Arc Tracker** | Track character/plot arcs |
| **Plot Hole Finder** | Identify logic gaps |
| **Thematic Analysis** | Examine themes and motifs |

### Copy Editor Prompts

| Prompt | Description |
|--------|-------------|
| **Full Copy Edit** | Comprehensive grammar/mechanics |
| **Dialogue Mechanics** | Quote marks, attribution |
| **Fact Check** | Internal consistency |
| **Consistency** | Character/setting details |

### Line Editor Prompts

| Prompt | Description |
|--------|-------------|
| **Show vs Tell** | Convert telling to showing |
| **Sensory Depth** | Add sensory details |
| **Word Choice** | Stronger verb/adjective alternatives |
| **Repetition** | Find overused words |

### Data Sources


Before running a prompt, select what context to include:
- **Series Bible** (select specific entries)
- **Book Bible**
- **Characters** (all or specific)
- **Relationships**
- **Timeline**
- **Chapters** (all or specific)

### How to Use

1. **Select Category**: Click a category from the grid
2. **Choose Prompt**: Select a specific prompt from the list
3. **Configure Data Sources**: Check what context to include
4. **Paste Text**: Enter the text to analyze in the input field
5. **Run Prompt**: Click **Generate** to get AI feedback
6. **Copy/Export**: Save the results

### Tips

- Start with **Developmental** prompts for big-picture issues
- Use **Line Editor** prompts in later passes
- Select **specific chapters** for focused feedback
- The **Pipeline tab** chains multiple prompts together

---

## 8. Pipeline Tab

![pipeline](https://github.com/user-attachments/assets/42e7c41a-98da-41cc-b049-d7df3c980137)


### Overview

The Pipeline tab lets you chain multiple AI prompts together for automated multi-pass editing workflows.

### Key Features

#### Pipeline Modes

| Mode | Description |
|------|-------------|
| **Refine** | Each step's output feeds into the next (sequential) |
| **Parallel** | All steps analyze the same input independently |

#### Pipeline Steps


Each step includes:
- **Category** - Which prompt category
- **Specific Prompt** - The exact prompt to use
- **Use Previous Output** - (Refine mode only) Feed prior output as input
- **Apply Style DNA** - Apply your writing preferences

#### Presets


- **Save Preset** - Store current pipeline configuration
- **Load Preset** - Restore saved configuration
- **Delete Preset** - Remove saved presets

### How to Use

1. **Choose Mode**: Select Refine or Parallel
2. **Add Step**: Click **+ Add Step**
3. **Configure Step**: Select category and prompt
4. **Set Options**: Toggle previous output or Style DNA
5. **Add More Steps**: Repeat for additional passes
6. **Run Pipeline**: Click **Run Pipeline**
7. **View Results**: See step-by-step outputs
8. **Save Preset**: (Optional) Save for reuse

### Example Pipelines

**Developmental Pass**:
1. Chapter Structure → 2. Pacing Analysis → 3. Plot Hole Finder

**Line Edit Pass**:
1. Show vs Telling → 2. Sensory Depth → 3. Word Choice

### Tips

- **Refine mode** is great for iterative improvements
- **Parallel mode** gives multiple perspectives at once
- Save **common workflows** as presets
- Start with **fewer steps** and add as needed

---

## 9. Settings Tab


![settings 2](https://github.com/user-attachments/assets/25d43fc0-f229-43b3-9451-b0226ddbcef8)
![settings 1](https://github.com/user-attachments/assets/aa5262b8-c9eb-468c-9fbe-6ca0feb72413)
![settings 3](https://github.com/user-attachments/assets/59a7f3cb-87f1-49ce-ab8d-3f790e3ea508)

### Overview

The Settings tab configures API connections, display preferences, and AI writing rules.

### Key Features

#### API Configuration

[IMAGE: API Settings Panel - Shows provider dropdown and model selection]

| Setting | Options |
|---------|---------|
| **Provider** | OpenRouter (default), Anthropic Direct, OpenAI Direct, Google Direct, LM Studio |
| **Model** | Claude 3.5 Sonnet, GPT-4o, Gemini Pro, etc. |
| **API Key** | Encrypted storage with optional plaintext |
| **Test Key** | Verify API connection |

#### Display Settings

[IMAGE: Display Settings - Shows theme and scale options]

| Setting | Options |
|---------|---------|
| **Theme** | 14 themes: Default Dark, Soft Beach, Pink Sand, Ice Cold, Purple Haze, etc. |
| **UI Scale** | 0.5x to 2.0x |
| **Header Scale** | 0.5x to 2.0x |

#### Generation Settings

| Setting | Range | Default |
|---------|-------|---------|
| **Max Tokens** | 256-16,000 | 4,096 |
| **Token Boost** | For single runs | - |

#### Writing Preferences

[IMAGE: Writing Preferences - Shows POV and AI Avoidance Rules]

| Setting | Options |
|---------|---------|
| **POV** | First Person, Third Person, Mixed |
| **Inner Monologue** | Italics for internal thoughts |

#### AI Avoidance Rules

[IMAGE: AI Avoidance Rules Panel - Shows toggleable rules]

| Rule | Description |
|------|-------------|
| **Punctuation Group** | Avoid em-dashes, semicolons, colons |
| **No Triplet Framing** | Avoid three adjectives/verbs in a row |
| **No Golden Sunset** | Avoid over-description of sunsets/nature |
| **No Inspirational Pivot** | Avoid forced positive endings |
| **No AI Bookending** | Avoid repetitive intros/outros |
| **Vary Sentence Structure** | Mix sentence lengths |
| **Filter Words** | Avoid weak filter words |
| **Snappy Dialogue** | Short, punchy exchanges |
| **Specific Over Generic** | Precise details vs vague |
| **Custom List** | Add your own banned words |

#### Additional Settings

| Setting | Description |
|---------|-------------|
| **TTS Voice** | 8 text-to-speech voice options |
| **Chat Context** | What data to include in Chat |
| **LangSearch API** | Web search functionality |

### How to Use

1. **Configure API**:
   - Select provider
   - Enter API key
   - Click **Test** to verify
2. **Set Display**:
   - Choose theme from dropdown
   - Adjust UI/Header scale
3. **Configure Generation**:
   - Set max tokens based on needs
4. **Set Writing Preferences**:
   - Choose POV
   - Toggle AI Avoidance rules
5. **Save Settings**: Click **Save** (note: some settings auto-save)

### Tips

- **Lower max tokens** = faster responses; **higher** = more thorough
- Use **AI Avoidance rules** to combat generic AI prose
- **Test your API key** before important writing sessions
- **Theme choice** affects eye strain - test different options

---

## 10. Timeline Tab


### Overview

The Timeline tab manages chronological events across your story world with visual and list views.

### Key Features

#### Event Types

| Type | Icon | Use Case |
|------|------|----------|
| Event | ◉ | General story events |
| Birth | ♀ | Character births |
| Death | † | Character deaths |
| War | ⚔ | Battles and conflicts |
| Magic | ✦ | Magical events |

#### Event Fields

| Field | Description |
|-------|-------------|
| **Year** | When the event occurs |
| **Title** | Event name |
| **Description** | What happened |
| **Type** | Event category |

#### Views

- **List View** - Chronological table of all events
- **Visual View** - Timeline graphic with event markers

### How to Use

1. **Add Event**: Click **+ Add Event**
2. **Fill Details**: Enter year, title, description, type
3. **Reorder**: Events auto-sort chronologically
4. **Edit**: Click any event to modify
5. **Delete**: Use trash icon to remove
6. **Switch View**: Toggle between List and Visual

### Tips

- Use **negative years** for "before" timeline events
- Link events to **characters** in descriptions
- Reference timeline in **prompts** for historical context

---

## 11. Analysis Tab


### Overview

The Analysis tab provides quantitative text analysis including word counts, sentence metrics, and common word frequency.

### Key Features

#### Basic Metrics

| Metric | Description |
|--------|-------------|
| **Word Count** | Total words in selection/chapter |
| **Sentence Count** | Total sentences |
| **Avg Words/Sentence** | Sentence length indicator |

#### Style Metrics

| Metric | Description |
|--------|-------------|
| **Passive Voice** | Count and percentage |
| **Adverbs** | Count of -ly words and others |
| **Dialogue %** | Percentage of dialogue |

#### Common Word Frequency


- Top 50 most frequently used words
- Useful for spotting overused terms

### How to Use

1. **Select Text**: Choose chapter(s) or paste text
2. **View Metrics**: Automatic calculation displays
3. **Check Passive/Adverbs**: Review flagged instances
4. **Analyze Frequency**: Identify overused words
5. **Export Report**: (If available) Download analysis

### Tips

- **Aim for 15-20 words/sentence** average
- **Minimize passive voice** for tighter prose
- **Replace frequency outliers** with synonyms
- Use with **Prompts tab** for AI-powered suggestions

---

## 12. Find Tab


### Overview

The Find tab provides powerful search and replace across all chapters with regex and case sensitivity support.

### Key Features

#### Search Options

| Option | Description |
|--------|-------------|
| **Case Sensitive** | Match exact case |
| **Regex** | Use regular expressions |
| **Whole Word** | Match complete words only |

#### Find & Replace

| Function | Description |
|----------|-------------|
| **Find Next** | Jump to next occurrence |
| **Replace** | Replace current instance |
| **Replace All** | Replace all occurrences |
| **Count** | Show total matches |

#### Scope

- **Current Chapter** - Search active document
- **All Chapters** - Search entire project

### How to Use

1. **Enter Search Term**: Type in Find field
2. **Set Options**: Toggle case/regex/whole word
3. **Choose Scope**: Current or all chapters
4. **Find**: Click Find Next or see Count
5. **Replace**: Enter replacement text
6. **Execute**: Replace single or all

### Example Regex Patterns

| Pattern | Matches |
|---------|---------|
| `\w+ed$` | Past tense words |
| `""[^""]*""` | Dialogue blocks |
| `\b\w{1,3}\b` | Short words (1-3 letters) |

### Tips

- Use **regex** for complex patterns like dialogue
- **Preview count** before replacing all
- **Case-sensitive** prevents accidental changes

---

## 13. Stats Tab


### Overview

The Stats tab displays comprehensive project statistics including word counts and section breakdowns.

### Key Features

#### Word Count Breakdown

| Section | Description |
|---------|-------------|
| **Series** | Total from series bible |
| **Book** | Total from book bible |
| **Chapters** | Total from all chapters |
| **Total** | Combined word count |

#### Project Counts

| Metric | Description |
|--------|-------------|
| **Chapters** | Number of chapters |
| **Characters** | Character count |
| **Locations** | Location count |
| **Timeline Events** | Event count |

#### Export

- **Export to Markdown** - Download all project stats

### How to Use

1. **View Stats**: Stats display automatically
2. **Check Breakdown**: See word distribution
3. **Review Counts**: Verify project scope
4. **Export**: Download statistics

### Tips

- Use for **tracking progress** toward word count goals
- Export for **query letters** or submissions

---

## 14. Branches Tab


### Overview

The Branches tab implements delta versioning, allowing you to create "what-if" story branches and merge them with AI assistance.

### Key Features

#### Delta Versioning

| Feature | Description |
|---------|-------------|
| **Create Branch** | Snapshot current version as new branch |
| **Branch List** | View all story branches |
| **Switch Branches** | Work on different versions |

#### Branch Management

| Action | Description |
|--------|-------------|
| **Create** | New branch from current state |
| **View** | See branch differences |
| **Merge** | Combine branches with AI help |
| **Delete** | Remove unwanted branches |

#### AI Merge Assistant

- AI helps resolve conflicts between branches
- Suggests how to combine different story directions

### How to Use

1. **Create Branch**: Click **+ New Branch**, name it
2. **Make Changes**: Edit in the branch
3. **View Differences**: Compare branches
4. **Merge**: Select branches to combine, use AI to resolve
5. **Switch**: Jump between branches

### Use Cases

- **What-if Scenarios**: Try different plot directions
- **Draft Versions**: Keep multiple revision approaches
- **Collaborator Branches**: Test different co-author inputs

### Tips

- Name branches **descriptively** ("romance-ending", "darker-tone")
- Use for **major plot decisions** before committing
- **Merge carefully** - review AI suggestions

---

## Quick Reference

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| Ctrl+S | Save |
| Ctrl+F | Find |
| Ctrl+H | Find & Replace |

### Data Source Selection

When using Prompts, select context from:
- Series Bible
- Book Bible
- Characters
- Relationships
- Timeline
- Chapters

### Pipeline Modes

- **Refine**: Sequential (output → input)
- **Parallel**: Simultaneous independent analysis

## Compare Tab

The Compare tab lets you stack multiple AI analyses of the same chapter and find where they agree or contradict each other. Instead of reading through two long outputs and mentally cross-referencing them, the app does it for you — surfacing conflicts, shared findings, and every original issue verbatim.

### When to use it

Run Compare when you've done more than one type of analysis on the same chapter. For example:

- A **Chapter Review** (broad editorial read) + a **Show/Tell Audit**
- A **Pacing Map** + a **Line Edit** pass
- Two runs of the same prompt with different models

Each prompt type catches different things. The conflict detector tells you where they disagree — and where they agree is your highest-confidence edit list.

---

### Step 1 — Add your first analysis

Run any prompt in the **Prompts** tab as normal. Once output appears, look for the **+ Compare** button in the output toolbar (right side, next to Visual Report).

Click it. The button flashes **✓ Added** to confirm. The slot is saved automatically with the prompt's label and category.

> **Tip:** Run two different prompt categories on the same chapter text before switching to Compare — e.g. select "Chapter Review" and run, then select "Show/Tell Audit" and run again.

---

### Step 2 — Add your second analysis

Run a second prompt on the same chapter (different category works best). Click **+ Compare** again.

You can add up to as many slots as you want. Each is stored independently with its label, category, timestamp, and full output text.

---

### Step 3 — Paste external analyses (optional)

If you've run analyses in Claude.ai, another session, or a different tool, you can add those too without re-running them.

In the **Compare tab**, click **+ Paste Analysis** in the sidebar footer. A modal opens with:

- **Label** (required) — e.g. "Claude.ai Editorial Read"
- **Category** (optional) — e.g. "Editorial", "Pacing"
- **Text area** — paste the full output

Click **+ Add to Compare**. It appears as a slot in the sidebar alongside your in-app analyses.

---

### Step 4 — Review your slots

Switch to the **Compare** tab. The left sidebar lists all your slots as numbered cards showing:

- The label and category
- The timestamp
- A two-line preview of the output

Click any label to rename it inline. Click **✕** to remove a slot. **Clear All** removes everything.

The **⇄ Run Conflict Analysis** and **Copy Prompt** buttons in the footer enable once you have 2 or more slots.

---

### Step 5 — Run the conflict analysis

You have two options:

#### Option A — Run via API (automatic)

Click **⇄ Run Conflict Analysis**. The app sends all your slot contents to the AI with a structured prompt that:

- Forbids summarising or merging any issue
- Requires every flag to be reproduced verbatim
- Detects contradictions between analyses (conflicts)
- Detects independently-flagged problems (consensus)
- Returns JSON with three arrays: `conflicts`, `consensus`, `allIssues`

Results appear in the main panel.

#### Option B — Copy Prompt (for Claude.ai or another chat)

Click **Copy Prompt**. The full comparison prompt — including all your slot contents — is copied to your clipboard. Paste it into Claude.ai or any other chat interface and send. When you get the response, copy it and paste it back using **+ Paste Analysis** if you want to run a Visual Report on it.

> **Note:** Copy Prompt respects the mode dropdown — set it to "Conflicts only" or "Consensus only" before copying if you want a narrower focus.

---

### Step 6 — Read the results

Results are displayed in three sections:

#### ⚡ Conflicts
Passages where two analyses give contradictory advice. Each conflict card shows:
- The element or passage in question
- Side-by-side panels with the exact wording from each analysis
- A one-line explanation of the contradiction
- Severity tag (Critical / Important / Minor)

Conflicts don't mean one analysis is wrong — they mean you have an editorial decision to make. Read both stances and decide which direction serves your chapter.

#### ✓ Consensus
Issues independently flagged by two or more analyses. These are your **highest-confidence edits** — when an editorial read and a show/tell audit both flag the same passage without knowing what the other said, that's a strong signal.

#### 📋 All Issues
Every flag from every analysis, reproduced in full, grouped by source. Nothing is condensed or paraphrased. Use this section as your working edit checklist.

---

### Step 7 — Change the view mode

Use the **mode dropdown** above the results to filter:

- **Full** — all three sections
- **Conflicts only** — just the contradictions
- **Consensus only** — just the shared findings

This also controls what gets sent if you use **Copy Prompt**.

---

### Step 8 — Generate a Visual Report

Click **⬡ Visual Report** in the Compare main panel to convert your conflict analysis into a formatted HTML document. See the [Visual Report](#visual-report) section below for full details.

---

---

## Visual Report

Visual Report converts any AI analysis output into a structured, printable HTML document — with sidebar navigation, section cards, and severity-coded tags.

### Opening Visual Report

**From the Prompts tab:** After any prompt run, click **⬡ Visual Report** in the output toolbar.

**From the Compare tab:** After running conflict analysis, click **⬡ Visual Report** in the main panel.

A modal opens with a preview of the source text and two mode options.

---

### Mode toggle

#### ⚡ Local Parser (default)
Parses the markdown structure of the output instantly, with no API call. It identifies headers, bullet points, severity keywords, and quoted passages to build the document structure.

Use this for: quick reads, well-structured outputs, saving API credits.

#### ✦ AI Enhanced
Sends the output to the API for smarter extraction. The AI identifies section boundaries, assigns severity levels, and structures irregular or dense outputs that the local parser may not handle cleanly.

Use this for: long outputs, outputs with unusual formatting, Compare conflict JSON.

> **Tip:** Start with Local mode. If the report looks garbled or sections are missing, switch to AI Enhanced and regenerate.

---

### Generating the report

1. Select your mode (Local or AI Enhanced)
2. The source text is pre-filled from the output — edit in the text area if needed
3. Click **Generate Visual Report**
4. The report opens in a new browser tab

The report includes:
- A hero header with the chapter title and analysis type
- Sidebar navigation with scroll-spy
- Collapsible section cards
- Severity tags on each issue (Critical / Important / Minor)
- All original text preserved — nothing summarised

---

### Saving or sharing

The report is a standalone HTML file. To save it:

- **Right-click → Save Page As** in your browser
- **Print → Save as PDF** for a portable version
- Copy the URL from the new tab if you want to return to it in the same session

---

### Using Visual Report with Compare

After running conflict analysis in the Compare tab, the Visual Report pre-loads the conflict JSON and generates a structured report with three sections: Conflicts, Consensus, and All Issues — each with source labels, severity tags, and verbatim issue text.

This is the most useful output format for sharing analysis results with a co-author, editor, or beta reader who doesn't use the app.


---

*Tutorial version 1.0 | The Novelist's Atelier*

