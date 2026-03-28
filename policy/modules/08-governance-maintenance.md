# Governance Maintenance Module

Use this module when a repository wants explicit maintenance rules for a
segmented governance corpus.

## Maintenance Rules

- When governance structure changes, update the `AGENTS.md` entrypoint and the
  affected governance files in the same change.
- Prefer updating an existing domain file over creating a new one unless the
  policy surface is materially distinct.
- Preserve the chosen file-type split between human-facing orientation files
  and machine-loaded policy files unless there is a deliberate structural
  change.
- Keep governance file names stable and descriptive.
- Update path references in the same change when files move.
- Keep the governance index or README aligned with the actual structure.
- When changing operative wording, review nearby files for duplicated or
  conflicting rules.
- Treat the entrypoint as an index and loader, not as a second full copy of the
  policy body, when a segmented corpus is in use.
- Avoid expanding terse machine-loaded policy files into prose-heavy restatements
  that materially increase token cost without adding new policy meaning.
