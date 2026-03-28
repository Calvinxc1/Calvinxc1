# Research Structure Module

Use this module when a repository wants explicit rules for organizing research
topics, notes, notebooks, and source material.

## Folder Structure

- Keep shared research-process documents at the `research/` root and keep topic
  materials inside topic folders.
- Use lowercase hyphenated names by default.
- Standard topic structure is `README.md`, `literature-review.md`, optional
  `notes/`, optional `notebooks/`, and optional `sources/`.
- Keep `literature-review.md` at topic root as the canonical source-backed
  document.
- Keep general working notes under `notes/`, not at topic root.
- If `notes/` exists, include `notes/README.md` as the note index.
- Prefer multiple purpose-specific note files over one omnibus note file when
  content spans distinct themes.
- If `notebooks/` exists, include `notebooks/README.md` as the notebook index.
- Notebook filenames should describe the experiment or diagnostic they contain.
- Use `sources/` for local reference material and do not commit its contents
  unless explicitly directed.

## Cross-Linking

- Include notebooks only when there is an actual prototype, experiment trail,
  or diagnostic artifact.
- Treat topic notebooks as prototype artifacts, not canonical summaries.
- Topic `README.md` files should link to the main research files, give brief
  descriptions, and note maturity when helpful.
- Keep `research/README.md` as the shared index linking to topic `README.md`
  files.
- When one research topic depends materially on another, note that relationship
  in the dependent topic `README.md`.
- Use relative documentation links where practical.
- When restructuring research folders, update affected README references and
  preserve cross-link consistency in the same change.
