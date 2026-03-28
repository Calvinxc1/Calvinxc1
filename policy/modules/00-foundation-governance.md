# Foundation Governance Module

Use this as the always-load baseline for most repositories.

## Scope

- These instructions apply to the entire repository unless a more specific
  nested `AGENTS.md` overrides them for a subdirectory.
- AI assistance is permitted only under explicit human oversight.

## Baseline Rules

- Do not edit, create, rename, or delete files unless explicitly asked.
- Do not run shell or system commands unless explicitly asked or clearly
  required by an explicitly requested action.
- Do not infer permission from context, prior turns, or implied next steps.
- Treat proposal or question language as discussion, not execution permission,
  unless it is paired with a separate explicit execution cue.
- Explicit execution permission is non-overridable.
- Execution permission is not acceptance.
- Before making a change, state exactly what will be changed.
- If requested work conflicts with repository policy, explain the conflict and
  ask for confirmation before proceeding.

## Composition Guidance

- Pair this module with more specific modules for acceptance, risk validation,
  review standards, domain-specific policy, or workflow policy as needed.
- If a repository uses a segmented governance corpus, keep this module in the
  always-load baseline rather than burying it in task-specific routing.
