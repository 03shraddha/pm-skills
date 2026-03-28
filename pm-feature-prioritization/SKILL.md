---
name: pm-feature-prioritization
description: Analyze and prioritize feature requests and product backlogs. Groups requests by theme, scores them on strategic alignment, impact, effort, and risk, and produces a prioritized roadmap recommendation. Use when triaging a backlog, processing customer requests, preparing for roadmap planning, or deciding what to build next.
---

# PM Feature Prioritization

## Purpose

Turn a messy list of feature requests or backlog items into a clear, defensible prioritization decision. Moves beyond gut feel by applying structured scoring and strategic framing.

## Input

$ARGUMENTS should provide:
- A list of feature requests or backlog items (paste directly or describe them)
- Optional: strategic goals or OKRs to align against
- Optional: team size / capacity constraints

## Analysis Steps

### 1. Theme Grouping
Cluster requests into 3-6 themes. Name each theme by the customer need it addresses, not the feature ("Faster onboarding" not "Onboarding redesign").

### 2. Scoring Each Item
Score every feature on four dimensions (1-5 scale):

| Dimension | What to assess |
|---|---|
| **Strategic Alignment** | How directly does this advance current OKRs or strategic goals? |
| **Customer Impact** | How many users are affected? How much does it improve their experience? |
| **Effort** | How much engineering + design time is required? (5 = lowest effort) |
| **Risk** | Technical, legal, or dependency risk. (5 = lowest risk) |

Priority Score = (Strategic Alignment + Customer Impact + Effort + Risk) / 4

### 3. Segmentation
Classify each item:
- **Quick Wins** — High impact, low effort (do now)
- **Big Bets** — High impact, high effort (plan carefully, needs phasing)
- **Fill-ins** — Low impact, low effort (do when capacity allows)
- **Deprioritize** — Low impact, high effort (cut or defer)

### 4. Surfacing Risks
Flag any items with:
- High customer demand but low strategic alignment (misaligned asks)
- High effort with unvalidated assumptions (build trap risk)
- Dependencies that block multiple other items (unlock value if done first)

## Output Format

1. Theme summary — grouped requests with request count per theme
2. Prioritized backlog — scored table sorted by Priority Score
3. Segmentation matrix — Quick Wins / Big Bets / Fill-ins / Deprioritize
4. Top 3 recommendations — what to build next with rationale
5. What to explicitly NOT build and why (important for stakeholder alignment)
