# GitHub Loopback

This folder is the control layer for AI-assisted development on this GitHub account.

## Purpose
- keep a machine-readable map of repositories
- define how GitHub work should be requested and tracked
- give future sessions a stable place to read intent, scope, and rules

## What this does
This loopback does **not** grant new GitHub permissions by itself.
It improves coordination by giving the account a structured inventory and workflow.

## Files
- `manifest.yaml` — machine-readable account and repo inventory
- `repo-map.md` — human-readable explanation of repo roles
- `agent-playbook.md` — rules and autonomous-action permissions for AI agents
- `github-guide.md` — plain-language glossary of GitHub concepts
- `tasks/TEMPLATE.md` — reusable intake format for changes

## Naming guidance
- Choose intent-revealing nouns for values (e.g., `invoiceTotal` instead of `data`).
- Use verbs for functions that perform actions and explicit subjects for what they operate on (e.g., `sendBillingEmail`, `calculateLatencyMillis`).
- Prefix booleans with `is/has/should/can` to signal true/false semantics.
- Pluralize collection variables and note the unit when helpful (e.g., `pendingOrders`, `userIds`).
- Avoid unclear abbreviations unless they are domain-standard; expand to full words where possible.
- Differentiate pure functions from mutating ones with precise verbs (`get/compute` vs. `update/replace`).
- Name callbacks and handlers to reflect the trigger and target (`onConnectionClosed`, `handleProfileSaved`).
