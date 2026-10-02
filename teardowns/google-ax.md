# Google AX: billions of agents in the headline, Kubernetes in the quickstart

## The launch
In the week of September 20, 2026, Google open-sourced AX (Agent Executor) under Apache 2.0 at github.com/google/ax: a declarative orchestrator for running agent workloads at scale. The repo sells "a high-throughput, declarative orchestrator to run billions of autonomous agent workloads in a cluster." v0.3.0 shipped the same week, splitting the runtime into three services (API frontend, reconciler, sandboxed task runner) and moving task state out of Kubernetes custom resources into Redis Streams. The launch thread hit the top of Hacker News, gathering 649 points and 296 comments in roughly 48 hours.
Source: https://dev.to/jamilxt/google-open-sourced-ax-an-orchestrator-for-billions-of-ai-agents-hacker-news-isnt-buying-the-5hgf
Source: https://ai-tldr.dev/releases/google-ax-0-3-0/

## What they did
- Opened with the biggest possible number: "billions of concurrent agent sessions per cluster without orchestrator limits." Four primitives declared in YAML (Task, Workspace, Gateway, Model) behind a kubectl-shaped CLI: `ax apply`.
- Buried the honest part in the README: core concepts are still being refined and "major breaking changes" are likely before a stable release. There is no single-machine path.
- Hid a genuinely clever engineering story under the marketing: moving task state off etcd onto Redis Streams because etcd was not built for millions of short-lived agent tasks, and multiplexing dozens of mostly-idle agent sessions onto each physical pod.
- Showed up in the thread: people working on the runtime answered hard questions, including the admission that per-agent identity injection via OIDC and SPIFFE would land "within a few weeks," not now.

## What worked
- The top-of-HN placement put AX in front of the entire agent-infrastructure audience in a day: 649 points, 296 comments in about 48 hours, the most discussed AI submission on HN that day.
  Source: https://dev.to/jamilxt/google-open-sourced-ax-an-orchestrator-for-billions-of-ai-agents-hacker-news-isnt-buying-the-5hgf
- Third-party breakdowns multiplied the reach: AI Weekly, 8020ai, WeSearch, and multiple dev.to deep-dives covered the v0.3.0 release independently.
  Source: https://aiweekly.co/alerts/google-ships-ax-v030-splits-agent-runtime-into-three-services-and-moves-task
  Source: https://www.8020ai.co/p/google-s-ax-agent-orchestrator-hit-1-on-hacker-news
- The repo sat at roughly 1,968 stars and 623 commits at the time of the writeup, and google/ax landed on GitHub Trending the same week.
  Source: https://dev.to/jamilxt/google-open-sourced-ax-an-orchestrator-for-billions-of-ai-agents-hacker-news-isnt-buying-the-5hgf
  Source: https://dev.to/fenju_fu/googles-ax-and-anthropics-financial-services-are-trending-but-who-solves-long-running-workflow-2ifp

## Takeaways for LegCli
- The headline number you cannot demonstrate becomes the story instead of the product. Never claim scale you cannot benchmark in the same week.
- HN will fact-check the gap between the homepage and the quickstart. The quickstart should make the headline claim feel true within ten minutes.
- Big companies can still win HN by showing up: the runtime team answering hard questions with roadmap honesty earned more goodwill than the marketing.
- Controversy is distribution only if the substance survives it. AX's real ideas (Redis task state, agent multiplexing) landed after the pile-on, because the team engaged instead of hiding.
