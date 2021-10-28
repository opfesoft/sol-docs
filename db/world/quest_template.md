# quest\_template

Contains all basic definitions of available quests.

## Structure

<table>
<thead>
<tr class="header">
<th>Field</th>
<th>Type</th>
<th>Null</th>
<th>Key</th>
<th>Default</th>
<th>Extra</th>
<th>Comment</th>
</tr>
</thead>
<tbody>
<tr>
<td><p><a href="#id">ID</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p>PRI</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#questtype">QuestType</a></p></td>
<td><p>tinyint(3) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>2</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#questlevel">QuestLevel</a></p></td>
<td><p>int(11)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>-1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#minlevel">MinLevel</a></p></td>
<td><p>int(11)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#questsortid">QuestSortID</a></p></td>
<td><p>smallint(6)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#questinfoid">QuestInfoID</a></p></td>
<td><p>smallint(5) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#suggestedgroupnum">SuggestedGroupNum</a></p></td>
<td><p>tinyint(3) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardnextquest">RewardNextQuest</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardxpdifficulty">RewardXPDifficulty</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardmoney">RewardMoney</a></p></td>
<td><p>int(11)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardbonusmoney">RewardBonusMoney</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewarddisplayspell">RewardDisplaySpell</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardspell">RewardSpell</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardhonor">RewardHonor</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardkillhonor">RewardKillHonor</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#startitem">StartItem</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#flags">Flags</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewarditem">RewardItem(X=1...4)</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardamount">RewardAmount(X=1...4)</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#itemdrop">ItemDrop(X=1...4)</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#itemdropquantity">ItemDropQuantity(X=1...4)</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardchoiceitemid">RewardChoiceItemID(X=1...6)</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardchoiceitemquantity">RewardChoiceItemQuantity(X=1...6)</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#poicontinent">POIContinent</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#poix">POIx</a></p></td>
<td><p>float</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#poiy">POIy</a></p></td>
<td><p>float</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#poipriority">POIPriority</a></p></td>
<td><p>int(11)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardtitle">RewardTitle</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#requiredplayerkills">RequiredPlayerKills</a></p></td>
<td><p>tinyint(3) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardtalents">RewardTalents</a></p></td>
<td><p>tinyint(3) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardarenapoints">RewardArenaPoints</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardfactionid">RewardFactionID(X=1...5)</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardfactionvalue">RewardFactionValue(X=1...5)</a></p></td>
<td><p>int(11)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#rewardfactionoverride">RewardFactionOverride(X=1...5)</a></p></td>
<td><p>int(11)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#timeallowed">TimeAllowed</a></p></td>
<td><p>int(10) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#allowableraces">AllowableRaces</a></p></td>
<td><p>int(11)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>-1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#logtitle">LogTitle</a></p></td>
<td><p>text</p></td>
<td><p>YES</p></td>
<td><p><br />
</p></td>
<td><p>(NULL)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#logdescription">LogDescription</a></p></td>
<td><p>text</p></td>
<td><p>YES</p></td>
<td><p><br />
</p></td>
<td><p>(NULL)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#questdescription">QuestDescription</a></p></td>
<td><p>text</p></td>
<td><p>YES</p></td>
<td><p><br />
</p></td>
<td><p>(NULL)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#areadescription">AreaDescription</a></p></td>
<td><p>text</p></td>
<td><p>YES</p></td>
<td><p><br />
</p></td>
<td><p>(NULL)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#questcompletionlog">QuestCompletionLog</a></p></td>
<td><p>text</p></td>
<td><p>YES</p></td>
<td><p><br />
</p></td>
<td><p>(NULL)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#requirednpcorgo">RequiredNpcOrGo(X=1...4)</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#requirednpcorgocount">RequiredNpcOrGoCount(X=1...4)</a></p></td>
<td><p>smallint(5) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#requireditemid">RequiredItemId(X=1...6)</a></p></td>
<td><p>mediumint(8) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#requireditemcount">RequiredItemCount(X=1...6)</a></p></td>
<td><p>smallint(5) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#requiredfactionid">RequiredFactionId(X=1...2)</a></p></td>
<td><p>smallint(5) unsigned</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#requiredfactionvalue">RequiredFactionValue(X=1...2)</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>NO</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#objectivetext">ObjectiveText(X=1...4)</a></p></td>
<td><p>text</p></td>
<td><p>YES</p></td>
<td><p><br />
</p></td>
<td><p>(NULL)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#verifiedbuild">VerifiedBuild</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>YES</p></td>
<td><p><br />
</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
</tbody>
</table>

