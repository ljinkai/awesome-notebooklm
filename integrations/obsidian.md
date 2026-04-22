# Obsidian + NotebookLM Integration Guide

A practical guide for building a bidirectional workflow between NotebookLM (for AI-assisted synthesis) and Obsidian (for long-term knowledge storage and linking).

---

## Why These Tools Complement Each Other

| NotebookLM | Obsidian |
|------------|---------|
| AI synthesis over a specific source set | Long-term storage and retrieval |
| Grounded answers with citations | Bidirectional linking and graph view |
| Audio overviews and study guides | Full-text search across all notes |
| Ephemeral (sessions, no version history) | Persistent, local, yours forever |
| Bad at connecting across many unrelated topics | Excellent at surfacing connections over time |

Use NotebookLM for **active research sessions**. Use Obsidian for **building cumulative knowledge**.

---

## Setup: Folder Structure in Obsidian

Create a dedicated folder structure for NotebookLM-derived content:

```
vault/
├── Sources/               ← One note per source processed in NotebookLM
├── Notebooks/             ← One note per NotebookLM notebook (project-level)
├── Atomic Notes/          ← Zettelkasten-style atomic insights
└── Synthesis/             ← Synthesized arguments and drafted sections
```

---

## Workflow 1: Importing a Source into Your Vault

When you finish processing a source in NotebookLM, create a permanent note in Obsidian.

### Step 1 — Generate the permanent note in NotebookLM
Use this prompt:

> Write a permanent note for [Source Title] in Obsidian-compatible markdown. Include:
> - **Metadata block** at top (author, year, type, URL/DOI if available)
> - **Core argument** in 2–3 sentences
> - **Key insights** as a bulleted list (5–8 items, each a complete thought)
> - **Surprising or counterintuitive points** (2–3 items)
> - **Open questions this raises** (3–5 questions)
> - **Potential links** to concepts: [list 3–5 topics from your vault]
> - **NotebookLM notebook:** [notebook name]
>
> Format everything in markdown. Use `[[double brackets]]` for any concept that might be a note in my vault.

### Step 2 — Copy output to Obsidian
Copy the full response. In Obsidian, create a new note in `/Sources/` with the filename format: `LastName Year - Title.md`

Paste. The `[[double brackets]]` in the output will auto-link to existing notes.

### Step 3 — Add connections manually
Review the "Potential links" section and manually visit each linked note to add a backlink. The backlink is the value — it is what makes the knowledge findable years later.

---

## Workflow 2: Saving a NotebookLM Research Session

At the end of a productive NotebookLM session, capture the session's output as a notebook note in Obsidian.

### Step 1 — Generate a session summary
Run this prompt before closing NotebookLM:

> Summarize this session in Obsidian markdown format:
> - **Session date:** [today]
> - **Research question:** [your question]
> - **Key findings:** (bulleted list of the most important things I learned)
> - **Claims I can now make with confidence:** (with source references)
> - **Claims that need more evidence:**
> - **Open questions for next session:**
> - **Sources used:** (list the titles)

### Step 2 — Save to Obsidian
Create a note in `/Notebooks/[Project Name]/` with filename `YYYY-MM-DD Session.md`. Paste the output.

### Step 3 — Update your project note
Each project should have a top-level note in `/Notebooks/` that tracks:
- The research question
- Sessions conducted (with links)
- Current state of confidence in the thesis
- Next steps

---

## Workflow 3: Generating Atomic Notes from NotebookLM

Atomic notes are single-idea notes in Zettelkasten style. They are the building blocks of a connected knowledge base.

### Step 1 — Run the Zettelkasten prompt
Use the [Zettelkasten Note Generator](../prompts/reading.md) prompt on your sources.

### Step 2 — Process each atomic note
For each note in the output:
1. Create a new note in `/Atomic Notes/` with the note title as the filename (it should be a full sentence)
2. Add the content
3. Manually add `[[links]]` to related atomic notes
4. Add tags from the suggested tags

### Step 3 — Build the index
In your top-level project note, add links to the atomic notes that are most central to the project. This creates a mini-MOC (Map of Content) for the project.

---

## Workflow 4: Feeding Obsidian Notes Back into NotebookLM

The workflow is bidirectional. Use your Obsidian notes as sources in NotebookLM.

### When to do this
- You have accumulated many notes on a topic and want to synthesize them
- You want to draft a piece of writing based on your own processed knowledge
- You want to find connections across notes accumulated over months

### Step 1 — Export relevant notes from Obsidian
In Obsidian, use the "Export to PDF" plugin or simply copy the text of relevant notes. Group related notes into a single document if they are short.

### Step 2 — Create a synthesis notebook in NotebookLM
Create a new notebook titled "[Topic] Synthesis — [Date]". Upload your Obsidian exports as sources.

### Step 3 — Run synthesis prompts
> I have uploaded notes I have collected over [time period] on [topic]. Based on these notes, what is the strongest argument I can make about [thesis]? What evidence is strongest? What gaps remain?

This turns your accumulated Obsidian notes into active research material.

---

## Useful Obsidian Plugins for This Workflow

| Plugin | Purpose |
|--------|---------|
| **Dataview** | Query your notes database to find all notes tagged with a topic |
| **Templater** | Create templates for Source notes, Session notes, and Atomic notes |
| **Obsidian Git** | Auto-backup your vault to GitHub |
| **Tag Wrangler** | Manage and rename tags as your taxonomy evolves |
| **QuickAdd** | Fast capture of new notes with predefined templates |

---

## Limitations to Know

- NotebookLM does not accept Obsidian `.md` files directly — paste content as Notes or export to PDF
- There is no sync between the two tools; all transfers are manual
- NotebookLM session history is not persistent — save important outputs before closing
