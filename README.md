# My Second Brain – Starter Vault

This repository is your personal Second Brain. An agent (Claude Code) maintains it for you. You curate sources and ask questions. The agent ingests sources, writes wiki pages, links them, maintains the catalog and the log, and checks for contradictions.

## Structure

```
CLAUDE.md          Job description of your agent (identity, structure, workflows, boundaries)
raw/               Your sources. The agent reads here and never writes here.
  alpstein/        Sample documents of a fictional company (Alpstein Robotics AG)
wiki/              Knowledge pages maintained by the agent
  _index.md        Catalog of all pages (the agent keeps it up to date)
  _log.md          Log: what did the agent do, and when?
.claude/agents/    Additional agents (e.g., reviewer = checker)
.claude/settings.example.json   Example for technical boundaries (governance)
```

## How to start (Task 1 in the course)

1. At the top right: **Use this template → Create a new repository**. Name it, e.g., `second-brain`. Set the visibility to **Private**.
2. Go to **claude.ai/code**, connect GitHub (one time only), and select your new repository.
3. Leave the permission mode on **Accept edits**.
4. First prompt:

```
Read CLAUDE.md and README.md. Introduce yourself in three sentences: who are you, what is your job, and which folders exist? Do not change anything yet.
```

## Saving = Merging

The agent works on its own branch. Your changes get into the repository like this:
**View diff → Create PR → in GitHub "Merge pull request"**. Only then are they permanent. You are the approval gate.

## Important rule

No confidential data in `raw/`. Use the sample documents or non-critical texts of your own (book notes, public articles, your own talks).

## Continuing after the course

- Ingest one source every day, and run a Lint every week.
- Optional: clone the repo locally and open it in Obsidian (folder as vault) to see the graph and links.
