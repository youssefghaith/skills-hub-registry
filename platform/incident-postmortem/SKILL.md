---
name: incident-postmortem
description: Draft a blameless postmortem from incident timeline, root cause analysis, and follow-up actions.
---

# Incident postmortem

Use this skill after an incident is resolved to draft a postmortem document the team can review.

## Steps

1. Reconstruct the timeline. Pull from Slack, PagerDuty, dashboards. Each entry: timestamp (UTC), who saw what, what changed.
2. Identify the *trigger* (the change or event that lit the fuse) separately from the *root cause* (the underlying gap that allowed the trigger to cause damage).
3. List the action items. Each must have an owner and a target date. Action items without owners get cut.
4. Capture what went well — fast detection, good comms, useful runbooks. Postmortems that only list failures rot.

## Output sections

- **Summary** — one paragraph a stakeholder can read in 30 seconds.
- **Impact** — users affected, duration, revenue/SLO impact if measurable.
- **Timeline** — bulleted, UTC, terse.
- **Root cause** — one or two paragraphs. Avoid "human error" as a root cause.
- **What went well** — 2-3 bullets.
- **Action items** — checklist with owner + due date.

## Anti-patterns

- Don't blame individuals. Systems failed; people responded.
- Don't write action items the team won't actually do.
- Don't skip "what went well" — it's load-bearing for morale.
