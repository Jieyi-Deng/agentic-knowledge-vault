---
title: "Portable Information Structures - Weeks 1-5 Class Synthesis"
aliases: ["PIS class synthesis", "UW PIS weeks 1-5"]
type: "class_note"
status: "processed"
created: "2026-05-04"
updated: "2026-05-04"
tags: ["uw", "portable-information-structures", "information-architecture", "fair", "data-portability"]
summary: "Weeks 1-5 frame portable information structures as human-and-machine-readable structures that preserve meaning, access, interoperability, and reuse across contexts while managing privacy and security."
source_paths:
  - "00_Raw/Inbox/Class Notes/Portable Information Structure - class discussion.md"
source_urls:
  - "https://strategy.data.gov/proof-points/2019/06/07/usagov-uses-human-centered-design-to-roll-out-ai-chatbot/"
  - "https://schema.org/"
  - "https://www.dbpedia.org/"
  - "https://www.storytellingwithdata.com/makeovers"
related: ["[[Portable Information Structures]]", "[[Data Portability vs Data Usability]]", "[[Information Stories]]", "[[FAIR Principles for Agentic Knowledge Bases]]", "[[LLM Wiki as a Portable Information Structure]]"]
confidence: "medium"
provenance: "Synthesized from the preserved public UW class-discussion raw note without modifying the raw source."
course: "UW Portable Information Structures"
week: "1-5"
instructor: ""
---
# Portable Information Structures - Weeks 1-5 Class Synthesis

## Summary

The first five weeks build a working view of portable information structures: they are not merely files that can be moved, but designed structures that keep data meaningful, interpretable, accessible, and reusable across contexts. The course repeatedly connects technical formats such as CSV, JSON, RDF, XML, APIs, Markdown, and knowledge graphs with social questions about users, access, privacy, power, and organizational decision-making.

## Integrated Definition

A **portable information structure** is a standardized, documented, human-and-machine-readable structure that enables user access, control, transfer, interpretation, and reuse across systems by using stable formats, metadata, identifiers, and shared semantics while addressing privacy, security, and contextual constraints.

This definition synthesizes the class exercise that identified these recurring properties:

- standardized formats
- human and machine readability
- user access and control
- transfer across systems
- reusability
- privacy and security constraints
- FAIR alignment: findable, accessible, interoperable, reusable

## Week-by-Week Development

### Week 1 — Information structure as human and technical design

Key distinction:

- **Information system**: broader environment through which people access, manage, and use information.
- **Information structure**: a more specific organization of information inside a system, such as a Canvas course, CSV file, JSON object, data dictionary, schema, or API response.

The course introduction emphasized that technically correct structures can still fail if they do not match stakeholder needs. The startup example of JSON versus CSV showed that the best structure is not only a technical question; it also depends on what users can inspect, trust, open, and use.

Important concepts introduced:

- focus, givenness, and topic as linguistic roots of information structure
- structured versus unstructured data
- metadata as context for interpretation
- human readability and computer readability as joint design requirements
- information formats as part of course practice

### Week 2 — Access, portability, and social consequences

The access-to-information discussion reframed access as more than availability. Information may technically exist but still be unusable if it is hidden in scans, oversized files, redactions, inaccessible formats, or systems that ordinary users cannot navigate.

Examples included:

- data.gov formats: CSV, RDF, JSON, XML, TIFF, PDF, HTML
- FOIA reading rooms and redacted/scanned documents
- Federal Depository Libraries as preservation and access infrastructure
- Flint water crisis and air-quality data as examples where access affects accountability
- tax-code opacity and performance reviews as examples of information, power, and institutional control

The portability discussion moved from data movement to meaningful reuse. Data portability was connected to:

- user rights over personal data
- transfer between services
- prevention of vendor lock-in
- interoperability and competition
- privacy and security risks

A central insight emerged: **portable does not automatically mean usable**.

### Week 3 — Definitions, knowledge graphs, integration, and machine use

The class collectively coded definitions of portable information structures and converged on terms such as interoperability, standardized formats, self-descriptiveness, transparency, user access and control, reusability, privacy, and security.

The week also connected PIS to:

- knowledge graphs
- schema.org
- DBpedia
- linked open data
- data integration
- API-based access
- human-centered chatbot design
- domain knowledge as a way to make data more self-descriptive

