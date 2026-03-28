---
name: pm-customer-research
description: Create structured customer interview scripts or synthesize interview transcripts into actionable PM insights. Includes JTBD probing questions and, in 2026, questions to surface how customers are already using AI agents with your product. Transcript synthesis extracts jobs-to-be-done, pain points, and agent use signals. Use when preparing for customer interviews, analyzing research sessions, or turning raw transcripts into structured discovery output.
---

# PM Customer Research

> **What it does:** Prepares structured customer interview scripts or synthesizes completed transcripts into PM-ready insight summaries.
> **Input:** Mode (script or summarize), plus a product area/hypothesis (for scripts) or a transcript (for synthesis).
> **Output:** A complete interview guide with JTBD questions (script mode), or a structured insight summary with pain points, opportunity signals, agent use signals, and action items (summarize mode).

---

## Frameworks Used

- **Jobs-to-be-Done** (Christensen / Competing Against Luck) — probe for functional, emotional, and social job dimensions; the best interviews reveal why, not just what
- **Continuous Discovery Habits** (Teresa Torres) — weekly 30-minute interviews with 2-3 customers is sustainable; treat every interview as opportunity-finding, not solution validation
- **Working Backwards** (Amazon) — after synthesis, ask: "Could we write a press release for a product that solves what we just heard?" If yes, there's a real opportunity
- **Opportunity-Solution Tree** (Torres) — map interview findings directly to opportunity branches on the tree; insights without a home in the tree are noise

In 2026, "customers" include AI agents. Your human customers are increasingly using AI tools to interact with your product — and the workflows they wish they could automate represent the next frontier of unmet needs. Probing for agent use in interviews reveals what people are trying to offload, what they trust automation to do, and what they still want to control themselves. Use this skill for single-interview depth; use AI batch synthesis for cross-interview pattern detection across 10+ transcripts.

---

## Input

$ARGUMENTS should specify:
- **Mode**: script (create an interview guide) or summarize (synthesize a transcript)
- For script mode: the product area, hypothesis, or specific assumption to explore
- For summarize mode: paste the transcript or describe the key topics covered

If mode is unclear, infer from whether a transcript is provided.

---

## Script Mode

Create a structured 45-60 minute interview guide:

### Warm-up (5 min)
- Role, context, and day-to-day background
- "Walk me through a typical [relevant work day / task]"
- Goal: establish rapport; do not mention the product or solution yet

### Current Behavior Exploration (15 min)
- "Walk me through the last time you had to [relevant task]..."
- "What does your current process look like from start to finish?"
- "What tools, workarounds, or hacks are you using?"
- Probe: frequency, frustration level, cost of the workaround, what triggers the task

### JTBD Deep Dive (20 min)
Jobs-to-be-done questions surface the underlying motivation, not the surface request:
- "What were you ultimately trying to accomplish when you [did X]?"
- "How did it make you feel when [pain point] happened?"
- "How do others on your team / your manager perceive this process?"
- "If this problem disappeared tomorrow, what would change for you?"
- "What would the perfect version of this look like?"

Probe all three job dimensions: functional (task), emotional (feeling), social (perception).

In 2026, also probe for agent use — these questions reveal what customers are already trying to automate and what programmatic access they wish existed:
- "Are you using any AI tools or agents as part of this workflow today?"
- "If an AI agent could handle this task entirely on your behalf, what would it need to do — step by step?"
- "What would you still want to do yourself, even if an agent could do it?"
- "Have you ever tried to automate or script any part of this process? What happened?"

### Solution Probing (10 min — only if validating a specific hypothesis)
- Describe the concept or show a prototype — do not lead with a demo
- "Does this solve the problem you described? Why or why not?"
- "What's missing? What would you remove?"
- Listen for hesitation as much as enthusiasm — both are signal

### Wrap-up (5 min)
- "Is there anything I didn't ask that you think I should know?"
- "Who else on your team or network deals with this problem?"
- Ask for referrals to 2-3 other potential participants

---

## Summarize Mode

Analyze the transcript and produce a structured summary:

### Participant Snapshot
- Role, company type, team size, how they currently solve the problem

### Jobs-to-be-Done
- **Primary job**: what they were fundamentally trying to accomplish
- **Emotional job**: how they want to feel while doing it
- **Social job**: how they want to be perceived by others

### Satisfaction Signals
- What is working well in their current approach
- Moments of delight or surprise mentioned in the session

### Pain Points and Friction
- Specific frustrations, quoted directly where possible
- Workarounds they have invented — strong signal of unmet need
- Frequency and severity rating for each pain point (1-5)

### Opportunity Signals
- Unmet needs no current solution addresses
- "If only..." or "I wish..." statements
- Behaviors that suggest latent demand

### Agent Use Signals
Surface any mentions of:
- AI tools or agents they are already using in this workflow (ChatGPT, Claude, Cursor, Zapier, etc.)
- Tasks they've tried to automate — what worked, what didn't
- "I wish this could just..." statements — these are requests for agent-native features in disguise
- Explicit requests for API access, integrations, or scripting capabilities
- Resistance to automation — what they explicitly want to keep doing themselves, and why

These signals indicate where agent-native features have real demand, and where human oversight is a genuine requirement rather than a gap to close.

### Working Backwards Check
- Based on this interview, could you write a press release for a product that solves what was described?
- If yes: what is the headline and the core customer benefit?

### Action Items
- Hypotheses confirmed, challenged, or newly surfaced
- Features or product directions to explore
- Follow-up questions for the next interview
- Suggested additions to the Opportunity Solution Tree
