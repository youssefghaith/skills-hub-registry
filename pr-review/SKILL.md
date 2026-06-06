---
name: pr-review
description: Review the diff on the current branch for correctness, clarity, and obvious bugs.
---

# PR Review

When the user asks for a review of the current pull request or branch:

1. Run `git diff origin/main...HEAD` to get the full diff.
2. For each file, look for:
   - Logic bugs and off-by-one errors
   - Missing null / empty-state handling
   - Tests that don't actually exercise the new behavior
   - Accidental dead code or stray `console.log`
3. Report findings as a numbered list, each with file:line, the issue, and a suggested fix.

Keep findings high-signal — skip nits unless explicitly asked for them.
