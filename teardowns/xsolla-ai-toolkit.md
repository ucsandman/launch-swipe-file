# Xsolla AI Toolkit: ship the SKILL.md, not the docs

## The launch
Xsolla launched the Xsolla AI Toolkit on August 4, 2026 and announced it via press release on September 15, 2026. It is a collection of agent skills that encode correct Xsolla API integration paths directly into AI coding tools: SKILL.md files in a public GitHub repo (xsolla/xsolla-ai-kit), distributed as plugins for Claude Code, GitHub Copilot, Codex CLI, and Cursor (coming soon). The promise: developers go from zero to a fully functional headless web shop in a single afternoon, with validation built in.
Source: https://www.media-outreach.com/news/united-states/2026/09/15/487503/xsolla-launches-ai-toolkit-enabling-engine-agnostic-game-commerce-setup-with-ai-coding-tools/

## What they did
- Diagnosed the failure everyone recognizes: AI coding tools generate syntactically correct code that fails in production because they lack platform-specific context. The press release names the pain before naming the product.
- Chose SKILL.md as the distribution format, shipping where developers already work instead of building a new dashboard or docs site.
- Embedded validation logic end to end: the skills verify integration behavior under real-world conditions, not just with isolated API calls, so "the first attempt is the right attempt."
- Launched with four complete skill areas (login, payments, catalog, merchant setup), each a full validated integration path. No partial coverage, no roadmap promises.
- Maintained by the teams that build the APIs, so the skills stay current as the platform evolves: distribution and maintenance are one motion.

## What worked
- One headline metric everyone repeats: weeks of docs-reading and debugging compressed into "an hours-long, guided build."
  Source: https://www.media-outreach.com/news/united-states/2026/09/15/487503/xsolla-launches-ai-toolkit-enabling-engine-agnostic-game-commerce-setup-with-ai-coding-tools/
- Zero to web shop in a single afternoon, with first-attempt correctness as the claim. A time-boxed outcome beats a feature list.
- Skills live in the AI tools developers already installed, so adoption needs no new habit: install the plugin, keep working.

## Takeaways for LegCli
- Your distribution channel can be a markdown file. A SKILL.md in a public repo reaches Claude Code and Codex users without a marketplace launch.
- Name the failure mode your launch eliminates. "The AI generates code that looks right but fails in production" sold the toolkit; the four skill areas just proved it.
- Ship complete paths, not samples. Four fully validated integration paths beat twenty partial examples for the same reason a full demo beats a teaser.
- Maintenance is a launch message. "Maintained by the teams building the APIs" is why developers will trust the skills six months from now.
