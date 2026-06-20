---
title: "Prompting 101 - Code with Claude"
aliases: ["Prompting 101", "Code with Claude prompting talk", "Anthropic prompting best practices"]
type: "source_note"
status: "processed"
created: "2026-06-19"
updated: "2026-06-19"
tags: ["source-note", "prompt-engineering", "claude", "anthropic", "llm"]
summary: "Anthropic's Applied AI team walks through prompt-engineering best practices by iteratively building a single prompt for a Swedish car-insurance claim task, demonstrating a ten-part prompt structure."
source_paths:
  - "00_Raw/Sources/YouTube/Prompting 101 Code w Claude.md"
source_urls:
  - "https://www.youtube.com/watch?v=ysPbXH0LpIE"
related: ["[[Prompt Engineering Structure]]", "[[HTML as an Agent Output Format]]"]
source_type: "youtube_video"
author: "Anthropic Applied AI team (Hannah, Christian)"
platform: "YouTube"
date_accessed: "2026-05-05"
confidence: "high"
provenance: "Synthesized from the preserved raw transcript without modifying the raw source."
---
# Prompting 101 - Code with Claude

## Source Context

A 25-minute Anthropic "Code w/ Claude" session (published 2025-07-31) in which two Applied AI team members build a production-style prompt from scratch. The running example is inspired by a real customer: a Swedish insurance company that wants Claude to read a car-accident report form plus a hand-drawn sketch and judge who is at fault. The talk shows the prompt evolving across console versions (V1 to V4), with each version adding one best practice.

## Summary

Prompt engineering is framed as an iterative, empirical practice: write clear instructions, give the model the context it needs, and arrange that information well. For one-shot API tasks the recommended shape is a layered prompt that front-loads role and task, supplies stable background as structured context, gives step-by-step instructions, and constrains the output format. The demo shows measurable improvement as each layer is added.

## Key Claims

- A minimal prompt makes Claude guess; the V1 prompt led Claude to call the scene a "skiing accident" because nothing set the scene.
- Adding **task context** and **tone context** (stay factual, only assert when confident) moved Claude to the correct car-accident framing.
- Stable, unchanging material (the blank form structure) belongs in the **system prompt** and is a good candidate for **prompt caching**; it stops Claude re-deriving the form every call and improves reading accuracy.
- **Order of operations matters**: instructing Claude to read the form first and the sketch second mirrors how a human would reason and produced a more reliable verdict.
- A closing **reminder** of the immediate task and guardrails (do not invent details, say so if the sketch is unintelligible) reduces hallucination.
- **Output formatting** and **prefilled responses** let you extract just the machine-usable result (e.g., wrap the verdict in XML tags, or force JSON by prefilling an opening bracket).
- **Extended thinking** (Claude 3.7 and Claude 4 hybrid reasoning) can act as a "crutch" for prompt engineering: the scratchpad transcript reveals how the model reasons, which you can then fold back into the system prompt.

## Useful Details

- Console settings used in the demo: temperature 0 and a large max-token budget.
- The recommended prompt skeleton (expanded into [[Prompt Engineering Structure]]): task context, tone context, background data/documents/images, detailed task instructions, examples, conversation history, immediate task/reminder, think step by step, output formatting, prefilled response.
- **Delimiters**: XML tags (and Markdown) help Claude separate sections; Claude is fine-tuned to respond well to XML structure, and tags can be referenced later in the prompt.
- **Few-shot examples** can include base64-encoded images plus a description of how to interpret them; real applications may carry tens or hundreds of hard cases.
- Result progression: V1 wrong (skiing) -> V2 right framing but unsure of fault -> V3 confident "vehicle B at fault" once the form was described in the system prompt -> V4 succinct, strictly formatted, confident verdict.

## Connections

- [[Prompt Engineering Structure]] - the reusable concept extracted from this talk.
- [[HTML as an Agent Output Format]] - a complementary take on the *output* side of working with Claude.

## Open Questions

- How much of the ten-part structure is necessary for simpler tasks versus this multi-modal judgment task?
- When is extended thinking worth the extra tokens versus baking the reasoning into the system prompt?
