# PromptLens Examples — Research & Factual Queries

Research prompts carry the highest hallucination risk. These examples show how to
constrain AI to facts and flag uncertainty.

---

## Example 1 — General Research

**❌ Before:**
```
tell me about climate change
```

**✅ PromptLens Improved:**
```
Give me a factual overview of the scientific consensus on climate change.

Focus on:
- What is causing it (key drivers, ranked by contribution)
- What the evidence shows is already happening (observable effects)
- What is projected to happen (distinguish between high-confidence and uncertain predictions)

Audience: An educated adult with no science background.
Format: 4 short paragraphs, no bullet points.

Important:
- Distinguish clearly between established consensus and areas of ongoing scientific debate
- Do not invent statistics — only cite well-known figures (e.g. IPCC reports)
- If you are uncertain about a specific figure, say "approximately" or "estimates vary"
- Do not editorialize — stick to what the evidence shows
```

---

## Example 2 — Fact-Checking Style Query

**❌ Before:**
```
is coffee good or bad for you
```

**✅ PromptLens Improved:**
```
Summarize what the current scientific evidence says about coffee's health effects.

Cover both potential benefits and risks. For each point:
- Indicate how strong the evidence is (well-established vs. preliminary findings)
- Note if effects differ by population (e.g. pregnant women, people with anxiety)

Keep it balanced — don't lean toward either "coffee is great" or "coffee is harmful".
Under 300 words.

Do not present contested findings as settled facts.
If a claim is based on limited research, say so.
```

---

## Example 3 — Historical Research

**❌ Before:**
```
what caused world war 1
```

**✅ PromptLens Improved:**
```
Explain the main causes of World War 1 for a high school student writing a history essay.

Cover:
- The immediate trigger (assassination of Franz Ferdinand)
- The underlying long-term causes (use the MAIN framework: Militarism, Alliances,
  Imperialism, Nationalism)
- Why historians debate which cause was most significant

Format: Clear paragraphs with a heading for each cause.
Do not invent quotes from historical figures.
If there is genuine historical debate about something, present both sides briefly.
```

---

## Example 4 — Current Events / Recent Information

**❌ Before:**
```
what's happening with AI regulation
```

**✅ PromptLens Improved:**
```
Summarize the state of AI regulation as of your knowledge cutoff date.

Cover:
- Key regulatory developments in the EU, US, and UK (the three most active regions)
- What each approach focuses on (risk-based? sector-specific? voluntary?)
- Areas where there is broad agreement vs. significant disagreement between countries

Format: One paragraph per region, then a short comparison paragraph.

Important:
- Clearly state your knowledge cutoff at the start so I know how current this is
- Do not speculate about what might have happened after your cutoff
- If something was still being debated or unresolved at your cutoff, say so
```
