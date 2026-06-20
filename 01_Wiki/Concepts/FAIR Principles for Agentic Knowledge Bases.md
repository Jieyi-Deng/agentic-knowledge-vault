---
title: "FAIR Principles for Agentic Knowledge Bases"
aliases: ["FAIR for agents", "agentic FAIR", "FAIR-lite"]
type: "concept_note"
status: "processed"
created: "2026-05-04"
updated: "2026-05-04"
tags: ["concept", "fair", "agentic-ai", "knowledge-base", "metadata"]
summary: "FAIR principles can be adapted for agentic knowledge bases by making notes findable, accessible, interoperable, and reusable for both humans and AI agents."
source_paths:
  - "00_Raw/Inbox/Class Notes/Portable Information Structure - class discussion.md"
source_urls:
  - "https://strategy.data.gov/proof-points/2019/06/07/usagov-uses-human-centered-design-to-roll-out-ai-chatbot/"
  - "https://schema.org/"
  - "https://www.dbpedia.org/"
  - "https://www.storytellingwithdata.com/makeovers"
related: ["[[Portable Information Structures]]", "[[LLM Wiki as a Portable Information Structure]]", "[[Data Portability vs Data Usability]]", "[[HTML as an Agent Output Format]]"]
confidence: "medium"
provenance: "Synthesized from the preserved public UW class-discussion raw note without modifying the raw source."
---
# FAIR Principles for Agentic Knowledge Bases

## Summary

The class discussion extends FAIR beyond research datasets. If an AI agent creates or consumes a knowledge base, the knowledge base should also be findable, accessible, interoperable, and reusable so future humans and agents can interpret it without rebuilding context from scratch.

## FAIR for Agentic Systems

### Findable

Agentic notes should have:

- clear titles and aliases
- stable file paths
- frontmatter summaries
- tags
- indexes
- manifest entries
- wikilinks and backlinks

For this vault, `02_Meta/index.md`, `02_Meta/topic_index.md`, and `02_Meta/vault_manifest.json` provide findability.

### Accessible

Information should be retrievable through simple, durable mechanisms:

- Markdown files in Git
- predictable folder structure
- open text formats
- source paths to raw notes

Access does not always mean public access. Sensitive or private information may be restricted while metadata remains useful.

### Interoperable

Agentic notes should use structures that both humans and machines understand:

- Markdown body text
- YAML frontmatter
- ISO dates
- controlled `type` and `status` values
- consistent source-path fields
- Obsidian wikilinks

This makes the vault usable by Obsidian, shell tools, GitHub, scripts, and AI agents.

### Reusable

Reusable agentic knowledge should preserve:

- provenance
- source paths and source URLs
- transformation notes
- confidence levels when synthesis is uncertain
- related concepts and projects
- licensing or access context when known

## Design Insight

The class noted that HTML is machine-renderable and semantically rich, while Markdown is compact and agent-friendly. For an LLM wiki, Markdown can be a good portable structure, but only if metadata and links compensate for context that may otherwise be lost. See [[HTML as an Agent Output Format]] for a practical version of this same trade-off when an agent decides how to present its output.

## Related Notes

- [[Portable Information Structures]]
- [[LLM Wiki as a Portable Information Structure]]
- [[Data Portability vs Data Usability]]
- [[HTML as an Agent Output Format]]
