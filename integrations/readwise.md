# Readwise + NotebookLM Integration Guide

A workflow for routing Readwise highlights into NotebookLM as structured sources — turning your reading highlights into a research-grade knowledge base.

---

## Why This Combination Works

**Readwise** captures highlights from Kindle, Instapaper, Pocket, web articles, Twitter/X, and more. It resurfaces them via spaced repetition and syncs to Obsidian/Notion.

**NotebookLM** takes documents as sources and lets you query, synthesize, and generate content from them.

The combination: Readwise captures what you found interesting *while reading*. NotebookLM helps you *think with* those highlights when you are ready to work.

---

## Method 1: Export Highlights as a Source (Manual)

The simplest approach.

### Step 1 — Export highlights for a book or article from Readwise

In Readwise:
1. Go to your Library
2. Find the book or article
3. Click "Export" → "Markdown" or "Plain Text"
4. Copy the output (or download the file)

### Step 2 — Add to NotebookLM as a source

**Option A: Paste as a Note source**
In your NotebookLM notebook, click "Add source" → "Copied text". Paste the highlights. Title the Note: "[Book Title] — Readwise Highlights"

**Option B: Upload as a file**
If you downloaded the Markdown export, upload the `.md` file directly as a source.

### Step 3 — Use prompts designed for highlights

Highlights are fragmentary by nature. Use these prompts to work with them effectively:

> I have uploaded my Readwise highlights from [Book Title]. These are passages I marked as interesting while reading. Based on these highlights: (1) What themes appear most frequently across my highlights? (2) What argument or story do these highlights collectively tell? (3) Which highlights seem most important in retrospect, and which are more peripheral? (4) What questions do these highlights raise that I should investigate further?

---

## Method 2: Readwise Export to Obsidian → NotebookLM

If you use Readwise Reader or Readwise + Obsidian sync:

### Step 1 — Enable Readwise → Obsidian sync
In Readwise, go to Export → Obsidian. Configure it to sync highlights to your vault in markdown format.

### Step 2 — Curate highlights in Obsidian
After syncing, your highlights appear in your Obsidian vault as formatted markdown notes. Review and edit them — add your own annotations, fix formatting, remove highlights that are no longer interesting.

### Step 3 — Feed curated notes into NotebookLM
When starting a research project, gather the Obsidian notes that are relevant. Paste their content (or export to PDF) and upload to a NotebookLM notebook as sources.

### Step 4 — Synthesize
> I have uploaded my curated highlights and annotations from [list of books/articles]. I am working on the question: [your question]. Based on these sources, what is the most relevant evidence and thinking I have already collected? What connections emerge across these sources that I may not have noticed while reading them individually?

---

## Method 3: Daily Review Feed

Use Readwise's Daily Review (the email or app feature) as a trigger to revisit highlights in NotebookLM.

### Step 1 — When a highlight resurfaces in Daily Review, check if it belongs in an active notebook

Keep a running list of your active NotebookLM notebooks. When Readwise resurfaces a highlight, ask: "Does this belong in one of my current notebooks?"

### Step 2 — If yes: add context to the source Note
In NotebookLM, open the relevant notebook. Find the Note for the source this highlight came from. Add the highlight and your current reaction as an annotation.

### Step 3 — Run a "fresh eyes" prompt
> I added a new highlight to this notebook that I had forgotten about: [paste highlight]. How does this change or enrich the synthesis I have built so far? Does it support, challenge, or add nuance to any of the main claims?

---

## Prompt: Synthesizing Highlights from Multiple Books on One Topic

When you have accumulated highlights from 5+ books on a theme in Readwise, this prompt turns them into structured knowledge:

> I have uploaded highlights from multiple books on [topic]. These highlights were collected over time while reading. Please:
> 1. Identify the 5–7 most important ideas that appear across multiple books
> 2. Note where the books agree or reinforce each other
> 3. Note where the books disagree or offer competing perspectives
> 4. Identify insights that appear in only one book but seem particularly important
> 5. Generate 3 synthesis statements — claims I could make that are supported by multiple books

---

## Readwise Reader Integration

Readwise Reader (the read-later app) allows you to highlight web articles, PDFs, and newsletters in a unified interface.

### Using Reader highlights in NotebookLM

1. In Reader, after finishing an article, use the "Export" function to get your highlights in markdown
2. Add the exported highlights as a source in your relevant NotebookLM notebook
3. Immediately run: "I just finished reading [article title] and added my highlights. How does this source relate to the other sources in this notebook? Does it change the synthesis in any meaningful way?"

### Building a topic-specific highlights notebook

1. In Readwise Reader, tag all articles on a topic consistently (e.g., #spaced-repetition)
2. Monthly, export all highlights with that tag
3. Create a new NotebookLM notebook: "[Topic] — Readwise Monthly [Month Year]"
4. Upload the export
5. Run: "These are my reading highlights from the past month on [topic]. What are the most important ideas, what patterns do I see, and what should I read next?"

---

## Limitations

- Readwise does not natively push to NotebookLM
- Highlight context can be limited — a highlight without surrounding text is sometimes ambiguous; include a few sentences of surrounding context when the passage is not self-contained
- Very large highlight exports (400+ highlights) may exceed NotebookLM's Note size limit; split by book or article
