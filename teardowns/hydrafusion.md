# GitHub HydraFusion: the router, not the model

## The launch
GitHub announced Project HydraFusion on September 4, 2026 as a research preview for Copilot, then pushed it into Copilot CLI's `/experimental` flag in the September 7 weekly releases (changelog published September 10). The press wave ran through the week of September 7-18. HydraFusion is routing software, not a new frontier model: you select HydraFusion the way you would pick Claude or GPT, and Copilot decides how many models to run on that one task, and in what order.
Source: https://github.blog/changelog/2026-09-10-github-copilot-weekly-releases-september-7/

## What they did
- Launched a *mode*, not a model. "You pick HydraFusion, not a single model" is one sentence that reframes the whole product.
- Named three concrete execution patterns anyone can remember: Single (one model), Cascade (cheap model drafts, quality gate escalates), Critique (one model writes, another family reviews, no repo write access).
- Published benchmark tables with both cost and quality, side by side. No cherry-picking: they printed the benchmark where quality dropped.
- Rolled it out as a research preview behind `/experimental`, so the bar was "try and give feedback" rather than a big-bang claim. The September 7 weekly releases changelog bundled it with Jira canvas and voice mode, making the launch week feel full.
Source: https://www.shashi.co/2026/09/github-launches-hydrafusion-copilot.html

## What worked
- Estimated cost 36% to 67% lower than Claude Opus 5 across three benchmarks (TerminalBench 2.1, DeepSWE, CheckpointBench), per GitHub's own figures: TerminalBench 67% lower at +4.9 quality points; DeepSWE 36% lower at -1.5 points; CheckpointBench 65% lower at -0.1 points.
  Source: https://www.shashi.co/2026/09/github-launches-hydrafusion-copilot.html
- Framed as GitHub's "first bet" on a move from "choosing the best model" to "dynamically constructing the best way to solve each task." The narrative upgrade did the marketing: press called it "a multi-model future for AI coding."
  Source: https://www.techtarget.com/it-infrastructure/news/366650182/GitHub-tests-multi-model-routing-with-HydraFusion
- Available on all Copilot plans with no separate product fee: the preview is distribution into an existing install base, not a new funnel.

## Takeaways for LegCli
- Launch a mode before you launch a product. A named workflow inside an existing tool gets tried; a whole new product gets bookmarked.
- Ship numbers that admit a downside. GitHub printed the benchmark where HydraFusion lost on quality, and nobody noticed the loss: they noticed the honesty.
- Cost is a narrative, not a feature. "You pay the standard token rate for each model it called" makes the pricing boring on purpose so the routing story stays interesting.
- A changelog post can be the launch. GitHub's September 7 weekly releases did as much distribution work as the original blog post.
