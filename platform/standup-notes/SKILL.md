---
name: standup-notes
description: Generate concise daily standup notes from yesterday's git activity and today's task list.
---

# Standup notes

Use this skill at the start of the day to draft a standup update from your local activity.

## Steps

1. Run `git log --author=$(git config user.email) --since=yesterday --oneline` and read the messages.
2. Read the active task list (TODO, ticket queue, or pinned doc) for today's focus.
3. Draft three lines:
   - **Yesterday**: 1-2 concrete things that landed.
   - **Today**: the single most important thing, named specifically.
   - **Blockers**: only if there is one. Don't invent blockers to fill space.

## Output format

```
Yesterday: <thing> · <thing>
Today: <thing>
Blockers: <thing or "none">
```

## Anti-patterns

- Don't list every commit. Group related ones.
- Don't say "continuing on X" — say what *specifically* you'll finish today.
