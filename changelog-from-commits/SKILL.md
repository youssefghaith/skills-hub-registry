---
name: changelog-from-commits
description: Generate a user-facing changelog entry from a range of git commits.
---

# Changelog From Commits

When the user asks for a changelog for a release:

1. Run `git log <from>..<to> --pretty=format:"%h %s"` for the requested range.
2. Group commits into: **Added**, **Changed**, **Fixed**, **Removed**.
3. Rewrite each entry in user-facing language — drop refactors and chores unless they have visible impact.
4. Output Markdown with a `## <version> — <date>` header.

If no range is given, default to the last tag → HEAD.
