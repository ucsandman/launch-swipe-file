# Docker Agent

## The launch
Docker open-sourced Docker Agent in early October 2026: a CLI plugin that defines AI agents in a declarative YAML file and runs them with the same command grammar as containers. It surfaced on GitHub and picked up attention on Hacker News the same week.
Sources: https://aiweekly.co/alerts/docker-open-sources-yaml-ai-agent-builder-with-mcp-and-rag and http://dev.to/magnus_ferm_maffelu/dev-news-digest-8-oct-2026-0600-3moe

## What they did
- Made agents feel like containers. `docker agent run myorg/agent:tag` pulls an agent definition straight from any OCI registry; a plain `agent.yaml` versions, reviews, and shares like infrastructure as code.
- Stayed model neutral: OpenAI, Anthropic, Gemini, AWS Bedrock, Mistral, xAI, and Docker Model Runner for local inference, with MCP native for tool integration plus built-in think, todo, and memory tools.
- Shipped Apache-2.0 and preinstalled it inside Docker Desktop 4.63+, with Homebrew as the alternate install. The release train moved fast: v1.149.0 was the current build within days.
- Framed multi-agent orchestration as "teams of specialized agents that delegate tasks automatically," planting a flag in the crowded agent-builder category.

## What worked
- Distribution beat announcement. The plugin arrives on "several million dev machines quietly gaining an agent runtime, one auto-update at a time," via Desktop auto-updates rather than a launch-day download.
  Source: https://dev.to/slabb/docker-just-shipped-the-agent-wall-i-wanted-its-off-by-default-f18
- The YAML-as-config choice made the security story reviewable: tool permissions declared as an allowlist in a diffable file, which won over the policy-minded crowd on day one.
  Source: https://dev.to/slabb/docker-just-shipped-the-agent-wall-i-wanted-its-off-by-default-f18
- Instant community coverage: walkthroughs and security commentary appeared within 48 hours, doing launch amplification Docker never had to buy.
  Source: https://aiweekly.co/alerts/docker-open-sources-yaml-ai-agent-builder-with-mcp-and-rag

## Takeaways for LegCli
- Piggyback on an installed base. Docker skipped the distribution problem by riding Desktop updates. LegCli's equivalent is shipping where agents already run, not asking users to install a new home.
- Borrow the grammar, not just the branding. `docker agent run` inherits years of muscle memory. LegCli commands should mirror the session verbs people already type.
- Make the security posture diffable. A permissions block a reviewer can read in a PR beats a trust-me paragraph. LegCli's session handoff should look auditable on its face.
- Silent rollout has a trust cost. The same auto-update distribution that won the reach drew "off by default" commentary. If you ship quietly, say so loudly.
