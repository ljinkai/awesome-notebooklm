# Awesome NotebookLM [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) ![GitHub Stars](https://img.shields.io/github/stars/yourusername/awesome-notebooklm?style=social)

> A curated list of prompts, workflows, tools, and resources for NotebookLM power users.

[NotebookLM](https://notebooklm.google.com) is Google's AI-powered research assistant that lets you upload documents, PDFs, YouTube videos, and websites as sources, then ask questions, generate summaries, and create content grounded in your own material.

This list focuses on practical, tested techniques — prompts that actually work, workflows that save real time, and tools that extend NotebookLM's capabilities.

---

## Contents

- [Prompts](#prompts)
- [Workflows](#workflows)
- [Integrations](#integrations)
- [Tools](#tools)
- [Resources](#resources)
- [Contributing](#contributing)

---

## Prompts

Organized by use case. Every prompt has been tested against real NotebookLM sources.

- [Research Prompts](prompts/research.md) — Literature analysis, gap finding, argument extraction, counter-argument generation
- [Writing Prompts](prompts/writing.md) — Drafting, outlining, restructuring, tone refinement
- [Reading Prompts](prompts/reading.md) — Book synthesis, concept mapping, Socratic questioning
- [Meeting Prompts](prompts/meetings.md) — Agenda extraction, action item capture, decision logging

---

## Workflows

Step-by-step guides for common use cases.

- [Research Workflow](workflows/research-workflow.md) — Systematic literature review and synthesis using NotebookLM
- [Writing Workflow](workflows/writing-workflow.md) — From raw sources to polished draft
- [PKM Workflow](workflows/pkm-workflow.md) — Personal knowledge management with NotebookLM + Obsidian/Notion

---

## Integrations

How to connect NotebookLM with other tools in your stack.

- [Obsidian](integrations/obsidian.md) — Bidirectional workflow between NotebookLM and your Obsidian vault
- [Notion](integrations/notion.md) — Syncing NotebookLM outputs into Notion databases
- [Readwise](integrations/readwise.md) — Feeding Readwise highlights into NotebookLM as sources

---

## Tools

- [Tools & Extensions](tools/README.md) — Browser extensions, companion apps, and automation tools

---

## Resources

- [Official Docs & Community](resources/README.md) — Google's documentation, tutorials, Reddit, Discord

---

## Tips & Tricks

### Source Management
- **Keep notebooks focused.** NotebookLM works best with 10–20 tightly related sources rather than 50 loosely connected ones.
- **Name your sources.** Rename uploaded files to descriptive titles — NotebookLM uses filenames when citing, so `smith-2023-attention-mechanisms.pdf` beats `paper.pdf`.
- **Use YouTube transcripts.** Paste YouTube URLs directly; NotebookLM ingests the full transcript, making video content searchable.

### Prompting
- **Ask for citations.** End prompts with "cite the specific sources that support each claim." NotebookLM will include inline source references.
- **Constrain the scope.** "Based only on the uploaded papers, not general knowledge..." prevents the model from hallucinating outside your sources.
- **Iterate with follow-ups.** NotebookLM maintains context within a session — use short follow-up prompts to drill deeper rather than rewriting long prompts.

### Audio Overviews
- **Guide the conversation.** Before generating an Audio Overview, add a note specifying the angle: "Focus on the practical implications for engineers, not the theoretical background."
- **Regenerate with constraints.** If the first Audio Overview is too broad, add a note like "The audience already understands X, skip basics" and regenerate.

---

## Tools

**Browser Extensions**

**[NotebookLM Hub](https://chromewebstore.google.com/detail/notebooklm-hub/opeemcbkbfbfdcbacbigjekphiclcegb?utm_source=github&utm_medium=awesome-list&utm_campaign=organic)** — Chrome extension for one-click web import, source management, and link extraction. Lets you add any webpage to a NotebookLM notebook without copy-pasting URLs.

---

## Contributing

Contributions welcome. Please read the guidelines below before submitting a PR.

**What belongs here:**
- Prompts you have personally tested in NotebookLM (not hypothetical)
- Workflows with clear steps and expected outcomes
- Tools that are actively maintained
- Resources from credible sources

**What does not belong:**
- Generic ChatGPT prompts rebranded for NotebookLM
- Tools that are abandoned or broken
- Affiliate links or paid promotions

**How to contribute:**
1. Fork this repository
2. Add your contribution in the appropriate file
3. Test any prompts against actual NotebookLM sources
4. Submit a pull request with a brief description of what you added and why

**Format for prompts:**
```markdown
### Prompt Name
**Use case:** One sentence describing when to use this.
**Prompt:**
> Full prompt text here
```

---

## License

[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) — public domain. Use freely.
