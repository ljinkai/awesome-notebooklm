# Writing Workflow

A workflow for using NotebookLM to move from raw sources to a polished written piece. Works for articles, essays, reports, and long-form content.

---

## Overview

**Time investment:** 2–6 hours depending on length and complexity
**Best for:** Articles, essays, research reports, white papers, thought leadership pieces
**Output:** Full draft grounded in your sources, ready for final editing

---

## Phase 1: Source Preparation

### Step 1.1 — Decide what you are writing before collecting sources
Write a single sentence: "I am writing a [format] that argues [thesis] for [audience]."

Example: "I am writing a 2,000-word article that argues remote work reduces mid-career burnout for knowledge workers."

This sentence determines which sources belong in your notebook.

### Step 1.2 — Assemble relevant sources
Upload sources that provide:
- Evidence for your central claim
- Context and background
- Counter-arguments (important — acknowledging them makes writing stronger)
- Examples and case studies
- Relevant statistics or data

For an article, 5–15 sources is usually right. Too many sources creates noise; too few limits what you can say with confidence.

### Step 1.3 — Add your own rough notes as a source
If you have prior thinking on this topic — notes, an outline, a previous draft — add it as a Note source. NotebookLM will treat your own thinking as source material alongside the research.

---

## Phase 2: Orientation and Angle

### Step 2.1 — Understand what your sources actually say
Before drafting anything, run this prompt:

> I am writing about [topic]. Based on the uploaded sources, what are the strongest arguments and most compelling evidence? What are the key counter-arguments? What are the most surprising or counterintuitive findings?

### Step 2.2 — Identify your strongest evidence
> For the claim that [your thesis], which uploaded sources provide the strongest evidence? Rank them and explain why.

This tells you which sources to lean on most heavily.

### Step 2.3 — Check your thesis against the evidence
> Does the evidence in the uploaded sources support the following thesis: [your thesis]? Where is the evidence strong? Where is it weak or absent? What qualifications or nuances does the evidence suggest I should add?

Be honest here. If the evidence does not support your thesis cleanly, adjust the thesis before drafting.

---

## Phase 3: Structure

### Step 3.1 — Generate a detailed outline
Use the [Argument Outline Builder](../prompts/writing.md) prompt.

Review the outline critically:
- Does each section advance the argument, or is it just background?
- Is there a logical sequence, or do sections feel randomly ordered?
- Is the counter-argument section positioned where it is most effective?

### Step 3.2 — Identify the best opening hook
> Based on the uploaded sources, what is the most surprising, counterintuitive, or emotionally resonant fact or story I could open with? Give me 3 options for an opening hook, ranging from data-driven to narrative.

Choose or adapt the hook before drafting the introduction.

### Step 3.3 — Map evidence to sections
For each section in your outline:
> I am writing the section on [topic]. Which uploaded sources are most relevant to this section? What specific evidence, quotes, or findings should I draw on?

This pre-work makes drafting fast.

---

## Phase 4: Drafting

Draft section by section. Do not try to draft the full piece in one prompt — you will get a generic summary, not a real draft.

### Step 4.1 — Draft the body sections first
Skip the introduction. Draft the meat of the piece first, then write the introduction once you know what you are actually arguing.

For each body section:
> Draft the section on [topic] for my article about [subject]. The section should: (1) make the main point that [your point], (2) use evidence from the uploaded sources to support it, (3) be approximately [X] words, (4) end with a transition toward [next section topic]. Use a [tone: journalistic / academic / conversational] voice.

### Step 4.2 — Handle the counter-argument section
> Draft a section that presents and responds to the strongest objection to my argument. The objection is [state it]. Use the uploaded sources to find the best version of this objection, then draft a response that takes it seriously rather than dismissing it.

### Step 4.3 — Draft the introduction last
Once all body sections are drafted:
> I have now drafted the full body of my article. Based on the argument as developed in the body, draft an introduction that: (1) opens with the hook I selected ([your hook]), (2) establishes the stakes in 2–3 sentences, (3) previews the argument without giving away all the evidence, and (4) ends with a clear thesis statement.

### Step 4.4 — Draft the conclusion
Use the [Conclusion Drafter](../prompts/writing.md) prompt.

---

## Phase 5: Revision

### Step 5.1 — Add the draft as a source and audit it
Paste your assembled draft into a new Note. Then:

> I have added my draft as a Note. Review it and identify: (1) the three weakest paragraphs where the argument is least convincing, (2) any claims that are not grounded in the uploaded sources, (3) any section that is too long relative to its importance, (4) any section that feels rushed and should be expanded.

### Step 5.2 — Strengthen specific weak sections
For each weak section identified:
> Rewrite the following paragraph to make it more persuasive, using evidence from the uploaded sources: [paste paragraph]. Keep the same core point but make the evidence clearer and the logic tighter.

### Step 5.3 — Consistency and flow check
> Does the draft read as a coherent piece or does it feel like disconnected sections? Identify the two weakest transitions and suggest improved connective language. Also note any tone inconsistencies.

### Step 5.4 — Final evidence check
> For each factual claim in the draft, confirm it is supported by an uploaded source. Flag any claim that is not, or where the source only partially supports the claim as I have stated it.

---

## Phase 6: Polish

At this stage, move the draft out of NotebookLM into your writing tool (Google Docs, Word, etc.) for final polish. NotebookLM is excellent for grounded drafting but human judgment is better for:
- Voice and rhythm
- Sentence-level editing
- Final headline and subheading work
- Formatting decisions

Use NotebookLM for one final pass:
> I am about to finalize this piece. What is the single most important thing I should change before publishing? What would a critical reader find most questionable?
