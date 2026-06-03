---
description: Stage and commit the current changes with a clear, conventional message
allowed-tools: Bash(git status:*), Bash(git diff:*), Bash(git add:*), Bash(git log:*), Bash(git commit:*)
---

Create a git commit for the current changes.

## Context

- Current status: !`git status`
- Staged + unstaged diff: !`git diff HEAD`
- Recent commits (for style): !`git log --oneline -10`

## Your task

1. Review the changes above to understand what was done.
2. If nothing is staged, stage the relevant changed files with `git add` (do NOT
   blindly `git add -A` — only add files that belong in this commit; mention if you
   skip anything).
3. Write a clear, descriptive commit message that matches the style of the recent
   commits. If `$ARGUMENTS` is provided, use it verbatim as the summary line (the
   commit title); otherwise write your own concise summary line (imperative mood,
   ~50 chars). Add a short body if the change needs explanation.
4. Commit with the message.

5. Show the resulting `git log --oneline -1` so the user can confirm.

Usage: `/commit [title]` — the optional `title` becomes the commit's summary line.
Do NOT push unless explicitly asked.
