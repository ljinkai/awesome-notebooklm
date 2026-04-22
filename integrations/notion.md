# Notion + NotebookLM Integration Guide

A workflow for routing NotebookLM outputs into Notion databases for team-friendly knowledge management.

---

## Why Notion Works Well with NotebookLM

Notion's database structure makes it excellent for:
- Tracking which sources have been processed
- Organizing synthesis by project or topic
- Sharing research outputs with a team
- Building a searchable library of insights over time

NotebookLM handles the hard thinking; Notion handles the organization and sharing.

---

## Recommended Notion Database Structure

### Database 1: Source Library

Create a database called "Source Library" with these properties:

| Property | Type | Purpose |
|----------|------|---------|
| Title | Title | Source name (Author - Year - Title) |
| Type | Select | Paper, Book, Article, Video, Report |
| Topic | Multi-select | Research areas |
| NotebookLM Notebook | Text | Which notebook it lives in |
| Status | Select | Unread, Processing, Processed, Archived |
| Core Argument | Text | 2–3 sentence summary |
| Key Insights | Text | Bulleted list |
| Date Processed | Date | When you ran it through NotebookLM |
| URL/DOI | URL | Link to source |

### Database 2: Atomic Insights

A database for single-idea notes extracted from NotebookLM.

| Property | Type | Purpose |
|----------|------|---------|
| Title | Title | The insight as a full sentence |
| Source | Relation | Link to Source Library |
| Topic | Multi-select | Tags |
| Content | Text | 2–4 sentence elaboration |
| Confidence | Select | High / Medium / Speculative |
| Created | Date | Auto |

### Database 3: Research Projects

| Property | Type | Purpose |
|----------|------|---------|
| Project | Title | Project name |
| Research Question | Text | The question driving the project |
| Status | Select | Active, On Hold, Complete |
| Thesis | Text | Current working thesis |
| NotebookLM Notebooks | Text | List of relevant notebooks |
| Sources | Relation | Links to Source Library |
| Open Questions | Text | What still needs answering |

---

## Workflow 1: Processing a Source into Notion

### Step 1 — Generate structured output in NotebookLM

> Create a structured source entry for [Source Title] that I can add to a Notion database. Format the output with these labeled sections:
>
> **TITLE:** [Author - Year - Title]
> **TYPE:** [Paper / Book / Article / Video / Report]
> **CORE ARGUMENT:** [2–3 sentences]
> **KEY INSIGHTS:**
> - [Insight 1]
> - [Insight 2]
> - [Insight 3]
> - [Insight 4]
> - [Insight 5]
> **SURPRISING POINTS:**
> - [Point 1]
> - [Point 2]
> **OPEN QUESTIONS:**
> - [Question 1]
> - [Question 2]
> - [Question 3]
> **SUGGESTED TOPICS:** [comma-separated tags]

### Step 2 — Create a new entry in Source Library
Open your Notion Source Library database. Create a new entry. Copy each labeled section into the corresponding property.

### Step 3 — Extract atomic insights
For each Key Insight that is worth preserving as a standalone note:
1. Create a new entry in Atomic Insights database
2. Set the title to the insight phrased as a full sentence claim
3. Add a brief elaboration
4. Link back to the source in Source Library

---

## Workflow 2: Tracking a Research Project in Notion

### Step 1 — Create a project entry
Add a new entry to your Research Projects database. Fill in:
- Research question
- Initial thesis (even if tentative)
- List of NotebookLM notebooks you are using

### Step 2 — Log each research session
At the end of each NotebookLM session:

Run this prompt before closing:
> Write a brief research log entry for today's session on [topic]. Include: (1) what I investigated today, (2) the most important finding, (3) how it changes or confirms my current thesis, (4) what to investigate in the next session. Maximum 200 words.

Create a new sub-page in your project entry titled "Session Log — [Date]" and paste the output.

### Step 3 — Update the thesis field regularly
After each session, update the "Thesis" field in your project entry to reflect your current best thinking. Seeing how the thesis evolves over time is valuable.

---

## Workflow 3: Building a Team Research Hub

For teams using both NotebookLM and Notion:

### Shared source library
All team members add processed sources to the same Notion Source Library database. This prevents duplicate processing and surfaces what has already been analyzed.

Convention: whoever processes a source in NotebookLM adds the entry to Notion immediately.

### Shared synthesis notes
Create a "Synthesis Notes" database where team members post NotebookLM-generated synthesis on shared research questions. Properties:
- Topic
- Author (team member)
- Date
- NotebookLM Notebook Name
- Content

### Async collaboration on a research question
1. One team member creates a Research Project entry with a clear research question
2. Each team member processes relevant sources in their own NotebookLM notebooks
3. All synthesis is logged to the shared Synthesis Notes database
4. Weekly: one person creates a "Synthesis Notebook" in NotebookLM with all team members' synthesis notes as sources, then runs: "Based on these notes from multiple researchers, what is the current state of our understanding on [question]? Where do we agree, where do we disagree, and what is still unresolved?"

---

## Limitations

- Notion's API can theoretically be used for automated import, but this requires custom development (Zapier or Make workflows)
- NotebookLM does not push to Notion natively — all transfers are manual copy-paste
- Notion's full-text search does not search inside relation-linked databases by default; use Dataview-style linked database views to improve discoverability
