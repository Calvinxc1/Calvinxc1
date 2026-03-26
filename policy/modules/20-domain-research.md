# Research Domain Module

Use this module for repositories centered on experiments, scientific modeling,
literature review, or research documentation.

## Research Document Standards

- Distinguish clearly between source-backed summary, inference, hypothesis,
  implementation assumption, recommendation, and future validation work.
- Use cautious modality where needed, such as `suggests`, `appears`,
  `hypothesis`, or `to be tested`.
- Do not claim downstream validity from a local prototype unless the relevant
  downstream evaluation was actually performed.
- When uncertainty language mixes cited practice with local implementation,
  identify which part is source-derived and which part is a local approximation.

## Citation Verification

- Cite only sources that actually support the claim being made.
- Label inference as inference rather than attributing it directly to the
  source.
- If a source was not checked directly, say so instead of implying verification.
- Do not compress multiple uncertain steps into a single authoritative claim.

## Research Review Workflow

- Before recommending acceptance of a substantive research claim, identify the
  claim, the evidence basis, the remaining uncertainty, and the next validation
  step.
- When reviewing notes or literature summaries, look for overclaiming, hidden
  assumptions, unsupported causal language, and mismatches between citation and
  conclusion.
- When reviewing prototype code or notebooks, distinguish exploratory utility
  from validated method quality.

## Research Folder Conventions

- Keep research topics organized in dedicated topic folders under a shared
  `research/` directory when the repo materially includes research work.
- Prefer each topic folder to include:
  - `README.md`
  - `literature-review.md`
  - `research-notes.md`
  - optional `research-notebook.ipynb`
  - optional `sources/`
- Use topic `README.md` files as orientation documents, not as full literature
  reviews.
- Keep shared indexes and cross-links updated when research folders are added,
  renamed, or materially restructured.
