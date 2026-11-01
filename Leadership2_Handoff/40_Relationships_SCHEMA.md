# Relationships: Schema

**Status: proposed.** Claude drafted this. Confirm it with Eduardo before building.

**What this database is:** the real people a group depends on, one person per entry. Roles say what work exists. Relationships say who is actually there, how much trust there is, and when someone last reached out.

## Fields

| Field | Type | Options or notes |
|---|---|---|
| Name | Title | The person's name |
| Connection | Text | How they relate to the group and what they bring |
| Context | Select | Volunteer group, Enterprise team, Digital org |
| Trust | Select | New, Building, Solid |
| Last contact | Date | The last real conversation, not a group message |
| Next step | Text | One small next move, if there is one |

**Why Trust has only three options:** it only needs to show where the effort should go. New means just met, Building means some loops closed, and Solid means you could ask them for something hard.

**Why Context is a single select:** a person usually belongs to one kind of group. If someone shows up in two, give them two entries.

## Privacy

- This is the only database that holds personal names. Principles, Roles and Plays stay name free.
- Entries live in Notion only. Don't put names or contact details in this repo.
- No phone numbers, emails or addresses in any field. Use whatever contact app already holds those.

## Color

**Purple, everywhere in this database.** That covers the database icon, its heading on the Leadership 2.0 page, and every option in every select field (Context, Trust).

## Relations (add after all four databases exist)

| Field | Links to | Two-way field on the other side |
|---|---|---|
| Roles | Roles | People |
| Plays used | Plays | Used with |

## Views

| View | Type | Setup |
|---|---|---|
| All people | Table | Sorted by Name, A to Z |
| By trust | Board | Grouped by Trust, in this order: New, Building, Solid |
| Going cold | Table | Filter: Last contact is before one month ago. Sorted by Last contact, oldest first |

## Done means

All the fields, relations and views above exist, with these exact names and options, and nothing extra.
