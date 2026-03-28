---
name: pm-assumption-mapping
description: Identify, map, and prioritize the riskiest assumptions behind a product idea. Covers both existing products (Value, Usability, Viability, Feasibility) and new products (8 risk categories including Go-to-Market, Strategy, Team). Outputs a prioritized assumption list with recommended experiments. Use when stress-testing a feature, evaluating a new product concept, or preparing for a discovery sprint.
---

# PM Assumption Mapping

## Purpose

Surface and prioritize the assumptions that could kill a product idea before any code is written. Forces PM thinking to move from "what do we want to build" to "what must be true for this to work."

## Input

$ARGUMENTS should specify:
- The feature idea or product concept to stress-test
- Whether it's for an **existing product** or a **new product**

## Identifying Assumptions

### Existing Product
Map assumptions across four risk categories (VUVF):

| Category | Question |
|---|---|
| **Value** | Do users actually want this? Will it solve a real problem? |
| **Usability** | Can users understand and use it without friction? |
| **Viability** | Does this make business sense? Will the unit economics work? |
| **Feasibility** | Can the team build this with available resources and tech? |

Generate 4-6 assumptions per category. Write each as a falsifiable statement: "We believe that [assumption]."

### New Product
Map assumptions across 8 risk categories:

1. **Desirability** — Do enough people have this problem?
2. **Value** — Does our solution actually solve it better than alternatives?
3. **Usability** — Will people understand how to use it?
4. **Feasibility** — Can we build it?
5. **Viability** — Can we build a sustainable business around it?
6. **Go-to-Market** — Can we reach and acquire our target customer?
7. **Strategy** — Can we defend this position over time?
8. **Team** — Do we have the capabilities and resources to execute?

Generate 3-5 assumptions per category.

## Prioritizing Assumptions

Score each assumption on two axes:
- **Impact**: If this assumption is wrong, how badly does it break the idea? (1-5)
- **Evidence**: How much evidence do we currently have that it's true? (1-5, where 1 = none)

Priority = High Impact + Low Evidence. Highlight the top 5-7 assumptions that are both high-impact and evidence-poor — these are the ones to test first.

## Output Format

1. Full assumption map by category (table format)
2. Top 5-7 prioritized assumptions with Impact and Evidence scores
3. For each priority assumption: suggest one experiment to test it (type, method, success criteria)
4. Recommended discovery sprint focus — which assumption to tackle first and why
