# Universal Fable 5 System Prompt

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Compatibility](https://img.shields.io/badge/Compatibility-Claude%20%7C%20ChatGPT%20%7C%20Gemini%20%7C%20DeepSeek%20%7C%20Qwen-blue)

A vendor-neutral adaptation of Anthropic's publicly available **Claude Fable 5 / Mythos 5** system prompt.

The original prompt contains a large amount of infrastructure that exists specifically for Claude's production environment, including XML conventions, tool interfaces, product-specific behavior, and internal implementation guidance. While appropriate for Claude, much of that content provides little or no benefit when reused with other frontier LLMs.

This repository filters out those implementation details while retaining the behavioral guidance that generalizes well across modern models.

---

## Goals

* Reduce prompt size for better context efficiency.
* Remove Claude-specific implementation details.
* Preserve high-impact behavioral guidance.
* Maintain compatibility across major frontier LLMs.

---

## Versions

| File                    | Purpose                                                                               |
| ----------------------- | ------------------------------------------------------------------------------------- |
| `universal/core.md`     | Core behavioral principles with minimal token usage.                                  |
| `universal/balanced.md` | Recommended for most use cases. Balances prompt size with behavioral coverage.        |
| `universal/complete.md` | Retains nearly all vendor-neutral behavioral guidance while remaining model-agnostic. |

---

## What's Removed

This project intentionally excludes Claude-specific implementation such as:

* XML wrappers and formatting conventions
* MCP and tool-specific infrastructure
* Product-specific instructions
* Internal UI behavior
* Storage and artifact management
* Environment-specific implementation details

---

## What's Preserved

The filtered prompts retain behavioral guidance including:

* Understanding user intent before responding
* Honest handling of uncertainty
* Clear communication and natural writing
* High-quality code generation
* Practical recommendations with trade-off analysis
* Verification before finalizing responses
* Objective error correction
* Avoiding unnecessary meta-commentary

---

## Compatibility

The prompts are designed to work well across modern frontier models, including:

* Claude
* ChatGPT
* Gemini
* DeepSeek
* Qwen
* Grok
* GLM
* Other instruction-following LLMs

---

## Usage

### API Platforms

Paste the contents of the desired prompt into your model's system prompt or system instructions field.

### Consumer Interfaces

Where supported, the prompts can also be used as custom instructions, custom GPT system prompts, Gems, or equivalent features.

---

## Philosophy

This project is not intended to replace Anthropic's original system prompt or claim to improve it.

Instead, it asks a different question:

> **Which behavioral principles from Claude's system prompt remain valuable after removing implementation details that are specific to Claude itself?**

The result is a set of prompts optimized for portability rather than platform-specific functionality.

---

## Contributing

Contributions are welcome.

If you discover vendor-specific behavior that should be generalized, redundant instructions that can be simplified, or opportunities to improve compatibility across modern LLMs, feel free to open an issue or submit a pull request.
