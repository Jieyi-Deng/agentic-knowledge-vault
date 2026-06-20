---
title: "LLM Wiki as a Portable Information Structure"
aliases: ["LLM Wiki project", "agentic wiki project"]
type: "project_note"
status: "processed"
created: "2026-05-04"
updated: "2026-05-04"
tags: ["project", "llm-wiki", "portable-information-structures", "fair", "agentic-ai"]
summary: "The LLM Wiki project applies portable information structure and FAIR-lite ideas to a Git-backed Markdown knowledge base for personal AI agents."
source_paths:
  - "00_Raw/Inbox/Class Notes/Portable Information Structure - class discussion.md"
source_urls:
  - "https://strategy.data.gov/proof-points/2019/06/07/usagov-uses-human-centered-design-to-roll-out-ai-chatbot/"
  - "https://schema.org/"
  - "https://www.dbpedia.org/"
  - "https://www.storytellingwithdata.com/makeovers"
related: ["[[Portable Information Structures]]", "[[FAIR Principles for Agentic Knowledge Bases]]", "[[Information Stories]]", "[[Data Portability vs Data Usability]]"]
confidence: "medium"
provenance: "Synthesized from the preserved public UW class-discussion raw note without modifying the raw source."
---
# LLM Wiki as a Portable Information Structure

## Summary

The raw notes include a project idea: integrate personal experience and online open resources into a wiki for a personal AI agent by organizing raw source materials into a persistent, interconnected Markdown wiki. This project is a direct example of a portable information structure.

## Information Story

As a person using AI agents for learning and research, I need my raw sources, processed notes, and reusable concepts organized into a persistent, indexed Markdown wiki so that future agents can answer questions without re-reading every original source and without losing provenance.

## Why This Is a Portable Information Structure

The project is portable because it uses:

- **Markdown** for human-readable and tool-friendly notes.
- **Git** for versioning, synchronization, and provenance.
- **YAML frontmatter** for lightweight FAIR metadata.
- **Wikilinks** for local semantic relationships.
- **Stable folders** separating raw sources from processed wiki notes.
- **Indexes and manifests** for agent routing and retrieval.

## FAIR Mapping

- **Findable**: notes have frontmatter titles, aliases, tags, summaries, and manifest entries.
- **Accessible**: files are plain Markdown in a Git repository on the server.
- **Interoperable**: notes use controlled `type`, `status`, `source_paths`, `source_urls`, and `related` fields.
- **Reusable**: raw sources are preserved, processed notes link back to sources, and concepts are extracted for future synthesis.

## Design Decisions

### Raw layer

`00_Raw/` should remain immutable so future processing can always return to original context.

### Wiki layer

`01_Wiki/` should contain cleaned, connected notes that are useful for learning, answering questions, and creating new artifacts.

### Meta layer

`02_Meta/` should remain lightweight and navigation-oriented. Its purpose is not to store full content, but to help agents decide what to read next.

## Risks and Constraints

- Over-summarization can erase useful context.
- Too many notes without metadata can reduce findability.
- Too much metadata can create maintenance overhead.
- Agents must not store secrets or private credentials in the vault.
- Raw sources should not be edited during processing.

## Next Improvements

- Add more concept pages as repeated themes appear.
- Add source-note entries for major readings or web resources.
- Periodically lint for orphan notes and duplicate concepts.
- Consider defining a small controlled vocabulary for tags.

## Related Notes

- [[Portable Information Structures]]
- [[FAIR Principles for Agentic Knowledge Bases]]
- [[Information Stories]]
- [[Data Portability vs Data Usability]]
