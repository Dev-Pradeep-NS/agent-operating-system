# Agent Operating System

This document defines how work is executed.
Hard constraints live in `rules.md`.

## 1. When To Plan

Enter planning mode for any task that is non-trivial, including when:

- Work likely needs 3 or more meaningful steps
- Architecture, data model, or cross-file behavior may change
- There is meaningful regression risk

For simple, low-risk requests, execute directly and keep notes lightweight.

---

## 2. Planning Standard

Before implementation, write a concise plan in `tasks/todo.md`:

1. Problem definition
2. Root cause hypothesis
3. Proposed solution
4. Verification approach

Planning must remove ambiguity, not just list actions.
If new evidence invalidates the plan, stop and re-plan.

---

## 3. Execution Workflow

Follow this sequence:

1. Understand current behavior and constraints
2. Implement minimal focused changes
3. Verify with objective evidence
4. Update progress notes in `tasks/todo.md`
5. Finalize with review summary and risks

Execution should prioritize root-cause fixes over symptom patches.
Follow project tooling policy during execution (for JavaScript/TypeScript workflows, use `pnpm`, not `npm`).

---

## 4. Verification Standard

Do not declare completion without evidence.
Use whichever proof applies to the task:

- Automated tests
- Build/lint/type checks
- Logs and runtime behavior
- Before/after comparison

Final quality gate:
Would the result be acceptable in a senior engineering review?

---

## 5. Subagent Usage

Use subagents only when they reduce risk or cycle time.

Use one task per subagent and prefer them for:

- Parallel investigation
- Isolated research
- Independent implementation chunks

Keep ownership boundaries clear and consolidate results before finalizing.

---

## 6. Learning Loop

After any correction, add an entry to `tasks/lessons.md`.
Each entry must include:

- What failed
- Root cause
- Trigger signal (how to detect early next time)
- Preventive rule
- Concrete example

Review relevant lessons before starting similar work.

---

## 7. Completion Checklist

A task is complete only when all are true:

- Requested scope is delivered
- Verification evidence is recorded
- Risks and follow-ups are documented
- Lessons learned are updated when a correction was involved
