# Leadership 2.0 Kit

The build kit for the Leadership 2.0 databases in Notion: Principles, Roles and Plays.

## What lives where

| Files | Role | Source of truth |
|---|---|---|
| `00_MASTER.md`, `*_SCHEMA.md`, `99_CHECK.md` | The kit: structure, rules, build order, checks | This repo |
| `*_CONTENT.md` | Entries for the first build | This repo until the first build, then Notion |

After the first build, Notion holds the entries. Edit them there, not here. If a later build needs the current entries, export them from Notion at that time instead of keeping these files in sync.

## How to use it

1. Open a Claude Code session on this repo with the Notion connector on.
2. Paste the opening prompt from `Leadership2_Handoff/00_MASTER.md`.
3. Done means every check in `Leadership2_Handoff/99_CHECK.md` passes.

## Status

- The schema is still a proposal. Eduardo needs to approve the three SCHEMA files before the first build.
- First build: not run yet.

## Adding a database later

Add a SCHEMA and CONTENT pair with the next number (for example `40_Field_cases_SCHEMA.md` and `41_Field_cases_CONTENT.md`), add one line to the file table in `00_MASTER.md`, and give it an unused color.
