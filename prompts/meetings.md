# Meeting & Work Prompts

Prompts for processing meeting transcripts, project documents, and work-related materials. Upload meeting recordings (as transcripts), project briefs, Slack exports, or email threads as sources.

---

## Meeting Processing

### Action Item Extractor
**Use case:** After a meeting, quickly extract every commitment made with owner and deadline.
**Prompt:**
> From the uploaded meeting transcript, extract all action items. For each action item, identify: (1) what needs to be done (specific and concrete), (2) who is responsible (the person who committed to it), (3) any deadline mentioned, and (4) the context — what decision or discussion triggered this action. Format as a table. If ownership or deadline is ambiguous, flag it rather than guessing.

---

### Decision Log Generator
**Use case:** Creating a record of decisions made for future reference or onboarding.
**Prompt:**
> From the uploaded meeting transcript or project documents, extract every decision that was made. For each decision: (1) state what was decided, (2) who made or ratified the decision, (3) what alternatives were considered (if mentioned), (4) what reasoning was given for the chosen direction, and (5) any conditions or caveats attached to the decision. Format as a numbered decision log with date if available.

---

### Meeting Summary for Stakeholders
**Use case:** Writing a summary that non-attendees can read in 2 minutes.
**Prompt:**
> Based on the uploaded meeting transcript, write an executive summary for stakeholders who were not present. Include: (1) the purpose of the meeting in one sentence, (2) 3–5 key decisions made, (3) major action items with owners, (4) any blockers or risks raised that leadership should know about, and (5) the next meeting or milestone. Keep the total summary under 300 words. Write in plain language, not meeting jargon.

---

### Follow-up Email Drafter
**Use case:** Sending a recap immediately after a meeting.
**Prompt:**
> Based on the uploaded meeting transcript, draft a follow-up email. The email should: (1) open with a 2-sentence summary of what was accomplished, (2) list action items with owners and deadlines in a clean format, (3) note any open questions that still need resolution, and (4) close with the date/time of the next check-in if mentioned. Use a professional but conversational tone. Subject line should be specific, not "Meeting Recap."

---

### Blocker and Risk Identifier
**Use case:** Surfacing problems raised in a meeting that might be lost in a long transcript.
**Prompt:**
> From the uploaded meeting transcript or project documents, identify all blockers, risks, and concerns that were raised. For each item: (1) describe the blocker or risk specifically, (2) who raised it, (3) how urgent or severe it appears to be based on the discussion, (4) any proposed solutions or mitigation steps mentioned, and (5) whether it was resolved in the meeting or remains open. Flag items that appear unresolved and unowned.

---

## Project & Work Documents

### Project Brief Analyzer
**Use case:** Quickly understanding a new project brief or request for proposal.
**Prompt:**
> Based on the uploaded project brief or requirements document, answer: (1) What is the core problem being solved? (2) Who is the primary audience or beneficiary? (3) What are the explicit success criteria or deliverables? (4) What constraints are specified (timeline, budget, technical, organizational)? (5) What is unclear or underspecified that would need clarification before starting work? (6) What are the riskiest assumptions in this brief?

---

### Requirements Gap Finder
**Use case:** Before starting a project, finding what has not been specified.
**Prompt:**
> Review the uploaded requirements document and identify: (1) requirements that are vague or lack measurable criteria, (2) requirements that appear to conflict with each other, (3) scenarios or edge cases that are not addressed, (4) dependencies or prerequisites that are implied but not explicitly stated, and (5) questions I should ask the stakeholder before proceeding. For each gap, suggest a specific clarifying question.

---

### Stakeholder Communication Drafter
**Use case:** Writing updates that match what different audiences actually need to know.
**Prompt:**
> Based on the uploaded project documents and status information, draft a stakeholder update for [audience: executives / technical team / clients]. Tailor it to what that audience cares about: executives need decisions and risk; technical teams need clarity on scope and blockers; clients need progress and next steps. Keep it under 200 words. Do not include technical details that are irrelevant to this audience.

---

### Retrospective Facilitator
**Use case:** Generating structured retrospective prompts from project documents.
**Prompt:**
> Based on the uploaded project documents, post-mortems, or meeting transcripts, help me prepare for a team retrospective. Generate: (1) 3 specific questions about what went well, grounded in events mentioned in the documents, (2) 3 specific questions about what could be improved, based on blockers or issues raised, (3) 2 questions about team dynamics or communication, and (4) 1 forward-looking question about what the team should commit to doing differently. Make the questions specific to this project, not generic retrospective templates.
