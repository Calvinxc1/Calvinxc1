# Governance Structure Module

Use this module when a repository stores policy in a segmented governance
corpus rather than a single monolithic `AGENTS.md`.

## Entry Point And Precedence

- Keep the top-level `AGENTS.md` as the policy entrypoint and loading
  instructions, not the full policy body, when the repository uses a segmented
  governance corpus.
- Define precedence across the entrypoint, standing policy files, process
  files, and override records explicitly.
- If ambiguity remains after applying precedence rules, ask before acting.

## File Type Strategy

- Keep the human-facing entrypoint and orientation docs in Markdown when that
  makes the structure easier to understand quickly.
- Prefer concise structured files such as YAML for standing policy, routing
  maps, process rules, and override records when the goal is low-token machine
  loading.
- Use one structured format consistently across the segmented policy body
  unless there is a clear reason to mix formats.
- Keep machine-loaded policy files terse and declarative rather than rewriting
  long narrative guidance in every file.

## Segment Boundaries

- Keep standing policy in one dedicated namespace or directory.
- Keep process rules in a separate namespace or directory.
- Keep override records and their data definition separate from standing
  policy.
- Use an always-load baseline plus selectively loaded domain or task segments
  when that reduces unnecessary policy loading.
- Keep routing maps concise and descriptive rather than turning them into full
  policy bodies.
