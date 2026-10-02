# Claude Sonnet 5.5: flat price, efficiency story

## The launch
Anthropic released Claude Sonnet 5.5 on September 28, 2026, the second model in the Claude 5.5 family, positioned as the faster everyday workhorse. It shipped the same day on the Claude Platform, AWS, Google Cloud, Microsoft Azure, and Microsoft Foundry with zero data retention. GitHub added the model to Copilot the same day for Pro, Pro+, Max, Business, and Enterprise users across VS Code, Visual Studio, the Copilot CLI, JetBrains, Xcode, and github.com.
Sources: https://pondero.ai/news/2026-09-29-anthropic-claude-sonnet-5-5/ and https://thinkreview.dev/blog/claude-sonnet-5-5-now-available-in-thinkreview

## What they did
- Split the family in one sentence: Opus 5.5 is for complex work that needs careful judgment, Sonnet 5.5 is for well-scoped everyday tasks, fixing bugs, and polished documents.
- Held list prices flat ($2 input, $10 output per million tokens, half of Opus 5.5's $4/$20) and sold efficiency instead: fewer tokens per task, output over 30% faster, up to 30% less cost per task.
- Led the benchmark table with the number that stuns: Terminal-Bench 4.0 jumped from 10.3% (Sonnet 5) to 70.6%, ahead of Opus 5.5's 66.4%, while stating plainly that Opus remains stronger on the other benchmarks.
- Made Sonnet 5.5 the model used for the free tier on claude.ai, so every free user runs the launch.
- Shipped it with the frontier cybersecurity controls and anti-distillation classifiers previously reserved for the flagship, positioning mid-tier as enterprise-safe.

## What worked
- Terminal-Bench 4.0: 70.6% for Sonnet 5.5 versus 10.3% for Sonnet 5 and 66.4% for Opus 5.5, at half the per-token price, per Anthropic's launch benchmarks.
  Source: https://pondero.ai/news/2026-09-29-anthropic-claude-sonnet-5-5/
- 30%+ faster output generation and up to 30% less cost per task, per Anthropic's announcement.
  Source: https://everydayaiblog.com/claude-sonnet-5-5/
- Same-day availability in GitHub Copilot across every IDE surface, billed at provider list pricing, turning the Copilot channel into launch-day distribution.
  Source: https://pondero.ai/news/2026-09-29-anthropic-claude-sonnet-5-5/

## Takeaways for LegCli
- When the price cannot move, sell the cost per outcome. "30% less per task" is a better launch headline than any discount an indie could afford.
- One killer number plus one honest concession. The Terminal-Bench jump sells the release; the admission that Opus wins elsewhere makes the claim believable.
- Free tier as distribution. Putting your strongest option in front of free users turns every usage stat into a marketing number.
- Split the line in one sentence. "Opus for judgment, Sonnet for everyday tasks" tells every buyer exactly which product is theirs without a comparison page.
