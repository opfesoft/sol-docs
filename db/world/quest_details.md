# quest\_details

This table handles Quest NPC emotes with emote delays.

## Structure 

| Field                           | Type         | Attributes | Key | NULL | Default | Comment                                                |
|---------------------------------|--------------|------------|-----|------|---------|--------------------------------------------------------|
| [ID](#id)                       | mediumint(8) | unsigned   | PRI | NO   | 0       | Unique ID ([quest\_template.ID](quest_template.md#id)) |
| [Emote1](#emote1)               | smallint(5)  | unsigned   |     | NO   | 0       | Quest NPC [Emote](../../dbc/Emotes.md)                 |
| [Emote2](#emote2)               | smallint(5)  | unsigned   |     | NO   | 0       | Quest NPC [Emote](../../dbc/Emotes.md)                 |
| [Emote3](#emote3)               | smallint(5)  | unsigned   |     | NO   | 0       | Quest NPC [Emote](../../dbc/Emotes.md)                 |
| [Emote4](#emote4)               | smallint(5)  | unsigned   |     | NO   | 0       | Quest NPC [Emote](../../dbc/Emotes.md)                 |
| [EmoteDelay1](#emotedelay1)     | int(10)      | unsigned   |     | NO   | 0       | Emote delay in milliseconds                            |
| [EmoteDelay2](#emotedelay2)     | int(10)      | unsigned   |     | NO   | 0       | Emote delay in milliseconds                            |
| [EmoteDelay3](#emotedelay3)     | int(10)      | unsigned   |     | NO   | 0       | Emote delay in milliseconds                            |
| [EmoteDelay4](#emotedelay4)     | int(10)      | unsigned   |     | NO   | 0       | Emote delay in milliseconds                            |
| [VerifiedBuild](#verifiedbuild) | smallint(5)  |            |     | NO   | 0       | Game client Build number or manually set value         |

## Description of the fields

### ID

Unique ID ([quest\_template.ID](quest_template.md#id))

### Emote1

Emote (from [Emotes.dbc](../../dbc/Emotes.md)) played by NPC

### Emote2

Emote (from [Emotes.dbc](../../dbc/Emotes.md)) played by NPC

### Emote3

Emote (from [Emotes.dbc](../../dbc/Emotes.md)) played by NPC

### Emote4

Emote (from [Emotes.dbc](../../dbc/Emotes.md)) played by NPC

### EmoteDelay1

Emote delay in milliseconds

### EmoteDelay2

Emote delay in milliseconds; if 0 played directly after Emote1

### EmoteDelay3

Emote delay in milliseconds; if 0 played directly after Emote2

### EmoteDelay4

Emote delay in milliseconds; if 0 played directly after Emote3

### VerifiedBuild

This field is used by the AzerothCore Team to determine whether a template has been verified from WDB files (ADB files for this one).

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is [-Client Build](../auth/realmlist.md "DB:Auth:realmlist") then it was parsed with WDB files from that specific [client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist") and manually edited later for some special necessity.
