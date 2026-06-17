# RAY MEMORY AND DECISIONS — Cross-Project Continuity Log

**Status:** ACTIVE  
**Owner:** Rayhan Pramudya  
**Scope:** Global preferences, reusable lessons, owner decisions, and cross-project memory

---

## 1. Purpose

This file preserves durable knowledge about how Ray works across projects.

It exists to:

- prevent repeated onboarding from zero;
- preserve active owner decisions;
- record reusable lessons from completed work;
- distinguish global preferences from project-specific facts;
- prevent old chats from overriding newer evidence;
- provide future projects with concise, auditable context;
- reduce duplicated discussion and accidental roadmap drift.

This is not a dumping ground for every project detail. Only information with clear cross-project value belongs here.

---

## 2. Memory Classification

Every candidate memory must be classified before it is added.

### 2.1 Global owner preference

A recurring Ray preference that should guide multiple projects.

Examples:

- ask before materially assuming;
- do not fabricate evidence;
- prefer local-first systems where practical;
- finish usable work instead of stopping at advice;
- save reusable structures to `TEMPLATES/`;
- preserve existing architecture and formatting;
- report limitations honestly.

### 2.2 Global workflow rule

A repeatable operating rule that improves project execution.

Examples:

- inspect before editing;
- define acceptance criteria before implementation;
- use entry and exit gates;
- separate research, proposal, decision, implementation, and validation;
- keep one bounded implementation unit active at a time;
- document owner overrides separately from technical PASS.

### 2.3 Cross-project lesson

A lesson proven useful in more than one context.

Examples:

- a current-state handoff reduces repeated questions;
- decision logs prevent old instructions from silently returning;
- independent validation is stronger than self-declared success;
- reusable templates reduce inconsistency and wasted effort.

### 2.4 Project-specific knowledge

Keep this inside the originating project unless Ray explicitly promotes it to global memory.

Examples:

- a product's exact technology stack;
- project-only model IDs;
- implementation commits;
- project-specific API contracts;
- unique UI decisions;
- temporary blockers;
- a single project's phase status.

### 2.5 Temporary context

Do not store globally unless it becomes durable.

Examples:

- current debugging output;
- temporary file paths;
- one-time credentials;
- transient pricing;
- short-lived errors;
- unverified ideas.

---

## 3. Decision Authority

Ray is the final decision authority.

A decision becomes globally active only when one of these is true:

1. Ray explicitly states it should apply across projects.
2. Ray approves a proposed global update.
3. The decision is already documented as ACTIVE in this repository.

Questions, brainstorming, curiosity, experiments, and suggestions do not automatically become decisions.

---

## 4. Decision Record Format

Use this format for every global decision:

```text
## RAY-D-XXX — Decision title

Date:
Decision:
Reason:
Scope:
Replaces:
Impact:
Evidence or source:
Status:
```

Valid status values:

- `ACTIVE`
- `SUPERSEDED`
- `REJECTED`
- `DEFERRED`
- `EXPERIMENTAL`

When a decision changes, do not erase the old record. Mark it `SUPERSEDED` and reference the replacement.

---

## 5. Active Global Decisions

## RAY-D-001 — Ask before materially assuming

**Date:** 2026-06-18  
**Decision:** When missing information could materially affect scope, architecture, data, security, cost, irreversible work, or final quality, ask Ray instead of inventing an answer or silently choosing a direction.  
**Reason:** Prevents incorrect work based on hidden assumptions.  
**Scope:** All projects and agents.  
**Replaces:** Silent material assumptions.  
**Impact:** Agents must distinguish known facts from assumptions and only ask when clarification is genuinely necessary.  
**Evidence or source:** Explicit Ray instruction.  
**Status:** ACTIVE

---

## RAY-D-002 — Evidence must support completion claims

**Date:** 2026-06-18  
**Decision:** Do not claim PASS, complete, secure, production-ready, approved, or locked without relevant evidence.  
**Reason:** A plausible result is not the same as a verified result.  
**Scope:** All projects, documents, tests, releases, and reports.  
**Replaces:** Self-declared success without proof.  
**Impact:** Completion reports must include actual validation, skipped checks, and limitations.  
**Evidence or source:** Proven CLIPPERS PREMIUM workflow and explicit Ray preference.  
**Status:** ACTIVE

---

## RAY-D-003 — Useful structures belong in `TEMPLATES/`

**Date:** 2026-06-18  
**Decision:** Reusable workflows, prompts, checklists, reports, handoffs, gates, and configuration structures should be preserved as clean templates.  
**Reason:** Future projects should not rebuild mature structures from zero.  
**Scope:** All projects.  
**Replaces:** Recreating useful structures repeatedly from chat history.  
**Impact:** Project closeout should include a template promotion review.  
**Evidence or source:** Explicit Ray instruction.  
**Status:** ACTIVE

---

## RAY-D-004 — Repository state outranks old chat memory

**Date:** 2026-06-18  
**Decision:** Current repository files, active decisions, verified commits, tests, and current-state handoffs outrank older chat messages when they conflict.  
**Reason:** Repositories provide more durable and auditable evidence than conversational history.  
**Scope:** All repository-backed projects.  
**Replaces:** Treating old chat text as the strongest source of truth.  
**Impact:** New agents must inspect the repository before relying on remembered context.  
**Evidence or source:** Proven CLIPPERS PREMIUM source-of-truth workflow.  
**Status:** ACTIVE

---

## RAY-D-005 — Owner override is not technical PASS

