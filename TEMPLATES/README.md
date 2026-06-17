# TEMPLATES — Ray's Reusable Project Structures

This directory contains clean, reusable structures promoted from proven project workflows.

Use these templates to bootstrap new projects without rebuilding Ray's operating system from zero.

## Rules

- Copy a template into the target project before filling project-specific details.
- Replace every placeholder enclosed in `[BRACKETS]`.
- Do not place secrets, credentials, personal tokens, operational records, or temporary machine data in templates.
- Keep templates generic unless the filename clearly identifies a project-specific variant.
- Preserve sections that protect source-of-truth order, scope, evidence, recovery, and limitations.
- Improve a template only when the new structure has clear reusable value.
- Record meaningful structural changes in the profile repository.

## Available templates

- `PROJECT_BOOTSTRAP_PROMPT.md` — instructs a new project or AI agent to read Ray's profile repository and initialize correctly.
- `CURRENT_STATE_HANDOFF_TEMPLATE.md` — active operational handoff for continuity across chats and agents.
- `DECISION_RECORD_TEMPLATE.md` — auditable project or global decision record.
- `OWNER_OVERRIDE_TEMPLATE.md` — records risk acceptance without misrepresenting technical status.
- `TASK_COMPLETION_REPORT_TEMPLATE.md` — evidence-based completion report.
- `OFFICIAL_DOCUMENT_WORKFLOW_TEMPLATE.md` — source mapping, bounded editing, data reconciliation, rendered-page verification, and completion reporting for formal administrative documents.

## Promotion test

A structure belongs here when it is:

- useful in more than one project;
- generic enough to adapt safely;
- stable enough to avoid constant rewriting;
- clear about required inputs and outputs;
- free from hidden project assumptions and private operational data;
- valuable for reducing repeated onboarding or mistakes.

> Reuse proven structure. Re-verify project facts.
