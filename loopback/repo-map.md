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
