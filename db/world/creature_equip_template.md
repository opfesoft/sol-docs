# creature\_equip\_template

## **Table: creature\_equip\_template**

This table contains all the equipment combinations that can be sent for each creature.

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
<td><p><a href="#creatureid">CreatureID</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p>Unique entry</p></td>
</tr>
<tr>
<td><p><a href="#id">ID</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>1</p></td>
<td><p><br />
</p></td>
<td><p>Unique entry</p></td>
</tr>
<tr>
<td><p><a href="#itemid1">ItemID1</a></p></td>
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
<td><p><a href="#itemid2">ItemID2</a></p></td>
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
<td><p><a href="#itemid3">ItemID3</a></p></td>
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
</tbody>
</table>

**
**

## Description of the fields

### CreatureID

The direct corresponding [id](creature.md#id) in [creature](creature.md) table or [entry](creature_template.md#entry) in [creature\_template](creature_template.md) table.

### ID

An additional identifier for each individual entry, enabling multiple equipment for one creature entry. Counter **must** start with 1 and grow accordingly.

### ItemID1

This is the item number of the equipment used in the right hand from Item.dbc (see [item\_template.entry](item_template.md#entry).

### ItemID2

This is the item number of the equipment used in the left hand from Item.dbc (see [item\_template.entry](item_template.md#entry).

### ItemID3

This is the item number of the equipment used in the ranged slot from Item.dbc (see [item\_template.entry](item_template.md#entry).
