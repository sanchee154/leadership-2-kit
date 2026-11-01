# Principles: Schema

**Status: proposed.** Claude drafted this. Confirm it with Eduardo before building.

**What this database is:** the core ideas of Leadership 2.0, one per entry. Each one is a rule you can act on, not a quote to admire.

## Fields

| Field | Type | Options or notes |
|---|---|---|
| Principle | Title | A short name for the idea |
| Statement | Text | The full wording, copied exactly from the CONTENT file |
| Layer | Select | Lens, Signal, Structure |
| Applies to | Multi-select | Volunteer group, Enterprise team, Digital org |
| Source | Text | Where the idea comes from |
| Source type | Select | Book or framework, Field run, Own synthesis |
| Status | Select | Draft, Tested, Core |

**Why Layer has these three options:** it follows Eduardo's rule from "The Group Runs on Unnamed Roles": when something breaks, work top down. Check the lens, then the signal, and only then the structure.

## Color

**Blue, everywhere in this database.** That covers the database icon, its heading on the Leadership 2.0 page, and every option in every select and multi-select field (Layer, Applies to, Source type, Status). Eduardo chose one color per database.

## Relations (add after all three databases exist)

| Field | Links to | Two-way field on the other side |
|---|---|---|
| Plays | Plays | Principles served |
| Roles | Roles | Principles |

## Views

| View | Type | Setup |
|---|---|---|
| All principles | Table | Sorted by Principle, A to Z |
| By layer | Board | Grouped by Layer, in this order: Lens, Signal, Structure |
| Core only | Table | Filter: Status is Core |

## Done means

All the fields, relations and views above exist, with these exact names and options, and nothing extra.