## Description of the fields

### ID

The quest ID. This column is the Primary Key for the Table. Each quest ID must be unique!

### QuestType

Accepted values: 0, 1 or 2. Their meaning is described in table below.

| Value | Result                                                                                                   |
|-------|----------------------------------------------------------------------------------------------------------|
| 0     | Quest is enabled, but it is auto-completed when accepted; this skips quest objectives and quest details. |
| 1     | Quest is disabled (not yet implemented in the core).                                                     |
| 2     | Quest is enabled (does not auto-complete).                                                               |

### QuestLevel

Level of quest. Player receives full experience amount only if their level is less than or equal to Level+5. If Level is set to -1, the player's level will be used as (Quest)Level for the experience calculation.

### MinLevel

Minimum level at which a player can get the quest.

### QuestSortID

This field defines under what category the quest falls in the quest log.

If **value &gt; 0** then value is Zone IDs taken from AreaTable.dbc.

if **value &lt; 0** then (**-value**) is quest sort id: (in general profession or class quests.) Value is ID from [QuestSort.dbc](../../dbc/QuestSort.md)

### QuestInfoID

These values are ID taken from [QuestInfo.dbc](../../dbc/QuestInfo.md)

### SuggestedGroupNum

Recommended number of players to do the quest together.

### TimeAllowed

Time in seconds that the player has to complete this quest.

### AllowableRaces

Races allowed to get the quest. 0 means the quest is accessible for all races. Field value is a decimal value which must transform to an 8 bits binary in order to be understandable. In binary form, each different bit represents a different race. They're assigned as follows :

**Race**

These values are 2^ID taken from ChrRaces.dbc

Examples:

0,1791 = All Races

690 (2 + 16 + 32 + 128 + 512) = Horde Quest

1101 (1 + 4 + 8 + 64 + 1024) = Alliance Quest

### RewardNextQuest

The quest entry from a **creature** or **gameobject** that ends a quest and starts a new one. The result is, that if you end the quest, the new quest instantly appears from the quest giver.

