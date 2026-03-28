# GitFlow Workflow Module

Use this module for repositories that follow GitFlow-style branch discipline.

## GitFlow Requirements

- Reserve `main` for production-ready history.
- Use `dev` as the integration branch for upcoming work when the repo follows
  GitFlow.
- Branch `feature/*` from `dev` and merge back into `dev`.
- Branch `release/*` from `dev` and merge into `main`.
- Branch `hotfix/*` from `main` and merge into `main`.
- Do not commit directly to `main` or `dev`.
- Use pull requests for merges.
- Keep branches and commits scoped to one logical purpose whenever practical.
- If the repository uses conventional commits, keep commit types aligned with
  that workflow.

## Workflow Alignment

- Align written branch policy with actual branch protections, merge controls,
  and CI trigger behavior.
- If CI, release dry runs, publish steps, or recovery flows differ by branch or
  event type, document that explicitly in the target repo's `AGENTS.md`.

## Enforcement And Overrides

- Distinguish between hard controls enforced by repository settings and softer
  defaults that rely on developer judgment.
- If a policy is overridden for a specific operation, record the policy being
  bypassed and the immediate reason.
- Treat repeated overrides as a signal that the policy should be reviewed rather
  than bypassed ad hoc indefinitely.
