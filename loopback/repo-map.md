# Repository Map

Summary of repositories owned by `9rn59htpxb-beep` with purpose, stability, and security posture notes to guide AI-assisted work.

## 9rn59htpxb-beep/flutter
- Role: Upstream Flutter SDK fork for experimentation and customization.
- Default branch: `master`; track upstream before proposing changes.
- Status: Active; prefer short-lived branches for spikes.
- Security: Avoid committing credentials; respect upstream security advisories and keep local toolchains updated.

## 9rn59htpxb-beep/ios-nrf-wi-fi-provisioner
- Role: iOS Wi-Fi provisioning library for Nordic devices.
- Default branch: `main`.
- Status: Active; production-adjacent—prioritize stability and regression testing.
- Security: Treat provisioning keys and device identifiers as sensitive; do not log secrets or device-specific data.

## 9rn59htpxb-beep/openaimacpaw
- Role: Swift OpenAI client and API experimentation repo.
- Default branch: `main`.
- Status: Active; experimentation-friendly but adhere to API usage limits.
- Security: Never commit API keys; rotate tokens when debugging issues and scrub captured traces.

## 9rn59htpxb-beep/David-Anthony-Cafaro
- Role: Control/coordination repository and loopback home.
- Default branch: `main`.
- Status: Active; lightweight docs and task intake live here.
- Security: Keep account-level rules current; avoid storing secrets and prefer links to secured storage.
