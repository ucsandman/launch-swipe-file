# Herdr

## The launch
On October 29, 2026, Herdr announced a native desktop app built on a new runtime called herdr-core. Terminals and agents live in the core rather than in the window, so you can close the app, quit, or update it and your sessions keep running. You can start Claude Code, Codex, or any other program from the tab bar, and status is reported through an open protocol, so your own scripts can show up as agents too. The app, herdr-core, and the Herdr TUI are all open source under Apache 2.0 and free.
Sources: https://herdr.dev/, https://dev.to/jathurshan_sownthararasa_/three-new-ai-agent-tools-to-try-this-week-super-agent-cartesia-herdr-5a80

## What they did
- Made the survival claim the whole product. "Close it, they keep working" is the headline on the site, and everything else is supporting detail. One promise, repeated in every surface.
- Split the architecture so the promise is structural, not a feature. Agents run in herdr-core, a small server on the machine, not in the window. The design makes the headline true by construction, and the launch explains the split in one paragraph.
- Published the honesty footnote. The FAQ says plainly that a machine reboot stops the programs, panes come back with a shell in the same folder, and Herdr does not restart an agent or resume its work in progress. That candor is part of the pitch.
- Shipped an open protocol instead of a walled garden. OSC 7501 lets any agent report working, done, or blocked with one line, so the app works with agents Herdr never heard of, and a user's own script counts as an agent.
- Let the agent edit the app. Layout, sidebar, tabs, keys, and themes are plain files in ~/.config/herdr-app with an AGENTS.md explaining them, so you can ask your agent to change the interface in plain language.

## What worked
- The persistence hook landed exactly on the pain every multi-agent developer feels: closing a window should not kill the work. The launch was picked up in same-week agent-tool round-ups within two days.
  Source: https://dev.to/jathurshan_sownthararasa_/three-new-ai-agent-tools-to-try-this-week-super-agent-cartesia-herdr-5a80
- The one-line install from the download page plus a free, open-source license made the trial cost zero, so curiosity converted to installs with no decision in between.
  Source: https://herdr.dev/download/
- Multi-machine support over SSH gave the launch a second story for teams: every machine in one sidebar, agents keep running while the laptop sleeps.
  Source: https://herdr.dev/

## Takeaways for LegCli
- Herdr is the closest adjacent launch to LegCli, and the contrast is the positioning. Herdr keeps agents alive while the app is closed; LegCli keeps a session alive across machines and agent restarts. The launch should say that difference in one line.
- A structural promise beats a feature promise. Herdr's split architecture makes its headline true by design. LegCli's handoff bundle should be presented the same way: the artifact is the guarantee, not a setting.
- Publish the gap honestly. Herdr admitting reboots stop agents builds trust. LegCli should name its own boundary (for example, what a handoff cannot carry) in the launch post.
- An open protocol is a distribution strategy. If LegCli's handoff format is open and documented, other tools can read and write it, and every integration becomes a channel.
