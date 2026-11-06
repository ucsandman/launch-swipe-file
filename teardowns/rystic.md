# Rystic

## The launch
On October 26, 2026, founders Zachary Kiihne and Evan Whitehouse publicly launched Rystic (YC Fall 2026) with an X post and a launch post on Y Combinator: local copies (simulators) of the APIs an agent uses, including Slack, GitHub, Stripe, PayPal, Okta, Linear, and S3. The simulators keep state, so if an agent adds a customer, the next call sees it. Free tier: 10 hours a month on one seat. Pro is $89.99 per seat a month with $100 of credit per seat and adds fault injection. Enterprise runs fully offline.
Sources: https://www.thetoolnerd.com/p/new-ai-tools-this-week-oct-27-2026, https://medium.com/@zkiihne/launching-rystic-25885e5bcb0d

## What they did
- Launched on X and YC on the same day, with the founder's own account as the channel. The X post ("local copies of Slack, Stripe, S3 and the rest of your stack") is one sentence of product, no thread of hype. The YC launch post carried the longer explanation, so each channel did what it is good at.
- Named the gap between two bad options. The launch post's argument: mocks are not real enough, and live APIs are too dangerous for agents that take real actions. A simulator that keeps state is the third option, and the pitch is legible in one paragraph.
- Published a fidelity number instead of a feature list. Before each release, Rystic sends the same requests to the live API and the simulator and publishes how often they match: Slack matched 96.7% across 538 checks. A verifiable accuracy claim beats a screenshot for a testing tool.
- Priced the free tier in hours, not requests. Ten free hours a month maps to how a developer actually tries a testing tool (a session, not a quota), and Pro's $100 credit per seat softens the $89.99 sticker by making the first month feel prepaid.
- Rode the YC batch wave. Rystic launched into a Fall 2026 batch where at least nine companies sell ways to run or test agents, so "agent infrastructure" was already a funded category. The YC label did the credibility work a solo launch would have to earn post by post.

## What worked
- The launch post's framing (mocks too fake, live APIs too risky) was picked up verbatim by round-ups within a day, and the 96.7% Slack fidelity figure became the detail every summary repeated.
  Source: https://www.thetoolnerd.com/p/new-ai-tools-this-week-oct-27-2026
- The X launch post drew 6.02K views on day one from a founder account, respectable for a first announcement with no paid boost, and the YC post gave it a second, more durable home for search.
  Source: https://www.thetoolnerd.com/p/new-ai-tools-this-week-oct-27-2026
- The category tailwind was real. YC's Fall 2026 batch lists Rystic alongside other agent-testing companies (Hue, Mirrors, Papaya), so buyers already had a mental shelf for it.
  Source: https://www.ycroaster.com/blog/what-is-yc-funding-fall-2026-f26-companies-yc-w27-application

## Takeaways for LegCli
- A fidelity-style number is LegCli's best launch asset too. "Sessions resumed with full context" is a claim; a measured number (for example, context items preserved across a handoff, counted on a public test repo) is evidence. Publish the method with the number.
- One sentence on X plus a long post elsewhere is a good channel split for an indie launch. LegCli's launch should have the same shape: a single quotable line for the feed, and a full teardown-ready post for the people who click through.
- Price the free tier in the unit the user thinks in. Rystic's hours map to a session; LegCli's free artifact maps to one handoff. Both let a developer finish something real before paying.
- A batch, cohort, or event label is borrowed credibility. LegCli has the hackathon entry and the open-source repos; the launch should name whichever affiliation is real and let it do the trust work.
