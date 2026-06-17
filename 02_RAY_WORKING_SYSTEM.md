# RAY WORKING SYSTEM — Cross-Project Operating Contract

**Status:** ACTIVE  
**Owner:** Rayhan Pramudya  
**Scope:** Default operating workflow for new projects, chats, agents, and repositories

---

## 1. Purpose

This file defines how work should be performed for Ray across projects.

It adapts the strongest workflow patterns proven in CLIPPERS PREMIUM into a reusable cross-project operating system.

The objective is to prevent every new project from starting with zero context, repeating old mistakes, or silently changing established decisions.

---

## 2. Mandatory Startup Sequence

Before substantial work begins, perform this sequence:

1. Confirm the correct repository or workspace.
2. Read `01_RAY_IDENTITY.md`.
3. Read this file.
4. Read `03_RAY_MEMORY_AND_DECISIONS.md`.
5. Inspect `TEMPLATES/` for reusable structures.
6. Read the target project's own authoritative documents.
7. Inspect the actual current files and repository state.
8. Identify the active task, scope, constraints, and success criteria.
9. Identify conflicts, missing prerequisites, and risky assumptions.
10. State or internally establish the smallest complete implementation plan.

Do not start broad edits before understanding the repository and its governing documents.

---

## 3. Source-of-Truth Resolution

Use this order unless Ray explicitly defines another order for the project:

1. Ray's latest explicit instruction.
2. Actual repository state and current files.
3. Active project decisions and owner overrides.
4. Approved or locked architecture, scope, security, and workflow documents.
5. Verified commits, tags, tests, runtime evidence, and artifacts.
6. Current-state handoff documents.
7. Historical chats, notes, and proposals.

When two sources conflict:

- identify the exact conflicting sources;
- do not silently choose based on convenience;
- prefer the higher-authority and newer valid source;
- ask Ray when the conflict materially affects scope, architecture, data, cost, security, or irreversible work;
- document the resolution.

---

## 4. Classify Before Acting

Every important statement should be treated as one of:

- **FACT** — directly verified from repository, runtime, official source, or provided evidence;
- **ASSUMPTION** — plausible but not verified;
- **PROPOSAL** — suggested direction, not approved;
- **DECISION** — explicitly approved by Ray or active authoritative record;
- **IMPLEMENTED** — present in code or deliverable;
- **VALIDATED** — implementation supported by relevant evidence;
- **LIMITATION** — known incomplete, degraded, deferred, or unverified area;
- **OWNER OVERRIDE** — explicit Ray decision accepting risk or changing normal workflow.

Do not convert curiosity, brainstorming, or a question into a roadmap decision.

---

## 5. Prerequisite-First Rule

Before commands, edits, migrations, installations, or destructive operations, inspect what matters for the task, including:

- repository path;
- current branch;
- Git status;
- existing files and directories;
- required prior checkpoint, phase, tag, or baseline;
- environment and toolchain state;
- required dependencies;
- permissions and credentials;
- whether the target already exists;
- whether backups or recovery points exist;
- whether the operation could modify or delete user data.

Never assume a prerequisite is complete.

For risky operations:

1. take one bounded step;
2. know the expected result;
3. verify the actual result;
4. stop if it differs materially.

---

## 6. Plan Before Editing

For non-trivial work:

1. Read relevant specifications.
2. Inspect the current implementation.
3. Define the exact scope.
4. Identify files expected to change.
5. Define acceptance criteria.
6. Define tests or evidence required for success.
7. Confirm the task does not enter excluded scope.
8. Implement the smallest complete slice.
9. Validate.
10. Report evidence, limitations, and repository state.

Do not begin an unbounded refactor without a written or clearly established plan.

---

## 7. Scope Discipline

Maintain explicit separation between:

- current approved work;
- future work;
- optional ideas;
- research;
- experiments;
- deprecated or rejected directions.

Rules:

- implement only the active approved scope;
- do not add later-phase features because they were mentioned somewhere;
- do not expand dependencies, permissions, cloud usage, or architecture silently;
- do not treat a prototype as production architecture automatically;
- do not mark placeholders as completed features;
- do not bundle unrelated cleanup into a focused task.

---

## 8. Work in Reviewable Units

Prefer changes that are:

- small enough to inspect;
- complete enough to be useful;
- isolated from unrelated modules;
- reversible where practical;
- supported by clear tests or evidence;
- documented when they affect future work.

Avoid:

- unrelated reformatting;
- casual renaming of public contracts;
- duplicate implementations;
- unnecessary rewrites;
- hidden dependency upgrades;
- temporary scripts left in production paths;
- silent architecture changes.

---

## 9. Validation and Evidence Rules

A task is not complete because the code looks reasonable or a script prints `PASS`.

Valid evidence may include:

- successful exit codes;
- expected output;
- correct generated files;
- schema or contract validation;
- tests relevant to the change;
- clean or explained Git status;
- runtime verification;
- visual verification;
- no unintended modifications;
- preserved user data;
- reproducible commands.

Always report:

- what was tested;
- commands or methods used;
- actual result;
- tests skipped and why;
- known limitations;
- evidence not yet obtained.

