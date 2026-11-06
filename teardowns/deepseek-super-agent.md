# DeepSeek Super-Agent

## The launch
On October 31, 2026, DeepSeek's Harness team published Super-Agent as an open-source prototype of a proactive coding agent on GitHub. It is scoped to one GitHub repository at a time and can also listen to Feishu, ByteDance's workplace chat app, for requests from approved team members. Its stated design goal is to use as little human attention as possible while delivering as much value as possible. DeepSeek calls it a research prototype, not an official product, and says the public code differs from its internal version.
Sources: https://dev.to/jathurshan_sownthararasa_/three-new-ai-agent-tools-to-try-this-week-super-agent-cartesia-herdr-5a80, https://github.com/deepseek-ai/dsh-superagent-prototype

## What they did
- Launched with a single GitHub repo and a manual, no landing page, no pricing page, no waitlist. The repo is the launch artifact, and the README does the selling.
- Led with a behavior, not a benchmark. The hook is an agent that watches developer group chats and suggests solutions without being summoned. Proactive beats reactive as a one-sentence pitch because every developer has felt the cost of the summons.
- Scoped the promise hard. One repo at a time, approved Feishu members only. A narrow scope makes a research prototype credible instead of vaporous, and it gives skeptics a concrete thing to try.
- Disclaimed loudly and early. "Research prototype, not an official DeepSeek product" plus "review and adapt the code before running it" is unusual candor from a big lab, and it reads as confidence rather than hedging because the code is right there to inspect.
- Priced it at zero with MIT licensing. You pay only for whatever model access you connect, so the cost of trying it is an afternoon, not a budget decision.

## What worked
- The launch was covered within a day by The Next Web and dev-tool round-ups, riding the DeepSeek name plus a genuinely new behavior (an agent that acts before being asked).
  Source: https://thenextweb.com/news/deepseek-super-agent-open-source-coding-agent
- The repo-first launch meant the entire funnel was one click: read the announcement, open the repo, clone it. No email capture in between to leak interest.
  Source: https://github.com/deepseek-ai/dsh-superagent-prototype
- The Feishu angle gave the story a second hook for team-tool coverage: an agent that lives in the group chat, not in a separate dashboard nobody opens.
  Source: https://dev.to/jathurshan_sownthararasa_/three-new-ai-agent-tools-to-try-this-week-super-agent-cartesia-herdr-5a80

## Takeaways for LegCli
- A behavior is a better hook than a capability. LegCli's version: an agent session that survives the machine, not a tool that saves context. Name the moment it changes, the way Super-Agent names the unsummoned suggestion.
- A narrow, honest scope beats a broad, hedged one. LegCli should launch with one crisp promise (resume any session on any machine) and say plainly what it does not do yet.
- Open source is the cheapest trust mechanism available. If LegCli's core stays open, the launch post can point at code instead of claims, and the disclaimer that would sink a paid product becomes a strength.
- Big-lab launches prove the category, not the winner. DeepSeek validating proactive agents makes room for an indie to own the narrower slice: session persistence across machines, which a single-repo prototype does not touch.
