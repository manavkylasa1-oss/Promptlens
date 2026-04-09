# 🔍 PromptLens

> **See your prompts clearly. Get exactly what you want from AI.**

PromptLens is an open-source prompt engineering framework that teaches anyone — beginner or expert — how to write better prompts for any AI model. Instead of silently rewriting your prompt, PromptLens **shows you what's wrong and why**, so you get smarter over time.

---

## Why PromptLens?

Most people use AI like a search engine. They type a vague question and hope for the best.

The result? Generic answers. AI-sounding text. Made-up statistics. Missed context. Frustration.

PromptLens fixes this by showing you **how an LLM actually thinks** — and coaching you to work with it, not against it.

---

## What It Does

When you run your prompt through PromptLens, it:

1. **Diagnoses your prompt** — scores it across 6 dimensions with clear explanations
2. **Shows you what's wrong** — in plain English, no jargon
3. **Reveals hidden risks** — hallucination triggers, token waste, context gaps
4. **Offers an improved prompt** — which you can accept, tweak, or reject
5. **Teaches the lesson** — so your next prompt is better without needing help

---

## The 6 Dimensions PromptLens Scores

| Dimension | What It Checks |
|---|---|
| 🎯 **Clarity** | Is your request unambiguous? |
| 📐 **Specificity** | Have you given enough detail? |
| 🧠 **Context** | Does the AI have enough background? |
| 🌀 **Hallucination Risk** | Are you inviting the AI to make things up? |
| 🪙 **Token Efficiency** | Are you wasting tokens on unnecessary words? |
| 🧩 **Context Window Usage** | Are you using your context window wisely? |

---

## How to Use PromptLens

PromptLens works with **any LLM** — Claude, ChatGPT, DeepSeek, Gemini, or any other.

### Option 1 — Paste into any AI chat (easiest)
1. Open `promptlens.md`
2. Copy the entire contents
3. Paste it as your **first message** in any AI chat (Claude, ChatGPT, etc.)
4. The AI will now act as PromptLens for that session
5. Paste any prompt you want analyzed and hit send

### Option 2 — Use as a System Prompt (for power users)
If your AI interface supports system prompts (e.g. ChatGPT API, Claude API, Open WebUI):
1. Copy the contents of `promptlens.md`
2. Set it as your system prompt
3. Every conversation will automatically use PromptLens

### Option 3 — Claude Skill (for Claude Code users)
1. Copy the `skill/` folder into your Claude skills directory
2. PromptLens will auto-trigger whenever you ask for prompt help

---

## Example

**Before PromptLens:**
```
write me an essay about climate change
```

**After PromptLens diagnosis:**
- Clarity: 5/10 — What angle? What argument?
- Specificity: 2/10 — No length, no audience, no format
- Hallucination Risk: 6/10 — Will likely invent statistics
- Token Efficiency: 3/10 — Three words to describe a complex task wastes the model's potential

**PromptLens improved prompt:**
```
Write a 600-word argumentative essay on the economic costs of delaying climate action.
Audience: university students. Tone: direct and evidence-based. Structure: intro, 3 argument
paragraphs, conclusion. Do not invent statistics — flag where data should be verified.
Avoid filler phrases like "It is important to note" or "In conclusion".
```

See more examples in the `/examples` folder.

---

## Repository Structure

```
promptlens/
├── README.md              ← You are here
├── promptlens.md          ← Universal system prompt (paste into any AI)
├── LICENSE                ← MIT License
├── skill/
│   └── SKILL.md           ← Claude skill file
└── examples/
    ├── homework.md        ← Student / homework scenarios
    ├── reports.md         ← Professional reports and documents
    ├── coding.md          ← Code generation prompts
    └── research.md        ← Research and factual queries
```

---

## Contributing

PromptLens is open source and community-driven. Contributions welcome!

- 🐛 Found a gap in the framework? Open an issue
- 💡 Have a new example or dimension? Submit a pull request
- 🌍 Want to translate PromptLens? Fork and go!

Please read `CONTRIBUTING.md` before submitting a pull request.

---

## Roadmap

- [x] Core prompt scoring framework
- [x] Universal system prompt (works on any LLM)
- [x] Claude skill file
- [x] Example library
- [ ] Web app (paste prompt, get instant analysis)
- [ ] API endpoint (integrate PromptLens into your own tools)
- [ ] VS Code extension
- [ ] Token counter integration
- [ ] Multi-language support

---

## License

MIT License — free to use, modify, and distribute. See `LICENSE` for details.

---

## Created By

PromptLens was created to give everyone — students, professionals, developers, and curious minds — the ability to use AI to its fullest potential.

> *"The quality of your output is determined by the quality of your input."*

---

⭐ If PromptLens helped you, star the repo and share it with someone who struggles with AI outputs.
