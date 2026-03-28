# Release Changelog Module

Use this module for repositories that keep a single changelog or release-notes
file as the main record of staged and released changes.

## Changelog Discipline

- Identify one authoritative changelog or release-notes file and keep that
  choice stable.
- Keep unreleased work in a dedicated staging section when the repository uses
  staged release notes.
- Update the changelog for user-visible, operator-visible, or otherwise
  release-relevant changes intended for the integration branch unless a human
  explicitly defers the entry.
- Internal-only changes need no changelog entry unless they materially affect
  contributors, operators, workflows, or documented behavior.
- When preparing a release, promote the staging section into a versioned
  release section and reset the staging area.
- If the changelog is not the authoritative current-version source, say that
  explicitly in the target repo's `AGENTS.md`.
- Flag missing changelog updates in review when a pull request changes
  release-relevant behavior.
