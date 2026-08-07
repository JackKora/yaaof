---
id: poc-001-remote-workspaces-label
title: Rename the Workspaces UI label to Remote Workspaces
source: local
source_ref: ""
repo: yaaos/yaaos
branch: factory/poc-001-remote-workspaces-label
created: 2026-08-07T21:31:35Z
---

## Problem

The web UI labels the organization’s remote-agent fleet surface as “Workspaces.” The requested product wording is “Remote Workspaces.”

## In scope / Out of scope

**In scope**

- Replace the user-visible “Workspaces” label with “Remote Workspaces” on the primary organization navigation item, the remote-agent fleet page heading, and the corresponding Org Settings navigation item.
- Preserve the existing routes, access controls, icons, page behavior, and underlying workspace terminology.

**Out of scope**

- Renaming routes, URL paths, test IDs, source symbols, API contracts, database entities, or agent-protocol fields.
- Changing descriptive copy where “workspaces” refers to actual workspace resources rather than the UI surface name.

## Acceptance criteria

1. The organization sidebar link at `/org/:slug/workspaces` displays “Remote Workspaces.”
2. The page at `/org/:slug/workspaces` displays “Remote Workspaces” as its page heading.
3. The Org Settings sidebar item linking to `/org/:slug/settings/workspaces` displays “Remote Workspaces.”
4. The paths `/org/:slug/workspaces` and `/org/:slug/settings/workspaces`, their existing role gates, and their existing test IDs remain unchanged.

## Assumptions & open questions

- The requested label applies to the three existing user-visible navigation and heading labels, not to technical references to workspace resources.
- No unanswered questions.
