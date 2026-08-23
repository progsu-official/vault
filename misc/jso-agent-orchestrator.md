---
title: "JSO: an agent that runs your whole dev workflow"
author:
  name: "John Sang"
  handle: "@johnsang"
readTime: "2 min read"
publishDate: 2026-08-19T00:00:00.000Z
updated: 2026-08-19T00:00:00.000Z
tags: [productivity, ai, tools, agents]
category: misc
---

[JohnSang16/jso](https://github.com/JohnSang16/jso) on GitHub.

A real dev task isn't just "write the code." Done properly it's scoping the ticket, implementing it, testing it, debugging when something breaks, and drafting the PR, every single time. Skip a step and you ship a half-workflow: unscoped, untested, or undocumented. Doing all of that thoroughly, on every ticket, is exactly the kind of tedious, repeatable work that can be automated. That's why I built JSO.

## install it and run it

```
claude plugin marketplace add JohnSang16/jso
claude plugin install jso@jso-marketplace
```

restart claude code so the skill and the `jso-debugger` subagent register, then just hand it a ticket like you would a teammate, no separate command to learn.

## how it solves it

JSO is a terminal-native agent orchestrator: hand it a ticket, and it works through that whole loop itself, gated at every step that actually matters.

- **scopes the ticket** before writing anything, using a bundled `jso:scope` skill, a scoping interview (one-liner, success criteria, definition of done, risks) that runs before anything substantial gets built, so you're not guessing at requirements mid-implementation
- **implements with minimal diffs**, the smallest correct change instead of a sprawling rewrite. it leans on an optional external dependency, [ponytail](https://github.com/DietrichGebert/ponytail), to enforce that lazy-build discipline in more detail and save time on diffs; if ponytail isn't installed, JSO falls back to the same discipline built in
- **runs tests**, and hands failures to `jso-debugger`, a separate subagent that fixes the root cause with a minimal diff and re-runs tests on its own
- **drafts the PR** using real templates, not a generic one-size-fits-all summary
- **gates every risky step** (spawning a parallel run, pushing, merging) behind a yes, nothing ships silently

