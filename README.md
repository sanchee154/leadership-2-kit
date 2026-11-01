# Leadership 2.0 Kit

The build kit for the Leadership 2.0 databases in Notion: Principles, Roles, Plays and Relationships.

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

- All four schemas (Principles, Roles, Plays, Relationships): approved by Eduardo, Nov 1, 2026.
- First build: done Nov 1, 2026. Notion page: https://app.notion.com/p/40b1bffd379a81e480a2c1413018f82e
- From here on, Notion holds the entries. The CONTENT files are a snapshot of the first build.

## Adding a database later

Add a SCHEMA and CONTENT pair with the next number (for example `50_Field_cases_SCHEMA.md` and `51_Field_cases_CONTENT.md`), add one line to the file table in `00_MASTER.md`, and give it an unused color.
