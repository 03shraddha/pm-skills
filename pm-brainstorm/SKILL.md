---
name: pm-brainstorm
description: Brainstorm product ideas and experiments for PMs. Generates ideas from PM, Designer, and Engineer perspectives. Handles both existing products (feature ideation) and new products (initial discovery). Also designs lean experiments and pretotypes to test ideas. Use when brainstorming features, ideating on a new product concept, or designing experiments to validate a hypothesis.
---

# PM Brainstorm

## Purpose

Generate diverse product ideas or design experiments to test them — for existing or new products. Uses multi-perspective ideation and lean startup thinking to produce actionable, testable output.

## Input

$ARGUMENTS should specify:
- **What**: product name or concept
- **Mode**: ideas (brainstorm features/directions) or experiments (design tests for a specific idea)
- **Stage**: existing product or new product

If mode is not specified, default to ideas. Infer stage from context if not stated.

## Brainstorming Ideas

### Existing Product
Generate ideas from three lenses, then synthesize:

**PM lens** — Unmet user needs, metrics to move, adjacent use cases
**Designer lens** — UX friction, missing delight moments, broken flows
**Engineer lens** — Underutilized technical capabilities, high-value low-cost builds

Output: 5-7 ideas per lens with a one-line rationale. Then synthesize: top 5 ranked by impact/effort with reasoning.

### New Product
Focus on early discovery — avoid over-specifying. Identify:
- Target user and their core frustration
- 5-7 distinct product directions (not just feature variations)
- For each: the core value prop, the riskiest assumption, and the minimum version to test

## Designing Experiments

### Existing Product
Validate a specific feature idea before building:
- State the hypothesis: "If we build X, we expect Y, because Z"
- Identify the riskiest assumption
- Design 3 experiments: quantitative signal, qualitative signal, fake-door or concierge test
- Define success metrics and timeline for each

### New Product (Pretotypes)
Use lean startup / pretotype thinking:
- Identify the leap-of-faith assumption
- Design the smallest possible test (landing page, wizard-of-oz, paper prototype, etc.)
- Define what "validated" looks like before running the test
- Suggest channels to recruit participants

## Output Format

1. Brief restatement of the problem or opportunity
2. Ideas or experiments (structured per mode above)
3. Recommended next step — one specific action to take this week
