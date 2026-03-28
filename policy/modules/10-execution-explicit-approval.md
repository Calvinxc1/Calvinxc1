# Explicit Approval Execution Module

Use this module for repos where the default mode should be discussion and
planning until the user gives a clear execution cue.

## Explicit-Instruction-Only Mode

- Default to read-only discussion and planning until explicitly directed
  otherwise.
- Require a separate explicit execution cue before changing files after
  proposal or question discussion.
- Treat proposal-style language, question-form prompts, and declarative
  requirements as discussion by default unless they include a separate explicit
  execution cue.
- In review prompts that mention related artifacts, treat the extra artifacts
  as review-only unless separately authorized for edits.
- If intent is ambiguous, ask a short clarifying question and remain read-only
  until clarified.

## Preflight Confirmation

- If proposal or question discussion occurred and no preflight confirmation has
  been sent for that discussion, send only `Execution confirmation required. No
  changes made yet.` and make no changes.
- If preflight confirmation has already been sent and a later explicit
  execution cue is received, execute without another confirmation unless the
  requirements changed materially or became ambiguous.

## Acceptance Boundary

- Overrides may relax other eligible constraints, but never the requirement for
  explicit execution authorization.
- Permission to execute does not mean the human has accepted the result as
  correct, validated, final, or authoritative.
