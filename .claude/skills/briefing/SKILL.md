---
name: briefing
description: Write a one-page briefing for the Executive Board on a topic, using only the wiki, with a wikilink for every claim. Use when the user asks for a briefing, a memo for the board, or writes "/briefing <topic>".
---

# Briefing

A workflow that moved out of CLAUDE.md into its own folder, so it can be reused and shared.

When the user asks for a briefing on a topic:

1. Read `wiki/_index.md`, then every page that mentions the topic.
2. Write a one-page briefing with four parts:
   - **Decision needed** – one sentence.
   - **Facts** – every statement with a wikilink to its page; numbers always with date and source.
   - **Open points and contradictions** – flagged, not resolved.
   - **Recommendation** – clearly marked as the agent's suggestion, not a fact.
3. State what the wiki does **not** know.
4. Show the briefing in the chat and ask whether to save it as `wiki/syntheses/<YYYY-MM-DD>-briefing-<topic>.md`. Save only after a yes.
5. Append an entry to `wiki/_log.md`: date, "briefing", topic.
