---
name: pm-brainstorm
description: Brainstorm product ideas and experiments for PMs. Generates ideas from PM, Designer, and Engineer perspectives. Handles both existing products (feature ideation) and new products (initial discovery). Also designs lean experiments and pretotypes to test ideas. Use when brainstorming features, ideating on a new product concept, or designing experiments to validate a hypothesis.
---

# PM Brainstorm

> **What it does:** Generates diverse product ideas or experiment designs using multi-perspective ideation and lean startup thinking.
> **Input:** A product name or concept, plus mode (ideas or experiments) and stage (existing or new product).
> **Output:** A structured list of ideas or experiments with rationale, ranked by impact/effort, plus one recommended next step.

---

## Frameworks Used

This skill draws on:
- **Jobs-to-be-Done** (Christensen) — generate ideas by asking "what job is the customer hiring this product to do?" across functional, emotional, and social dimensions
- **Lean Startup** (Eric Ries) — design the smallest possible experiment that tests a leap-of-faith assumption
- **Working Backwards** (Amazon) — before brainstorming solutions, write the press release for the finished product to clarify the customer need
- **Continuous Discovery Habits** (Teresa Torres) — treat brainstorming as opportunity-finding first, solution-finding second

In 2026, AI PMs use AI to synthesize customer signals (support tickets, reviews, interviews) before brainstorming, so ideas are grounded in real unmet needs rather than internal intuition.

---

## Input

$ARGUMENTS should specify:
- **What**: product name or concept
- **Mode**: ideas (brainstorm features/directions) or experiments (design tests for a specific idea)
- **Stage**: existing product or new product

If mode is not specified, default to ideas. Infer stage from context.

---

## Brainstorming Ideas

### Existing Product
Before generating ideas, identify the job the product is currently hired to do. Then generate ideas from three lenses:

**PM lens** — Unmet jobs-to-be-done, metrics to move, adjacent use cases, underserved segments
**Designer lens** — UX friction, emotional job failures, missing delight moments, broken flows
**Engineer lens** — Underutilized technical capabilities, high-value low-cost builds, API opportunities

Output: 5-7 ideas per lens with one-line rationale. Synthesize: top 5 ranked by impact/effort, with the reasoning.

### New Product
Use early discovery framing — avoid over-specifying solutions. For each direction:
- Target user and their core job-to-be-done (functional + emotional + social)
- 5-7 distinct product directions (not just feature variations)
- For each: the core value prop, the riskiest assumption, and the minimum version to test
- Apply Working Backwards: draft a one-sentence press release for each direction — if it's hard to write, the idea probably won't work

---

## Designing Experiments

### Existing Product
Validate a specific feature idea before building. Apply Lean Startup thinking:
- State the hypothesis: "If we build X, we expect Y, because Z"
- Identify the leap-of-faith assumption (what must be true for this to work?)
- Design 3 experiments: quantitative signal, qualitative signal, fake-door or concierge test
- Define success metrics and timeline for each
- Recommend the cheapest test that could invalidate the riskiest assumption

### New Product (Pretotypes)
- Identify the leap-of-faith assumption (demand, behavior, or willingness-to-pay)
- Design the smallest possible test: landing page, wizard-of-oz, paper prototype, smoke test
- In 2026: use AI-assisted prototyping (vibe coding with tools like Claude Code) to generate working HTML prototypes in minutes instead of hours
- Define what "validated" looks like before running the test
- Suggest channels to recruit participants

---

## Output Format

1. Brief restatement of the problem or opportunity
2. Ideas or experiments (structured per mode above)
3. Recommended next step — one specific action to take this week
