# Writing Prompts

Prompts for drafting, outlining, restructuring, and refining written work using NotebookLM sources. These work best when your sources include relevant research, reference material, or examples of the writing style you are targeting.

---

## Outlining & Structure

### Argument Outline Builder
**Use case:** Before drafting, generate a logical structure grounded in your sources.
**Prompt:**
> Based on the uploaded sources, create a detailed outline for an essay/article arguing that [your thesis]. The outline should: (1) include a clear thesis statement, (2) list 3–5 main sections with a one-sentence summary of each section's argument, (3) under each section, list 2–3 specific claims with the source(s) that support them, (4) include a section addressing the strongest counter-argument, and (5) end with a conclusion that connects back to the thesis. Every claim in the outline should be traceable to an uploaded source.

---

### Section-by-Section Scaffolding
**Use case:** Generating a structured scaffold for a long piece before writing full prose.
**Prompt:**
> I am writing a [article/report/chapter] about [topic]. Using the uploaded sources, create a section-by-section scaffold with the following for each section: (1) a working heading, (2) the main point of the section in one sentence, (3) the key evidence or examples from the sources that belong here, (4) how this section connects to the previous and next sections. Make the scaffold detailed enough that I could write each section from it without re-reading the sources.

---

### Counter-Argument Section Drafter
**Use case:** Writing the "steelman" section that addresses objections.
**Prompt:**
> Based on the uploaded sources, draft a section that presents and then responds to the strongest objections to [your argument]. For each objection: (1) state the objection fairly and in its strongest form, (2) cite the source(s) that best represent this position, (3) provide a direct response that acknowledges any valid points while defending the main argument. The tone should be intellectually honest, not dismissive.

---

## Drafting Assistance

### Introduction Drafter
**Use case:** Writing the opening of a piece that establishes stakes and context.
**Prompt:**
> Using the uploaded sources, draft an introduction for a [academic paper/article/report] on [topic]. The introduction should: (1) open with a hook that establishes why this topic matters now, (2) briefly describe the current state of knowledge in 2–3 sentences, (3) identify the specific gap or problem this piece addresses, (4) state the thesis or argument clearly, and (5) preview the structure of what follows. Keep it under 300 words. Cite specific sources where relevant.

---

### Transition Paragraph Generator
**Use case:** Connecting sections that cover different aspects of a topic.
**Prompt:**
> I have just written a section on [topic A] and need to transition to a section on [topic B]. Based on the uploaded sources, write a transition paragraph that: (1) summarizes the key takeaway from the previous section, (2) identifies a genuine connection or tension between topic A and topic B as reflected in the sources, and (3) sets up the question or point that the next section will address.

---

### Evidence Integration Helper
**Use case:** Weaving quotations and citations into prose naturally.
**Prompt:**
> I need to make the following argument: [your argument]. From the uploaded sources, identify the 3–5 most relevant passages or findings that support this argument. For each piece of evidence, provide: (1) the specific quote or finding, (2) the source it comes from, (3) a suggested sentence or two that integrates it into prose without just dropping a quote. Show me how to build a paragraph that uses multiple sources in conversation with each other rather than just listing them.

---

### Conclusion Drafter
**Use case:** Writing a conclusion that does more than summarize.
**Prompt:**
> Based on the uploaded sources and the argument I have been developing, draft a conclusion that: (1) restates the thesis in fresh language (not a copy of the introduction), (2) synthesizes the key evidence rather than merely listing it, (3) addresses the "so what" — why this argument matters beyond the immediate topic, (4) identifies 1–2 genuinely open questions that this work raises but does not answer, and (5) ends with a memorable final sentence. Avoid clichés like "in conclusion" or "as we have seen."

---

## Revision & Refinement

### Clarity Audit
**Use case:** Finding sections that are unclear or overly technical.
**Prompt:**
> Review the following draft: [paste your draft]. For each paragraph, identify: (1) the main point of the paragraph, (2) whether that point is stated clearly in the first or last sentence, (3) any jargon or technical terms that are used without explanation, (4) any paragraphs that are doing more than one thing and should be split. Suggest specific rewrites only for the two or three most problematic passages.

---

### Tone Consistency Checker
**Use case:** Ensuring a piece reads as written by one voice throughout.
**Prompt:**
> I have uploaded my draft as a source. Read through it and identify: (1) sections where the tone shifts unexpectedly (e.g., from formal to casual), (2) passages that use hedging language inconsistently, (3) sections that seem to address a different audience than the rest of the piece. For each issue, quote the specific passage and suggest a revision that brings it in line with the dominant tone of the piece.

---

### Argument Strengthening Pass
**Use case:** After drafting, finding where your argument is weakest.
**Prompt:**
> Based on the uploaded sources, identify the three weakest points in the following argument: [paste argument or draft]. For each weak point: (1) explain why it is vulnerable to objection, (2) identify whether there is evidence in the uploaded sources that could strengthen it, and (3) suggest how to revise that section using the available evidence. If a claim cannot be supported by the uploaded sources, flag it explicitly.

---

### Abstract / Executive Summary Generator
**Use case:** Producing a tight summary after the full piece is written.
**Prompt:**
> Based on the uploaded document and sources, write a [150-word abstract / 250-word executive summary] that covers: (1) the central problem or question, (2) the approach or methodology, (3) the key findings or arguments, and (4) the main implication or recommendation. Use plain language. Do not include citations. The summary should be self-contained and readable by someone who has not seen the full document.
