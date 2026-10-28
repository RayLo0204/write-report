# Report Writing Style

A reusable Codex skill for clear reports and knowledge-base documentation across subjects.

The skill favors concise numbered sections, concrete explanations, useful tables, focused Mermaid diagrams, and step-by-step workflows. It follows the requested outline and language rather than enforcing a fixed report template.

## Files

| File | Purpose |
|---|---|
| [SKILL.md](SKILL.md) | Report-writing instructions |
| [agents/openai.yaml](agents/openai.yaml) | Skill display name and default prompt |
| [references/writing-style.md](references/writing-style.md) | Writing patterns distilled from a user-authored report |

## Install

Clone this repository into your personal Codex skills directory:

```bash
git clone https://github.com/RayLo0204/write-report.git "$HOME/.codex/skills/write-report"
```

If `CODEX_HOME` is customized, use its `skills/write-report` directory instead. If that destination already contains a skill, keep a backup and review differences before replacing it.

## Use

Ask Codex to use `$write-report`, then provide the subject, available material, intended audience, and any preferred outline or output language.

For example:

> Use $write-report to organize these notes into a concise report. Explain the roles first, separate preparation from repeated operation, and place each diagram next to its explanation.

## Scope

This repository contains the reusable skill and writing guidance. It does not include the original report, private source pages, credentials, program source, test logs, or demo media.
