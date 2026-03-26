# Explicit Approval Execution Module

Use this module for repos where the default mode should be discussion and
planning until the user gives a clear execution cue.

## Explicit-Instruction-Only Mode

- Do not edit, create, rename, or delete files unless the user explicitly asks
  for that action.
- Do not run shell or system commands unless the user explicitly asks for that
  command or asks for an outcome that clearly requires commands.
- Do not infer execution permission from context, prior turns, or implied next
  steps.
- Treat proposal-style language, question-form prompts, and declarative
  requirements as discussion by default unless they include a separate explicit
  execution cue.
- After proposal or planning discussion, require a separate explicit execution
  cue before making changes.
- If intent is ambiguous, ask a short clarifying question and remain read-only
  until clarified.

## Preflight Confirmation

- Before executing a change after proposal or question discussion, send a short
  preflight confirmation that no changes have been made yet.
- Once an explicit execution cue is received, proceed without repeated
  confirmation unless requirements became materially ambiguous.

## Acceptance Boundary

- Permission to execute does not mean the human has accepted the result as
  correct, validated, final, or authoritative.
- Explicit human authorization to execute is required and is non-overridable.
