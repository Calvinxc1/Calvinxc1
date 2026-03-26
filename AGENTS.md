# AGENTS.md

This file defines required behavior for coding agents working in this
repository. These instructions apply to the entire repo tree unless a more
specific nested `AGENTS.md` overrides them.

## 1) Repository Purpose

- This repository is primarily a public-facing profile and documentation repo.
- The root `README.md` is the primary public artifact and should remain clean,
  concise, and presentation-oriented.
- The `policy/` directory stores reusable policy source material for future
  repo-specific `AGENTS.md` documents.
- Files under `policy/modules/` are opinionated building blocks, not active
  policy for other repositories unless copied and adapted there.

## 2) Execution And Change Control

- Do not edit, create, rename, or delete files unless the user explicitly asks
  for that action.
- Do not run shell or system commands unless the user explicitly asks for that
  command or asks for an outcome that clearly requires commands.
- Treat discussion, brainstorming, and recommendation requests as read-only by
  default.
- If the user asks for a recommendation, review, or proposed structure, do not
  implement changes unless the user separately asks for execution.
- If intent is ambiguous, ask a short clarifying question before making changes.

## 3) Public-Facing Repo Guardrails

- Prefer minimal, deliberate changes over broad restructuring.
- Do not add promotional, noisy, or attention-drawing references to internal
  policy material unless the user explicitly asks for that.
- Keep the root `README.md` focused on public profile content rather than
  internal workflow details.
- Avoid adding incidental tooling, automation, or repo-management files unless
  they are explicitly requested.

## 4) Policy Module Maintenance

- Keep policy modules reusable, opinionated, and modular.
- Do not assume a module is universally applicable; preserve specificity where
  the module is intentionally tied to a workflow or repo type.
- When editing module text, optimize for reuse as source material for future
  repo-local `AGENTS.md` files.
- Keep the policy index descriptive and lightweight; do not turn it into a
  template catalog unless the user explicitly asks for that.
- If a module reflects a specific workflow pattern, state that directly rather
  than pretending it is generic.

## 5) AI Oversight And Acceptance

- AI may propose, analyze, summarize, critique, and draft changes.
- AI output remains draft material unless explicitly accepted by a human.
- Explicit instruction to execute does not, by itself, mean the output is
  accepted as correct, final, or complete.
- When recommending policy language, distinguish clearly between reusable
  guidance, repo-specific decisions, and unresolved judgment calls.

## 6) Review And Recommendations

- When asked to review, prioritize clarity, policy fit, reuse quality,
  over-specific language, and structural confusion.
- When asked to recommend policy text, prefer concise starting points over
  exhaustive governance systems.
- Surface where wording is too repo-specific, too vague to reuse, or too heavy
  for this repository's lightweight purpose.

## 7) Transparency

- Before making a substantive change, state what will be changed.
- After making a change, summarize exactly what changed and where.
- If a requested action conflicts with these instructions, explain the conflict
  before proceeding.
