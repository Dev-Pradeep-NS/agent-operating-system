# Reusable Prompts

## Short Everyday Prompt

```text
Before starting, strictly follow:
- /home/vscode/projects/personal/ruleset/agents.md
- /home/vscode/projects/personal/ruleset/rules.md
- /home/vscode/projects/personal/ruleset/tasks/todo.md
- /home/vscode/projects/personal/ruleset/tasks/lessons.md

Use pnpm only (never npm), record plan/progress/verification in tasks/todo.md, and add lessons.md entries for any corrections.
```

---

## Full Strict Prompt

```text
Follow these project docs strictly before doing any work:

1) /home/vscode/projects/personal/ruleset/agents.md
2) /home/vscode/projects/personal/ruleset/rules.md
3) /home/vscode/projects/personal/ruleset/tasks/todo.md
4) /home/vscode/projects/personal/ruleset/tasks/lessons.md

Requirements:
- For non-trivial tasks, start by filling tasks/todo.md with plan and success criteria.
- Execute according to agents.md workflow.
- Enforce all hard constraints in rules.md.
- Use pnpm only, never npm.
- Do not mark complete without verification evidence.
- If a correction/issue occurs, add an entry to tasks/lessons.md.
```
