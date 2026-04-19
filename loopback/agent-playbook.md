# Agent Playbook

Rules and guidance for AI agents working on this GitHub account.

## Identity

- Account owner: David Cafaro (`9rn59htpxb-beep`)
- Control repo: `9rn59htpxb-beep/David-Anthony-Cafaro`
- Loopback version: 2

## Scope of Work

Agents operating on this account should:

1. **Read `loopback/manifest.yaml` first** to understand the repository inventory and capabilities before taking any action.
2. **Plan changes in the control repo** before touching large upstream forks.
3. **Open a task issue or branch** for any non-trivial change, using `loopback/tasks/TEMPLATE.md` as the intake format.
4. **Prefer small, reversible commits** over large rewrites.
5. **Document intent** in commit messages and pull request descriptions.
6. **Record every action taken** in the task file under "Agent Actions Taken" so the owner can audit decisions.

## Autonomous Actions

Agents may proceed **without asking the owner** for the following low-risk operations:

| Action | Condition |
|--------|-----------|
| Add or update documentation files (`.md`, `.yaml`) in the control repo | Change does not alter behavior of any running code |
| Create a task file from `TEMPLATE.md` | No existing task file covers the same issue |
| Create a feature branch and open a draft PR | Branch is off `main`, named with a clear intent prefix (`feat/`, `fix/`, `docs/`) |
| Update `manifest.yaml` and `repo-map.md` to reflect new or renamed repos | Owner has mentioned the new repo in context |
| Refresh `agent-playbook.md` to add decision rules | Additive only; no existing rules are removed |

For everything else, follow the decision rules below.

## Decision Rules

| Situation | Action |
|-----------|--------|
| Unclear scope | Log uncertainty in the task file, then ask the owner before proceeding |
| Breaking change to upstream fork | Create a draft PR, do not merge, add a `⚠️ breaking` label |
| Secrets or credentials encountered | Stop immediately, do not log or commit |
| Capability listed as `not_guaranteed` | Verify availability before relying on it |
| Task already tracked in `tasks/` | Update the existing task file, do not duplicate |
| Conflicting instructions from owner vs. playbook | Follow the owner's explicit instruction and note the conflict in the task file |
| Proposed change touches more than 3 files outside the control repo | Pause and summarize the plan in the PR description before committing |

## Reporting to the Owner

After completing any non-trivial action, agents must:

1. Add an **"Agent Actions Taken"** section to the relevant task file listing every file created, modified, or deleted and why.
2. Include a plain-language **summary sentence** at the top of any PR description so the owner can understand the change in one read.
3. Use a **`[AGENT LOG]`** prefix in any PR comment that was machine-generated, so the owner can distinguish agent notes from human review comments.

## Workflow

```
1. Read manifest.yaml and this playbook
2. Identify the affected repository and branch
3. Create or update a task file in loopback/tasks/
4. Make changes in a feature branch
5. Record actions in the task file under "Agent Actions Taken"
6. Open a pull request with a plain-language summary
7. Request owner review
```

## Off-Limits

- Do not push directly to `main` or `master` on any repo.
- Do not install or uninstall GitHub Apps without owner approval.
- Do not modify repository settings or secrets.
- Do not expose private data in commit messages, PR descriptions, or issue comments.
