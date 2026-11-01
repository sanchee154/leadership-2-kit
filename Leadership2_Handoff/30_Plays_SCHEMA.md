# Plays: Schema

**Status: approved** by Eduardo, Nov 1, 2026.

**What this database is:** small, repeatable moves a leader makes. Each one is cheap to try and easy to drop if it doesn't work.

## Fields

| Field | Type | Options or notes |
|---|---|---|
| Play | Title | Short name |
| The move | Text | What you do, in one or two sentences |
| Script | Text | The exact words, if the play has any |
| When | Select | Before, Arrival, During, After, Weekly |
| Cost | Text | What it costs to try, for example "one sentence" |
| Status | Select | Untested, Tried once, Proven twice |
| Applies to | Multi-select | Volunteer group, Enterprise team, Digital org |
| Source | Text | Where the play comes from |

**Why Status stops at "Proven twice":** it follows Run 2 of "The Group Runs on Unnamed Roles": if it works twice in a row, the pattern is real.

## Color

**Orange, everywhere in this database.** That covers the database icon, its heading on the Leadership 2.0 page, and every option in every select and multi-select field (When, Status, Applies to). Eduardo chose one color per database.

## Relations (add after all three databases exist)

| Field | Links to | Two-way field on the other side |
|---|---|---|
| Principles served | Principles | Plays |
| Roles supported | Roles | Plays |

## Views

| View | Type | Setup |
|---|---|---|
| By moment | Board | Grouped by When, in this order: Before, Arrival, During, After, Weekly |
| To try | Table | Filter: Status is Untested |
| All plays | Table | Sorted by Play, A to Z |

## Done means

All the fields, relations and views above exist, with these exact names and options, and nothing extra.
