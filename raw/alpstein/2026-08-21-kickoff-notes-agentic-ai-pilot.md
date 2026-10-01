# Meeting Notes: Kickoff Pilot "Agentic AI in Service"

**Date:** 21 August 2026, 14:00–15:30
**Participants:** Jonas Weber (project lead), Priya Raman (technology), Nadia Frei (Service Desk, team lead), Lukas Amrein (software development), Marco Steiner (guest, finance)
**Notes:** Lukas Amrein

---

## Goal of the pilot

An AI agent ("service triage agent") reads incoming service tickets from AlpMind and from the email mailbox, classifies them (fault, maintenance, question, complaint), resolves standard cases with an answer from the knowledge base, and forwards everything else to a human. Goal: a response time of under 10 minutes in the standard case (today: 3 hours on average).

Pilot duration: September to November 2026. Budget: CHF 180,000 (approved).

## What the agent may do – first draft

| Action | Allowed? | Comment |
|---|---|---|
| Read and categorize ticket | yes | – |
| Suggest an answer from the knowledge base | yes | A human approves |
| Send an answer directly to customers | **no** (pilot phase) | to be decided after the pilot |
| Give price information | no | Price questions always go to Sales |
| Promise a credit note or compensation | **never** | Lesson from the Bergland case |
| Trigger a technician call-out | suggestion only | Dispatch decides |
| Close ticket | no | – |

Nadia Frei: "The agent may suggest, not promise."

## Architecture (Priya Raman)

- One agent, no multi-agent solution in the pilot. First show that a single agent classifies reliably.
- Knowledge base: the service manuals and the last 2,000 resolved tickets, prepared as a wiki.
- Every action of the agent is logged. The log is part of the evaluation.
- Second expansion stage (after the pilot): a checker agent that checks the suggestions against the rules before a human sees them.

## Open questions

1. Who is responsible if the agent classifies a ticket incorrectly and a downtime lasts longer as a result? (Marco Steiner)
2. How do we measure quality, not just speed? Proposal from Nadia Frei: a 10% sample of the tickets reviewed by the team.
3. May customer data from tickets go into the language model? To be clarified with data protection by 15 September.
4. What happens if the agent fails? Falling back to today's process must be possible at any time.

## Next steps

| What | Who | By |
|---|---|---|
| Finalize the rule set "What the agent may do" | Jonas Weber, Nadia Frei | 5 September 2026 |
| Build the knowledge base | Lukas Amrein | 19 September 2026 |
| Data protection clarification | Priya Raman | 15 September 2026 |
| Quality measurement concept | Nadia Frei | 12 September 2026 |
| Status report to the Executive Board | Jonas Weber | 30 September 2026 |
