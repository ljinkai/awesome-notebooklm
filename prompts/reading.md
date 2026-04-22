# Reading Prompts

Prompts for deep reading, book synthesis, and concept mapping. Upload a book, paper, or long-form article as a source and use these prompts to extract maximum value.

These prompts are inspired by active reading traditions — Mortimer Adler's *How to Read a Book*, the Feynman technique, and Socratic questioning — adapted for NotebookLM's grounded AI.

---

## The 6-Prompt Active Reading Framework

A structured sequence for deep engagement with any non-fiction book or long document.

### Step 1 — Structural Read
**Use case:** Understanding the architecture of the book before engaging with arguments.
**Prompt:**
> Based on the uploaded book/document, answer: (1) What is the author trying to accomplish? What problem are they solving or question are they answering? (2) What is the structure of the argument — how is the book organized and why? (3) What does the author assume the reader already knows? (4) What kind of book is this — theoretical, practical, narrative, reference? Give me a one-paragraph overview of what this book is and is not.

---

### Step 2 — Core Argument Extraction
**Use case:** Identifying what the book actually claims, in the most precise terms.
**Prompt:**
> What is the single most important argument or claim in the uploaded book? State it in one sentence. Then: (1) what are the 3–5 sub-claims that support this central argument? (2) what evidence or reasoning does the author use for each sub-claim? (3) what does the author say would have to be false for their central argument to fail?

---

### Step 3 — Concept Inventory
**Use case:** Building a working vocabulary before digging into details.
**Prompt:**
> From the uploaded text, identify the 8–12 key concepts or terms that are central to the author's argument. For each concept: (1) provide the author's definition or the clearest statement of how they use the term, (2) explain why this concept is load-bearing for the argument, (3) identify any tension or ambiguity in how the term is used across the book. Where concepts are used inconsistently, flag it.

---

### Step 4 — Socratic Challenge
**Use case:** Testing the argument by asking what the author would say to hard questions.
**Prompt:**
> Generate 6 Socratic questions that probe the weakest points in the argument presented in the uploaded book. For each question: (1) state the question clearly, (2) explain what assumption or claim it challenges, (3) provide the best answer the author gives (or implies) in the text, and (4) note whether you find that answer satisfying or whether it leaves the question open. I want to stress-test the argument, not just summarize it.

---

### Step 5 — Personal Application
**Use case:** Connecting the book's ideas to your own context.
**Prompt:**
> Based on the ideas in the uploaded book, help me think through how they apply to [your specific context or problem]. For each major idea that is relevant: (1) summarize the idea in plain language, (2) explain how it might apply to my situation, (3) identify what the author would likely say I should do differently, and (4) note any limitations of applying this idea outside the context the author wrote for.

---

### Step 6 — Integration & Synthesis
**Use case:** Connecting this book to other sources in your notebook.
**Prompt:**
> I have uploaded multiple sources to this notebook. Compare the main book to the other sources: (1) where do the sources agree or build on each other? (2) where do they contradict each other? (3) which source makes the strongest case for its position? (4) what synthesis is possible — is there a view that incorporates the valid points of multiple sources? Present this as a synthesis, not just a list of comparisons.

---

## Deep Reading Prompts

### Hidden Premises Finder
**Use case:** Uncovering what the author takes for granted.
**Prompt:**
> What premises does the author assume but never explicitly state or defend in the uploaded text? List the 5 most important hidden premises. For each: (1) state the premise, (2) explain where in the argument it appears as an assumption, (3) assess whether the argument would hold if this premise were false, and (4) note whether any other source in this notebook challenges this premise.

---

### Author's Worldview Mapper
**Use case:** Understanding the deeper framework behind the argument.
**Prompt:**
> Based on the uploaded text, what worldview or philosophical commitments underlie the author's argument? Consider: (1) what do they value most, and how does this shape what they study or recommend? (2) what do they seem to believe about human nature, society, or [relevant domain]? (3) what would someone with a very different worldview say about this book? (4) does the author acknowledge these commitments anywhere, or are they invisible in the text?

---

### Zettelkasten Note Generator
**Use case:** Extracting atomic, reusable insights in a format suitable for a personal knowledge base.
**Prompt:**
> From the uploaded source, generate 10 atomic notes in Zettelkasten format. Each note should: (1) have a title that is a full sentence stating a claim or insight, (2) be self-contained in 2–4 sentences, (3) cite the specific location in the source, (4) include 3–5 tags for linking. Focus on the most surprising, non-obvious, or useful insights rather than summaries of obvious points.

---

### Dialogue Simulation
**Use case:** Deepening understanding by having the author "respond" to questions.
**Prompt:**
> I want to have a dialogue with the author of the uploaded text. Based strictly on what they write in the text, answer the following questions as the author would answer them: [your questions]. After each answer, note the specific passage in the text that supports this response. If the text does not contain a clear answer, say so rather than speculating.

---

### Reading Group Discussion Questions
**Use case:** Preparing for a book club, seminar, or team discussion.
**Prompt:**
> Based on the uploaded book, generate 8 discussion questions that would provoke genuine disagreement and reflection in a reading group. The questions should: (1) not have obvious yes/no answers, (2) connect the book's ideas to broader issues, (3) include at least 2 questions that challenge the author's assumptions, (4) include at least 1 question about methodology or evidence quality, and (5) be specific enough to point back to particular passages in the text.
