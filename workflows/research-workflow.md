# Research Workflow

A systematic workflow for using NotebookLM to conduct literature reviews, synthesize research, and produce evidence-based writing. This workflow has been tested on academic literature reviews, competitive analyses, and policy research.

---

## Overview

**Time investment:** 2–8 hours depending on scope
**Best for:** Literature reviews, research papers, evidence-based reports, due diligence
**Output:** Structured synthesis, argument outline, first draft sections

---

## Phase 1: Source Curation (Before NotebookLM)

The most important phase. NotebookLM cannot find sources for you — that is your job.

### Step 1.1 — Define the research question
Write your research question in one sentence before collecting any sources. A clear question determines which sources belong in your notebook and which are distractions.

Example: "What does the evidence say about the effectiveness of spaced repetition for long-term retention in adult learners?"

### Step 1.2 — Collect sources with purpose
For each source, ask before adding: "Does this directly address my research question?" Sources that are tangentially related dilute your notebook.

Target 10–25 sources for a focused review. More is not better.

Supported source types:
- PDFs (papers, reports, books)
- Google Docs
- Web URLs (paste directly; NotebookLM scrapes the content)
- YouTube URLs (NotebookLM uses the transcript)
- Copied text (paste into a Note source)

### Step 1.3 — Name your sources descriptively
Before uploading, rename files to something like:
- `roediger-2011-test-enhanced-learning.pdf`
- `kornell-2009-spacing-effects-review.pdf`

NotebookLM uses filenames in citations. Descriptive names make citations usable.

### Step 1.4 — Create a new dedicated notebook
Do not reuse notebooks across research projects. One research question = one notebook. This keeps citations clean and prevents cross-contamination.

---

## Phase 2: Orientation (30–45 minutes)

Get a map of what you have before diving deep.

### Step 2.1 — Source inventory
Run this prompt immediately after uploading all sources:

> Give me a brief overview of each uploaded source: author(s), year, central claim, and methodology in 2–3 sentences each. Format as a list.

Review the output. Are any sources clearly off-topic? Remove them now.

### Step 2.2 — Identify the key debates
> Based on all the uploaded sources, what are the 3–5 main debates or unresolved questions in this literature? For each debate, list which sources take which position.

This tells you the intellectual landscape before you start detailed analysis.

### Step 2.3 — Flag gaps in your source collection
> Based on the uploaded sources, what important perspectives, methodologies, or time periods appear to be missing from my source collection? What types of sources would strengthen this review?

This is your checklist for finding additional sources if needed.

---

## Phase 3: Deep Analysis (1–3 hours)

Systematic extraction from each source and across sources.

### Step 3.1 — Extract key arguments per source
Use the [Core Argument Extractor](../prompts/research.md) prompt on each cluster of related sources.

Save the output as a Note titled "Argument Map."

### Step 3.2 — Map agreements and contradictions
> Which findings or claims are supported by multiple independent sources? Which are contested? List each position and the sources that support it.

Save as a Note titled "Consensus and Debate."

### Step 3.3 — Assess evidence quality
> For the three most important claims in this literature, evaluate how strong the evidence is: What type of studies support it? Has it been replicated? What are the main methodological limitations?

### Step 3.4 — Find the gaps
Use the [Literature Gap Finder](../prompts/research.md) prompt.

Save the output as a Note titled "Research Gaps."

---

## Phase 4: Synthesis (1–2 hours)

Turning analysis into a coherent story.

### Step 4.1 — Draft your thesis
Before asking NotebookLM to help structure your argument, write your own thesis statement in a Note. Example:

> *My thesis: "Current evidence strongly supports spaced repetition for vocabulary acquisition but the evidence for conceptual learning is weaker and more context-dependent."*

### Step 4.2 — Generate a thematic outline
> Based on the uploaded sources and the thesis in my notes, create a thematic outline for a literature review. Organize by themes, not by source. For each theme, list the sources that contribute to it and the main point the theme will make.

### Step 4.3 — Draft each section
For each section of the outline:

> I am writing the section on [theme]. Based on the sources in this notebook, draft this section. It should make the argument that [your point], use 3–5 sources as evidence, acknowledge the strongest counter-evidence, and be approximately [X] words. Use inline citations.

### Step 4.4 — Synthesize across sections
After drafting all sections:

> Based on what I have drafted so far, does the overall argument hang together? Are there contradictions between sections? Is there a logical gap anywhere? What is missing?

---

## Phase 5: Verification (30 minutes)

Before treating your draft as reliable.

### Step 5.1 — Citation check
> Review the draft I have uploaded. For each claim that cites a source, confirm that the source actually supports the claim as stated. Flag any claim where the citation is weak or where I have overstated what the source says.

### Step 5.2 — Completeness check
> Based on the uploaded sources, what important evidence or counter-arguments should be in this review but currently is not? What am I missing that a reviewer would notice?

### Step 5.3 — Manually verify key citations
For your most important claims, open the original source and verify the citation yourself. NotebookLM is very good but not infallible.

---

## Tips for Large Research Projects

- **Use multiple notebooks for phases.** One notebook for raw literature, another for notes and synthesis.
- **Date your notes.** Add a date to each Note so you can track how your thinking evolved.
- **Export regularly.** Copy important Notes and chat outputs to a separate document outside NotebookLM. The platform has evolved — export critical work.
- **Use the Audio Overview as a sanity check.** Generating an Audio Overview from your synthesis notebook is a fast way to catch logical gaps — the conversational format makes structural problems audible.
