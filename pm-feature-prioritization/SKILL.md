---
name: pm-feature-prioritization
description: Analyze and prioritize feature requests and product backlogs. Groups requests by theme, scores them on strategic alignment, impact, effort, and risk — including the asymmetric leverage of agent-access features. Produces a prioritized roadmap recommendation. Use when triaging a backlog, processing customer requests, preparing for roadmap planning, or deciding what to build next.
---

# PM Feature Prioritization

> **What it does:** Turns a messy list of feature requests or backlog items into a scored, defensible prioritization recommendation.
> **Input:** A list of feature requests or backlog items, plus optional strategic goals/OKRs and team capacity.
> **Output:** Themed backlog with RICE scores, Quick Wins / Big Bets segmentation, top 3 build recommendations, and an explicit "what not to build" list.

---

## Frameworks Used

- **RICE Scoring** (Intercom) — Reach x Impact x Confidence / Effort: the standard for quantitative, defensible prioritization
- **ICE Scoring** (Sean Ellis) — faster alternative for rapid triage of many small items when precision is less critical
- **Kano Model** (Noriaki Kano) — categorize features as Must-Haves (ship now), Performance (improve over time), or Delighters (differentiation); what delights today becomes table stakes tomorrow
- **Shape Up** (Basecamp) — treat prioritization as a betting decision with a fixed appetite, not a backlog to clear
- **Jobs-to-be-Done** — group requests by the underlying customer job, not the surface feature request

In 2026, features that unlock agent access — APIs, MCP servers, structured outputs, CLIs — can have asymmetric RICE scores. A single developer integration can generate the same workflow volume as hundreds of manual human users, meaning Reach is often underestimated for agent-access items. AI PMs also use AI to pre-cluster and pre-score feature requests automatically, then review and debate the output — shifting the PM's role from data entry to strategic judgment.

---

## Input

$ARGUMENTS should provide:
- A list of feature requests or backlog items (paste directly or describe them)
- Optional: strategic goals or OKRs to align against
- Optional: team size or capacity constraints

---

## Analysis Steps

### 1. Theme Grouping
Cluster all requests into 3-6 themes using JTBD framing. Name each theme by the customer job it addresses, not the feature:
- "Faster onboarding" not "Onboarding redesign"
- "Reduce churn from power users" not "Advanced features"
- "Enable agent-driven workflows" not "API improvements" — if agent-access requests are present, treat this as its own theme

Flag requests that don't map to any strategic goal — these are candidates to cut.

### 2. Kano Classification
Before scoring, classify each item:
- **Must-Have** — customers are angry if absent; ship in next sprint
- **Performance** — satisfaction scales with quality; invest proportionally
- **Delighter** — unexpected, creates competitive differentiation; these are your bets

Must-Haves have no upside from over-engineering. Delighters are where you win.

In 2026, for developer-facing or data-heavy products: **API access and MCP compatibility are shifting from Delighters → Must-Haves.** If your product lacks programmatic access, AI agents route around it — and so do the developers building on top of AI agents. Treat agent-accessibility as a Must-Have for any product where developers or power users are a meaningful segment.

### 3. RICE Scoring
Score every feature on four dimensions (1-5 or estimated numbers):

| Dimension | What to assess |
|---|---|
| **Reach** | How many users affected per month? |
| **Impact** | How much does this move the needle? (0.25 / 0.5 / 1 / 2 / 3) |
| **Confidence** | How certain are the estimates? (low = 50%, medium = 80%, high = 100%) |
| **Effort** | Person-months to ship (lower = better) |

**RICE Score = (Reach x Impact x Confidence) / Effort**

For agent-access features, score Reach carefully: consider agent reach separately from human reach. A single developer integrating your product via API can generate the same workflow volume as hundreds of manual human users — and that integration unlocks downstream usage by multiple AI agents operating on behalf of those developers' users.

Use ICE (Impact x Confidence x Ease, all 1-10) for quick triage of small items where RICE would be overkill.

### 4. Segmentation Matrix
Classify using impact vs. effort:
- **Quick Wins** — high impact, low effort: ship now
- **Big Bets** — high impact, high effort: plan carefully, consider phasing
- **Fill-ins** — low impact, low effort: ship when there's slack capacity
- **Deprioritize** — low impact, high effort: cut or defer indefinitely

Apply Shape Up thinking to Big Bets: set a fixed appetite (e.g., 6 weeks max) and scope the solution to fit — don't let it expand.

### 5. Risk Flags
Surface any items with:
- High demand but low strategic alignment (stakeholder pressure vs. actual value)
- High effort with unvalidated assumptions (build trap risk — needs discovery first)
- Dependencies that unlock multiple other items (do these first)
- **Agent-access blockers**: features that prevent agents from using the product (CAPTCHA on critical flows, session-only auth with no API equivalent, UI actions with no API counterpart). In 2026, these are technical debt — flag them explicitly, because they don't show up in human user complaints but silently kill developer and agent adoption

---

## Output Format

1. Theme summary with request count per theme
2. Kano classification for all items
3. Prioritized backlog sorted by RICE score (table format)
4. Segmentation matrix: Quick Wins / Big Bets / Fill-ins / Deprioritize
5. Top 3 build recommendations with rationale
6. Explicit "do not build" list with reasons — critical for stakeholder alignment
