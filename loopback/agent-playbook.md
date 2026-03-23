# Agent Playbook

Standard workflow for ChatGPT to automate GitHub work in this account.

## Guiding principles
- Stay aligned with `loopback/manifest.yaml` and `loopback/repo-map.md` before touching any repo.
- Prefer small, reviewable changes with clear intent and traceability.
- Run the repo’s existing tests and linters before and after changes when available; if none exist, call that out.
- Never add secrets or external dependencies without explicit need.

## Automation flow
1. **Intake** — Read the request and the relevant task file (see `tasks/`). If missing, ask for clarification or create one from the template.
2. **Scope check** — Map the work to the correct repository using the repo map. Confirm default branch and any fork/upstream expectations.
3. **Plan** — Outline a concise checklist (what to change, tests to run, docs to update). Share early.
4. **Execute** — Make surgical changes. Keep commits scoped. Update documentation alongside code when it clarifies the change.
5. **Validate** — Run targeted tests/linters that already exist in the repo. Report any pre-existing failures separately from new ones.
6. **Record** — Summarize what changed, why, and how to verify. Note remaining risks or follow-ups.

## Task handling
- Use `loopback/tasks/TEMPLATE.md` to capture new requests. Include scope, constraints, and acceptance criteria.
- Prefer automation-friendly descriptions: inputs, expected outputs, and success checks.
- When closing tasks, link to the verification steps that were executed.

## Repository-specific notes
- **flutter** — Treat as an upstream fork: keep changes small, document divergences, and avoid breaking sync with upstream without explicit approval.
- **ios-nrf-wi-fi-provisioner** — Maintain API stability; update samples and note platform/version requirements when altering provisioning flows.
- **openaimacpaw** — Track API compatibility; add smoke tests for new endpoints when feasible.
- **David-Anthony-Cafaro** — Keep loopback documents current; reflect any new repos or rule changes here.

## Communication
- Be explicit about what was tested and what was not.
- Call out unknowns, assumptions, and risks that could block automation or deployment.
- Provide quick-start verification steps so humans can confirm the automated changes.
