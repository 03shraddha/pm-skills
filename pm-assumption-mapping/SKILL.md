---
name: pm-assumption-mapping
description: Identify, map, and prioritize the riskiest assumptions behind a product idea. Covers both existing products (VUVF + Agent Accessibility) and new products (8 risk categories including Go-to-Market, Strategy, Team, and agent user viability). Outputs a prioritized assumption list with recommended experiments. Use when stress-testing a feature, evaluating a new product concept, or preparing for a discovery sprint.
---

# PM Assumption Mapping

> **What it does:** Surfaces and prioritizes the assumptions that could kill a product idea before any code is written.
> **Input:** A feature idea or product concept, plus whether it is for an existing or new product.
> **Output:** A full assumption map by category, a prioritized top 5-7 by Impact x Evidence, and one recommended experiment per priority assumption.

---

## Frameworks Used

- **Inspired** (Marty Cagan) — the VUVF model: Value, Usability, Viability, Feasibility risk categories
- **Jobs-to-be-Done / Competing Against Luck** (Christensen) — surface assumptions across functional, emotional, and social job dimensions
- **Lean Startup** (Eric Ries) — leap-of-faith assumptions: identify what must be true for the business to work, then test the riskiest one first
- **Continuous Discovery Habits** (Teresa Torres) — assumptions are branches on the Opportunity Solution Tree; test before building

In 2026, a product's viability increasingly depends on agent-accessibility. Whether your product needs an MCP server, public API, or structured outputs is not a technical detail — it's a product assumption that needs to be tested. Treat agent users as a distinct assumption category: who are they, what do they need, and what breaks if agents try to use the product today? AI can also be used to cross-reference assumptions against customer review data, support tickets, and behavioral analytics before scoring — reducing gut-feel bias in the prioritization.

---

## Input

$ARGUMENTS should specify:
- The feature idea or product concept to stress-test
- Whether it is for an **existing product** or a **new product**

---

## Identifying Assumptions

### Existing Product
Map assumptions across the VUVF framework (Marty Cagan, Inspired), plus an Agent Accessibility category:

| Category | Question to ask |
|---|---|
| **Value** | Do users actually want this? Will it solve a real problem in a way they care about? |
| **Usability** | Can users understand and use it without friction or support? |
| **Viability** | Does this make business sense? Will the unit economics work? |
| **Feasibility** | Can the team build this with available resources, data, and tech stack? |
| **Agent Accessibility** | Can AI agents use this product without a human in the loop? Do they need to? What breaks today if an agent tries? |

Generate 4-6 assumptions per category. Write each as a falsifiable statement: "We believe that [assumption]."

For Agent Accessibility, example assumptions to stress-test:
- "We believe agents don't need programmatic access to this feature because it's too decision-heavy for automation"
- "We believe our current API surface is sufficient for agent workflows"
- "We believe our per-seat pricing model still works even if 30% of sessions are agent-initiated"

### New Product
Map assumptions across 8 risk categories:

1. **Desirability** — Do enough people have this problem and care about solving it? Also: who are the agent users of this product, if any? What jobs are they hired to do that differ from human users?
2. **Value** — Does our solution solve it better than current alternatives (including doing nothing)?
3. **Usability** — Will people understand how to use it without hand-holding?
4. **Feasibility** — Can we build it with the team and tech we have?
5. **Viability** — Can we build a sustainable business model around it? Does the business model still work if a significant portion of usage comes from agents rather than humans? (pricing by seat vs. by API call)
6. **Go-to-Market** — Can we reach, acquire, and retain the target customer at viable cost?
7. **Strategy** — Can we defend this position over time? Is there a moat? Is agent-accessibility a moat or a commodity in this market — will competitors with better MCP/API coverage outcompete us?
8. **Team** — Do we have the capabilities, focus, and resources to execute?

Generate 3-5 assumptions per category. Apply Lean Startup thinking: identify the leap-of-faith assumption for each — the one assumption that, if wrong, kills the entire idea.

---

## Prioritizing Assumptions

Score each assumption on two axes:

- **Impact** (1-5): If this assumption is wrong, how badly does it break the idea?
- **Evidence** (1-5): How much existing evidence supports it being true? (1 = none, 5 = strong)

**Priority = High Impact + Low Evidence.** These are the assumptions to test first — high stakes, low confidence.

Highlight the top 5-7. Flag any that are both high-impact and have conflicting evidence — these need qualitative research, not just A/B tests.

---

## Output Format

1. Full assumption map by category in table format
2. Top 5-7 prioritized assumptions with Impact and Evidence scores
3. For each priority assumption: one experiment to test it (type, method, success criteria)
4. Recommended discovery sprint focus — which assumption to tackle first and why
5. Leap-of-faith call: the single assumption that, if wrong, invalidates the entire initiative
