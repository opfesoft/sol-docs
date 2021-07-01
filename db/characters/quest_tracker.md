# quest\_tracker

**The \`quest_tracker\` table**

This table is used if quest tracking is enabled via worldserver config, see parameter "Quests.EnableQuestTracker".

| Field                                         | Type         | Attribute | Key | Null | Default | Extra | Comment |
|-----------------------------------------------|--------------|-----------|-----|------|---------|-------|---------|
| [id](#id)                                     | mediumint(8) | unsigned  |     | NO   | 0       |       |         |
| [character\_guid](#character_guid)            | int(10)      | unsigned  |     | NO   | 0       |       |         |
| [quest\_accept\_time](#quest_accept_time)     | datetime     |           |     | NO   | NULL    |       |         |
| [quest\_complete\_time](#quest_complete_time) | datetime     |           |     | YES  | NULL    |       |         |
| [quest\_abandon\_time](#quest_abandon_time)   | datetime     |           |     | YES  | NULL    |       |         |
| [completed\_by\_gm](#completed_by_gm)         | tinyint(1)   |           |     | NO   | 0       |       |         |
| [core\_hash](#core_hash)                      | varchar(120) |           |     | NO   | 0       |       |         |
| [core\_revision](#core_revision)              | varchar(120) |           |     | NO   | 0       |       |         |

### id

Quest [id](../world/quest_template.md#id))

### character\_guid

[characters.guid](characters.md#guid).

### quest\_accept\_time

When the quest was accepted.

### quest\_complete\_time

When the quest was completed.

### quest\_abandon\_time

When the quest was abandoned.

### completed\_by\_gm

If a GM completed the quest for the player.

### core\_hash

### core\_revision