**Date:** 2026-06-18  
**Decision:** Ray may accept risk or continue work despite an unresolved limitation, but the override must not be represented as technical validation.  
**Reason:** Preserves honest project status while respecting owner authority.  
**Scope:** All projects.  
**Replaces:** Conflating risk acceptance with successful testing.  
**Impact:** Owner overrides must document accepted risk, unresolved evidence, and next authorized action.  
**Evidence or source:** CLIPPERS PREMIUM owner-override practice.  
**Status:** ACTIVE

---

## RAY-D-006 — Build usable outcomes, not theory alone

**Date:** 2026-06-18  
**Decision:** When tools, files, access, and safety allow execution, complete the actual deliverable rather than stopping at instructions or examples.  
**Reason:** Ray learns through real implementation and expects practical results.  
**Scope:** Administrative, creative, software, documentation, and automation work.  
**Replaces:** Tutorial-only responses when execution is available.  
**Impact:** Agents should perform the work and report the result.  
**Evidence or source:** Repeated Ray instruction across projects.  
**Status:** ACTIVE

---

## RAY-D-007 — Preserve project-specific boundaries

**Date:** 2026-06-18  
**Decision:** Global memory must not silently import product-specific stacks, models, providers, constraints, or phase decisions into unrelated projects.  
**Reason:** A proven workflow can be global even when its technical implementation is not.  
**Scope:** Profile repository and all connected projects.  
**Replaces:** Blindly copying CLIPPERS-specific technical rules into every project.  
**Impact:** Promote principles and structures globally; keep product implementation details local.  
**Evidence or source:** Current profile-repository design.  
**Status:** ACTIVE

---

## RAY-D-008 — Verified-source discipline for formal documents

**Date:** 2026-06-18  
**Decision:** Formal documents, structured records, and official submissions must use an explicit source hierarchy. Identity data, identifiers, dates, references, signatories, and other authoritative fields must come from verified inputs; missing values must be flagged or represented by visible placeholders rather than invented.  
**Reason:** Polished formatting cannot compensate for incorrect official data, and silent guessing creates avoidable administrative risk.  
**Scope:** Administrative documents, reports, forms, spreadsheets, certificates, official correspondence, and document automation across projects.  
**Replaces:** Guessing missing official values, copying from lower-authority examples, or treating plausible matches as verified facts.  
**Impact:** Document agents must classify inputs, reconcile records one-to-one, preserve leading zeroes and exact spelling, expose material ambiguity, and report source checks in completion evidence.  
**Evidence or source:** Repeated KERJAAN document workflows and explicit Ray instructions to use the correct source, preserve formats, and never invent personnel data.  
**Status:** ACTIVE

---

## 6. Reusable Cross-Project Lessons

### L-001 — Current-state handoffs preserve continuity

A concise active handoff should record:

- product or project identity;
- source-of-truth order;
- authoritative documents;
- verified implementation baseline;
- current task or phase;
- known limitations;
- next authorized action;
- recovery baseline.

### L-002 — Entry and exit gates reduce accidental drift

Before work starts, verify prerequisites. Before completion is claimed, verify acceptance criteria, evidence, documentation, limitations, and repository state.

### L-003 — Research must not silently become roadmap

Research, curiosity, comparisons, and feature exploration remain non-binding until Ray explicitly approves a decision.

### L-004 — One bounded implementation unit is easier to validate

Large work should be divided into small complete units with explicit scope and evidence.

### L-005 — Independent validation is stronger than self-approval

The same agent that implemented a major change should not be the sole authority declaring the phase approved and locked.

### L-006 — Recovery must be designed before risky action

Approved commits, tags, backups, immutable source files, and non-destructive branches provide safer recovery than improvised rollback after failure.

### L-007 — Known limitations belong in the official state

Limitations should be visible, classified, routed, and separated from completed behavior.

### L-008 — Clear agent mandates improve complex projects

Separate orchestration, architecture, implementation, quality, UI/UX, research, and provider/security responsibilities when the project is large enough to benefit.

### L-009 — Generated documents require both data and visual validation

A document that saves successfully may still be wrong. Verify authoritative data against designated sources and inspect rendered pages for clipping, table overflow, broken pagination, headers, footers, and signature placement before calling the deliverable ready.

---

## 7. Promotion Protocol

At a milestone or project closeout, ask:

1. Did Ray express a new recurring preference?
2. Did the project discover a reusable workflow?
3. Did a decision supersede an older global rule?
4. Did a useful document or prompt structure emerge?
5. Is the lesson truly cross-project, or only local?
6. Is there enough evidence to preserve it?

Then choose one action:

- keep it project-local;
- propose a global memory entry;
- add or update a global decision;
- save a generic structure to `TEMPLATES/`;
- mark an older decision `SUPERSEDED`;
- discard it as temporary noise.

Material global changes should be explicit and auditable.

---

## 8. Update Rules

When updating this file:

- preserve historical decisions;
- use dates in `YYYY-MM-DD` format;
- state exact scope;
- identify what is replaced;
- avoid duplicate rules with slightly different wording;
- do not include secrets or private credentials;
- do not store volatile facts without a verification requirement;
- link important decisions to evidence when available;
- update templates when a structural lesson becomes reusable.

---

## 9. New Project Reading Rule

A new project should read this file before substantial planning or implementation.

The project must not assume every global preference is a technical requirement. It must combine this global context with its own repository, users, constraints, architecture, and approved scope.

---

## 10. Final Memory Principle

> Preserve what will save future work. Keep temporary noise local. Never turn an assumption into permanent memory.
