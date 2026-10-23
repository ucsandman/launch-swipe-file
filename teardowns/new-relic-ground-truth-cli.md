# New Relic Ground Truth CLI

## The launch
New Relic announced Ground Truth CLI on October 6, 2026: a command-line interface bringing operational intelligence into developer and AI agent workflows. The pitch: engineers and agents can investigate production issues, verify recovery criteria, and preserve evidence without leaving the terminal. It extends the existing Ground Truth MCP connector into command-line workflows.
Sources: https://digitalitnews.com/new-relic-launches-ground-truth-cli-for-developer-and-ai-agent-workflows/

## What they did
- Launched a CLI, not a feature, as a first-class product with its own announcement, press syndication, and named head of AI quote (Camden Swita: "Every developer and AI agent needs trusted operational context").
- Framed it for two drivers at once: "whether a human or an AI agent is driving," so the same launch speaks to SREs and to the agent-workflow audience in one breath.
- Built the story around four verbs: investigate with operational context, verify recovery criteria, preserve and review evidence, and bring operational intelligence into AI workflows programmatically.
- Named the resume capability outright: captured findings "can then support follow-up analysis or a handoff to another engineer." Persistence across sessions is the headline, not a footnote.
- Bundled it into the "New Relic Now October 2026" round-up alongside AI Evaluation for generative AI observability and Infrastructure 360, so the CLI launch rides a month-long news cycle instead of standing alone.

## What worked
- The "preserve and review evidence" hook lands because it names a pain everyone has lived: restarting an investigation from zero. The quote-worthy sentence did the syndication work.
- Dual audience doubles the channels. The same announcement runs in SRE press and agent-workflow press, since the CLI serves humans, agents, scripts, and CI pipelines.
- Two entry points compound. Ground Truth already shipped as an MCP connector; the CLI gives the same intelligence to people and agents who live in terminals rather than tool-enabled assistants.
  Source: https://digitalitnews.com/new-relic-launches-ground-truth-cli-for-developer-and-ai-agent-workflows/

## Takeaways for LegCli
- Launch the CLI as the product, not the feature. A command-line announcement with its own press run treats terminal-first users as first-class, which is exactly LegCli's audience.
- Name resume explicitly. New Relic said "so work can be resumed, reviewed and shared without restarting the investigation" in the launch copy. LegCli should say the handoff promise in the headline too.
- Frame for both drivers. Every LegCli demo should show a human resuming AND an agent resuming; the same artifact serves two audiences at once.
- Ride a round-up. Shipping the launch inside a monthly or weekly news cycle gives it a second wave of pickup. LegCli's hackathon wins, releases, and guides can bundle the same way.
