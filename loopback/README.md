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
- `agent-playbook.md` — rules and workflow for AI-driven automation
- `tasks/TEMPLATE.md` — reusable intake format for new work

## How to use
1. Start with `agent-playbook.md` to follow the standard ChatGPT automation flow.
2. Check `repo-map.md` and `manifest.yaml` to confirm the right target repo and branching expectations.
3. Capture new requests using `tasks/TEMPLATE.md` so scope, constraints, and acceptance criteria are clear before execution.
- `agent-playbook.md` — rules for future AI GitHub work
- `status.md` — live status dashboard (auto-generated daily by GitHub Actions)
- `tasks/TEMPLATE.md` — reusable intake format for changes
