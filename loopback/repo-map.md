# Repository Map

Use this map to understand the active repositories in the 9rn59htpxb-beep account and decide where automated work should happen. Align incoming requests with the repo purpose before proposing changes.

## Repositories

- **flutter** — Fork of the Flutter SDK for experimentation and customization. Default branch: `master`. Treat as an upstream fork; avoid diverging without a clear intent.
- **ios-nrf-wi-fi-provisioner** — Swift library for provisioning Nordic devices over Wi‑Fi. Default branch: `main`. Library-quality changes should include API stability notes and sample updates.
- **openaimacpaw** — Swift OpenAI client and API experimentation repo. Default branch: `main`. Expect rapid iteration and compatibility checks with OpenAI API changes.
- **David-Anthony-Cafaro** — Control and coordination repo (this repo). Default branch: `main`. Store automation instructions, task intake, and account inventory here.

## How to use this map

1. Confirm the target repository matches the request (feature, fix, or research).
2. Review the default branch and branching expectations before proposing a workflow.
3. Apply the correct level of testing and documentation based on the repo’s role (SDK fork vs. library vs. control docs).
4. Keep this file aligned with `manifest.yaml` when repositories are added, archived, or change status.
| Repo | Role | Language | Branch |
|------|------|----------|--------|
| [flutter](https://github.com/9rn59htpxb-beep/flutter) | Flutter SDK fork for experimentation and customization | Mixed | `master` |

## Libraries

| Repo | Role | Language | Branch |
|------|------|----------|--------|
| [ios-nrf-wi-fi-provisioner](https://github.com/9rn59htpxb-beep/ios-nrf-wi-fi-provisioner) | iOS Wi-Fi provisioning library for Nordic devices | Swift | `main` |
| [openaimacpaw](https://github.com/9rn59htpxb-beep/openaimacpaw) | Swift OpenAI client and API experimentation repo | Swift | `main` |

## Notes

- This map is derived from `manifest.yaml`. When adding a new repository, update both files.
- Repos marked `upstream-fork` track an external open-source project; keep customizations in a dedicated branch to ease rebasing.

## Automation

The `.github/workflows/update-status.yml` workflow runs daily and on manual trigger. It queries the GitHub API and commits an updated `loopback/status.md` to `main`. No secrets beyond the built-in `GITHUB_TOKEN` are required.
