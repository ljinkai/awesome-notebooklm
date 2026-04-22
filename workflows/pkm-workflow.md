# PKM Workflow — Personal Knowledge Management

A workflow for integrating NotebookLM into a long-term personal knowledge management system. NotebookLM excels at synthesis and questioning; tools like Obsidian and Notion excel at storage, linking, and retrieval. This workflow connects them.

---

## Overview

**Best for:** Researchers, students, writers, and knowledge workers who read heavily and want to build cumulative understanding over time
**Tools:** NotebookLM + Obsidian (or Notion)
**Core principle:** NotebookLM is your thinking partner; your PKM tool is your memory.

---

## The Core Loop

```
Read / Consume → Import to NotebookLM → Extract insights → Store in PKM → Connect to existing notes
```

The loop closes when you can retrieve a past insight when you need it — not just when you first processed it.

---

## Phase 1: Intake

### Step 1.1 — Decide what deserves deep processing
Not everything you read deserves a NotebookLM notebook. Apply a filter:
- Is this a primary source I will cite or build on?
- Is this a book or paper I want to understand deeply, not just skim?
- Am I comparing 3+ sources on the same topic?

If yes to any: NotebookLM. If no: bookmark or Readwise highlight.

### Step 1.2 — Create a focused notebook per topic or project
One notebook per project or research question. Avoid the temptation to create a single massive "everything" notebook — the model's quality drops when sources are unrelated.

Good notebook structures:
- "Book: [Title] + 3 related papers"
- "Research: [Topic] — [Month Year]"
- "Project: [Name] — Background Research"

### Step 1.3 — Add sources systematically
Upload sources in batches. For books: if it is not a PDF, paste key chapters as a Note (up to the note size limit). For web articles, paste the URL directly.

---

## Phase 2: Active Processing with NotebookLM

### Step 2.1 — Generate atomic insights
Use the Zettelkasten Note Generator from the [Reading Prompts](../prompts/reading.md):

> From the uploaded source, generate 10 atomic notes in Zettelkasten format. Each note should have a title that is a full sentence stating a claim or insight, be self-contained in 2–4 sentences, cite the specific location in the source, and include 3–5 tags for linking.

### Step 2.2 — Surface connections to prior knowledge
After generating insights:

> I have been building a knowledge base on [your domain]. Based on the ideas in the uploaded sources, what connections might these ideas have with concepts in [related area 1], [related area 2]? Where do these ideas challenge or extend conventional thinking in those areas?

This is how NotebookLM helps you think, not just summarize.

### Step 2.3 — Generate questions to live with
> Based on the uploaded sources, what are the 5 most interesting open questions these ideas raise? Not questions the text answers, but questions the text makes you want to investigate further.

Add these questions to your PKM as open threads.

### Step 2.4 — Create a source summary note
For each source processed in NotebookLM, generate a summary you will store in your PKM:

> Write a permanent note summary for [source title] suitable for a Zettelkasten system. Include: (1) the core argument in 2–3 sentences, (2) 3–5 key insights as bullet points with page/section references, (3) 3 questions this raises, (4) potential connections to: [topics in your PKM]. Maximum 400 words.

---

## Phase 3: Capture to PKM

### Step 3.1 — Export from NotebookLM

Currently, NotebookLM does not have a native export function. Use these methods:

**For individual responses:** Copy the text from the chat panel. NotebookLM formats output in markdown, which pastes cleanly into Obsidian.

**For Notes:** Open each Note and copy the content. Notes are the most reliable export surface.

**For saving an entire session:** Before closing a productive session, run:
> Summarize the key insights, decisions, and open questions from this entire conversation in a format I can save as a reference note.

Then copy and paste to your PKM.

### Step 3.2 — Structure in Obsidian (or Notion)

**Obsidian structure for NotebookLM outputs:**

```
/Sources
  /[Author Last Name - Year - Title].md  ← permanent note per source
/Projects
  /[Project Name]/
    synthesis.md
    open-questions.md
    source-list.md
/Atomic Notes
  /[Note title as sentence].md
```

**For each permanent note, include:**
- Source metadata (author, year, type)
- Core argument (3 sentences max)
- Key insights (bullets with references)
- Open questions
- Links to related notes
- NotebookLM notebook name (so you can return to it)

### Step 3.3 — Create links deliberately
When adding a new note to Obsidian, ask:
- What existing notes does this connect to?
- What existing notes does this challenge or update?

Add bidirectional links explicitly. Do not rely on automatic tag matching alone.

---

## Phase 4: Retrieval and Reuse

### Step 4.1 — Return to NotebookLM for synthesis projects
When starting a writing project or making a decision, go back to NotebookLM and create a synthesis notebook:
- Add the 5–10 most relevant sources from your history
- Add your saved synthesis notes as a source (paste text into a Note)
- Run synthesis prompts to find connections across your accumulated knowledge

### Step 4.2 — Use Obsidian for daily connection
Daily or weekly, review your "open questions" list in Obsidian. When you encounter new information that addresses an open question:
- Add the new source to the relevant NotebookLM notebook
- Run: "Based on the new source I just added, how does it change the picture on [open question]?"

### Step 4.3 — Quarterly review
Every quarter, review your NotebookLM notebooks:
- Archive or delete notebooks for completed projects
- Identify recurring themes across notebooks — these are often your most important intellectual interests
- Create a "synthesis notebook" for recurring themes, pulling the best sources from multiple notebooks

---

## Integrating with Specific PKM Tools

- **Obsidian:** See [Obsidian Integration Guide](../integrations/obsidian.md) for detailed setup
- **Notion:** See [Notion Integration Guide](../integrations/notion.md)
- **Readwise:** See [Readwise Integration Guide](../integrations/readwise.md) for routing highlights into NotebookLM

---

## Common Mistakes

**Mistake 1: Treating NotebookLM as storage.**
NotebookLM is ephemeral — sessions end, UI may change, notebooks may be lost. Always export anything you want to keep into your PKM.

**Mistake 2: Creating one massive notebook.**
A "general reading" notebook with 50 unrelated sources produces poor synthesis. Keep notebooks focused.

**Mistake 3: Never returning to past insights.**
The value of a PKM compounds only if you retrieve and connect old notes. Schedule time to browse your Obsidian graph or Notion database.

**Mistake 4: Capturing without connecting.**
Adding a note to Obsidian without linking it to related notes is like shelving a book with no index. The link is the value.
