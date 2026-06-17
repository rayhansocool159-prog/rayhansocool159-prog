# [PROJECT NAME] — Current Project State

> Operational handoff for `[REPOSITORY OR WORKSPACE]`.
>
> **Document status:** ACTIVE HANDOFF  
> **Authority:** Operational summary only  
> **Owner:** Rayhan Pramudya  
> **Last updated:** [YYYY-MM-DD, Asia/Jakarta]

---

## 1. Purpose

This document gives every new project chat, coding agent, and human contributor a compact, auditable view of the current project state.

It exists to:

- preserve continuity across chats and sessions;
- prevent repeated questions and duplicated work;
- distinguish verified repository state from proposed ideas;
- record the latest approved baseline;
- route work correctly;
- prevent accidental changes to locked decisions, commits, tags, scope, or architecture.

This document does not override newer approved project documents.

---

## 2. Source-of-Truth Order

1. Ray's latest explicit instruction.
2. Current repository and actual files.
3. Active decisions and owner overrides.
4. Approved or locked project documents.
5. Verified commits, tags, tests, runtime evidence, and artifacts.
6. This current-state handoff.
7. Historical chat context.

---

## 3. Project Identity

- **Project:** [PROJECT NAME]
- **Purpose:** [PURPOSE]
- **Primary users:** [USERS]
- **Repository:** [OWNER/REPOSITORY]
- **Default branch:** [BRANCH]
- **Platform/environment:** [ENVIRONMENT]
- **Operating principles:** [PRINCIPLES]

---

## 4. Authoritative Documents

Read before changing architecture, scope, workflow, security, providers, or phase order:

- `[PATH]`
- `[PATH]`
- `[PATH]`

If this handoff conflicts with a newer approved document, the newer approved document wins.

---

## 5. Latest Verified Baseline

- **Baseline name:** [BASELINE]
- **Status:** [STATUS]
- **Commit:** [COMMIT]
- **Tag/checkpoint:** [TAG OR CHECKPOINT]
- **Validation summary:** [SUMMARY]
- **Repository state at verification:** [STATE]

---

## 6. Current Active Work

- **Active task/phase:** [TASK OR NONE]
- **Authorized scope:** [SCOPE]
- **Excluded scope:** [EXCLUSIONS]
- **Assigned chat/agent:** [OWNER]
- **Expected deliverable:** [DELIVERABLE]
- **Acceptance criteria:** [CRITERIA]

---

## 7. Verified Implemented State

List only behavior supported by actual repository or runtime evidence:

- [IMPLEMENTED ITEM]
- [IMPLEMENTED ITEM]

---

## 8. Proposed or Not Yet Implemented

Do not describe these as implemented:

- [PROPOSED ITEM]
- [NOT IMPLEMENTED ITEM]

---

## 9. Validation Evidence

| Check | Command or method | Result | Evidence/notes |
|---|---|---|---|
| [CHECK] | `[COMMAND]` | [PASS/FAIL/NOT RUN] | [NOTES] |

Important qualification:

- [WHAT THE EVIDENCE PROVES]
- [WHAT THE EVIDENCE DOES NOT PROVE]

---

## 10. Known Limitations and Risks

| Item | Severity | Impact | Status | Routing/owner |
|---|---|---|---|---|
| [LIMITATION] | [LEVEL] | [IMPACT] | [OPEN/ACCEPTED/DEFERRED] | [OWNER] |

---

## 11. Active Decisions and Overrides

- **Decision:** [DECISION]
- **Owner override:** [NONE OR REFERENCE]
- **Superseded direction:** [REFERENCE]

---

## 12. Recovery Baseline

- **Safe checkpoint:** [COMMIT/TAG/BACKUP]
- **Recovery method:** [METHOD]
- **Source data protection:** [RULE]
- **Destructive operations requiring approval:** [LIST]

---

## 13. Mandatory Workflow Policy

- inspect prerequisites before editing;
- implement only active scope;
- validate claims with evidence;
- preserve unrelated files and user data;
- report tests skipped and limitations;
- do not silently change architecture, dependencies, permissions, or roadmap;
- promote reusable structures to `TEMPLATES/` when appropriate.

---

## 14. Next Authorized Action

`[NEXT_SINGLE_ACTION]`

Why this is next:

[REASON]

---

## 15. Handoff Summary

[ONE-PARAGRAPH CURRENT STATE SUMMARY]
