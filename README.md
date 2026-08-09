# Agentic Knowledge Vault: Markdown Knowledge Work for Humans and AI Agents

This repository is a sanitized public demonstration of a portable Markdown knowledge vault. It shows how a YouTube transcript and a saved web post can be transformed into structured notes that are readable in GitHub, useful in Obsidian, and easier for AI agents to search, interpret, and maintain.

## Information Story

Raw information often starts as a long transcript or web capture. It may be useful, but its length and inconsistent structure make it expensive to retrieve and reuse. This vault converts raw sources into structured Markdown files with YAML frontmatter, exact source paths, topic indexes, and links between related notes.

The human role is judgment: deciding what belongs in the vault, what should stay private, which sources are trustworthy, and whether a processed note is faithful. The agent role is execution under explicit project rules: formatting notes, adding metadata, linking related pages, updating indexes, preserving provenance, and checking for broken references.

The result has three layers: raw evidence remains available, processed notes explain and connect the source material, and lightweight metadata helps people and agents decide what to read next.

## Project Structure

Top-level folders use numbered prefixes so they sort in reading order: raw input first (`00_Raw`), processed knowledge next (`01_Wiki`), and navigation/governance metadata last (`02_Meta`).

```text
agentic-knowledge-vault/
├── 00_Raw/                         # Original source layer (immutable)
│   └── Sources/
│       ├── YouTube/
│       │   └── Prompting 101 Code w Claude.md
│       └── Web_Posts/
│           └── Thariq - ... - The Unreasonable Effectiveness of HTML.md
├── 01_Wiki/                        # Processed knowledge layer
│   ├── Concepts/
│   │   ├── Prompt Engineering Structure.md
│   │   └── HTML as an Agent Output Format.md
│   └── Source_Notes/
│       ├── Prompting 101 - Code with Claude.md
│       └── Thariq - The Unreasonable Effectiveness of HTML.md
├── 02_Meta/                        # Navigation and governance layer
│   ├── index.md
│   ├── topic_index.md
│   ├── vault_manifest.json
│   ├── metadata_schema.md
│   ├── log.md
│   └── templates/
├── AGENTS.md
├── LICENSE
└── README.md
```

## FAIR-Lite Principles

This project applies FAIR as a lightweight operating convention rather than as heavy research-data infrastructure.

- **Findable:** meaningful filenames, frontmatter titles, aliases, tags, summaries, topic indexes, and a machine-readable manifest.
- **Accessible:** plain Markdown and JSON that work in GitHub, Obsidian, terminal tools, and agent workflows.
- **Interoperable:** Markdown links, Obsidian wikilinks, YAML frontmatter, ISO dates, controlled note types, and consistent metadata fields.
- **Reusable:** exact source paths, source URLs, provenance, related notes, and reusable templates.

## Worked Examples

The repository contains two public examples:

- A YouTube transcript: [`00_Raw/Sources/YouTube/Prompting 101 Code w Claude.md`](00_Raw/Sources/YouTube/Prompting%20101%20Code%20w%20Claude.md)
- A web post: [`00_Raw/Sources/Web_Posts/Thariq - Using Claude Code - The Unreasonable Effectiveness of HTML.md`](00_Raw/Sources/Web_Posts/Thariq%20-%20Using%20Claude%20Code%20-%20The%20Unreasonable%20Effectiveness%20of%20HTML.md)

Each source demonstrates the same raw-to-processed workflow:

| Raw source | Source note | Extracted concept |
| --- | --- | --- |
| Prompting 101 (YouTube) | [Prompting 101 - Code with Claude](01_Wiki/Source_Notes/Prompting%20101%20-%20Code%20with%20Claude.md) | [Prompt Engineering Structure](01_Wiki/Concepts/Prompt%20Engineering%20Structure.md) |
| Thariq on HTML (web) | [Thariq - The Unreasonable Effectiveness of HTML](01_Wiki/Source_Notes/Thariq%20-%20The%20Unreasonable%20Effectiveness%20of%20HTML.md) | [HTML as an Agent Output Format](01_Wiki/Concepts/HTML%20as%20an%20Agent%20Output%20Format.md) |

## How To Use This Vault

### 1. Route before reading

Start with [`02_Meta/index.md`](02_Meta/index.md), [`02_Meta/topic_index.md`](02_Meta/topic_index.md), and [`02_Meta/vault_manifest.json`](02_Meta/vault_manifest.json). These files provide enough metadata to select relevant notes before opening long raw sources.

### 2. Preserve raw evidence

Place a new source under the matching `00_Raw/` subfolder. Use `00_Raw/Inbox/` for user-provided material awaiting processing, `00_Raw/Sources/YouTube/` or `00_Raw/Sources/Web_Posts/` for stable external captures, and `00_Raw/Assets/` for attachments. Do not rewrite a raw source in place.

### 3. Create processed notes

Use the templates in `02_Meta/templates/` to create notes under `01_Wiki/`. A useful default is one **source note** that faithfully summarizes and routes the source, plus focused **concept notes** for ideas worth reusing.

Every processed note should:

- follow the [`02_Meta/metadata_schema.md`](02_Meta/metadata_schema.md) frontmatter schema;
- point `source_paths` to the exact raw file;
- preserve external URLs and transformation provenance;
- use Obsidian semantic links only for notes that exist;
- distinguish source claims from agent synthesis.

### 4. Update routing metadata

After creating or changing a processed note:

- add it to [`02_Meta/index.md`](02_Meta/index.md);
- add it to the relevant cluster in [`02_Meta/topic_index.md`](02_Meta/topic_index.md);
- add or update its entry in [`02_Meta/vault_manifest.json`](02_Meta/vault_manifest.json);
- record meaningful maintenance in [`02_Meta/log.md`](02_Meta/log.md).

Keep these files lightweight. They are routing tools, not copies of note content.

### 5. Use with an AI agent

Use [`AGENTS.md`](AGENTS.md) as the project-level operating instructions. A typical request is: *"Read the index, topic index, manifest, and metadata schema first. Then process the new YouTube transcript into a source note and any reusable concept notes, update routing metadata, and verify links and provenance."*

> [!TIP]
> Companion agent skills are maintained separately. Browse the [`skills/` directory in `Jieyi-Deng/jieyi-skills`](https://github.com/Jieyi-Deng/jieyi-skills/tree/main/skills) for the skills used with this vault.

## Public Release Scope

The public demo intentionally contains only the two external sources above and their four directly derived processed notes. Personal notes, coursework, private account data, credentials, hidden configuration, caches, and unrelated source material are excluded.

## License

This project is released under the Creative Commons Attribution 4.0 International License. See `LICENSE` for details.
