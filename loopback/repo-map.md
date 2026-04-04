# Repository Map

Human-readable overview of all repositories tracked in this account.

## Control

| Repo | Role | Language | Branch |
|------|------|----------|--------|
| [David-Anthony-Cafaro](https://github.com/9rn59htpxb-beep/David-Anthony-Cafaro) | Personal coordination repo and loopback home | Markdown | `main` |

## Forks

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
