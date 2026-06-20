---
title: "Portable Information Structures"
aliases: ["PIS", "portable info structures"]
type: "concept_note"
status: "processed"
created: "2026-05-04"
updated: "2026-05-04"
tags: ["concept", "portable-information-structures", "metadata", "interoperability"]
summary: "Portable information structures are documented structures that preserve meaning, access, and reuse as information moves across contexts and systems."
source_paths:
  - "00_Raw/Inbox/Class Notes/Portable Information Structure - class discussion.md"
source_urls:
  - "https://strategy.data.gov/proof-points/2019/06/07/usagov-uses-human-centered-design-to-roll-out-ai-chatbot/"
  - "https://schema.org/"
  - "https://www.dbpedia.org/"
  - "https://www.storytellingwithdata.com/makeovers"
related: ["[[Data Portability vs Data Usability]]", "[[Information Stories]]", "[[FAIR Principles for Agentic Knowledge Bases]]", "[[Portable Information Structures - Weeks 1-5 Class Synthesis]]"]
confidence: "medium"
provenance: "Synthesized from the preserved public UW class-discussion raw note without modifying the raw source."
---
# Portable Information Structures

## Summary

A portable information structure is not merely a file that can be copied. It is a structured representation of information that can move across systems while preserving enough context, documentation, and semantics for humans and machines to understand and reuse it.

## Working Definition

**Portable information structure**: a standardized and documented format that enables user access, control, transfer, interpretation, and reuse across systems by using stable formats, metadata, identifiers, and shared semantics while managing privacy and security constraints.

## Core Properties

- **Standardized format**: the structure uses predictable conventions such as CSV, JSON, XML, RDF, Markdown, or a documented API schema.
- **Human readability**: a person can inspect the structure, understand labels, and infer what the fields mean.
- **Machine readability**: software can parse the structure reliably.
- **Self-descriptiveness**: metadata, data dictionaries, schemas, or field names explain what values mean.
- **Interoperability**: the structure can work across tools, platforms, or contexts with minimal transformation.
- **Reusability**: the structure can support future use cases beyond the original one.
- **Access and control**: users can obtain, move, and act on the information.
- **Privacy and security awareness**: portability does not expose sensitive data unnecessarily.

## Why Metadata Matters

Metadata makes portability meaningful because it carries interpretation with the data. Examples include:

- entity relationships
- data dictionaries
- lineage mappings
- schema and layout documentation
- identifiers such as URLs, URIs, and DOIs
- licensing and provenance

Without metadata, data can be moved but may lose meaning.

## Common Tensions

- Openness versus protection of sensitive information.
- Ease of transfer versus risk of misuse.
- Machine precision versus human inspectability.
- Standardization versus local context.
- Technical access versus practical usability.

## Examples

- A CSV is portable when headers and documentation make the fields interpretable.
- A JSON API is portable when its schema, identifiers, and field semantics are stable and documented.
- A knowledge graph is portable when shared vocabularies and ontologies allow relationships to be interpreted across contexts.
- This Markdown vault becomes more portable when every processed note has frontmatter, source paths, stable folders, and wikilinks.

## Related Notes

- [[Data Portability vs Data Usability]]
- [[FAIR Principles for Agentic Knowledge Bases]]
- [[Information Stories]]
- [[LLM Wiki as a Portable Information Structure]]
