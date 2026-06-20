---
title: "How should an LLM wiki apply FAIR principles"
aliases: ["FAIR for LLM wiki", "How to make an agent wiki FAIR"]
type: "question_note"
status: "processed"
created: "2026-05-04"
updated: "2026-05-04"
tags: ["question", "fair", "llm-wiki", "agentic-ai", "metadata"]
summary: "An LLM wiki applies FAIR by making raw sources and processed notes findable, accessible, interoperable, and reusable through paths, metadata, links, and provenance."
source_paths:
  - "00_Raw/Inbox/Class Notes/Portable Information Structure - class discussion.md"
source_urls:
  - "https://strategy.data.gov/proof-points/2019/06/07/usagov-uses-human-centered-design-to-roll-out-ai-chatbot/"
  - "https://schema.org/"
  - "https://www.dbpedia.org/"
  - "https://www.storytellingwithdata.com/makeovers"
related: ["[[LLM Wiki as a Portable Information Structure]]", "[[FAIR Principles for Agentic Knowledge Bases]]", "[[Portable Information Structures]]"]
confidence: "medium"
provenance: "Synthesized from the preserved public UW class-discussion raw note without modifying the raw source."
---
# How should an LLM wiki apply FAIR principles?

## Short Answer

An LLM wiki should apply FAIR by preserving raw sources, creating processed Markdown notes with consistent metadata, linking concepts with wikilinks, keeping lightweight indexes and manifests, and recording provenance so humans and agents can find, interpret, and reuse knowledge later.

## Practical Mapping

### Findable

- Use clear filenames.
- Add YAML frontmatter with `title`, `aliases`, `tags`, and `summary`.
- Maintain `02_Meta/index.md`, `02_Meta/topic_index.md`, and `02_Meta/vault_manifest.json`.
- Use wikilinks between related concepts, projects, source notes, and questions.

### Accessible

- Store notes as plain Markdown files.
- Keep raw sources under `00_Raw/` and processed notes under `01_Wiki/`.
- Use Git for synchronization and history.
- Preserve source paths so future agents can locate original context.

### Interoperable

- Use consistent YAML fields and controlled values.
- Prefer ISO dates.
- Keep metadata lightweight and machine-readable.
- Use standard formats such as Markdown, JSON manifests, CSV, JSON, and APIs when appropriate.

### Reusable

- Preserve provenance and transformation context.
- Link processed ideas back to raw sources.
- Extract reusable concepts into `01_Wiki/Concepts/`.
- Create project and question notes when an insight is likely to be useful again.

## Why This Matters

Without FAIR practices, an agent may have to repeatedly re-read raw notes, infer structure again, or answer from incomplete context. FAIR-lite turns the wiki into a portable information structure: compact enough for agents, readable enough for humans, and structured enough for future reuse.

## Related Notes

- [[FAIR Principles for Agentic Knowledge Bases]]
- [[LLM Wiki as a Portable Information Structure]]
- [[Portable Information Structures]]
