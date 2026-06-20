---
title: "Data Portability vs Data Usability"
aliases: ["portable does not mean usable", "data usability"]
type: "concept_note"
status: "processed"
created: "2026-05-04"
updated: "2026-05-04"
tags: ["concept", "data-portability", "usability", "accessibility"]
summary: "Data can be portable without being usable when meaning, context, tools, size, access paths, or user needs are not preserved."
source_paths:
  - "00_Raw/Inbox/Class Notes/Portable Information Structure - class discussion.md"
source_urls:
  - "https://strategy.data.gov/proof-points/2019/06/07/usagov-uses-human-centered-design-to-roll-out-ai-chatbot/"
  - "https://schema.org/"
  - "https://www.dbpedia.org/"
  - "https://www.storytellingwithdata.com/makeovers"
related: ["[[Portable Information Structures]]", "[[Information Stories]]", "[[FAIR Principles for Agentic Knowledge Bases]]"]
confidence: "medium"
provenance: "Synthesized from the preserved public UW class-discussion raw note without modifying the raw source."
---
# Data Portability vs Data Usability

## Summary

The course repeatedly separates the ability to move data from the ability to use it meaningfully. Portability is necessary but insufficient: a dataset may be downloadable, exportable, or transferable while still being unreadable, too large, poorly documented, redacted, locked into an ecosystem, or detached from the user’s actual goal.

## Portability

Data portability often refers to a user’s ability to take data from one service and move it elsewhere. It supports:

- user control
- backups
- reduced vendor lock-in
- competition between platforms
- transfer to third parties
- integration with other systems

## Usability

Usability asks whether the moved data can actually be interpreted and acted on. It depends on:

- understandable labels and field names
- documentation and metadata
- file size and technical constraints
- availability of tools to open or process the data
- preservation of meaning across systems
- alignment with a user need or information story

## Why the Distinction Matters

Examples from class show that information can be technically available but practically unusable:

- FOIA materials delivered as zipped scans or heavy redactions.
- Government data published in multiple formats but difficult for non-experts to understand.
- Tax information that exists but is too complex for ordinary citizens.
- A large class file that crashed student devices.
- A JSON format that is technically rich but less inspectable for stakeholders who expect CSV.

## Design Implication

A good portable information structure should be designed for movement, interpretation, and action. It should carry enough context to be reusable without assuming that the next user already knows the original system.

## Related Notes

- [[Portable Information Structures]]
- [[Information Stories]]
- [[FAIR Principles for Agentic Knowledge Bases]]
