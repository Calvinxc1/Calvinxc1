# Policy Modules

This folder stores modular `AGENTS.md` policy components that can be mixed and
matched when assembling a repo-local policy.

The modules are opinionated building blocks rather than full repo templates.

## Intended Use

Use these files as building blocks for a target repo's `AGENTS.md`.

They are meant to provide reusable policy structures and defaults for recurring
repo needs, not to serve as fully neutral boilerplate.

Copy the selected content into the target repo's `AGENTS.md` and edit repo
specifics there.

## Core Structure

The module set is organized by policy segment so a target repo can keep major
concerns separate instead of bundling them into one broad document.

- `00` to `08`: baseline governance, acceptance, validation, review, safety,
  overrides, and segmented-governance structure.
- `10`: explicit execution-authorization behavior.
- `20` to `24`: research-domain base policy plus structure, citations, framing,
  and review.
- `30` to `32`: workflow, release, and changelog policy.

If a target repo uses a segmented governance corpus instead of a single
monolithic `AGENTS.md`, the intended split is:

- entrypoint and precedence rules
- file-type split between human-facing orientation docs and low-token
  machine-loaded policy files
- always-load baseline rules
- selectively loaded standing policy segments
- process and maintenance rules
- override records for temporary exceptions

The Argo governance work also demonstrates a useful file-type pattern for this
kind of structure:

- keep `AGENTS.md` short and Markdown-based as the entrypoint
- keep standing policy, task routing, process rules, and override logs in
  concise YAML when token efficiency matters
- keep indexes and orientation documents in Markdown instead of turning the
  policy body back into long prose

## Module Set

### Foundation And Governance

- `modules/00-foundation-governance.md`: always-load baseline rules for
  execution permission, conflict handling, and scope.
- `modules/01-ai-acceptance.md`: AI oversight and explicit acceptance
  boundaries.
- `modules/02-risk-validation.md`: risk tiers and minimum validation gates.
- `modules/03-epistemic-discipline.md`: claim labeling, uncertainty handling,
  and human-owned decision areas.
- `modules/04-review-standards.md`: findings-first review posture and residual
  gap handling.
- `modules/05-safety-transparency.md`: change communication and guardrail
  handling.
- `modules/06-enforcement-overrides.md`: enforced controls, temporary
  exceptions, and override records.
- `modules/07-governance-structure.md`: segmented-governance entrypoint,
  precedence, file-type strategy, and segment boundaries.
- `modules/08-governance-maintenance.md`: maintenance rules for structured
  policy corpora.

### Execution

- `modules/10-execution-explicit-approval.md`: explicit execution cues,
  preflight confirmation, and read-only defaults.

### Research Domain

- `modules/20-domain-research.md`: base research-artifact roles and high-level
  structure guidance.
- `modules/21-research-structure.md`: research folder structure, indexes, and
  cross-linking.
- `modules/22-research-citations.md`: citation verification and cross-artifact
  source support.
- `modules/23-research-framing.md`: uncertainty framing and claim-calibration
  rules.
- `modules/24-research-review.md`: research-specific review workflow and
  consistency checks.

### Workflow And Release

- `modules/30-workflow-gitflow.md`: GitFlow branch roles, merge discipline, and
  workflow alignment.
- `modules/31-release-semver.md`: semantic-versioning and release-discipline
  expectations.
- `modules/32-release-changelog.md`: changelog staging and release-note update
  expectations.
