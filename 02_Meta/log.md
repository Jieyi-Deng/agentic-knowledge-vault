# Wiki Log

This file records meaningful ingest, organization, lint, and update operations for the public demo vault.

## 2026-06-03

- Created a public-safe demonstration vault from the private `agentic-knowledge-vault` structure.
- Established the three-layer Raw / Wiki / Meta structure and preserved the class discussion raw note plus directly related processed notes.
- Added a public `README.md`, public-safe `AGENTS.md`, metadata schema, index, topic index, manifest, templates, and license.
- Copied `files/information_story.png` for the README information story diagram.
- Excluded private Git history, hidden configuration folders, unrelated notes, local caches, credentials, and unrelated source materials.

## 2026-06-19

- Renumbered the top-level folders to `00_Raw`, `01_Wiki`, and `02_Meta` for stable ordering, and updated every internal reference.
- Renamed the `UW` folders to `Class Notes` under both `00_Raw/Inbox/` and `01_Wiki/Projects/` to generalize away the course-specific name for public release.
- Flattened `01_Wiki/Projects/Class Notes/Portable_Information_Structures/` up one level into `01_Wiki/Projects/Class Notes/`.
- Ingested two new external sources and processed each into a source note plus a concept note:
  - `00_Raw/Sources/YouTube/Prompting 101 Code w Claude.md` -> `Prompting 101 - Code with Claude` source note and `Prompt Engineering Structure` concept.
  - `00_Raw/Sources/Web_Posts/Thariq - Using Claude Code - The Unreasonable Effectiveness of HTML.md` -> `Thariq - The Unreasonable Effectiveness of HTML` source note and `HTML as an Agent Output Format` concept.
- Cross-linked the new HTML concept into `FAIR Principles for Agentic Knowledge Bases`, which already discussed the Markdown-versus-HTML trade-off.
- Updated `02_Meta/index.md`, `02_Meta/topic_index.md`, and `02_Meta/vault_manifest.json` with the new sources and notes.
- Raw source files were not modified.
