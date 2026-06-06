---
name: runbook-to-skill
description: Convert an existing runbook or workflow document into a SKILL.md. Use when the user has a markdown doc describing a repeatable process and wants to make it agent-runnable.
---

# Runbook → Skill

Take the pasted runbook and produce a SKILL.md:

1. Extract the trigger conditions into the description (when should this skill fire?)
2. Convert numbered steps into agent-actionable instructions
3. Replace human-only language ("ping the team") with explicit fallbacks
4. Add a short example at the bottom if the runbook has one

