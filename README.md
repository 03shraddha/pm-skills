# product management skills &nbsp;·&nbsp; [try it live →](https://03shraddha.github.io/pm-skills)

**skills vs prompts:** prompts are one-time instructions you retype every session. skills are saved workflows: type `/skill-name` and claude runs a structured process with built-in frameworks and the right output format. write once, reuse forever.

**skills can also bundle** python scripts, reference files, and assets, loaded progressively. only what claude needs, when it needs it. no wasted tokens.

6 claude code skills i think every product person will find helpful. use them to move faster, think clearer, and skip the repetitive stuff.

---

**building for 2026:** products now need to serve two kinds of users: humans through a UI, and AI agents through structured interfaces. agents need:

- a REST or GraphQL API with machine-readable responses (no scraping UIs)
- an MCP server so orchestrators like Claude or Cursor can call your product as a tool
- structured JSON outputs they can parse without regex hacks
- atomic endpoints that do one thing, not bundled workflows
- auth that doesn't require a browser session

notion without MCP, figma without a proper API: agents can't use them. these skills are updated to help PMs design for both surfaces.

---

## skills

| skill | what it does | file |
|-------|-------------|------|
| competitor analysis | maps 5 direct competitors: moats, gaps, pricing, and agent accessibility<br>**in:** product or company name<br>**out:** competitor profiles, differentiation opportunities, battlecard-ready positioning | [competitor-analysis/SKILL.md](./competitor-analysis/SKILL.md) |
| pm brainstorm | generates ideas (PM / designer / engineer / agent layer lenses) or designs lean experiments<br>**in:** product name + mode (ideas or experiments) + stage (existing or new)<br>**out:** ranked ideas or experiment designs with hypothesis and success metrics | [pm-brainstorm/SKILL.md](./pm-brainstorm/SKILL.md) |
| pm assumption mapping | surfaces and prioritizes the riskiest assumptions before you build<br>**in:** feature or product idea + stage (existing or new)<br>**out:** assumption map by category, top 5-7 by impact x evidence, one experiment each | [pm-assumption-mapping/SKILL.md](./pm-assumption-mapping/SKILL.md) |
| pm feature prioritization | scores and segments a backlog into what to build, bet on, or cut<br>**in:** feature requests or backlog items + optional OKRs<br>**out:** RICE-scored backlog, quick wins / big bets matrix, do-not-build list | [pm-feature-prioritization/SKILL.md](./pm-feature-prioritization/SKILL.md) |
| pm customer research | writes interview scripts or synthesizes transcripts into PM insights<br>**in:** mode (script or summarize) + topic/hypothesis or transcript<br>**out:** JTBD interview guide, or insight summary with pain points and opportunities | [pm-customer-research/SKILL.md](./pm-customer-research/SKILL.md) |
| pm product metrics | designs a metrics dashboard or builds an opportunity solution tree<br>**in:** mode (dashboard or ost) + product area or desired outcome<br>**out:** north star + input + health metrics system, or full OST with experiments | [pm-product-metrics/SKILL.md](./pm-product-metrics/SKILL.md) |

---

## how to install

1. download the `SKILL.md` file you want
2. drop it into `~/.claude/skills/` (mac/linux) or `C:\Users\<name>\.claude\skills\` (windows)
3. type `/skill-name` in claude code

---

## why i made this

i got tired of rewriting the same prompts over and over. if you're a pm who uses claude code, these might save you a ton of time too.

more coming: user story writing, prd drafting, sprint retros, stakeholder updates.