See the [examples section](#examples-dealing-with-quests) for examples.

### RewardXPDifficulty

According to the Level, the basic experience with index *RewardXPDifficulty* is taken from QuestXP.dbc.

This field also controls the XP given as the XP is calculated from the value in this field by the following formula. If the quest is repeatable, XP will be given only once. The total XP that a character will receive is also affected by the level difference between the character's level and the quest's level.

### RewardMoney

Money earned by completing the quest (if value &gt; 0) or money requirement to complete the quest (if value &lt; 0). If &gt; 0 and [QuestLevel](#questlevel) is -1 this field is ignored and the player receives money depending on the player level.

### RewardBonusMoney

The money a character at level 80 would get when they complete this quest.

### RewardDisplaySpell

TODO

### RewardSpell

Spell that is shown to be casted on quest completion in the quest log.

NOTE: This field comes straight from the WDB and should not be changed.

### RewardHonor

Number of honorable kill honor rewarded for completing this quest.

Example: An example value is 15 for quest 8388: At level 80 an honorable kill is 124 honor worth. Multiply this with 15 and you receive 1860, after the multiplication the value is rounded up. So the honor rewarded at level 80 is 1860 for this quest.

### RewardKillHonor

TODO

### StartItem

Items given by the quest giver at beginning of the quest. Items will be deleted when quest is abandoned.

### Flags

This flag field defines more specifically the type of quest it is. Aside from the daily flag and sharable flag, this field is used just for grouping purposes and NOT for any other quest requirements. The quest requirements are calculated from non-zero values in other quest template fields. Also, while some of these flags are known, others have yet an unknown purpose and the comments below is simply guesswork on them.

<table>
<thead>
<tr class="header">
<th><p>Flag</p></th>
<th><p>Name</p></th>
<th><p>Comments</p></th>
</tr>
</thead>
<tbody>
<tr>
<td><p>0</p></td>
<td><p>QUEST_FLAGS_NONE</p></td>
<td><p>No flags, so no groups assigned to this quest.</p></td>
</tr>
<tr>
<td><p>1</p></td>
<td><p>QUEST_FLAGS_STAY_ALIVE</p></td>
<td><p>If the player dies, the quest is failed.</p></td>
</tr>
<tr>
<td><p>2</p></td>
<td><p>QUEST_FLAGS_PARTY_ACCEPT</p></td>
<td><p>Escort quests or any other event-driven quests. If player in party, all players that can accept this quest will receive confirmation box to accept quest.</p></td>
</tr>
<tr>
<td><p>4</p></td>
<td><p>QUEST_FLAGS_EXPLORATION</p></td>
<td><p>Involves the activation of an areatrigger.</p></td>
</tr>
<tr>
<td><p>8</p></td>
<td><p>QUEST_FLAGS_SHARABLE</p></td>
<td><p>Allows the quest to be shared with other players.</p></td>
</tr>
<tr>
<td><p>16</p></td>
<td><p>QUEST_FLAGS_HAS_CONDITION</p></td>
<td><p>Not used currently</p></td>
</tr>
<tr>
<td><p>32</p></td>
<td><p>QUEST_FLAGS_HIDE_REWARD_POI</p></td>
<td><p>Not used currently: Unsure of content</p></td>
</tr>
<tr>
<td><p>64</p></td>
<td><p>QUEST_FLAGS_RAID</p></td>
<td><p>Can be completed while in raid</p></td>
</tr>
<tr>
<td><p>128</p></td>
<td><p>QUEST_FLAGS_TBC</p></td>
<td><p>Not used currently: Available if TBC expansion enabled only</p></td>
</tr>
<tr>
<td><p>256</p></td>
<td><p>QUEST_FLAGS_NO_MONEY_FROM_XP</p></td>
<td><p>Not used currently: Experience is not converted to gold at max level</p></td>
</tr>
<tr>
<td><p>512</p></td>
<td><p>QUEST_FLAGS_HIDDEN_REWARDS</p></td>
<td><p>Item and monetary rewards are hidden in the initial quest details page and in the quest log but will appear once ready to be rewarded.</p></td>
</tr>
<tr>
<td><p>1024</p></td>
<td><p>QUEST_FLAGS_TRACKING</p></td>
<td><p>These quests are automatically rewarded on quest complete and they will never appear in quest log client side.</p></td>
</tr>
<tr>
<td><p>2048</p></td>
<td><p>QUEST_FLAGS_DEPRECATE_REPUTATION</p></td>
<td><p>Not used currently</p></td>
</tr>
<tr>
<td><p>4096</p></td>
<td><p>QUEST_FLAGS_DAILY</p></td>
<td><p>Daily repeatable quests (only flag that the core applies specific behavior for)</p></td>
</tr>
<tr>
<td><p>8192</p></td>
<td><p>QUEST_FLAGS_FLAGS_PVP</p></td>
<td><p>Having this quest in log forces PvP flag</p></td>
</tr>
<tr>
<td><p>16384</p></td>
<td><p>QUEST_FLAGS_UNAVAILABLE</p></td>
<td><p>Used on quests that are not generically available</p></td>
</tr>
<tr>
<td><p>32768</p></td>
<td><p>QUEST_FLAGS_WEEKLY</p></td>
<td><p>Weekly repeatable quests (only flag that the core applies specific behavior for)</p></td>
</tr>
<tr>
<td><p>65536</p></td>
<td><p>QUEST_FLAGS_AUTOCOMPLETE</p></td>
<td><p>Auto complete</p></td>
</tr>
<tr>
<td><p>131072</p></td>
<td><p>QUEST_FLAGS_DISPLAY_ITEM_IN_TRACKER</p></td>
<td><p>Displays usable item in quest tracker</p></td>
</tr>
<tr>
<td><p>262144</p></td>
<td><p>QUEST_FLAGS_OBJ_TEXT</p></td>
<td><p>Use Objective text as Complete text</p></td>
</tr>
<tr>
<td><p>524288</p></td>
<td><p>QUEST_FLAGS_AUTO_ACCEPT</p></td>
<td><p>The client recognizes this flag as auto-accept. However, NONE of the current quests (3.3.5a) have this flag. Maybe blizz used to use it, or will use it in the future.</p></td>
</tr>
<tr>
<td>1048576</td>
<td>QUEST_FLAGS_PLAYER_CAST_ON_ACCEPT</td>
<td>Quests with this flag player submit automatically by special button in player GUI</td>
</tr>
<tr>
<td>2097152</td>
<td> QUEST_FLAGS_PLAYER_CAST_ON_COMPLETE</td>
<td>Automatically suggestion of accepting quest. Not from npc.</td>
</tr>
<tr>
<td>4194304</td>
<td>QUEST_FLAGS_UPDATE_PHASE_SHIFT</td>
<td><br />
</td>
</tr>
<tr>
<td>8388608</td>
<td>QUEST_FLAGS_SOR_WHITELIST</td>
<td><br />
</td>
</tr>
<tr>
<td>16777216</td>
<td>QUEST_FLAGS_LAUNCH_GOSSIP_COMPLETE</td>
<td><br />
</td>
</tr>
<tr>
<td>54432</td>
<td>QUEST_FLAGS_REMOVE_EXTRA_GET_ITEMS</td>
<td><br />
</td>
</tr>
<tr>
<td>67108864</td>
<td>QUEST_FLAGS_HIDE_UNTIL_DISCOVERED</td>
<td><br />
</td>
</tr>
<tr>
<td>134217728</td>
<td>QUEST_FLAGS_PORTRAIT_IN_QUEST_LOG</td>
<td><br />
</td>
</tr>
<tr>
<td>268435456</td>
<td>QUEST_FLAGS_SHOW_ITEM_WHEN_COMPLETED</td>
<td><br />
</td>
</tr>
<tr>
<td>536870912</td>
<td>QUEST_FLAGS_LAUNCH_GOSSIP_ACCEPT</td>
<td><br />
</td>
</tr>
<tr>
<td>1073741824</td>
<td>QUEST_FLAGS_ITEMS_GLOW_WHEN_DONE</td>
<td><br />
</td>
</tr>
<tr>
<td>2147483648</td>
<td>QUEST_FLAGS_FAIL_ON_LOGOUT</td>
<td><br />
</td>
</tr>
</tbody>
</table>

Like all flag based fields, **QuestFlags** can be added for the different types of quest.

Note that some flags may not be supported by core.

### RewardTitle

The title the character will receive upon completion of the quest. See [CharTitles.dbc](../../dbc/CharTitles.md)

### RequiredPlayerKills

Displays how much players you need to kill before completing the quest.

### RewardTalents

Will give X bonus talents to the player completed the quest. Leave"0"for No Bonus Talent Points.''

### RewardArenaPoints

Will Give X Arena Points to the player that completes the quest. Leave"0"For no Arena Points Reward.

### RewardChoiceItemId

Id of item available for reward choice.
Number of Charges in rewarded item available.

### RewardChoiceItemQuantity

Will choose how many items will be added for reward. E.g "RewardChoiceItemId" is the reward item and "RewardChoiceItemQuantity" is the count of how many items will be added as a reward.

### RewardItem

[item Id](item_template.md#entry) given for reward (no choice).

### RewardAmount

Amount of the rewarded item.

### ItemDrop

TODO

### ItemDropQuantity

TODO

### RewardFactionId

Faction Id (from [Faction.dbc](../../dbc/Faction.md)) for which the quest give reputation points.
Number of gain or lost reputation points for Faction at quest completion. This is special reputation rewarding. Normal reputation reward to quest rewarding creature faction calculated and added automatically.

### RewardFactionValue

This field is used for reputation lookup in [QuestFactionReward.dbc](../../dbc/QuestFactionReward.md) if RewardFactionValue is 0. Value X in this field indicates RepX column of QuestFactionReward.dbc. If RewardRepValueId is positive, reputation from the first row of QuestFactionReward.dbc will be used, for negative values the second row is used.

### RewardFactionOverride

This field is used to give reputation values not present in QuestFactionReward.dbc or to override them if [RewardFactionValue](#rewardfactionvalue) is wrong for some reason. The value in this field is 100× the intended reputation reward (if you want to give 400 rep, put 40000 in RewardFactionValueIdOverride).

### POIContinent

MapId of a quest point of interest (POI - Point Of Interest). POI will be shown on the map when quest is active.

### POIx

X coordinate of quest POI.

### POIy

Y coordinate of quest POI.

### POIPriority

TODO

### LogTitle

Title of the quest.

### LogDescription

Objectives of the quest. If empty, quest is an auto-complete quest that can be immediately finished without accepting it first.

### QuestDescription

The quest text. You can use certain placeholders that will be filled in in-game: $B - line break, $N - name, $R - race, $C - class, $Gmale:female; (male and female can be replace with any synonymn you want, but the order must stay the same. IE: boy:girl / man:woman / sir:madam / dude:chick)

### AreaDescription

Additional objectives shown as summary in the quest tracker.

### QuestCompletionLog

Text shown after the quest has been completed.

### RequiredNpcOrGo

Value &gt; 0:required creature\_template ID the player needs to kill in order to complete the quest.
Value &lt; 0:required gameobject\_template ID the player needs to use in order to complete the quest (only gameobject type GAMEOBJECT\_TYPE\_GOOBER).

### RequiredNpcOrGoCount

The number of times the creature or gameobject must be killed or used.

### RequiredItemId

[Item\_template](item_template.md#id) 

Id of required item to complete the quest.

### RequiredItemCount

Amount of required items

### RequiredFactionId

TODO

### RequiredFactionValue

TODO

### ObjectiveText

Used to define non-standard objective texts, that show up in the questlog. Example, "Heal fallen warrior" and the number gets added by Count values.

### VerifiedBuild

This field is used by the AzerothCore Team to determine whether a template has been verified from WDB files (ADB files for this one).

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is [-Client Build](../auth/realmlist.md "DB:Auth:realmlist") then it was parsed with WDB files from that specific [client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist") and manually edited later for some special necessity.

## Examples dealing with quests

Always use PrevQuestId before using NextQuestId. NextQuestId is considered optional and to be used only when PrevQuestId is not sufficient

### Basic quest

Single, stand-alone quest with no prerequisites

``` cpp
    questA
```

``` cpp
entry = questA        PrevQuestId = 0        NextQuestId = 0        ExclusiveGroup = 0        NextQuestInChain = 0
```

### Prequest

When this quest require another quest to be rewarded

``` cpp
    questA
```

``` cpp
entry = questA        PrevQuestId = questX   NextQuestId = 0        ExclusiveGroup = 0        NextQuestInChain = 0
```

### Chain of quests

Player get quests in a strict chain that must be completed in a specific order.

``` cpp
    questA
      |
    questB
      |
    questC
      |
    questD
```

``` cpp
entry = questA      PrevQuestId = 0          NextQuestId = 0       ExclusiveGroup = 0       NextQuestInChain = questB
entry = questB      PrevQuestId = questA     NextQuestId = 0       ExclusiveGroup = 0       NextQuestInChain = questC
entry = questC      PrevQuestId = questB     NextQuestId = 0       ExclusiveGroup = 0       NextQuestInChain = questD
entry = questD      PrevQuestId = questC     NextQuestId = 0       ExclusiveGroup = 0       NextQuestInChain = 0
```

### Chain of quests with multiple start quests.

Player should only be allowed to complete one of three possible

``` cpp
    questA     questB    questC
      \           |         /
        ------ questD -----
                  |
               questE
```

``` cpp
entry = questA      PrevQuestId = 0        NextQuestId = questD    ExclusiveGroup = questA    NextQuestInChain = questD    
entry = questB      PrevQuestId = 0        NextQuestId = questD    ExclusiveGroup = questA    NextQuestInChain = questD
entry = questC      PrevQuestId = 0        NextQuestId = questD    ExclusiveGroup = questA    NextQuestInChain = questD
entry = questD      PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0         NextQuestInChain = questE
entry = questE      PrevQuestId = questD   NextQuestId = 0         ExclusiveGroup = 0         NextQuestInChain = 0
```

### Chain of quests with multiple start quests.

Player must complete all three initial quests before D becomes available

``` cpp
    questA    questB    questC
      \         |          /
       ------ questD -----
                |
              questE
```

``` cpp
entry = questA      PrevQuestId = 0        NextQuestId = questD   ExclusiveGroup = -questA    NextQuestInChain = questD
entry = questB      PrevQuestId = 0        NextQuestId = questD   ExclusiveGroup = -questA    NextQuestInChain = questD
entry = questC      PrevQuestId = 0        NextQuestId = questD   ExclusiveGroup = -questA    NextQuestInChain = questD
entry = questD      PrevQuestId = 0        NextQuestId = 0        ExclusiveGroup = 0          NextQuestInChain = questE
entry = questE      PrevQuestId = questD   NextQuestId = 0        ExclusiveGroup = 0          NextQuestInChain = 0
```

### Quests with split and a child quest

Completing A unlocks B and C that can be done at the same time. They both need to be completed before D becomes available. X is needed to obtain item for C and this quest should only be available if C is active

``` cpp
                questA
              /        \
          questB     questC  -  questX
              \        /
                questD
```

``` cpp
entry = questA       PrevQuestId = 0        NextQuestId = 0        ExclusiveGroup = 0         NextQuestInChain = 0
entry = questB       PrevQuestId = questA   NextQuestId = questD   ExclusiveGroup = -questB   NextQuestInChain = 0
entry = questC       PrevQuestId = questA   NextQuestId = questD   ExclusiveGroup = -questB   NextQuestInChain = 0
entry = questX       PrevQuestId = -questC  NextQuestId = 0        ExclusiveGroup = 0         NextQuestInChain = 0
entry = questD       PrevQuestId = 0        NextQuestId = 0        ExclusiveGroup = 0         NextQuestInChain = 0
```

### Multiple quest chains, leading to one final quest

Player may complete (not required to) X, but has to complete all three quest chains before final quest becomes available

``` cpp
                *questX*
                   |
    *questA*    *questC*    *questE*
       |           |            |
    *questB*    *questD*    *questF*
       \           |           /
         ------ *questG* -----
```

``` cpp
PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = questC    entry = questX
PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = questB    entry = questA
PrevQuestId = questA   NextQuestId = questG    ExclusiveGroup = -questB    NextQuestInChain = 0         entry = questB
PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = questD    entry = questC
PrevQuestId = questC   NextQuestId = questG    ExclusiveGroup = -questB    NextQuestInChain = 0         entry = questD
PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = questF    entry = questE
PrevQuestId = questE   NextQuestId = questG    ExclusiveGroup = -questB    NextQuestInChain = 0         entry = questF

PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = 0         entry = questG
```

### Complicated

Player must first complete A, then B to unlock the chain from C to E. Three other quests in a group will also be unlocked, those can be done at the same time. The three grouped quests must all be completed before I becomes available. Completion of E and I is required to obtain the final quest.

``` cpp
                *questA*
                   |
                *questB*
              /          \
          *questC*     *questF*
             |         *questG*
          *questD*     *questH*
             |            |
          *questE*     *questI*
             \           /
                *questJ*
```

``` cpp
PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = questB    entry = questA
PrevQuestId = questA   NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = 0         entry = questB

PrevQuestId = questB   NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = questD    entry = questC
PrevQuestId = questC   NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = questE    entry = questD
PrevQuestId = questD   NextQuestId = questJ    ExclusiveGroup = -questE    NextQuestInChain = 0         entry = questE

PrevQuestId = questB   NextQuestId = questI    ExclusiveGroup = -questF    NextQuestInChain = 0         entry = questF
PrevQuestId = questB   NextQuestId = questI    ExclusiveGroup = -questF    NextQuestInChain = 0         entry = questG
PrevQuestId = questB   NextQuestId = questI    ExclusiveGroup = -questF    NextQuestInChain = 0         entry = questH

PrevQuestId = 0        NextQuestId = questJ    ExclusiveGroup = -questE    NextQuestInChain = 0         entry = questI

PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = 0         entry = questJ
```

### Impossible - many quests may unlock many

Player can choose between two alternative chains (Chain A or B, but not both chains). A2 or B2 should unlock C, D and E when complete. When all three complete, F should be unlocked. If player get A3 or B3 after complete F, depends on if chain A or B was chosen

``` cpp
                *questA1*           *questB1*
                    |                   |
                *questA2*           *questB2*
                    \                  /
                     ---- *questC* ----
                          *questD*
                          *questE*
                             |
                          *questF*
                         /        \
                    *questA3*   *questB3*
```

``` cpp
PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = questA2   entry = questA1
PrevQuestId = questA1  NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = 0         entry = questA2

PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = questB2   entry = questB1
PrevQuestId = questB1  NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = 0         entry = questB2

PrevQuestId = 0        NextQuestId = questF    ExclusiveGroup = -questC    NextQuestInChain = 0         entry = questC
PrevQuestId = 0        NextQuestId = questF    ExclusiveGroup = -questC    NextQuestInChain = 0         entry = questD
PrevQuestId = 0        NextQuestId = questF    ExclusiveGroup = -questC    NextQuestInChain = 0         entry = questE

PrevQuestId = 0        NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = 0         entry = questF

PrevQuestId = questF   NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = 0         entry = questA3
PrevQuestId = questF   NextQuestId = 0         ExclusiveGroup = 0          NextQuestInChain = 0         entry = questB3
```

Note:

If player can choose between chain A or B may be determined by faction status (aldor or scryer), using ReqMinRepFaction = 1. Player should not be able to be neutral+1 with both at the same time. This may be the common threshold to obtain aldor or scryer quests (this is unsure). If that is the case, only the unlock of C, D and E after complete A2 *or* B2 is the impossible part.\_Note 2: With the [Conditions](conditions.md) table now every quest chain is possible.''

/table
