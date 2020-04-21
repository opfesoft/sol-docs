# quest\_request\_items

**Table: quest\_request\_items**

This table basically handles 3 quest details:

1.  NPC Emote when quest is completed
2.  NPC Emote when quest is incomplete
3.  Completion text for quests requiring quest items

 

| Field                                   | Type         | Attributes        | Key | NULL | Default | Comment                                                |
|-----------------------------------------|--------------|-------------------|-----|------|---------|--------------------------------------------------------|
| [ID](#id)                               | mediumint(8) | unsigned          | PRI | NO   | 0       | Unique ID ([quest\_template.ID](quest_template.md#id)) |
| [EmoteOnComplete](#emoteoncomplete)     | smallint(5)  | unsigned          |     | NO   | 0       | Quest ender NPC [Emote](../../dbc/Emotes.md)           |
| [EmoteOnIncomplete](#emoteonincomplete) | smallint(5)  | unsigned          |     | NO   | 0       | Quest ender NPC Emote                                  |
| [CompletionText](#completiontext)       | text         | utf8\_general\_ci |     | YES  | NULL    | Quest completion text                                  |
| [VerifiedBuild](#verifiedbuild)         | smallint(5)  |                   |     | NO   | 0       | Game client Build number                               |

 

## Description of the fields

### ID

Quest ID for quests showing a completion text upon turning in an item delivery quest.
Primary Key for this table. Each quest ID must be unique.

### EmoteOnComplete

Emote (from [Emotes.dbc](../../dbc/Emotes.md)) played by the quest ender NPC when all quest objectives are completed.

### EmoteOnIncomplete

Emote (from [Emotes.dbc](../../dbc/Emotes.md)) played by the quest ender NPC if any of the quest objectives are incomplete.

### CompletionText

Quest gossip text shown in the final gossip dialogue window when turning in an item delivery quest.
The quest item(s) involved in the quest can either be provided by the quest giver or collected by the player.

### VerifiedBuild

This field is used by the AzerothCore Team to determine whether a template has been verified from WDB files (ADB files for this one).

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is [-Client Build](../auth/realmlist.md "DB:Auth:realmlist") then it was parsed with WDB files from that specific [client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist") and manually edited later for some special necessity.
