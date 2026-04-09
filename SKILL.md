---
name: prompt-coach
description: >
  Analyze, score, and improve any prompt a user writes for an AI. Use this skill whenever
  a user asks things like "is my prompt good?", "how do I get better answers from AI?",
  "can you improve my prompt?", "why is AI giving me bad results?", "make my prompt less
  AI-sounding", "help me with prompt engineering", or pastes a prompt and asks for feedback.
  Also trigger when a user describes a task they want AI to do but seems unsure how to ask
  for it — coach them to build the right prompt from scratch. Always use this skill when
  the user's core need is about *how to ask AI better*, not just what to ask.
---

# PromptLens — Claude Skill

This is the Claude skill version of PromptLens. It follows the full 6-step PromptLens
analysis framework defined in `../promptlens.md`.

When this skill is active, run the complete PromptLens analysis for every prompt the
user shares. Refer to `../promptlens.md` for the full framework, scoring dimensions,
anti-hallucination phrases, and special scenarios.

## Quick Reference — The 6 Steps

1. **Understand the Goal** — confirm what the user wants
2. **Score the Prompt** — 6 dimensions, each /10, with reasons
3. **Manual Diagnosis** — explain weaknesses in plain English
4. **How an LLM Reads This** — explain the model's internal interpretation
5. **Improved Prompt** — rewritten version in a code block, user chooses to use it
6. **The Lesson** — 3 takeaways the user can apply next time independently

## The 6 Scoring Dimensions

- 🎯 Clarity
- 📐 Specificity
- 🧠 Context
- 🌀 Hallucination Risk
- 🪙 Token Efficiency
- 🧩 Context Window Usage

See `../promptlens.md` for full scoring criteria and special scenario handling.
