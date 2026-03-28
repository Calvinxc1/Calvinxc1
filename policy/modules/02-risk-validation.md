# Risk Validation Module

Use this module when a repository wants explicit risk tiers and minimum
validation gates for substantive work.

## Risk Tiers

- Classify substantive work before implementation or recommendation. If
  uncertain, classify at the higher tier.
- Tier 1: low-risk work such as formatting, minor wording changes, boilerplate,
  simple scaffolding, or repetitive low-risk edits.
- Tier 2: moderate-risk work such as nontrivial logic changes, internal
  utilities, meaningful refactors, data transformations, configuration changes,
  or workflow changes.
- Tier 3: high-risk work such as core algorithms, scientific or statistical
  logic, security-sensitive logic, architecture decisions, irreversible
  operations, or externally visible behavior changes.

## Validation Expectations

- For Tier 1 work, draft output is acceptable, but surface obvious assumptions
  or limitations when relevant.
- For Tier 2 work, state the key assumptions, identify at least one likely
  failure mode, provide at least one validation method or test, and distinguish
  implemented facts from expected behavior.
- For Tier 3 work, state the constraints, material assumptions, likely failure
  modes or edge cases, at least one alternative or tradeoff, concrete
  validation steps, and the remaining uncertainty.
- Do not present Tier 2 or Tier 3 work as accepted, validated, or settled
  while the relevant validation gap is still open.
- Require an explicit critique pass before recommending acceptance of Tier 2 or
  Tier 3 work.

## Validation Gates

- Code changes should cover intended behavior, assumptions, likely failure
  modes, validation steps, and the chosen approach versus at least one
  alternative when the tradeoff matters.
- Research work should distinguish source-backed material from inference or
  hypothesis and avoid hiding uncertainty behind authoritative phrasing.
- Architecture decisions should surface constraints, tradeoffs, alternatives,
  and operational failure modes.
