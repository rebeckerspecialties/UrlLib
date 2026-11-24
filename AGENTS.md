# Repository notes

<!-- quest-qualification-handoff -->
## Runtime qualification

Historical transport error and CI mirror. The monorepo transport review is BabylonNative #2078.

Start with the [shared runtime handoff](https://github.com/rebeckerspecialties/BabylonNative/blob/wgpu/Documentation/QuestRuntimeHandoff.md) for artifact pins and related PRs. This is a historical pre-monorepo branch. Keep fork instructions out of upstream ports. Use the monorepo PR for new runtime development; exercise the same inputs on each supported JS engine.

- Implementation: Keep HTTP status distinct from transport failure and avoid porting CI-only commits into production code.
- Device: Check packaged and HTTP archives independently, including truncated bodies and an offline fetch on the Quest.
