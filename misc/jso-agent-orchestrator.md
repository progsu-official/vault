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

# jso: an agent that runs your whole dev workflow

JSO is a terminal-native agent orchestrator: hand it a ticket, and it scopes the change, implements it with minimal diffs, tests it, and drafts the PR, gated at every step that actually matters.

## what it does

- **scopes the ticket** before writing anything, so you're not guessing at requirements mid-implementation
- **implements with minimal diffs**, the smallest correct change instead of a sprawling rewrite, which saves both review time and token cost
- **runs tests**, and `jso-debugger` fixes failures on its own when something breaks
- **drafts the PR** using real templates, not a generic one-size-fits-all summary
- **gates every risky step** (spawning a parallel run, pushing, merging) behind a yes, nothing ships silently

## why it's worth knowing about

Most of a dev task isn't writing the code, it's scoping it right, keeping the diff small, and not skipping the boring parts (tests, a real PR description). JSO packages that whole loop so you spend your attention on the ticket, not the ceremony around it.

## the repo

[JohnSang16/jso](https://github.com/JohnSang16/jso) on GitHub.
