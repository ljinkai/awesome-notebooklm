# NotebookLM Prompts

A collection of tested prompts organized by use case. All prompts are designed to work with NotebookLM's grounded AI — they assume you have relevant sources uploaded.

## Categories

- [Research](research.md) — Literature analysis, argument extraction, gap finding, synthesis
- [Writing](writing.md) — Drafting, outlining, restructuring, tone editing
- [Reading](reading.md) — Book summaries, concept mapping, Socratic questioning
- [Meetings](meetings.md) — Agenda extraction, action items, decision logging

## How to Use These Prompts

NotebookLM prompts work differently from general LLM prompts because the model is constrained to your uploaded sources. Keep these principles in mind:

**Ground your prompts explicitly.** Phrases like "based on the uploaded sources" or "according to the documents in this notebook" activate NotebookLM's citation behavior and reduce the chance of the model drawing on general training data.

**Use the Note feature for context.** Before running a complex prompt in chat, add a Note with background context (your research question, audience, constraints). The Note becomes part of the context the model uses.

**Chain prompts in sequence.** Start broad (overview), then narrow (specific section), then synthesize (comparison across sources). Each follow-up builds on the previous response.

**Request structured output.** NotebookLM handles markdown well. Ask for numbered lists, tables, or headers to get scannable output.

**Ask for confidence signals.** Adding "and indicate which claims you are less certain about given the available sources" helps surface gaps.

---

## Prompt Formatting Convention

Each prompt in this collection follows this format:

```markdown
### Prompt Name
**Use case:** When and why to use this prompt.
**Prompt:**
> The full prompt text, ready to copy-paste into NotebookLM.

**Tips:** Optional notes on variations or follow-ups.
```

---

## Contributing Prompts

If you have a prompt that consistently produces useful output in NotebookLM, please contribute it. Requirements:
- Tested in NotebookLM (not just theoretically valid)
- Includes a real use case description
- Full prompt text (not a template with unexplained placeholders)
- Fits one of the existing categories, or clearly warrants a new one
