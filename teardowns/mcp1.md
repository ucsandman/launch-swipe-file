# MCP1 by Appwrite

## The launch
On November 9, 2026, Appwrite launched MCP1 on Product Hunt: a hosted gateway that puts every MCP server a team uses behind one URL. Humans authenticate once, admins decide which groups can call which tools, and every call is logged. It works with Claude, Cursor, ChatGPT, Codex, and other MCP clients, and it is free for individuals with paid team plans. Eldad Fux, Appwrite's founder, also posted the launch story on a developer forum on November 10.
Sources: https://mcp1.com/, https://www.producthunt.com/products/appwrite/launches/mcp1, https://vibingtalk.com/index.php?threads/we-replaced-everyones-mcp-configs-and-tokens-with-one-gateway.1946327/

## What they did
- Led with a one-line install. The whole pitch collapses into a single command: `claude mcp add --transport http appwrite https://mcp1.com/mcp/appwrite`. One command is the demo, the docs, and the onboarding.
- Told the dogfood story, not a feature list. Eldad's post opens with the internal mess: everyone had their own MCP servers, API tokens sat in local config files, and nobody knew who was calling what. MCP1 is the tool Appwrite built for itself, then opened up.
- Named the enemy: scattered tokens. The site repeats one idea: no more pasting server tokens into every laptop. The gateway seals tokens with AES-256-GCM and humans never see them.
- Shipped a catalog, not a blank box. About 150 servers are listed, many with one-click sign-in, so a new user gets value before configuring anything of their own.
- Priced the wedge at free. Individuals pay nothing, teams pay per member. The free tier is the distribution: one person on a team adopts it, then the team needs shared gateways.

## What worked
- Product Hunt placement: 146 upvotes and 15 comments, #8 Product of the Day on November 9, 2026, in the Developer Tools, Artificial Intelligence, and API topics.
  Source: https://www.hunted.space/product/appwrite
- 31 reviews on Product Hunt averaging 4.68/5, an unusually high review count for a launch day, which signals real users rather than a launch-day crowd.
  Source: https://www.hunted.space/product/appwrite
- The founder's forum post carried the launch further than the listing: a first-person "we replaced everyone's configs" story with the exact command to copy, posted the day after Product Hunt.

## Takeaways for LegCli
- A single copy-paste command beats a setup guide. LegCli's launch should open with its one install command and treat everything else as supporting detail.
- Dogfood stories convert better than feature lists. "We built this because our own team had this exact mess" is the frame LegCli should use for session handoffs: the team lost context, so they built the bundle.
- Free for the individual, paid for the team is a proven wedge. LegCli already prices one-time; the lesson is to make the solo path frictionless and let team sharing be the upsell.
- A catalog is a launch asset. If LegCli ships with a few ready-made handoff templates or example bundles, new users get value before they create anything.