Never claim a command, test, build, inspection, or verification occurred when it did not.

Never weaken a test solely to make it pass.

---

## 10. Entry and Exit Gates

### Global Entry Gate

Before starting an implementation unit, confirm:

- correct repository;
- expected branch or workspace;
- repository state understood;
- required documents present;
- previous checkpoint satisfied;
- target scope approved;
- required tools available;
- recovery path understood;
- no unresolved conflict blocks the task.

Failure on a material entry condition means STOP and report.

### Global Exit Gate

Before declaring completion, confirm:

- acceptance criteria satisfied;
- relevant validation completed;
- no unrelated files changed;
- no hidden scope expansion;
- no unapproved architecture or dependency drift;
- no security or privacy weakening;
- documentation updated where required;
- known limitations listed;
- Git or file state reported;
- next state is unambiguous.

---

## 11. Stop Conditions

Stop and report when:

- a material prerequisite is missing;
- the wrong repository or branch is active;
- the working tree is unexpectedly dirty and changes could collide;
- a required authoritative document is missing;
- the requested work conflicts with an active locked decision;
- a security, privacy, licensing, cost, or data-loss risk is unresolved;
- dependency compatibility is uncertain;
- tests fail in a way that affects the task;
- expected command output differs materially;
- user data may be overwritten or deleted;
- the task would silently enter future or excluded scope;
- required permissions are unavailable;
- success cannot be verified honestly.

Do not silently work around a stop condition.

A stop condition should include:

- what failed;
- evidence;
- impact;
- smallest safe resolution;
- whether Ray's decision is required.

---

## 12. Decision Ownership

Agents may:

- inspect;
- analyze;
- implement approved scope;
- test;
- document;
- propose decisions;
- recommend the next step.

Agents must not silently:

- approve their own major architectural change;
- redefine project scope;
- move or delete approved baselines;
- accept owner-level risk;
- convert research into a product decision;
- alter global Ray preferences;
- claim final release approval.

Ray remains the final decision authority.

---

## 13. Recovery and Git Discipline

Before high-impact work, establish a recoverable baseline.

General rules:

- inspect Git status before editing;
- preserve unrelated user changes;
- avoid destructive reset, force operations, history rewrite, tag movement, or file deletion without explicit authorization and a recovery plan;
- do not include unrelated files in commits;
- approved tags or baselines should be treated as immutable unless Ray explicitly changes them;
- document the exact commit, tag, artifact, or backup used as a checkpoint;
- keep source files immutable when processing user media or documents unless modification is explicitly required.

---

## 14. Project Routing

Large projects may separate responsibilities into dedicated chats or agents, for example:

- **MASTER / ORCHESTRATION** — roadmap, task order, cross-domain decisions, final routing;
- **ARCHITECTURE** — stack, system boundaries, ADRs, scope, major tradeoffs;
- **IMPLEMENTATION** — bounded code and deliverable changes;
- **QUALITY & RELEASE** — validation, performance, packaging, evidence, release gates;
- **UI/UX** — interaction, design system, accessibility, workflow usability;
- **RESEARCH / FEATURE LAB** — proposals and experiments without automatic approval;
- **PROVIDERS / SECURITY** — external services, privacy, licensing, credentials, fallback design.

Each chat or agent should have:

- a clear mandate;
- allowed actions;
- forbidden actions;
- input sources;
- expected output;
- escalation path.

New ambiguous work should begin with orchestration rather than being silently implemented in the wrong domain.

---

## 15. Cross-Project Learning Protocol

At project milestones, review what was learned.

Classify each lesson as:

### Project-specific

Keep it inside the project when it depends on:

- that product's architecture;
- a unique user group;
- a project-only model, provider, or technology;
- temporary implementation details;
- project-specific risks or constraints.

### Global Ray preference

Propose or update the profile repository when it reflects a recurring owner preference, such as:

- workflow behavior;
- communication style;
- evidence standards;
- decision process;
- documentation structure;
- reusable quality gates;
- general risk tolerance;
- project bootstrap conventions.

### Reusable template

Save to `TEMPLATES/` when it is a generic reusable structure, including:

- project startup checklist;
- current-state handoff;
- decision record;
- implementation prompt;
- validation report;
- phase gate;
- release checklist;
- owner override record;
- project-chat mandate.

Do not pollute global memory with low-value noise or temporary facts.

---

## 16. Completion Report

At the end of a substantial task, report:

```text
Task or phase
Files changed
What was implemented
Commands/tests/inspection performed
Results and evidence
Known limitations
Repository or workspace state
Decisions added or changed
Templates created or updated
Recommended next single step
```

Be explicit about anything not tested or not verified.

---

## 17. Universal Execution Loop

```text
READ
→ INSPECT
→ CLASSIFY
→ PLAN
→ IMPLEMENT THE SMALLEST COMPLETE SLICE
→ VALIDATE WITH EVIDENCE
→ DOCUMENT
→ PRESERVE REUSABLE STRUCTURES
→ REPORT HONESTLY
→ ROUTE THE NEXT STEP
```

Never skip a material gate merely to move faster.
