# Sphinx

## The launch
On October 18, 2026, a solo developer posted Sphinx to Show HN: an MIT-licensed git hook that quizzes you on your AI agent's code before a push to a protected branch completes. The repository (github.com/parthh01/sphinx) had been created four days earlier, on October 14. No company, no funding, no marketing budget.
Sources: https://trendintech.com/sphinx-git-hook-ai-code-quiz-2026/, https://foundermag.co/launches/sphinx/

## What they did
- Led with a tagline that is the whole pitch: "You can outsource your thinking, but not your understanding." The README opens with a worked example of a wrong answer turning into a lesson, so a reader understands the product in 30 seconds.
- Inverted the crowded AI code-review category. Every other tool reviews the code; Sphinx reviews the developer. The reviewer model reads only the committed diff through read-only git operations, never the coding agent's conversation, so the agent cannot answer for you.
- Shipped a deliberately soft gate. `sphinx yolo` bypasses the quiz, and every skip is logged. It is a team norm instrument, not an enforcement layer, which defused the "another annoying gate" objection before it formed.
- Made cost a non-objection. Quizzes run on your existing coding agent, OpenRouter, or any OpenAI-compatible endpoint with minimal tokens; `.env` files and keys are never opened.
- Rode a live public anxiety. The next day, October 19, an Ask HN thread on shipping AI-written code you do not understand pulled 592 points and 709 comments.
  Source: https://stackness.dev/blog/comprehension-gate-ai-generated-code-before-shipping-sphinx

## What worked
- Show HN post reached 252 points with 85 comments; repo went from creation to front-page discussion in four days with zero marketing spend.
  Source: https://trendintech.com/sphinx-git-hook-ai-code-quiz-2026/
- Third-party coverage framed it as a new category ("comprehension gate"), not a new tool, within days: trendintech, foundermag, stackness, and dev.to taxonomy posts all covered it the same week.
  Sources: https://trendintech.com/sphinx-git-hook-ai-code-quiz-2026/, https://stackness.dev/blog/comprehension-gate-ai-generated-code-before-shipping-sphinx

## Takeaways for LegCli
- Name the category, not just the tool. "Comprehension gate" gave writers a phrase to reuse. LegCli should mint its own: session handoff, context persistence, the resume layer, whatever writers will repeat.
- Invert the expected axis. The saturated market reviewed code, so Sphinx reviewed the person. For LegCli, the saturated market ships agents that forget; LegCli is the part that remembers.
- Ship the escape hatch and log it. `sphinx yolo` turned a hard sell (a gate on every push) into an opt-out norm. LegCli's launch should make the default behavior generous and the bypass explicit, not the other way around.
- One tagline that survives quoting. Press repeated "you can outsource your thinking, but not your understanding" verbatim. LegCli's "your agent hits the limit, the next one keeps your place" plays the same role; keep it front and center.
