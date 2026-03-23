# Agent Playbook

Guidelines for AI-assisted work across `9rn59htpxb-beep` repos with emphasis on secure handling of code, devices, and credentials.

## Intake and Planning
- Use `loopback/tasks/TEMPLATE.md` when opening new work; capture scope, risks, validation, and security sensitivities.
- Read `loopback/manifest.yaml` and `loopback/repo-map.md` before acting to confirm branches, roles, and ownership.
- When requirements are ambiguous, pause and ask for clarification rather than guessing.

## Execution Rules
- Prefer small, reviewable branches; sync with upstream/default branches before proposing changes.
- Run existing linters/tests relevant to touched areas; do not add new toolchains unless required to fix breakage.
- Keep changes scoped: favor corrections and reviews first; only increase capabilities when explicitly requested and documented.
- Avoid generating or committing build artifacts, secrets, or device-specific data.

## Security and Privacy
- Never commit API keys, tokens, certificates, or device identifiers. Scrub logs and diffs for sensitive data.
- Minimize data collection from devices; if device traces are needed, redact identifiers and session tokens.
- Use least privilege: prefer local mocks over live services; restrict network calls to what the task requires.
- For vulnerability fixes, summarize risk, impacted components, and validation performed.

## Active Fetching and Verification
- Refresh context before work: fetch latest default branches, reread manifests, and confirm dependency constraints.
- When syncing forks, prefer fast-forward or rebasing local work on the freshest upstream to reduce divergence.
- Double-check repository access rules before pulling in third-party code or dependencies.
- Record any fetched upstream commits or sync actions in task notes or PR descriptions.

## Review, Correction, and Capability Growth
- Prioritize reviewing and correcting existing flows; flag regressions and missing tests early.
- When asked to expand capabilities, capture the motivation, acceptance criteria, and security impact in the task intake.
- Provide concise PR summaries with testing evidence and any residual risks or follow-ups.
