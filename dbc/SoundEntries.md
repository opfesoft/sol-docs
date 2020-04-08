# SoundEntries

**SoundEntries.dbc**

## Structure

| Column | Field | Type | Notes |
| --- | --- | --- | --- |
| 1 | ID | Integer |   |
| 2 | SoundType | Integer | Value to identify the type. See table below for values. |
| 3 | Name | String |   |
| 4-13 | Filenames[10] | String | One entry can have more subentries. Used for different sounds at weapons. |
| 14-23 | Freq[10] | String | Related to the files above. Maybe a count of how much they are played in any way? |
| 24 | FilePath | String | The filenames come without path. This is set here. |
| 25 | Volume | Float |   |
| 26 | Flags | Integer | Has the values 0, 1, 32, 33, 34, 512, 513, 544, 1024 and 1056. (hex: 0h, 1h, 20h, 200h, 400h) |
| 27 | minDistance | Float |   |
| 28 | distanceCutoff | Float |   |
| 29 | EAXDef | Integer |   |
| 30 | soundEntriesAdvancedID | Integer |   |

## Sound Types

| Value | Meaning |
| --- | --- |
| 0 | Unused/Miscellaneous |
| 1 | Spells |
| 2 | UI |
| 3 | Footsteps |
| 4 | Weapons/Impact |
| 6 | Weapons/Miss |
| 7 | Greetings |
| 8 | Casting |
| 9 | Pick Up/Put Down |
| 10 | NPC Combat |
| 12 | Errors |
| 13 | Birds |
| 14 | Objects |
| 16 | Death |
| 17 | NPC Greetings |
| 18 | Test/Temporary |
| 19 | Armor/Foley |
| 20 | Footsteps |
| 21 | Water/Character |
| 22 | Water/Liquid |
| 23 | Tradeskills |
| 25 | Doodads |
| 26 | Spell Fizzle |
| 27 | NPC Loops |
| 28 | Zone Music |
| 29 | Emotes |
| 30 | Narration Music |
| 31 | Narration |
| 50 | Zone Ambience |
