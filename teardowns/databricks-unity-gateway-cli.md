# Databricks Unity Gateway CLI: one command, freedom plus governance

## The launch
On September 24, 2026, Databricks introduced the Unity Gateway CLI in an official blog post: a command-line tool that connects coding agents such as Claude Code and Codex to Unity Gateway, where administrators manage approved models, tools, and spending policies. The pitch is a single `ug` command that pairs developer freedom to adopt new agents and models with centralized governance across thousands of developers.
Source: https://www.unite.ai/databricks-introduces-unity-gateway-cli-to-centralize-coding-agent-control/

## What they did
- Framed the release against model churn: GPT-6, Claude Opus 5.5, Gemini 3.8, and Grok 4.7 shipped in the prior six months, "a new frontier model roughly every five days." The villain is the pace, not a competitor.
- Diagnosed the platform-team squeeze precisely: standardize on one provider and miss better or cheaper options; support many agents and scatter access control, budgets, security policy, and usage logging. Then positioned the CLI as the answer to both sides.
- Launched with a customer proof point baked in: Concurrence CTO John Xing said its coding agents have processed more than 61 billion input tokens across roughly 360,000 requests through the CLI, with attribution down to the individual user.
- Stacked their own verified numbers: Smart Routing delivered 35% cost savings on their internal coding benchmark, and tracing plus Genie One found and fixed seven MCP tool bugs, estimated at $1.2 million per year in wasted AI spend and lost productivity.
- Made adoption safe to try: every overwritten config file is backed up with `ug revert` to restore, existing `ucode` commands keep working, and admins can push new default models as one published configuration change.
- Covered the whole agent surface at once: Codex, Claude Code, Gemini CLI, OpenCode, GitHub Copilot CLI, and Pi, plus Cursor Agent through MCP.

## What worked
- The customer number did the heavy lifting: 61 billion tokens across 360,000 requests is a scale proof no marketing claim could match, and every writeup led with it.
  Source: https://www.unite.ai/databricks-introduces-unity-gateway-cli-to-centralize-coding-agent-control/
- The "every five days" model-pace framing gave the story urgency independent of the product: it explains why governance tooling matters right now.
- Publishing their own savings (35% benchmark cut, $1.2M per year) let Databricks sell the same tool they dogfood, which enterprise buyers read as proof.

## Takeaways for LegCli
- When you ship to admins and developers at once, speak to both in one sentence: "freedom to adopt, centralized governance" is the whole launch in six words.
- A named customer with a real number beats ten feature bullets. Recruit one proof point before launch day.
- Backward compatibility is a launch feature: "existing ucode commands keep working" disarms the migration objection in a single line.
- Dogfood numbers are free marketing: Databricks' own org savings cost them nothing to publish and gave every outlet a headline.
