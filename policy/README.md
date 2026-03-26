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

## Module Set

- `modules/00-foundation-governance.md`: AI oversight, validation gates, epistemic
  discipline, transparency, and review routing.
- `modules/10-execution-explicit-approval.md`: strict user-approval requirements for
  file edits and command execution.
- `modules/20-domain-research.md`: research-specific standards for citation handling,
  uncertainty framing, and research folder conventions.
- `modules/30-workflow-gitflow.md`: branch-role and pull-request discipline for repos
  that follow GitFlow.
- `modules/31-release-semver.md`: versioning, release impact, and release-override
  expectations for repos that publish versions.
