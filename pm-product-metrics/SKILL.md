---
name: pm-product-metrics
description: Design product metrics dashboards or build Opportunity Solution Trees (OSTs) to structure product discovery. Metrics dashboards define North Star metrics, input metrics, health metrics, and alert thresholds. OSTs map a desired outcome to opportunities, solutions, and experiments. Use when setting up product measurement, preparing for a planning cycle, or structuring how a team approaches a specific outcome.
---

# PM Product Metrics

## Purpose

Either design a metrics framework for a product area, or build an Opportunity Solution Tree to structure how a team pursues a specific outcome.

## Input

$ARGUMENTS should specify:
- **Mode**: dashboard (metrics framework) or ost (opportunity solution tree)
- The product, product area, or outcome to focus on

If mode is unclear, infer from context — if an outcome or goal is described, default to OST; if measurement or tracking is the goal, default to dashboard.

## Metrics Dashboard Mode

Design a layered metrics system:

### North Star Metric
- One metric that best captures the value delivered to customers
- Should be: measurable, customer-centric, predictive of long-term growth
- Include: current baseline (if known), target, and why this metric

### Input Metrics (3-5)
Leading indicators that drive the North Star. These are the levers the team can pull:
- Name, definition, how to measure, expected direction

### Health Metrics (3-5)
Guardrail metrics — things that must not break while optimizing for the North Star:
- Examples: churn rate, error rate, support ticket volume, NPS
- Define alert thresholds for each

### Metrics Hierarchy Table
| Metric | Type | Definition | Data Source | Owner | Alert Threshold |
|---|---|---|---|---|---|
| (populate for each metric) |

### Dashboard Design Notes
- Recommended visualization type per metric (trend line, funnel, cohort, etc.)
- Suggested refresh cadence (real-time, daily, weekly)
- Key segmentation dimensions (by plan, cohort, region, user type)

## Opportunity Solution Tree Mode

Build an OST to connect a desired outcome to concrete experiments:

### Desired Outcome
- State the product outcome the team is accountable for (not an output like "ship feature X")
- Example: "Increase weekly active usage among free-tier users by 20%"

### Opportunities (4-6)
Each opportunity is an unmet need, pain point, or desire from the customer:
- Write from the customer's perspective: "Users struggle to [X] because [Y]"
- Rate each by: customer evidence strength, frequency, severity
- Identify which opportunities most directly connect to the desired outcome

### Solutions (2-3 per opportunity)
For each top opportunity, generate possible solutions:
- Keep solutions distinct — avoid converging on the same answer
- Flag the riskiest assumption behind each solution

### Experiments (1-2 per solution)
For each solution, define the smallest test:
- Hypothesis, test type, success metric, timeline
- Prioritize experiments that test the riskiest assumption at lowest cost

### OST Summary
Produce a text-based tree structure:

```
Desired Outcome
├── Opportunity 1
│   ├── Solution A -> Experiment
│   └── Solution B -> Experiment
├── Opportunity 2
│   └── Solution C -> Experiment
...
```

Recommend which branch to pursue first and why.
