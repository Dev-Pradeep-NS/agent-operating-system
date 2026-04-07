# Reusable Prompts

Replace `<PROJECT_ROOT>` with your repository's absolute path (for example, `/Users/alex/work/ruleset` or `C:\dev\ruleset`).

## Short Everyday Prompt

```text
Before starting, strictly follow:
- <PROJECT_ROOT>/agents.md
- <PROJECT_ROOT>/rules.md
- <PROJECT_ROOT>/tasks/todo.md
- <PROJECT_ROOT>/tasks/lessons.md

Use pnpm only (never npm), record plan/progress/verification in <PROJECT_ROOT>/tasks/todo.md, and add <PROJECT_ROOT>/tasks/lessons.md entries for any corrections.
```

---

## Full Strict Prompt

```text
Follow these project docs strictly before doing any work:

1) <PROJECT_ROOT>/agents.md
2) <PROJECT_ROOT>/rules.md
3) <PROJECT_ROOT>/tasks/todo.md
4) <PROJECT_ROOT>/tasks/lessons.md

Requirements:
- For non-trivial tasks, start by filling <PROJECT_ROOT>/tasks/todo.md with plan and success criteria.
- Execute according to <PROJECT_ROOT>/agents.md workflow.
- Enforce all hard constraints in <PROJECT_ROOT>/rules.md.
- Use pnpm only, never npm.
- Do not mark complete without verification evidence.
- If a correction/issue occurs, add an entry to <PROJECT_ROOT>/tasks/lessons.md.
```

---

## Relative Path Prompt (No Absolute Path Needed)

```text
Before starting, strictly follow:
- ./agents.md
- ./rules.md
- ./tasks/todo.md
- ./tasks/lessons.md

Use pnpm only (never npm), record plan/progress/verification in ./tasks/todo.md, and add ./tasks/lessons.md entries for any corrections.
```
