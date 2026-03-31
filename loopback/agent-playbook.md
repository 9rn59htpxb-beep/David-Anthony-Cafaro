# Agent Playbook

Rules and guidance for AI agents working on this GitHub account.

## Identity

- Account owner: David Cafaro (`9rn59htpxb-beep`)
- Control repo: `9rn59htpxb-beep/David-Anthony-Cafaro`
- Loopback version: 1

## Scope of Work

Agents operating on this account should:

1. **Read `loopback/manifest.yaml` first** to understand the repository inventory and capabilities before taking any action.
2. **Plan changes in the control repo** before touching large upstream forks.
3. **Open a task issue or branch** for any non-trivial change, using `loopback/tasks/TEMPLATE.md` as the intake format.
4. **Prefer small, reversible commits** over large rewrites.
5. **Document intent** in commit messages and pull request descriptions.

## Decision Rules

| Situation | Action |
|-----------|--------|
| Unclear scope | Ask the owner before proceeding |
| Breaking change to upstream fork | Create a draft PR, do not merge |
| Secrets or credentials encountered | Stop immediately, do not log or commit |
| Capability listed as `not_guaranteed` | Verify availability before relying on it |
| Task already tracked in `tasks/` | Update the existing task file, do not duplicate |

## Workflow

```
1. Read manifest.yaml and this playbook
2. Identify the affected repository and branch
3. Create or update a task file in loopback/tasks/
4. Make changes in a feature branch
5. Open a pull request referencing the task
6. Request owner review
```

## Off-Limits

- Do not push directly to `main` or `master` on any repo.
- Do not install or uninstall GitHub Apps without owner approval.
- Do not modify repository settings or secrets.
- Do not expose private data in commit messages, PR descriptions, or issue comments.
