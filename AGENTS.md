# Repository notes

<!-- quest-qualification-handoff -->
## Runtime qualification

HTTP/2 and optional HTTP/3 are separate from Worker APK asset resolution.

Start with the [shared runtime handoff](https://github.com/rebeckerspecialties/BabylonNative/blob/wgpu/Documentation/QuestRuntimeHandoff.md) for artifact pins and related PRs. This is a historical pre-monorepo branch. Keep fork instructions out of upstream ports. Use the monorepo PR for new runtime development; exercise the same inputs on each supported JS engine.

- Implementation: Test protocol negotiation and fallback without turning HTTP/3 into a requirement for local app URLs.
- Device: Verify a real HTTPS response, an offline failure, and packaged education on an unmodified transport configuration.
