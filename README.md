#  Universal Fable 5 Engine System Prompt

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![LLM Compatibility](https://img.shields.io/badge/Compatibility-Gemini%20%7C%20ChatGPT%20%7C%20Claude-blueOther_models%20%7C%20)

A high-performance, token-efficient distillation of the **leaked Claude Fable 5 / Mythos 5 system prompt** architecture. 

When the raw 120,000-character Anthropic system prompt was leaked, developers quickly realized it was too bloated for non-Claude models due to thousands of lines of environment-specific XML tools, safety overrides, and server-side functions. 

This repository fixes that. We have stripped away the proprietary Anthropic infrastructure bloat while perfectly preserving Fable 5's **autonomous reasoning, multi-turn horizon planning, self-verification loops, and distinct anti-chatbot behavioral rules**.

## 📊 Key Enhancements
* **Massive Token Savings:** Slashes prompt overhead from **~30,000 tokens down to ~500 tokens**, preventing context degradation and latency lag.
* **Universal Compatibility:** Removed Claude-native XML wrappers (`<antml>`) that break or confuse OpenAI's ChatGPT 5.5/5.6 or Google's Gemini 3.1 Pro/3.5 Flash.
* **Pure Operational Philosophy:** Retains the exact behavioral scaffolding that gives Fable 5 its elite, senior-engineer executive capabilities.

## 🛠️ How to Deploy

### For Google AI Studio / OpenAI Developer Platform:
Paste the raw text from `system_prompt.md` directly into the **System Instructions** wrapper of your model configuration.

### For Consumer Interfaces (ChatGPT Plus / Gemini Advanced):
* **ChatGPT:** Create a New GPT or paste the prompt text into your *Custom Instructions* profile settings.
* **Gemini Advanced:** Paste the text directly into the *Gems* builder system prompt panel.

## 🧠 Core Architectural Levers Preserved
1. **The Anti-Chatbot Prose Standard:** Actively forces the model out of typical conversational patterns (walls of bullets, aggressive nesting, fake enthusiasm) and mandates clean, high-density continuous prose.
2. **Structural Re-Deconstruction:** Prevents lazy summaries by forcing the model to systematically smash and rebuild incoming source data flows from scratch.
3. **No Thought Narration:** Shuts off conversational meta-commentary ("Let me think about that," "Now I will compute X"), saving user tokens and execution time.
4. **Zero-Engagement Traps:** Eliminates routine AI validation farming ("Let me know if you need more help!"). 

## 🤝 Contributing
Found a edge case where another frontier model misinterprets the prompt logic? Submit a Pull Request! Let's keep this prompt optimized for upcoming model architectures.
