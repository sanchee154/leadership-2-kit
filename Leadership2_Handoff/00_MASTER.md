# Handoff: Build the Leadership 2.0 databases in Notion

Nov 1, 2026 · Read this file first. It covers what to build, where to build it, the order, and the rules. The other files hold the details.

## Objective

Create a new top-level Notion page called **Leadership 2.0** that holds three linked databases: **Principles**, **Roles** and **Plays**. Fill each one with the entries listed in its CONTENT file.

**What Leadership 2.0 is:** Eduardo's own rework of organizational design and leadership, treated as one discipline instead of two. It has to work for three kinds of groups: small volunteer groups, enterprise teams, and digital organizations.

## The files

| File | What it holds | How often it changes |
|---|---|---|
| 00_MASTER.md | This file: goal, location, order, rules, opening prompt | Rarely |
| 10_Principles_SCHEMA.md | Fields and views for Principles | Rarely |
| 11_Principles_CONTENT.md | Principles entries | Often |
| 20_Roles_SCHEMA.md | Fields and views for Roles | Rarely |
| 21_Roles_CONTENT.md | Roles entries | Often |
| 30_Plays_SCHEMA.md | Fields and views for Plays | Rarely |
| 31_Plays_CONTENT.md | Plays entries | Often |
| 99_CHECK.md | What to verify before calling it done | Rarely |

## Decisions (and why)

- **File layout: one SCHEMA file and one CONTENT file per database, plus this master file.** Eduardo expects both the content and the overall structure to change. Keeping content separate means editing entries never touches the structure. Adding a new database means adding a pair of files and one line here.
- **Start with three databases: Principles, Roles and Plays.** Eduardo chose these. He said Plays had to be included.
- **Location: a new top-level page.** It's easy to find and has room to grow.
- **Colors: one color per database.** Principles is blue, Roles is green, Plays is orange. Each database's icon, its heading on the page, and all of its select options use that one color. Eduardo chose this over coloring options by meaning. A new database added later gets its own unused color.
- **Content comes from Eduardo's own writing.** The main source is "The Group Runs on Unnamed Roles" (v2, Google Doc id `1AXhtyH163zHv3ps-tQix_IiUiz7lRbZ-z3_bE-o6qXY`). The other sources are his August 2026 YSA handoff notes and his October 2026 goals plan. Every entry names its source.

## Left out on purpose (do not add)

- **A Field cases database.** It was offered and not chosen. It can be added later as 40_ and 41_ files.
- **Page templates and automations.** Not requested. Keep the first version simple.

## Build order

1. Create the page **Leadership 2.0** at the top level of the workspace, not inside another page.
2. Create the three databases inside it from the SCHEMA files (10, 20, 30). Leave out the relation fields on this pass.
3. Add the relation fields once all three databases exist. They're listed under "Relations" in each SCHEMA file.
4. Add the entries from the CONTENT files (11, 21, 31), then fill in the relations between entries.
5. Create the views listed in each SCHEMA file.
6. Run every check in 99_CHECK.md. Fix anything that fails, then report back.

## How the databases link

```
Principles  <->  Plays     (a play serves one or more principles)
Principles  <->  Roles     (a role exists because of a principle)
Roles       <->  Plays     (a play supports a role)
```
All relations are two-way.

## Rules for the build

- **Copy entry text exactly** from the CONTENT files. Don't reword it, shorten it or add to it.
- **Don't invent** fields, select options, entries or sources that aren't in these files. If something is missing or unclear, stop and ask Eduardo.
- **No personal names or personal details** from the source cases. The concepts carry over to any group; the people in the original cases stay out.
- **Plain language and no em dashes** in anything you write into Notion.
- **Never use the name "Single Mingles."** The activities are called "YSA activities."

## Open items

- **The schema is a proposal.** Claude drafted the fields, select options and views, and Eduardo hasn't approved them yet. Confirm with him before step 2.
- **Field cases** is a possible fourth database, for later.

## Suggested opening prompt (paste into the Claude Code cloud session)

```
Build the Leadership 2.0 databases in my Notion workspace using the
handoff files in Leadership2_Handoff/. Read 00_MASTER.md first, then
follow its build order exactly.

Before creating anything, look in Notion for an existing page called
"Leadership 2.0". If one exists, stop and ask me before building.

Done means: every check in 99_CHECK.md passes. Keep a checklist that
matches it and work until every item is done. Don't stop at a progress
update, and don't offer to continue: keep going until it's done.

Do not: add databases, fields, select options or entries that aren't
in the files; reword entry text; use em dashes; use the name
"Single Mingles"; put personal names into any entry.
```

## Done means

All three databases exist under the Leadership 2.0 page, every entry from the CONTENT files is in place with its relations, every view exists, and every check in 99_CHECK.md passes.
