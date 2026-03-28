# Enforcement Overrides Module

Use this module when a repository needs explicit rules for enforced controls,
temporary exceptions, and override records.

## Enforcement

- Distinguish between hard controls enforced by repository settings and softer
  defaults that rely on developer judgment.
- Enforced controls are mandatory unless they are temporarily bypassed for one
  specific declared operation.
- Unenforced controls remain discretionary defaults, but deliberate deviations
  should still be explicit and reasoned.
- Prefer documented defaults unless there is a clear reason to deviate.

## Override Governance

- Overrides must be explicit, case-specific, reasoned, temporary, and recorded
  when material.
- Override-governance rules are themselves non-overridable.
- An override is valid only for one explicitly declared operation.
- Mid-stream changes should amend the same override case instead of layering a
  new one on top.
- Overrides end when the supported operation completes.
- Restore bypassed protections or workflow state before the override is closed.
- If restoration cannot complete immediately, surface that as unresolved
  follow-up.
- Repeated materially similar overrides should trigger policy review.
- Override records document temporary exceptions; they do not replace standing
  policy.

## Override Records

- If the repository keeps an override log, define the required fields,
  restoration states, and amendment rule in one dedicated record format.
- Treat bypasses of meaningful safeguards, review expectations, or persistent
  workflow state as material overrides.
- Record the bypassed policy sections, immediate reason, exact exception,
  restoration status, and follow-up notes.
