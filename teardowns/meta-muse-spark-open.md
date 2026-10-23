# Meta Muse Spark Open

## The launch
On October 15, 2026, Meta Superintelligence Labs released Muse Spark Open: an 816-billion-parameter mixture-of-experts model (42B active per token, 1M-token context window, natively multimodal input), positioned for coding and agentic workloads. Meta called it "the most capable US open-weight model to date," a direct claim aimed at the Chinese labs dominating open-weight leaderboards.
Sources: https://tech-insider.org/meta-muse-spark-open-seven-clouds-launch-2026/

## What they did
- Turned distribution into the launch story. Muse Spark Open went live simultaneously on seven hosted-inference providers (Baseten, Fireworks AI, Groq, Modal, Nebius, OpenRouter, Together AI) and four weight channels (Amazon SageMaker AI, Google Cloud Model Garden, Hugging Face, Microsoft Foundry Models). Eleven partners lined up before the announcement, which means weeks of quiet enterprise business development behind the "research release."
- Named the enemy precisely. "Most capable US open-weight model" is aimed at DeepSeek, Qwen, and GLM by implication without naming them, and gives US enterprise buyers a permission structure to choose it.
- Demoed it running on two Apple M5 Ultra Mac Studios via MLX. Frontier-scale open models are usually framed around data-center clusters; a desk-under-workstation demo reframes the cost calculus against closed subscriptions.
- Ran a two-tier strategy in the open. Closed Muse Wonder stays the premium flagship while the open model builds developer goodwill and the fine-tuning ecosystem; Chief AI Officer Alexandr Wang has said Meta will generally not open-source its most powerful models.
- Fed the ecosystem on day zero. Intel announced day-zero support through its own newsroom, and Microsoft published its own Foundry Models post, so partners amplified the launch instead of Meta shouting alone.

## What worked
- Tech press framed the launch around the distribution footprint rather than benchmarks: "a rollout pattern that looks less like a research paper drop and more like a coordinated product launch."
  Source: https://tech-insider.org/meta-muse-spark-open-seven-clouds-launch-2026/
- Meta walked in with incumbency. McKinsey research cited in coverage found 61% of open-source adopters had used Llama versus 40% for Google's Gemma, so the launch landed on existing pipelines, not fresh installs.
  Source: https://tech-insider.org/meta-muse-spark-open-seven-clouds-launch-2026/

## Takeaways for LegCli
- Line up the distribution before the announcement. Eleven partners on day one means the launch lands in eleven inboxes at once. LegCli's launch should pre-seed the channels: HN, X, Reddit, the plugin marketplaces, the MCP registry.
- A named enemy sharpens the story. "US open-weight vs Chinese labs" is positioning, not benchmarks. LegCli needs its foil: what the handoff experience is like today without it.
- Show it running somewhere unexpected. The Mac Studio demo earned coverage beyond the model press. LegCli's equivalent is a demo in a session type nobody expects to survive, like a cheap phone agent or a dying container.
- The free tier is the acquisition engine. Open-weight goodwill builds the ecosystem that sells the closed flagship. LegCli's $79 tier and team tier need a free artifact (a great README, a working demo session) doing the same job.
