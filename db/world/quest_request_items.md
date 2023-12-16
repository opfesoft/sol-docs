# quest\_request\_items

This table basically handles 3 quest details:

1.  NPC Emote when quest is completed
2.  NPC Emote when quest is incomplete
3.  Completion text for quests requiring quest items

## Structure 

| Field                                   | Type         | Attributes        | Key | NULL | Default | Comment                                                |
|-----------------------------------------|--------------|-------------------|-----|------|---------|--------------------------------------------------------|
| [ID](#id)                               | mediumint(8) | unsigned          | PRI | NO   | 0       | Unique ID ([quest\_template.ID](quest_template.md#id)) |
| [EmoteOnComplete](#emoteoncomplete)     | smallint(5)  | unsigned          |     | NO   | 0       | Quest ender NPC [Emote](../../dbc/Emotes.md)           |
| [EmoteOnIncomplete](#emoteonincomplete) | smallint(5)  | unsigned          |     | NO   | 0       | Quest ender NPC Emote                                  |
| [CompletionText](#completiontext)       | text         | utf8\_general\_ci |     | YES  | NULL    | Quest completion text                                  |

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

