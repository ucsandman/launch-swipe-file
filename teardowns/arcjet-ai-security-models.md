# Arcjet AI security models

## The launch
On November 5, 2026, Arcjet announced a family of custom AI security models for coding agents, then launched them on Product Hunt on November 9. Himalia 1, a general-purpose prompt injection detector, went live immediately for every SDK call using prompt injection detection. Thebe 1 (for coding agents) and Carme 1 (for autonomous security agents) opened in early access. All three are small classifiers fine-tuned from Qwen3-0.6B, and each is named after a moon of Jupiter.
Sources: https://arcjet.com/blog/introducing-arcjets-custom-ai-security-models, https://www.prnewswire.com/news-releases/arcjet-launches-custom-ai-security-models-to-protect-ai-agents-302930835.html

## What they did
- Launched a family, not a feature. Three named models with three distinct jobs turns one capability (prompt injection detection) into a product line, and gives the press three things to write about.
- Named the models like a product, not a version number. Himalia, Thebe, and Carme are memorable, themed, and easy to reference in conversation. "Which model caught it?" has an answer people can repeat.
- Published the training story and the numbers. The blog explains the fine-tuning, the 0.6B-parameter base, and the classification architecture that returns a verdict without generating text. The press release gives F1 scores on two public datasets.
- Split availability on purpose. One model live today for everyone, two in early access for a narrower audience. The split creates a second news beat and a reason to talk to sales.
- Ran the press release and the Product Hunt launch as one campaign. The announcement (November 5), the trade press coverage, and the Product Hunt listing (November 9) all landed in the same week with the same three names.

## What worked
- Product Hunt: 238 upvotes and 40 comments, #4 Product of the Day on November 9, 2026, with a 5.00/5 average across its reviews.
  Source: https://www.hunted.space/product/arcjet
- Himalia 1 scored F1 0.964 and 0.971 on two public prompt injection datasets, a concrete number that every write-up quoted.
  Source: https://www.prnewswire.com/news-releases/arcjet-launches-custom-ai-security-models-to-protect-ai-agents-302930835.html
- Trade press picked up the story within a day: Computer Weekly ran a dedicated piece on why coding agents need prompt injection detectors, extending the launch beyond the Product Hunt audience.
  Source: https://www.computerweekly.com/blog/CW-Developer-Network/By-Jupiter-Arcjet-on-why-coding-agents-need-prompt-injection-detectors

## Takeaways for LegCli
- Name the parts. LegCli's handoff bundle has components (context, decisions, next steps); giving them names turns a format into a system people can talk about.
- One live, two in early access is a launch shape worth copying. Ship the core handoff now, put the next two capabilities (for example, cross-machine sync and team handoff) in early access, and the launch gets a second act.
- Publish the evaluation, not just the claim. Arcjet's F1 scores did the persuading. If LegCli can measure anything (handoff fidelity, tokens saved, time to resume), that number belongs in the launch post.
- A small model doing one job well is a story in itself. LegCli does not need to be a platform to launch; being the best at one narrow job (keeping a session alive) is the pitch.
