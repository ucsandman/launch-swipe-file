# Agent Swarm

## The launch
Desplega Labs' Agent Swarm, an open-source MIT "company operating system" for AI agents, resurfaced on Hacker News on October 9, 2026 with release v1.167.0. The pitch: a lead agent takes work in from Slack, GitHub, email, or an API and delegates it to worker agents (Claude Code, Codex, opencode, Cursor, Amp, Grok, Devin, and others), each running in an isolated Docker container with shared memory and review gates. Repo was created December 2025, so this was a relaunch after nearly a year of building.
Sources: https://explainx.ai/blog/agent-swarm-desplega-open-source-company-os-lead-agent-workers-guide-2026

## What they did
- Relaunched with a category name, not a feature list. "Company OS" gives people one mental model to carry: work in, PRs and replies out, memory and schedules in the middle.
- Framed as harness agnostic: a layer above Claude Code rather than a replacement for it. That turns every rival into a supported worker instead of a competitor.
- Listed concrete new additions in the HN comment: safe code-mode-like scripts, an agent-fs integration (described as a Google Drive rebuilt for agents), pages and apps (artifacts), and extensions as trusted TypeScript hooks installed as inert drafts that a trusted operator must activate.
- Shipped the install inside tools people already use: `npx skills add desplega-ai/agent-swarm`, Claude Code marketplace plugins, Docker Compose, Helm chart, npm and bun packages.
- Dogfooded aggressively: many recent PRs are authored by their own `desplega-bot`, and they ship daily (v1.165.0 and v1.166.0 on Oct 8, v1.167.0 on Oct 9). Velocity became part of the pitch.

## What worked
- GitHub API at launch time showed about 874 stars, 116 forks, 2,600+ commits, 15 open issues and 7 open PRs, real scale signals for a 10-month-old repo.
  Source: https://explainx.ai/blog/agent-swarm-desplega-open-source-company-os-lead-agent-workers-guide-2026
- Independent coverage amplified the relaunch: explainx.ai published a full guide the same day, reading the repo, release notes, and HN post for anyone who would not install first.
  Source: https://explainx.ai/blog/agent-swarm-desplega-open-source-company-os-lead-agent-workers-guide-2026
- The HN thread itself was thin, only a few comments with one calling it potentially revolutionary. The launch did not live or die on the thread; it lived on the packaging.

## Takeaways for LegCli
- A relaunch is a launch. Nearly a year of invisible building became the story when packaged as v1.167.0 plus new features plus MIT licensing in one week.
- Name the category, not the feature list. "Company OS" is doing more work than any feature bullet. LegCli needs its own one-phrase mental model.
- Harness agnostic beats harness captive. Supporting every worker means no audience feels excluded, and every competitor becomes an integration.
- Ship where people already are. The npx/plugin/Compose install routes mean traffic never has to learn a new tool to try the demo.
- Watch the dogfood signal. Bot-authored commits sell velocity but raise trust questions; a human reviewing the README and releases matters as much as the commit count.
