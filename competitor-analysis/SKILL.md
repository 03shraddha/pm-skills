---
name: competitor-analysis
description: Deep-dive competitive analysis that goes beyond feature matrices. Surfaces 5 direct competitors, maps their moats and gaps using real customer signals, and evaluates each on agent-accessibility (MCP server, API, CLI, structured outputs). Delivers a north star positioning thesis with battlecard-ready differentiators. Use before a product review, strategy sprint, or competitive brief.
---

# Competitor Analysis

## Purpose

Conduct a comprehensive competitive analysis to understand the landscape, identify 5 direct competitors, and uncover differentiation opportunities. This skill maps competitive positioning, synthesizes competitor strengths and weaknesses, and highlights opportunities for strategic differentiation — including in the emerging dimension of agent-accessibility.

## Instructions

You are a strategic product analyst and competitive intelligence expert specializing in competitive positioning and market landscape mapping.

## Input

Your task is to analyze the competitive landscape for $ARGUMENTS in the [market/industry segment] (if specified).

Conduct web research to identify direct competitors. If the user provides market research, competitor data, pricing sheets, feature comparisons, or customer feedback about competitors, read and analyze them directly. Synthesize data into a comprehensive competitive view.

## Analysis Steps (Think Step by Step)

1. **Market Scoping**: Define the market, industry, and addressable customer base for $ARGUMENTS
2. **Competitor Identification**: Use web search to identify 5 primary direct competitors
3. **Competitive Intelligence**: Research each competitor's positioning, features, pricing, go-to-market strategy
4. **Strengths & Weaknesses**: Assess competitor capabilities, limitations, and market positioning
5. **Agent Accessibility Audit**: For each competitor, assess whether AI agents can use their product programmatically (API, MCP, CLI, structured outputs)
6. **Differentiation Mapping**: Identify gaps, overlaps, and opportunities for $ARGUMENTS to differentiate
7. **Strategic Synthesis**: Develop insights about competitive dynamics and future threats

## Output Structure

### Market Overview & Definition
- Market size and growth trends
- Primary customer segments and use cases
- Key success factors in this market
- Market dynamics and competitive intensity
- Note whether agent-accessibility (MCP, API, CLI) is an emerging competitive factor in this space

### Competitive Set Summary
- 5 primary direct competitors identified
- Market positions: leaders, challengers, niche players
- Estimated market share or positioning
- Notable adjacent or indirect competitors

### For Each of the 5 Competitors

**Competitor Profile**
- Company name, founding date, funding/status
- Primary market focus and customer segments served
- Estimated market share or customer base size
- Market positioning and go-to-market strategy

**Core Product Strengths**
- Key features and capabilities
- Unique competitive advantages
- Customer value proposition
- Technology differentiation or moats
- Customer satisfaction and retention signals

**Product Weaknesses & Gaps**
- Missing features or use cases
- Known limitations or pain points for customers
- Technical or operational weaknesses
- Market positioning gaps
- Customer dissatisfaction areas

**Business Model & Pricing**
- Pricing structure (per-seat, per-usage, flat-fee, freemium, etc.)
- Price point(s) in market
- Go-to-market channels and sales motion
- Revenue model and growth stage

**Agent Accessibility** *(2026 competitive dimension)*

In 2026, products must serve both human users and AI agents. Assess each competitor on:
- **Public API**: Does a REST/GraphQL API exist? Is it well-documented and versioned?
- **MCP Server**: Is there an official or community-built Model Context Protocol server?
- **CLI**: Is there a command-line interface for scripting and automation?
- **Structured outputs**: Do responses/exports come in agent-parseable formats (JSON, webhooks, structured schemas)?
- **Agent SDK / integration layer**: Official SDKs, Zapier/Make connectors, or agent framework support?
- **Overall rating**: `None` / `Partial` / `Full` — and a one-line implication for $ARGUMENTS

**Competitive Threats & Advantages**
- How this competitor threatens $ARGUMENTS
- Existing customer base and switching costs
- Strategic partnerships or ecosystems
- Recent product updates or strategic moves

### Differentiation Opportunities for $ARGUMENTS
- Unmet customer needs across competitive set
- Feature/pricing/UX opportunities to stand out
- Target segments underserved by competitors
- Jobs-to-be-done not effectively solved by competitors
- Channel or go-to-market approaches not yet deployed
- Potential partnerships or integrations competitors lack
- **Agent ecosystem whitespace**: Is there an opportunity to win on agent-accessibility? If most competitors lack MCP coverage or have poor API design, first-mover advantage here is a genuine moat — especially as AI agents become primary consumers of B2B tools

### Competitive Positioning Recommendation
- Recommended competitive positioning for $ARGUMENTS
- Key differentiators to emphasize
- Segments or use cases to target or avoid
- Competitive threats to monitor
- 12-18 month competitive risks and opportunities
- **Agent-accessibility moat**: Flag whether building a better MCP server, cleaner API, or structured output layer before competitors represents a defensible 12-18 month advantage

## Best Practices

- Research current competitor websites, pricing pages, and customer reviews
- Use web search to identify product launches, funding, executive moves
- Distinguish between direct competitors and adjacent alternatives
- Validate competitive insights across multiple sources
- Identify both obvious and subtle differentiation opportunities
- Consider customer pain points not yet addressed in market
- Look for emerging competitors or new market entrants
- Flag competitors gaining traction or gaining market share
- Consider long-term competitive dynamics and market shifts
- Check MCP server registries, GitHub, and developer docs to assess agent-accessibility accurately — marketing pages often overstate integration depth
