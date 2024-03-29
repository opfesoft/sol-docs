# quest\_template\_addon

Contains extra definitions like linking quests, dependencies and requirements for the quests defined in the [quest\_template](quest_template.md) table to become available to the player.

## Structure

<table>
<thead>
<tr class="header">
<th><p><strong>Field</strong></p></th>
<th><p><strong>Type</strong></p></th>
<th><p><strong>Attributes</strong></p></th>
<th><p><strong>Key</strong></p></th>
<th><p><strong>Null</strong></p></th>
<th><p><strong>Default</strong></p></th>
<th><p><strong>Extra</strong></p></th>
<th><p><strong>Comment</strong></p></th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="#id">ID</a></td>
<td>mediumint(8)</td>
<td>unsigned</td>
<td>PRI</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><td><a href="quest_template.md#id">Unique ID linked to quest_template.ID</a></td>
Unique ID linked to quest_template.ID</td>
</tr>
<tr>
<td><a href="#maxlevel">MaxLevel</a></td>
<td>tinyint(3)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#allowableclasses">AllowableClasses</a></td>
<td>int(10)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#sourcespellid">SourceSpellID</a></td>
<td>mediumint(8)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#prevquestid">PrevQuestID</a></td>
<td>mediumint(8)</td>
<td><br />
</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#nextquestid">NextQuestID</a></td>
<td>mediumint(8)</td>
<td><br />
</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#exclusivegroup">ExclusiveGroup</a></td>
<td>mediumint(8)</td>
<td><br />
</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#rewardmailtemplateid">RewardMailTemplateID</a></td>
<td>mediumint(8)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#rewardmaildelay">RewardMailDelay</a></td>
<td>int(10)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#requiredskillid">RequiredSkillID</a></td>
<td>smallint(5)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#requiredskillpoints">RequiredSkillPoints</a></td>
<td>smallint(5)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#requiredminrepfaction">RequiredMinRepFaction</a></td>
<td>smallint(5)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#requiredmaxrepfaction">RequiredMaxRepFaction</a></td>
<td>smallint(5)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#requiredminrepvalue">RequiredMinRepValue</a></td>
<td>mediumint(8)</td>
<td><br />
</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#requiredmaxrepvalue">RequiredMaxRepValue</a></td>
<td>mediumint(8)</td>
<td><br />
</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#provideditemcount">ProvidedItemCount</a></td>
<td>tinyint(3)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#specialflags">SpecialFlags</a></td>
<td>tinyint(3)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
</tbody>
</table>

## Description of the fields

### ID

Unique quest ID, matching the same quest ID in [quest\_template.ID](quest_template.md#id)

### MaxLevel

Maximum player level at which a character can get the quest.

### AllowableClasses

Classes required to get the quest. 0 means the quest is available for all classes.
This field is a bitmask, you can combine class values. See [ChrClasses.dbc](../../dbc/ChrClasses.md)

### SourceSpellID

The spell ID cast on player upon starting the quest.

### PrevQuestID

-   **if value &gt; 0:** Contains the previous quest id, that must be completed before this quest can be started.
-   **If value &lt; 0:** Contains the parent quest id, that must be active before this quest can be started.

See the [examples section](quest_template.md#examples-dealing-with-quests) for examples.

### NextQuestID

Contains the next quest id, in case PrevQuestId of that other quest is not sufficient.

See the [examples section](quest_template.md#examples-dealing-with-quests) for examples.

### ExclusiveGroup

-   **if ExclusiveGroup &gt; 0**

Allows to define a group of quests of which only one may be chosen and completed. E.g. if from quests 1200, 1201 and 1202 only one should be allowed to be chosen, insert 1200 into ExclusiveGroup of all 3 quests.

-   **if ExclusiveGroup &lt; 0**

Allows to define a group of quests of which all must be completed and rewarded to start the next quest. E.g. if quest 1000 requires 1200, 1201 and 1202 and all these quests have the same exclusive group -1200 then all of them have to be completed and rewarded before quest 1000 can be started.

### RewardMailTemplateID

The ID has to match an entry in MailTemplate.dbc which contains the mail text. If the quest gives as a reward an item from a possible list of items, the ID here corresponds to the proper loot template in [mail\_loot\_template](loot_template.md). According to the rules in that loot template, items "looted" will be sent by mail at the completion of the quest.

### RewardMailDelay

How many seconds to wait until the mail is sent to the character that turned in a quest rewarding items from a loot template defined in [RewardMailTemplateId](quest_template_addon.md#rewardmailtemplateid)

### RequiredSkillID

Skill required to know to accept the quest. See [SkillLine.dbc](../../dbc/SkillLine.md)
0 means no skill is required.

### RequiredSkillPoints

Skill points required to have in order to accept the quest.

### RequiredMinRepFaction

Faction ID for reputation requirement. See [Faction.dbc](../../dbc/Faction.md)

### RequiredMaxRepFaction

The Faction ID for the faction that controls the maximum reputation value that the player can have and still get the quest. See [Faction.dbc](../../dbc/Faction.md)

### RequiredMinRepValue

Players must have this reputation or higher in order to receive the quest.

### RequiredMaxRepValue

The maximum reputation value that the player can have with a faction and still get the quest. If the player has more reputation than the value in this field, the quest will not be able to be taken anymore.

### ProvidedItemCount

Number of items given to the player (inserted in the player's bags) upon accepting the quest.

### SpecialFlags

This field is a bitmask and is for controlling server side quest functions. Blizzard keeps these data server-side and they are not sent to the client, so we have to populate the field manually.

-   0: No extra requirements

<!-- -->

-    1: Makes the quest repeatable.
-    2: Makes the quest only completable by some external event (an entry in [areatrigger\_involvedrelation](areatrigger_involvedrelation.md), spell effect quest complete or an entry in [spell\_scripts](scripts.md) with command 7 as some examples)
-    4: Make quest auto-accept. As of patch 3.3.5a only quests in the starter area need this flag.
-    8: Only used for Dungeon Finder quests
-   16: Makes the quest monthly
-   32: The quest requires RequiredOrNpcGo killcredit (a spell cast), but NOT an actual NPC kill. This action usually involves killing an invisible "bunny" NPC. **Note:** This is actually not working correctly, so better not use this flag for new quests.
