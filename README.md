# Ruleset Prompt Pack

This repository provides a strict operating workflow for coding agents, along with reusable prompts you can paste into your assistant.

Use `<PROJECT_ROOT>` in prompts to represent your local repo path (for example, `/Users/alex/work/ruleset` or `C:\dev\ruleset`).

## What This Is

- `agents.md`: execution workflow (planning, implementation, verification, completion)
- `rules.md`: hard constraints that must always be followed
- `tasks/todo.md`: task planning, progress, and verification log template
- `tasks/lessons.md`: correction and incident learning log
- `PROMPT.md`: copy-paste prompt templates that enforce this workflow

## How To Use

1. Open `PROMPT.md`.
2. Copy either:
   - **Short Everyday Prompt** for normal tasks
   - **Full Strict Prompt** when you want stricter execution discipline
   - **Relative Path Prompt** when your assistant is already running from the repository root
3. Paste the prompt into your coding assistant before work starts.
4. During execution, ensure the assistant:
   - Uses only `pnpm` (never `npm`)
   - Updates `tasks/todo.md` with plan, progress, and verification evidence
   - Updates `tasks/lessons.md` when corrections/issues occur

## Suggested Working Pattern

1. For non-trivial tasks, initialize `tasks/todo.md` first.
2. Implement only requested scope.
3. Verify with concrete evidence (tests/checks/output).
4. Finalize with risks/follow-ups and any lessons learned.

## Path Convention

- Use `<PROJECT_ROOT>` in prompt text.
- Replace it with the absolute path to your own repository before running.
- Or use the relative-path prompt variant to avoid machine-specific paths.
