---
name: pm-customer-research
description: Create structured customer interview scripts or synthesize interview transcripts into actionable PM insights. Interview scripts include JTBD probing questions, warm-up, core exploration, and wrap-up sections. Transcript synthesis extracts jobs-to-be-done, satisfaction signals, pain points, and action items. Use when preparing for customer interviews, analyzing research sessions, or turning raw transcripts into structured discovery output.
---

# PM Customer Research

## Purpose

Either prepare for a customer interview with a structured script, or synthesize a completed interview transcript into a PM-ready insight summary.

## Input

$ARGUMENTS should specify:
- **Mode**: script (create an interview guide) or summarize (synthesize a transcript)
- For script mode: the product area, hypothesis, or feature to explore
- For summarize mode: paste the transcript or describe what was discussed

If mode is unclear, infer from whether a transcript is provided.

## Interview Script Mode

Create a structured 45-60 minute interview guide:

### Warm-up (5 min)
- Role, context, and background questions
- Establish rapport; avoid leading with the product

### Current Behavior Exploration (15 min)
- "Walk me through the last time you [relevant task]..."
- "What does your current process look like?"
- "What tools or workarounds are you using?"
- Probe: frequency, frustration level, workarounds, triggers

### JTBD Deep Dive (20 min)
Jobs-to-be-done questions surface the underlying motivation:
- "What were you trying to accomplish when you [did X]?"
- "When [situation], you want to [motivation], so you [expected outcome]?"
- "What would make this easier? What would make it perfect?"
- "If this problem disappeared tomorrow, what would change for you?"

### Solution Probing (10 min — optional, use only if hypothesis is pre-formed)
- Show a concept or describe an approach
- "Does this solve the problem you described? Why or why not?"
- "What's missing? What would you change?"
- Avoid leading questions; listen for hesitation as much as enthusiasm

### Wrap-up (5 min)
- "Is there anything I didn't ask that you think I should know?"
- "Who else deals with this problem on your team?"
- Ask for referrals to other participants

## Transcript Synthesis Mode

Analyze the transcript and produce a structured summary:

### Participant Snapshot
- Role, company type, context, how they currently solve the problem

### Jobs-to-be-Done
- Primary job: what they were fundamentally trying to accomplish
- Secondary jobs: adjacent tasks that came up
- Emotional jobs: how they want to feel (in control, confident, fast)

### Satisfaction Signals
- What's working well in their current solution
- Moments of delight or surprise in the conversation

### Pain Points and Friction
- Specific frustrations quoted directly from the transcript
- Workarounds they've invented (strong signal of unmet need)
- Frequency and severity of each pain point

### Opportunity Signals
- Unmet needs that no current solution addresses
- "If only..." statements from the participant

### Action Items
- Features or bets to explore based on this session
- Follow-up questions for the next interview
- Hypotheses confirmed, challenged, or newly surfaced
