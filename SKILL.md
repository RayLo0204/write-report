---
name: write-report
description: Write, restructure, or review reports in the user's preferred style, using concise numbered sections, clear role explanations, useful tables, diagrams, and step-by-step workflows. Apply to report-writing and knowledge-base documentation requests across subjects, without requiring a POC, source-code audit, or fixed chapter template.
---

# Report Writing Style

Write reports that readers can scan, understand, and explain to someone else. Capture the user's way of arranging information, not the topic or implementation of a previous report.

Read [the writing-style reference](references/writing-style.md) when first applying this skill or when comparing a draft with the user's finished example. It records observed choices from the supplied report; its chapter titles and technical facts are not a universal template.

## Organize around the reader's questions

- Use the agreed title and a short numbered outline. If no outline exists, choose one suited to the subject and proceed with the requested draft; do not introduce a mandatory outline-approval stage.
- Give each section one clear job. Use familiar, concrete headings rather than long descriptions or invented terminology.
- Move from context to the overall picture, then relationships or workflow, relevant details, and results or supporting material. Adapt this order when the subject calls for it.
- Use a table of contents for a long wiki page when supported. A short report does not need one.
- Keep code listings, long command sequences, exhaustive dependencies, raw logs, and implementation walkthroughs in linked supporting material unless they are the requested subject.

## Keep the main text short and concrete

- Start a section with its useful point, usually in one or two sentences. Follow with the table, diagram, or steps that best explain it.
- Explain who does what, through which connection or mechanism, and what happens next. Introduce an unfamiliar term by its purpose before relying on its API name or acronym.
- Use short paragraphs and direct verbs. Cut repeated explanations, conversational history, defensive contrasts, and details that do not change the reader's understanding.
- Use bold for role names, phase labels, step actions, and a few essential distinctions. Do not emphasize entire paragraphs.
- Preserve meaningful qualifications. Shortening text must not turn a limited observation into a general guarantee or erase a distinction needed to interpret a result.
- Follow the requested language. The reference used English report text with Traditional Chinese discussion; that is a precedent, not a rule for every report.

## Choose the right form

| Information | Preferred presentation |
|---|---|
| Versions, settings, conditions, or other comparable facts | Compact table |
| Roles and responsibilities | Brief bullets, often followed by an overview diagram |
| Connections or handoffs | Table naming endpoints, mechanism, and information transferred |
| Ordered work | Numbered steps with a bold action and a short explanation |
| Relationships, states, timing, or branching | A focused diagram next to its explanation |
| Measured outcomes | Result/value table with enough context to interpret the numbers |
| Source files or supporting resources | Index table with item, link/name, and purpose |

Use these forms when they help. Do not add all of them to every report or put ordinary prose into a table merely to match the example.

## Explain a workflow in phases

- Separate work performed once from work repeated during operation when that distinction exists. Use the subject's own labels, such as **Startup** and **Per-frame cycle**, rather than forcing these names onto unrelated topics.
- Write each step as **Action.** followed by the actor, operation, and relevant outcome. Keep lower-level parameters after the conceptual flow unless needed to perform the task.
- Distinguish access, readiness, ownership, and completion when they are different concepts. In other subjects, identify the equivalent distinctions that readers might confuse.
- Describe work that continues independently and where coordination actually occurs. Initialization coordination does not automatically imply that repeated operation is sequential or dependent.
- If an explanation causes repeated questions, simplify its roles or divide the diagram instead of adding more paragraphs to the same confusing view.

## Make each diagram answer one question

- Prefer Mermaid for explanatory architecture, process, state, and sequence diagrams. Use real screenshots or videos for observed output or a demonstration.
- An overview shows the few main components and their responsibilities. A flow diagram shows transitions. A sequence diagram shows who communicates with whom and in what order. Avoid combining every detail into one diagram.
- Place a diagram beside the explanation it supports, usually immediately after the relevant bullets or numbered steps. Use consistent names in both.
- Use restrained colors consistently to distinguish roles, groups, or phases. Keep labels short and descriptive; label arrows with the action or information transferred.
- Separate startup and repeated-operation diagrams when a combined sequence hides the distinction. Show concurrent activity clearly without implying an exact schedule that the source material does not require.
- Keep diagrams readable at the target page width. If a wiki needs an image export, retain the Mermaid source where practical and use a legible render; do not reproduce clipping or tiny text from a reference.

## Match the content and the requested scope

- Check claims against the material available for this assignment: notes, data, documentation, source code, logs, or the user's explanations. Inspect implementation details only when needed for the requested report or consistency check; ordinary report writing is not automatically a code audit.
- Do not invent results or present proposed behavior as completed work. Distinguish what a result measures when similar numbers could be confused.
- Preserve the user's accepted design and interpretation unless evidence reveals a concrete problem. Explain the specific mismatch instead of redesigning the subject to fit a preferred architecture.
- A reference page provides style guidance; it does not make its factual contents correct for a new report. If access is blocked, state what could not be read rather than claiming to have inspected it.
- When asked for a standalone diagram, explanation, or review, provide that output without silently changing the report. Edit the report when requested or authorized by the task.
- Keep supporting media and source links usable. Creating a draft does not authorize publishing or modifying the reference page.

## Finish with a focused review

Check that a reader can identify the roles, connections, main sequence, outcome, and next action relevant to the subject. Resolve disagreement between text, tables, diagrams, and evidence without expanding the report unnecessarily.

Check terminology, numbers, units, links, and diagram readability. State validation limits accurately; a source review is not a fresh experiment, and a Mermaid syntax check is not a visual render check.

Deliver the requested report or revision with a short explanation of material changes. Offer or produce review questions only when requested, rather than adding an unrequested FAQ or audit appendix.
