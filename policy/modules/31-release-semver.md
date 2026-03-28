# Release SemVer Module

Use this module for repositories that publish versions and want explicit release
impact rules.

## Semantic Versioning

- Follow Semantic Versioning: `MAJOR.MINOR.PATCH`.
- Use `MAJOR` for breaking changes, `MINOR` for backward-compatible features,
  and `PATCH` for backward-compatible fixes.
- Do not change version numbers arbitrarily; tie the version bump to actual
  release impact.
- If release impact is unclear, require a human decision on version level.

## Release Discipline

- Keep written release policy aligned with actual workflow automation and branch
  protections.
- Keep release checks, publish steps, and recovery procedures aligned with the
  documented branch and event model.
- If release checks, publish steps, or recovery procedures differ by branch or
  event type, document that explicitly in the target repo's `AGENTS.md`.
- If release safeguards are bypassed for a specific operation, record the
  specific safeguard and the immediate reason.
