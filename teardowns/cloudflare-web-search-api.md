# Cloudflare Web Search API

## The launch
Cloudflare put a Web Search API into beta on October 2, 2026, during its Birthday Week. It arrived as a changelog entry and docs page rather than a keynote: agents and apps call one endpoint and get live web results routed through AI Gateway.
Sources: https://developers.cloudflare.com/changelog/post/2026-10-02-introducing-web-search-api/

## What they did
- Positioned it as a router, not an index. Three providers at launch (Ceramic.ai, Exa, Linkup) return the same result shape, so switching providers is one parameter.
- Shipped it inside a channel developers already used. Web search rides on AI Gateway, so requests land in existing gateway logs and bill to existing AI Gateway credits.
- Made price transparency the launch message: billing at each provider's list price with no markup, plus bring your own provider key.
- Kept the ask tiny: a REST endpoint and a Workers binding, no new auth, no new signup.

## What worked
- Front-page HN launch: 391 points and 188 comments on the discussion per an October 5 front-page roundup; other coverage that week reported 500-plus points.
  Source: https://duklee.net/blog/2026-10-05-hn-frontpage-roundup/
- Pricing became the story. Ceramic at $0.25 per 1,000 requests, Linkup at $5, Exa at $7, against $10 to $14 per 1,000 for model-native search tools.
  Source: https://www.digitalapplied.com/blog/web-search-apis-for-ai-agents-compared-2026
- The ecosystem did the marketing. Independent writeups within days covered provider fallback wrappers and fine-print warnings, extending the launch week for free.
  Source: https://blog.stackademic.com/cloudflare-made-web-search-a-one-line-api-call-heres-the-fallback-wrapper-it-needs-ba8765ec93d0?gi=14160a88cdf8

## Takeaways for LegCli
- Launch inside the user's existing workflow, not a new destination. Cloudflare put search where agents already ran; LegCli should land inside the session tools people already use.
- Price transparency is a narrative, not just a number. "No markup" traveled further than the feature list. A $79 one-time price deserves the same treatment.
- HN audits your claims. The launch said all three providers support Zero Data Retention; the thread found Exa's docs said otherwise. Verify every claim in the announcement before posting.
- Route, don't build. When the category is crowded, owning the integration layer is a defensible launch: one endpoint, one bill, one log stream.
