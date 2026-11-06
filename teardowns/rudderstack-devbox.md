# RudderStack DevBox

## The launch
On November 3, 2026, RudderStack open-sourced DevBox, the agent harness behind about 35% of its merged pull requests, with a Show HN post and the code on GitHub. DevBox runs one sandbox per task with no real secrets inside, on Kubernetes or your own machine, plus a CLI that spins up dependent services for end-to-end checks and hooks into Slack, Linear, and GitHub. RudderStack says it has merged over 1,900 PRs from it since April, mostly small to mid-sized features, while bigger projects still go to Claude or Codex.
Source: https://www.vibehacker.com/news/rudderstack-open-sources-devbox-the-agent-harness-behind-about-35-of-its-merged-

## What they did
- Open-sourced a tool they already depended on. DevBox was not built for the launch; it was extracted from production use, so every claim in the announcement had months of internal evidence behind it.
- Led with a production number, not a feature list. "About 35% of our merged PRs" is the whole pitch in one line, and it is a number only a real user of the tool could state.
- Scoped the claim honestly. Saying bigger projects still go to Claude or Codex costs nothing and buys credibility: a harness that admits its limits is easier to believe about its strengths.
- Shipped the boring parts as features. One sandbox per task, no real secrets inside, a CLI that spins up dependent services: these are the unglamorous details that make an agent harness usable in a real company, and they were front and center.
- Launched on Show HN with the repo as the only destination. No landing page funnel, no waitlist, no demo video required. The audience was developers, and developers were sent straight to the code.

## What worked
- The 35% figure did the distribution work. It is the detail every summary repeated, because it turns an abstract harness into a measured outcome.
  Source: https://www.vibehacker.com/news/rudderstack-open-sources-devbox-the-agent-harness-behind-about-35-of-its-merged-
- The 1,900-plus merged PRs since April gave the number a time dimension, so the story was sustained use rather than a one-week experiment.
  Source: https://www.vibehacker.com/news/rudderstack-open-sources-devbox-the-agent-harness-behind-about-35-of-its-merged-
- The Show HN post landed November 3, a Tuesday, catching the midweek developer audience instead of competing with weekend hobby launches.
  Source: https://www.vibehacker.com/news/rudderstack-open-sources-devbox-the-agent-harness-behind-about-35-of-its-merged-

## Takeaways for LegCli
- Dogfood numbers are the strongest launch asset an indie has. LegCli should launch with its own usage stat (sessions resumed, handoffs completed, context preserved) measured on its own work, not a benchmark run for the occasion.
- Admit the boundary. DevBox saying big projects still need Claude made the 35% believable. LegCli should name what handoffs do not solve yet, in the launch post itself.
- Open-sourcing the tool you actually use beats announcing a tool you just built. If LegCli's launch can point at months of real handoffs, the story writes itself.
- A single production metric beats a feature list. Pick one number for the LegCli launch (for example, share of sessions resumed without re-explaining context) and put it in the first sentence.
