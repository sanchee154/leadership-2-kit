# Roles: Schema

**Status: approved** by Eduardo, Nov 1, 2026.

**What this database is:** the roles a group actually runs on, written down so they're visible before the person holding them leaves.

## Fields

| Field | Type | Options or notes |
|---|---|---|
| Role | Title | Short name |
| What it covers | Text | The work the role does |
| Signal it sends | Text | What others see or hear when the role is being done |
| Status | Select | Unnamed, Described, Funded, Handed off |
| Holder | Text | Who holds it now. Left blank for Eduardo to fill in |
| Backup | Text | Who could take it over. Left blank |
| Applies to | Multi-select | Volunteer group, Enterprise team, Digital org |
| Source | Text | Where the role was identified |

**Why Status has these four options:** they follow the line from "The Group Runs on Unnamed Roles" that a described role "can be thanked and funded and rotated and handed off." "Thanked" and "rotated" were left out to keep the list short.

**Why Holder and Backup are Text, not Person:** the people who hold these roles usually aren't Notion users.

## Color

**Green, everywhere in this database.** That covers the database icon, its heading on the Leadership 2.0 page, and every option in every select and multi-select field (Status, Applies to). Eduardo chose one color per database.

## Relations (add after all three databases exist)

| Field | Links to | Two-way field on the other side |
|---|---|---|
| Principles | Principles | Roles |
| Plays | Plays | Roles supported |

## Views

| View | Type | Setup |
|---|---|---|
| Role board | Board | Grouped by Status, in this order: Unnamed, Described, Funded, Handed off |
| No backup | Table | Filter: Backup is empty |

## Done means

All the fields, relations and views above exist, with these exact names and options, and nothing extra.