The discussion of business intelligence was especially important. BI systems take distributed data sources, ETL them, map them with metadata, and produce views that answer specific questions. This parallels PIS design: an information structure becomes more useful when it is organized around a user need, business question, or information story.

Machine-machine and machine-human translation were separated:

1. **Machine-machine structuring** creates integrated datasets or APIs from distributed information systems.
2. **Machine-human translation** makes structured information operable, comprehensible, and useful to people.
3. Additional analysis, prediction, visualization, or automation makes the structure valuable for a specific task.

### Week 4 — Information architecture, user stories, and product development

Week 4 moved from data structure toward architecture and product design. The architecture discussion emphasized inhabiting the user’s space, understanding objects and contexts, and resisting the tendency to design around a technology rather than the user.

User stories were described as **boundary objects**: flexible artifacts that help groups coordinate around what people are trying to do. In this course, information stories adapt that idea by asking what information a person needs, from where, in what structure, and for what goal.

The Keller & Lima digital information product development reading introduced NPD stages:

- idea generation
- idea validation
- product creation
- product launch

This supports the course’s project logic: start from a user story and need, not from available data alone. Data becomes useful only when it serves a validated purpose.

Week 4 also reviewed file formats and access technologies:

- text-readable formats: text, JSON, XML, HTML, Markdown, CSV, RSS, YAML, RDF
- binary/proprietary formats: PDF, JPG, ZIP, MP3, MP4, executable and application-specific formats
- access methods: API, curl, SCP, SFTP, SSH, CLI, SDK, web scraping

### Week 5 — FAIR principles and agentic reuse

FAIR was introduced as a rubric for making data and metadata:

- **Findable**: indexed, referenced by URIs/DOIs, searchable by humans and machines.
- **Accessible**: retrievable through standard protocols with appropriate authorization.
- **Interoperable**: using stable syntax, recognized vocabularies, documented relationships, and integration-ready metadata.
- **Reusable**: rich metadata, licensing clarity, transformation provenance, community standards, and human/machine usability.

The discussion explicitly connected FAIR to agentic systems: a GenAI or AI agent that creates knowledge-base facts should also follow FAIR principles so that future agents and humans can locate, interpret, and reuse the information. Markdown may be compact and agent-friendly, while HTML may preserve rendering semantics; choosing a format is therefore a portability design decision.

## Important Concepts

- [[Portable Information Structures]]
- [[Data Portability vs Data Usability]]
- [[Information Stories]]
- [[FAIR Principles for Agentic Knowledge Bases]]
- information architecture
- structured and unstructured data
- metadata and data dictionaries
- FAIR metadata
- APIs and machine access
- knowledge graphs and ontologies
- business intelligence views
- user stories and boundary objects
- new product development for information products

## Assignment Relevance

The raw notes mention several assignment patterns:

- I2: connect portability to integration and produce JSON or CSV from an existing source.
- G3: produce an information story and possible structure.
- I3: build a lightweight application to visualize, predict, automate, or analyze something using an information structure.
- G4: develop user story, wireframes, concepts, and system architecture.
- G5: apply FAIR principles and evaluate examples.

For this vault, the most relevant assignment thread is the user’s project idea: an LLM wiki that organizes raw source materials into a persistent, interconnected Markdown knowledge base for AI agents. That project maps directly to FAIR by using frontmatter, stable paths, indexes, source provenance, and wikilinks.

## Discussion Questions

- When is information technically accessible but not practically usable?
- What metadata is necessary for a structure to remain interpretable across contexts?
- How much context should travel with data during portability?
- How can portability be designed without increasing privacy and security risk?
- What does FAIR mean when the future user is an AI agent rather than a human researcher?
- When should a structure prioritize human readability over machine precision, or vice versa?

## Possible Connections

- [[LLM Wiki as a Portable Information Structure]] is a direct application of the course ideas.
- [[FAIR Principles for Agentic Knowledge Bases]] turns the Week 5 discussion into operational design rules for this vault.
- [[Information Stories]] connects project design to user-centered information architecture.
- [[Data Portability vs Data Usability]] captures the course’s recurring distinction between movement and meaningful reuse.
