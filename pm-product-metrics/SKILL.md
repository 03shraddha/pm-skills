---
name: pm-product-metrics
description: Design product metrics dashboards or build Opportunity Solution Trees (OSTs) to structure product discovery. Metrics dashboards define North Star metrics, input metrics, health metrics, and alert thresholds. OSTs map a desired outcome to opportunities, solutions, and experiments. Use when setting up product measurement, preparing for a planning cycle, or structuring how a team approaches a specific outcome.
---

# PM Product Metrics

> **What it does:** Designs a product metrics framework or builds an Opportunity Solution Tree to connect a team's work to a desired outcome.
> **Input:** Mode (dashboard or ost), plus the product, product area, or outcome to focus on.
> **Output:** A layered metrics system with North Star, input, and health metrics (dashboard mode), or a full OST with opportunities, solutions, and prioritized experiments (ost mode).

---

## Frameworks Used

- **North Star Framework** — one metric that captures the core value delivered; all team OKRs should show a causal link to it
- **HEART Framework** (Google) — Happiness, Engagement, Adoption, Retention, Task Success; use for UX-centric products where revenue metrics alone miss the picture
- **Opportunity-Solution Tree** (Teresa Torres) — maps desired outcome to customer opportunities to solutions to experiments; prevents building solutions without connected customer needs
- **Continuous Discovery Habits** (Torres) — OSTs are living documents updated weekly as customer interviews surface new opportunities
- **OKR Alignment** — North Star is persistent (changes every 2-5 years); OKRs implement strategy quarterly; both must coexist without conflicting

In 2026, AI PMs use AI agents to continuously monitor whether actions are moving the North Star — replacing manual weekly metric reviews with real-time anomaly detection and automated insight surfacing.

---

## Input

$ARGUMENTS should specify:
- **Mode**: dashboard (metrics framework) or ost (opportunity solution tree)
- The product, product area, or specific outcome to focus on

If mode is unclear, infer from context: if an outcome or goal is described, default to OST; if measurement or tracking is the goal, default to dashboard.

---

## Dashboard Mode

Design a layered metrics system:

### North Star Metric
The single metric that best captures the value delivered to customers and predicts long-term business health.

A strong North Star is:
- **Customer-centric**: reflects value to the user, not just to the business
- **Leading indicator**: predicts future retention and growth
- **Actionable**: teams can directly influence it
- **Persistent**: rarely changes (Spotify: hours listened; Slack: messages sent; Airbnb: nights booked)

Include: definition, current baseline (if known), target, and why this metric over alternatives.

### Input Metrics (3-5)
Leading indicators that drive the North Star — the levers teams can pull:

| Metric | Definition | How to Measure | Expected Direction |
|---|---|---|---|
| (populate) | | | |

### Health Metrics (3-5)
Guardrail metrics — things that must not degrade while optimizing for the North Star.

Apply HEART where relevant: Happiness (NPS, CSAT), Engagement (DAU/MAU), Adoption (new user activation), Retention (30/60/90-day), Task Success (completion rate, error rate).

Define alert thresholds for each: "If [metric] drops below [X], investigate before shipping."

### Metrics Hierarchy Table

| Metric | Type | Definition | Data Source | Owner | Alert Threshold |
|---|---|---|---|---|---|
| (populate for each) | | | | | |

### Dashboard Design Notes
- Recommended visualization per metric (trend line, funnel, cohort, heatmap)
- Suggested refresh cadence (real-time, daily, weekly)
- Key segmentation dimensions (plan tier, cohort, region, user type)
- OKR connection: show how each input metric links to a team OKR and up to the North Star

---

## OST Mode

Build an Opportunity Solution Tree to connect a desired outcome to concrete experiments:

### Desired Outcome
State the product outcome the team owns — an impact, not an output:
- Good: "Increase weekly active usage among free-tier users by 20%"
- Bad: "Ship the new onboarding flow"

### Opportunities (4-6)
Each opportunity is an unmet customer need, pain point, or desire surfaced through research. Write from the customer's perspective:
- "Users don't know they're missing features that would help them"
- "Users lose their workflow context when switching between tasks"

Rate each opportunity:
- **Evidence strength** (1-5): how many interviews / data points support this?
- **Frequency** (1-5): how often does this affect users?
- **Severity** (1-5): how much does it hurt when it happens?

### Solutions (2-3 per top opportunity)
Generate distinct solutions — avoid converging on one answer. For each:
- One-line description of the approach
- Riskiest assumption behind it
- Effort estimate (S/M/L)

### Experiments (1-2 per solution)
Design the smallest test that validates or invalidates the riskiest assumption:
- Hypothesis, test type, success metric, timeline
- Prefer tests that could prove you wrong cheaply

### OST Summary

```
Desired Outcome
├── Opportunity 1
│   ├── Solution A -> Experiment (type, metric, timeline)
│   └── Solution B -> Experiment
├── Opportunity 2
│   └── Solution C -> Experiment
...
```

Recommend which branch to pursue first and why — based on opportunity evidence strength x solution confidence x experiment cost.
