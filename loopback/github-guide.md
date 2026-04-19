# GitHub Concepts — Plain-Language Guide

A quick reference so both humans and AI agents share the same vocabulary when discussing this account's repositories.

---

## Core Objects

| Term | What it is | Example in this account |
|------|-----------|------------------------|
| **Repository (repo)** | A folder on GitHub that stores a project's files and their full history. | `9rn59htpxb-beep/David-Anthony-Cafaro` |
| **Branch** | A parallel copy of the files that can be changed without affecting the main copy. | `copilot/fix-help-the-human` |
| **Commit** | A saved snapshot of changes, with a message explaining what changed and why. | "docs: add github-guide.md" |
| **Pull Request (PR)** | A request to merge one branch into another; the place where changes are reviewed before merging. | Any open PR in this account |
| **Fork** | A full copy of another person's repo, owned by you, so you can modify it independently. | `9rn59htpxb-beep/flutter` |
| **Issue** | A discussion thread used to track a bug, feature request, or question. | "Issue A — Help the human" |
| **Tag / Release** | A named point in history, typically used to mark a published version. | `v1.0.0` |

---

## Workflow Concepts

| Term | What it means |
|------|--------------|
| **Clone** | Copying a remote repo to a local machine to work on it. |
| **Push** | Sending local commits to the remote repo on GitHub. |
| **Pull / Fetch** | Bringing remote changes to your local copy. |
| **Merge** | Combining the history of two branches into one. |
| **Rebase** | Replaying commits from one branch on top of another, producing a linear history. |
| **Conflict** | When two branches change the same lines and Git cannot automatically combine them. |
| **Draft PR** | A PR marked as not ready to merge; useful for sharing work-in-progress for feedback. |

---

## Permissions and Visibility

| Term | What it means |
|------|--------------|
| **Public repo** | Anyone on the internet can read the code. |
| **Private repo** | Only invited collaborators can read or write. |
| **Collaborator** | A person granted push access to a repo. |
| **Organization** | A shared GitHub account owned by a team, with members and access controls. |
| **GitHub App** | A bot or integration that acts on behalf of an account with scoped permissions. |

---

## This Account's Vocabulary

| Term | Meaning here |
|------|-------------|
| **Control repo** | `David-Anthony-Cafaro` — stores the loopback, playbook, and task files. |
| **Loopback** | The `loopback/` folder that gives AI agents a stable, machine-readable starting point. |
| **Manifest** | `loopback/manifest.yaml` — the authoritative list of repos, capabilities, and rules. |
| **Task file** | A Markdown file in `loopback/tasks/` that tracks a single unit of work from plan to done. |
| **Upstream fork** | A repo (e.g., `flutter`) that mirrors an external open-source project; customizations live in a dedicated branch. |

---

## How a Change Flows

```
Owner or agent identifies work
        │
        ▼
Create task file (loopback/tasks/my-task.md)
        │
        ▼
Create feature branch  (feat/my-task or fix/my-task)
        │
        ▼
Commit small, focused changes with descriptive messages
        │
        ▼
Open a Pull Request — plain-language summary in the description
        │
        ▼
Owner reviews → approves → merges into main
        │
        ▼
Update task file status to `done`
```

---

## Quick Tips for Readable Commits

- Start with a lowercase type prefix: `feat:`, `fix:`, `docs:`, `refactor:`, `chore:`
- Finish the sentence "This commit will…" with your message body.
- Keep the subject line under 72 characters.
- Reference an issue number when one exists: `closes #12`
