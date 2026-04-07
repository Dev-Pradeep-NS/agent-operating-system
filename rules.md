# Rules

These are hard constraints.
Process details are defined in `agents.md`.

## 1. Scope Integrity

- Implement only requested scope.
- Do not add speculative features.
- Do not perform unrelated refactors.

---

## 2. Safety And Compatibility

- Do not introduce breaking changes without explicit approval.
- Preserve backward compatibility unless the task requires otherwise.
- Do not modify unrelated code paths.

---

## 3. Evidence Over Assumption

- Never claim success without verifiable evidence.
- Validate behavior through tests, checks, or observable runtime output.
- If verification cannot be executed, state that clearly.

---

## 4. Clarity And Maintainability

- Prefer readable, explicit, maintainable code.
- Avoid unnecessary abstraction and hidden behavior.
- Follow existing project conventions unless a change is justified.

---

## 5. Error Discipline

- Do not ignore errors.
- Handle meaningful edge cases.
- Fail loudly and diagnosably rather than silently.

---

## 6. Performance Discipline

- Avoid clearly inefficient solutions when practical alternatives exist.
- Do not prematurely optimize low-impact paths.

---

## 7. Security Baseline

- Never expose secrets or sensitive data.
- Validate untrusted inputs where applicable.
- Avoid unsafe operations without explicit justification.

---

## 8. Package Manager Policy

- In this project, use `pnpm` for dependency and script commands.
- Do not use `npm` commands.
- If migration or compatibility work requires exceptions, document and get explicit approval.
