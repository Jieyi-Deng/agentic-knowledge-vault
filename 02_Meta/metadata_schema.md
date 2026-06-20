# FAIR-lite Metadata Schema

This vault uses lightweight YAML frontmatter to make processed wiki notes findable, accessible, interoperable, and reusable without adding heavy database or ontology infrastructure.

## Scope

Apply this schema to processed notes under `01_Wiki/`. Raw files under `00_Raw/` remain immutable and do not need this frontmatter.

## Required Fields

Every processed note should include:

- title
- aliases
- type
- status
- created
- updated
- tags
- summary
- source_paths
- source_urls
- related

## Controlled Values

`type` should be one of:

- class_note
- source_note
- concept_note
- entity_note
- project_note
- area_note
- permanent_note
- question_note

`status` should be one of:

- draft
- processed
- reviewed
- evergreen
- archived

`confidence`, when used, should be one of:

- low
- medium
- high
- mixed

## Base Example

```yaml
---
title: ""
aliases: []
type: ""
status: ""
created: "YYYY-MM-DD"
updated: "YYYY-MM-DD"
tags: []
summary: ""
source_paths: []
source_urls: []
related: []
confidence: ""
provenance: ""
---
```

## Field Definitions

- `title`: Human-readable note title.
- `aliases`: Alternative names, abbreviations, or related search terms.
- `type`: Note class from the controlled values above.
- `status`: One of `draft`, `processed`, `reviewed`, `evergreen`, or `archived`.
- `created`: Date the processed note was created.
- `updated`: Date the note was last updated.
- `tags`: Topical tags using lowercase kebab-case.
- `summary`: One-sentence summary for quick search and agent navigation.
- `source_paths`: Local raw source paths from `00_Raw/`.
- `source_urls`: External URLs if available.
- `related`: Important Obsidian wikilinks.
- `confidence`: Optional confidence level for synthesis or extraction quality.
- `provenance`: Optional short explanation of how the note was produced.

## Optional Fields

- course
- week
- instructor
- source_type
- author
- platform
- date_accessed

## FAIR Alignment

- Findable: use clear titles, aliases, tags, summaries, and registry entries.
- Accessible: store notes as Markdown files in a Git-backed Obsidian vault.
- Interoperable: use Markdown, YAML frontmatter, ISO dates, and controlled fields.
- Reusable: preserve source paths, source URLs, provenance, status, and related links.

## Manifest Rule

When a processed note is created or meaningfully updated, add or update its lightweight routing entry in `02_Meta/vault_manifest.json`. The manifest should not contain full note text.
