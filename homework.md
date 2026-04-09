# PromptLens Examples — Student & Homework Scenarios

These examples show real before/after prompt transformations for common student use cases.

---

## Example 1 — Math Homework

**❌ Before:**
```
solve this math problem: if a train travels 60mph for 2 hours how far does it go
```

**PromptLens Score:** 4/10
- Clarity: 7 — clear enough
- Specificity: 2 — no request for explanation or working shown
- Context: 3 — what level is this? What has the student tried?
- Hallucination Risk: 8 — low risk, it's a calculation
- Token Efficiency: 6 — acceptable
- Context Window: 4 — no background given

**What's wrong:** This will just give you the answer (120 miles) with no explanation.
You won't learn anything. If this is homework, you'll get the answer but not understand
how to solve the next one.

**✅ PromptLens Improved:**
```
I'm a high school student learning about distance, speed, and time calculations.

Problem: A train travels at 60mph for 2 hours. How far does it go?

Please:
1. Show me the formula used (distance = speed × time)
2. Walk through the calculation step by step
3. Explain why this formula works in plain English
4. Give me one similar practice problem I can try myself

Do not just give me the answer — I need to understand the method.
```

**What made the difference:**
- Asking for the method, not just the answer, makes this genuinely useful for learning
- Requesting a practice problem reinforces the skill
- Specifying "high school student" calibrates the explanation level

---

## Example 2 — Essay Writing

**❌ Before:**
```
write an essay about the french revolution
```

**PromptLens Score:** 2/10
- Clarity: 4 — which aspect? Causes? Effects? Key figures?
- Specificity: 1 — no length, angle, audience, or format
- Context: 1 — no grade level, no assignment brief
- Hallucination Risk: 4 — high risk of invented dates/details
- Token Efficiency: 4 — too sparse
- Context Window: 2 — wastes the entire context window

**What's wrong:** The AI will write a generic 500-word overview that covers everything
and nothing. It may invent specific quotes from historical figures or misattribute events.
It will sound very AI-written.

**✅ PromptLens Improved:**
```
Write a 700-word essay arguing that economic inequality was the primary cause
of the French Revolution. This is for a 10th grade history class.

Structure:
- Introduction with a clear thesis statement
- 3 body paragraphs, each with one main argument and a historical example
- Conclusion that restates the thesis without copying the intro

Tone: Academic but readable for a 16-year-old audience.
Do not invent quotes or specific statistics — if data would strengthen a point,
note [DATA NEEDED] so I can research and insert it.
Avoid AI-sounding phrases like "It is worth noting" or "In conclusion, it is clear that".
```

**What made the difference:**
- Picking a specific argument angle (economic inequality) gives the essay a spine
- "[DATA NEEDED]" placeholder prevents hallucinated statistics
- Grade level calibrates complexity perfectly

---

## Example 3 — Science Concept

**❌ Before:**
```
explain photosynthesis
```

**PromptLens Score:** 3/10
- Clarity: 6 — clear topic
- Specificity: 1 — no depth, audience, or format requested
- Context: 1 — what does the student already know?
- Hallucination Risk: 7 — well-known topic, lower risk
- Token Efficiency: 5 — minimal but not wasteful
- Context Window: 2 — no background given

**✅ PromptLens Improved:**
```
I'm a 9th grade student who understands basic cell biology but hasn't studied
photosynthesis yet.

Explain photosynthesis in a way I can understand and remember for a test. Include:
1. What photosynthesis is (one sentence definition)
2. The inputs and outputs (what goes in, what comes out)
3. Why it matters for life on Earth
4. A simple analogy that makes it easy to remember

Keep it under 300 words. Use plain language — no technical jargon unless you explain it.
```

**What made the difference:**
- Stating prior knowledge prevents over-explanation or under-explanation
- Requesting an analogy dramatically improves memorability
- Word limit forces conciseness — no padding

---

## Example 4 — Coding Assignment

**❌ Before:**
```
write code for a calculator
```

**PromptLens Score:** 2/10
- Clarity: 4 — what kind of calculator? Basic? Scientific?
- Specificity: 1 — no language, no features, no UI
- Context: 1 — school project? Personal? What level?
- Hallucination Risk: 6 — code either works or it doesn't
- Token Efficiency: 4 — too sparse
- Context Window: 1 — completely empty

**✅ PromptLens Improved:**
```
Write a basic calculator in Python for a beginner programming assignment.

Requirements:
- Supports: addition, subtraction, multiplication, division
- Runs in the terminal (no GUI needed)
- Asks the user to input two numbers and choose an operation
- Handles division by zero with a clear error message
- Loops so the user can do multiple calculations without restarting

Please:
- Add comments explaining each section of the code
- Keep the code simple — I'm learning Python for the first time
- Don't use advanced features like classes or lambda functions
```

**What made the difference:**
- Specifying Python prevents the AI picking a language you don't know
- "No GUI" and "terminal only" prevents over-engineering
- "No advanced features" is critical for beginners — without it, AI often shows off
