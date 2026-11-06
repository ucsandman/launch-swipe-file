# Entire

## The launch
On October 26, 2026, former GitHub CEO Thomas Dohmke launched Entire, a Git forge built for teams whose AI agents write most of the code. The core product swap: pull requests are out, "Trails" are in. When code is submitted, review agents score it automatically and humans review a dashboard of scores instead of reading line by line. A second pillar, Continuous Memory, stores the context behind every change so future agent sessions can look up why a decision was made. Entire had disclosed a $60 million seed round in February 2026 at a $300 million valuation, and launched with a 50-person fully remote team.
Sources: https://www.geekwire.com/2026/former-github-ceo-launches-rival-platform-built-for-ai-coding-agents/, https://automater.ai/news/entire-git-forge-trails-replace-pull-requests/, https://www.techtimes.com/articles/329530/20261027/github-had-257-incidents-12-months-entire-ships-distributed-forge-ai-agents.htm

## What they did
- Launched two days before GitHub Universe 2026. The timing was either good fortune or a deliberate jab, and every Universe story became a chance to mention Entire as the alternative. A challenger with no distribution bought itself a news cycle by standing next to the incumbent's biggest week.
- Let the founder be the distribution. Dohmke ran GitHub for four years, so the story wrote itself: the person who built the old system explaining why it cannot hold agent traffic. No ad spend can buy that credibility, and the press led with his name, not the feature list.
- Replaced the unit, not the workflow. Trails keep the familiar shape of "propose, review, merge" but swap the diff for a scoreboard: agent-scored evals on security, quality, and risk, with agents looping on findings until evals pass. A new unit is easier to explain than a new process.
- Shipped the memory story as open-source, local-first CLI tools. entire-graph parses a repo with tree-sitter into a map of definitions and callers with no network or model calls, and entire-brain indexes agent session logs recorded in Git history. Giving away the plumbing buys trust with the exact audience being asked to migrate hosting.
- Softened the migration cliff. Entire offers GitHub mirroring and first-party CI importers (Buildkite and Depot) that convert existing GitHub Actions workflows, including secrets, with minimal rewriting. Public repos and self-hosting are roadmap, not launch, so the ask at launch is private-repo teams only.

## What worked
- The "former GitHub CEO launches rival" frame carried the launch across GeekWire, Tech Times, TechGig, and The New Stack within a day, with coverage adopting Entire's own language: "the Git forge for agent-human collaboration."
  Source: https://www.geekwire.com/2026/former-github-ceo-launches-rival-platform-built-for-ai-coding-agents/
- The comparison stories wrote themselves. Entire was benchmarked against Cursor Origin (launched August 2026) as the second agent-native forge, and its claimed 89x faster Git hosting versus GitHub became the pull quote in nearly every piece.
  Source: https://techgig.com/amp/news/software-devops/former-github-ceo-launches-entire-a-git-forge-for-humans-and-ai-agents/135221614
- The seed number did narrative work. A $60 million seed at a $300 million valuation, led by Felicis with Madrona and Microsoft's M12, signaled that serious money believed the incumbent was vulnerable, which is itself a launch asset.
  Source: https://automater.ai/news/entire-git-forge-trails-replace-pull-requests/

## Takeaways for LegCli
- Continuous Memory is the closest thing in the wild to LegCli's territory: session context that survives across agent runs. Entire bundles it inside a forge; LegCli's pitch is that the handoff layer should be forge-neutral. Name that difference on launch day, before someone else frames LegCli as a feature of a forge.
- Timing a launch against the incumbent's conference is free distribution, but only if the story is genuinely newsworthy. Entire earned it with a founder story and a product swap. A LegCli launch timed to a vendor event needs the same bar: a real artifact, not just a post.
- Open-source the plumbing, sell the coordination. Entire's local-first CLI tools are the trust anchor for a product asking teams to move their code. LegCli's free artifact (the resume bundle) plays the same role; keep it genuinely useful standalone.
- The 89x and 71% figures are Entire's own pre-release numbers, flagged as unverified in coverage. Borrow the ambition, not the method: LegCli's numbers on launch day should be numbers a third party can reproduce.
