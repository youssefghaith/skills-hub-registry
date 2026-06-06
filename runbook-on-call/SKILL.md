---
name: runbook-on-call
description: Walk through the on-call runbook for paging incidents — checks dashboards, recent deploys, and known-bad releases.
---

# On-Call Runbook

When the user is debugging a production incident:

1. Check the API latency dashboard at `grafana.internal/d/api-latency`.
2. Look at the last 3 deploys in the deploy channel — note any that landed in the last 30 minutes.
3. Check the incident log for the affected service (`#incidents-<service>`).
4. If a recent deploy is suspect, propose a rollback before deeper investigation.

Always summarize what you've checked and what's still unknown before suggesting an action.
