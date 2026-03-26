# Foundation Governance Module

Use this as the default starting module for most repositories.

## Scope

- These instructions apply to the entire repository unless a more specific
  nested `AGENTS.md` overrides them for a subdirectory.
- AI assistance is permitted only under explicit human oversight.

## AI Oversight And Acceptance

- AI may propose, analyze, summarize, critique, and draft implementations.
- AI output remains draft material unless explicitly accepted by a human or
  supported by completed validation.
- Explicit instruction to execute is not, by itself, acceptance of correctness,
  completeness, validation status, or release readiness.
- Silence, conversational continuation, or lack of objection do not count as
  acceptance.
- Final responsibility for code, documentation, release decisions, and policy
  interpretation remains with human developers.

## Risk Tiers And Validation Gates

- Classify substantive work before implementation or recommendation. If
  uncertain, classify at the higher tier.
- Tier 1: low-risk work such as formatting, minor wording changes, boilerplate,
  simple scaffolding, or repetitive low-risk edits.
- Tier 2: moderate-risk work such as nontrivial logic changes, internal
  utilities, meaningful refactors, data transformations, configuration changes,
  or workflow changes.
- Tier 3: high-risk work such as security-sensitive logic, core algorithms,
  irreversible operations, externally visible behavior changes, major design
  decisions, or claims a human may materially rely on.
- For Tier 2 work, state the key assumptions, identify at least one likely
  failure mode, and propose a validation method before recommending acceptance.
- For Tier 3 work, state the constraints, material assumptions, likely failure
  modes, at least one alternative or tradeoff, and concrete validation steps
  before recommending acceptance.
- Do not present substantive work as accepted, validated, or settled while the
  validation gap is still open.

## Proposal Status And Epistemic Discipline

- Keep proposal, implementation, validation, and acceptance status distinct.
- Label implemented facts as implemented facts.
- Label expectations, unverified behavior, inference, and hypothesis clearly.
- Do not imply that a human instruction to proceed means the human has accepted
  the result as correct or final.
- When confidence is limited, say so directly and identify what would reduce the
  uncertainty.

## Safety And Transparency

- Before making a substantive change, state what will be changed.
- After making a change, summarize what changed and where.
- If requested work conflicts with repository policy, surface the conflict
  explicitly before proceeding.
- If a guardrail is bypassed, identify the specific guardrail and the immediate
  reason for the exception.
- Treat overrides as operation-specific exceptions, not standing policy.

## Review Routing

- When asked for review, prioritize bugs, regressions, unsafe assumptions,
  missing validation, and policy mismatches.
- Separate findings from summaries.
- If no material findings are identified, say so explicitly and note remaining
  testing or validation gaps.
