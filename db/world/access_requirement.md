# access\_requirement

**The \`access\_requirement\` table**

This table contains the access requirements to enter an instance.

## Structure

<table>
<tbody>
<tr>
<td><p><strong>Field</strong></p></td>
<td><p><strong>Type</strong></p></td>
<td><p><strong>Attributes</strong></p></td>
<td><p><strong>Key</strong></p></td>
<td><p><strong>Null</strong></p></td>
<td><p><strong>Default</strong></p></td>
<td><p><strong>Extra</strong></p></td>
<td><p><strong>Comment</strong></p></td>
</tr>
<tr>
<td><p><a href="#mapid">mapId</a></p></td>
<td><p>mediumint (8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#difficulty">difficulty</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#level_min">level_min</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#level_max">level_max</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><a href="#item_level">item_level</a></td>
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
<td><p><a href="#item">item</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#item2">item2</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#quest_done_a">quest_done_A</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#quest_done_h">quest_done_H</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#completed_achievement">completed_achievement</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#quest_failed_text">quest_failed_text</a></p></td>
<td><p>text</p></td>
<td><p> </p></td>
<td><p><br />
</p></td>
<td><p>YES</p></td>
<td><p>NULL</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#comment">comment</a></p></td>
<td><p>text</p></td>
<td><p> </p></td>
<td><p><br />
</p></td>
<td><p>YES</p></td>
<td><p>NULL</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
</tbody>
</table>

## Description of the fields

### mapId

This is the [access\_id](instance_template.md#map) field from the [instance\_template](instance_template.md) table. It is an arbitrary number that merely links the requirements to an [instance\_template](instance_template.md), or [areatrigger\_teleport](areatrigger_teleport.md)

### difficulty

5 man dungeons - 0 for normal, 1 for heroic, 2 for epic (not used yet)

10 man dungeons - 0 for normal, 2 for heroic

25 man dungeons - 1 for normal, 3 for heroic

### level\_min

The minimum level that you must be in order to enter the instance.

### level\_max

The maximum level that you can be in order to enter the instance.

### item\_level

The at least required item level for a instance.

-   All WotLK Heroics require at least an average item level of 180.
-   Trial of the Champion, Pit of Saron, and the Forge of Souls require an average item level of 200.
-   Halls of Reflection requires an average item level of 219.

### item

An [item](item_template.md#entry) that you must have in your inventory to enter the instance. This item can not be in the bank.

### item2

A second [item](item_template.md#entry) that you must have in your inventory. This item can not be in the bank.

### quest\_done\_A

A [quest](quest_template.md#id) that you must have completed. This field is only for alliance.

### quest\_done\_H

A [quest](quest_template.md#id) that you must have completed. This field is only for horde.

### completed\_achievement

An [achievement](../../dbc/Achievement.md) that must be completed by the player to enter an instance.

### quest\_failed\_text

The text that is shown if you try and enter the instance without having completed the quest.

### comment

This field is for any comment you want to make about the requirements. It is arbitrary text.
