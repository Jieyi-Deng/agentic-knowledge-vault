---
title: "Prompt Engineering Structure"
aliases: ["prompt structure", "anatomy of a prompt", "ten-part prompt"]
type: "concept_note"
status: "processed"
created: "2026-06-19"
updated: "2026-06-19"
tags: ["concept", "prompt-engineering", "claude", "llm", "human-ai-workflow"]
summary: "A layered prompt structure - role, context, instructions, examples, reminders, and output controls - that makes one-shot LLM tasks more reliable."
source_paths:
  - "00_Raw/Sources/YouTube/Prompting 101 Code w Claude.md"
source_urls:
  - "https://www.youtube.com/watch?v=ysPbXH0LpIE"
related: ["[[Prompting 101 - Code with Claude]]", "[[HTML as an Agent Output Format]]", "[[FAIR Principles for Agentic Knowledge Bases]]"]
confidence: "high"
provenance: "Synthesized from the Prompting 101 raw transcript without modifying the raw source."
---
# Prompt Engineering Structure

## Summary

Prompt engineering is the practice of writing clear instructions, supplying the context the model needs, and arranging that information well. For a task you want a model to "nail the first time" through the API, a predictable, layered prompt structure works better than a conversational back-and-forth. The structure below comes from Anthropic's [[Prompting 101 - Code with Claude]] walkthrough.

## The Layered Structure

A full prompt can be built from up to ten ordered components. Not every task needs all of them, but the order is deliberate: set the scene before giving data, give data before instructions, and constrain the output last.

1. **Task context** - the role and what the model is here to accomplish.
2. **Tone context** - how it should behave (e.g., stay factual, only assert when confident).
3. **Background data, documents, and images** - stable reference material. Put unchanging content in the system prompt; it is a good candidate for prompt caching.
4. **Detailed task instructions** - a step-by-step list. Order matters: have the model process information in the order a careful human would.
5. **Examples (few-shot)** - worked input/output pairs, including images, that steer hard cases.
6. **Conversation history** - prior turns, when the task is user-facing and context-rich.
7. **Immediate task / reminder** - restate the current request.
8. **Think step by step** - allow reasoning space; extended thinking exposes a scratchpad you can inspect.
9. **Output formatting** - constrain the result (e.g., wrap the answer in XML tags) so it is easy to parse.
10. **Prefilled response** - put the first tokens in the model's mouth (an opening bracket or tag) to force JSON or a specific format.

## Supporting Techniques

- **Delimiters**: XML tags (or Markdown) separate sections and can be referenced later in the prompt; models are tuned to respond well to clear structure.
- **System prompt + caching**: stable material that never changes between calls is cheaper and more accurate when cached.
- **Empirical iteration**: treat prompting as an experiment - add one element, observe the change, and fold useful reasoning back into the system prompt.

## Why It Matters

A minimal prompt forces the model to guess at the scene and the goal. Each layer removes a class of guesswork: context fixes framing, instructions fix process, output controls fix parsing. The result is more reliable, more confident, and more machine-usable output.

## Related Notes

- [[Prompting 101 - Code with Claude]]
- [[HTML as an Agent Output Format]]
- [[FAIR Principles for Agentic Knowledge Bases]]
