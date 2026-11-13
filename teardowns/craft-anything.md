# craft-anything

## The launch
In early November 2026, storytold/craft-anything appeared on GitHub: a pure-Rust reverse-engineering engine with a desktop app, a CLI, and an MCP server. Point it at a website, app, game, or file and it studies how the target is built, then a coding agent rebuilds your own version from that study. The workflow is Study, Build, Check, Ready. It is early alpha, MIT or Apache-2.0 licensed, and it spread almost entirely through GitHub stars rather than a formal launch post.
Sources: https://hotrepo.ai/storytold/craft-anything, https://github.com/storytold/craft-anything

## What they did
- Shipped a four-word loop as the product. Study, Build, Check, Ready is the whole pitch: a process anyone can repeat, not a feature list to memorize.
- Made the demo the install. The README opens with `git clone` and two commands, and a rebuild is one more: `craft-anything-cli rebuild https://example.com "Recreate this website"`. Trying it takes minutes, and the first try is the viral moment.
- Built the controversy into the product. Clean room mode is the default and refuses tools that read the target's code or page source; Deep mode unlocks the full inspection engines. The README states the limit plainly: use it only on software you own or are allowed to examine.
- Rode the agent wave instead of fighting it. The tool does not replace the coding agent; it feeds Claude Code (the primary supported path) a studied brief, then checks the result against the original and refines it.
- Let the README do the launching. There was no big press push; the repo, its tool list (320 tools claimed), and its status page were the launch assets.

## What worked
- Star velocity: from 959 stars on November 1 to 20,533 on November 7, adding roughly 2.5k to 4.3k stars per day for seven consecutive records.
  Source: https://hotrepo.ai/storytold/craft-anything
- The HN thread on November 5 drew only 6 points and 3 comments, yet the repo kept climbing, which shows the growth came from GitHub discovery and word of mouth, not a front-page hit.
  Source: https://hotrepo.ai/storytold/craft-anything
- The ethics objection became part of the story rather than killing it: a commenter called one-click recreation of a product "gross" and filed it as issue #1044, and the clean-room default gave the project a credible answer.
  Source: https://hotrepo.ai/storytold/craft-anything

## Takeaways for LegCli
- Star velocity can come from the repo alone. A GitHub repo with a one-command demo and a clear README can outrun a formal launch; LegCli's repo page is a launch surface, not just a code host.
- A four-step loop is a better hook than a feature list. LegCli's handoff could be framed as a loop too (capture, bundle, hand off, resume), and every demo should walk that loop.
- Name the boundary before critics do. craft-anything's clean-room default turned its biggest objection into a feature. LegCli should state up front what a handoff will not carry, and that honesty becomes part of the pitch.
- Controversy is distribution if you have an answer. The ethics debate spread the repo. LegCli's adjacent debate (agents replacing human context) is worth engaging with a clear position, not avoiding.
