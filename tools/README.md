# Tools & Extensions for NotebookLM

A curated list of tools that extend, complement, or integrate with NotebookLM. Organized by category.

---

## Browser Extensions

**[NotebookLM Hub](https://chromewebstore.google.com/detail/notebooklm-hub/opeemcbkbfbfdcbacbigjekphiclcegb?utm_source=github&utm_medium=awesome-list&utm_campaign=organic)** — Chrome extension that adds a persistent sidebar to NotebookLM with three tabs:

- **Sources** — Add any webpage or YouTube link to the current notebook in one click, with live ingestion progress. Also extracts all links from the current page as a batch import list.
- **Prompts** — 20+ built-in templates (Academic, Business, Content, General) plus unlimited custom prompts created inline with `{{variable}}` support. Clicking "Use" injects the prompt directly into NotebookLM's query box. Pin any prompt to keep it permanently at the top of the list.
- **Settings** — Language preference and notebook management.

Free. No account required.

---

## Note-Taking & PKM

**[Obsidian](https://obsidian.md)** — Local-first markdown knowledge base with bidirectional linking and graph view. Pairs with NotebookLM via manual export workflow. See [Obsidian Integration Guide](../integrations/obsidian.md).

**[Notion](https://notion.so)** — All-in-one workspace with database views, great for team research. See [Notion Integration Guide](../integrations/notion.md).

**[Logseq](https://logseq.com)** — Open-source outliner-style PKM with bidirectional links, similar to Obsidian but outline-based. Supports the same manual export workflow.

**[Roam Research](https://roamresearch.com)** — Networked thought tool. Can receive NotebookLM exports via paste; Roam's daily notes structure works well for session logs.

---

## Read-Later & Highlights

**[Readwise Reader](https://readwise.io/read)** — Read-later app that captures highlights from articles, PDFs, newsletters, and ebooks. Syncs highlights to Obsidian/Notion. See [Readwise Integration Guide](../integrations/readwise.md).

**[Instapaper](https://www.instapaper.com)** — Clean read-later app with highlighting. Export highlights as text for NotebookLM sources.

**[Pocket](https://getpocket.com)** — Mozilla's read-later service. Articles can be exported and added to NotebookLM notebooks.

---

## PDF Management

**[Zotero](https://www.zotero.org)** — Free, open-source reference manager. Store and annotate PDFs, then export them for upload to NotebookLM. The Zotero browser extension captures academic papers in one click.

**[Paperpile](https://paperpile.com)** — Reference manager for academic papers, integrates with Google Docs. PDFs can be exported directly to your drive for NotebookLM upload.

**[PDF Expert](https://pdfexpert.com)** (macOS/iOS) — PDF reader with annotation. Annotated PDFs upload to NotebookLM; annotations are included in the ingested text.

---

## Writing & Editing

**[Hemingway Editor](https://hemingwayapp.com)** — Paste NotebookLM-drafted text here for readability scoring and clarity suggestions. Good for final polish.

**[Grammarly](https://grammarly.com)** — Grammar, style, and clarity checker. Works as a browser extension on any editing surface.

**[LanguageTool](https://languagetool.org)** — Open-source grammar and style checker, available as a browser extension. Good alternative to Grammarly for privacy-conscious users.

---

## Transcription & Audio

**[Otter.ai](https://otter.ai)** — Auto-transcribes meetings, interviews, and lectures. Export the transcript as text and upload to NotebookLM as a source.

**[Whisper](https://github.com/openai/whisper)** (open source) — OpenAI's speech-to-text model. Run locally to transcribe audio files for NotebookLM import.

**[MacWhisper](https://goodsnooze.gumroad.com/l/macwhisper)** (macOS) — Desktop app wrapping Whisper for easy local transcription. Drag audio in, get transcript out, paste to NotebookLM.

---

## Research & Search

**[Consensus](https://consensus.app)** — AI-powered search for academic papers. Find relevant papers on a topic, then upload them to NotebookLM for deep synthesis.

**[Elicit](https://elicit.com)** — AI research assistant for literature search. Use Elicit to identify key papers, then download and upload to NotebookLM.

**[Connected Papers](https://www.connectedpapers.com)** — Visual tool for exploring related academic papers. Use to find connected literature before building a NotebookLM notebook.

**[Perplexity](https://perplexity.ai)** — AI search with citations. Use for initial research and source discovery; then upload the source documents to NotebookLM for deeper analysis.

---

## Automation

**[Zapier](https://zapier.com)** — No-code automation. While native NotebookLM integration is not yet available, Zapier can automate upstream steps: save articles to read-later, export highlights, organize PDFs.

**[Make (formerly Integromat)](https://make.com)** — More powerful no-code automation. Similar use cases to Zapier for building workflows around NotebookLM.

---

## Submitting a Tool

To add a tool to this list, open a pull request with:
- Tool name (linked to official site)
- One-sentence description of what it does
- Specific explanation of how it integrates with or complements NotebookLM
- Category it belongs in

Tools must be actively maintained and free from critical security issues. Affiliate links are not accepted.
