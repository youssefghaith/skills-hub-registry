---
name: pr-review
description: Walk through a pull request file by file and surface correctness, style, and risk concerns before approval.
---

# PR review

Use this skill when reviewing a teammate's pull request. The goal is a focused, actionable review that catches real issues without rubber-stamping or nit-picking.

## Steps

1. Read the PR description first. If it doesn't say *why* the change is being made, ask before reviewing.
2. Walk the diff file by file. For each file:
   - Identify the intent of the change.
   - Check for obvious bugs (off-by-one, null handling, error paths).
   - Note style or naming inconsistencies with the surrounding code.
3. Check for missing tests when touching public APIs or fixing a bug.
4. Look for security concerns: input validation, injection, secrets in code.
5. Summarise blockers vs. nits separately so the author can triage.

## Anti-patterns

- Don't suggest renames purely to match personal style.
- Don't request changes for hypothetical future requirements that aren't in scope.
- Don't approve when you haven't actually read the diff.
