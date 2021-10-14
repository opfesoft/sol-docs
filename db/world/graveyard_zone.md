# game_graveyard_zone

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
</tr>
<tr>
<td><p><a href="#id">ID</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p><a href="#ghostzone">GhostZone</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p><a href="#ghostarea">GhostArea</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p><a href="#faction">Faction</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>unsigned</p></td>
<td><p></p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p><a href="#classmask">ClassMask</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>unsigned</p></td>
<td><p></p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p>Comment</p></td>
<td><p>text</p></td>
<td><p> </p></td>
<td><p></p></td>
<td><p>YES</p></td>
<td><p>NULL</p></td>
</tr>
</tbody>
</table>

## Description of the fields

### ID
Graveyard's ID. See [WorldSafeLocs.dbc](../../dbc/WorldSafeLocs.md)

### GhostZone
Zone's ID of ghost position before teleportation to graveyard. See [AreaTable.dbc](../../dbc/AreaTable.md)

### GhostArea
Default is 0. If >0 it will override the lookup for the closest graveyard and return the closest graveyard for the area (subzone) even if another graveyard is closer to the player. See [AreaTable.dbc](../../dbc/AreaTable.md) for subzone values.

### Faction
Graveyard's team.

0 - Any team accepted

469 - Alliance team only

67 - Horde team only

### ClassMask
Allowed classes. This field is a bitmask, you can combine any class values, see [ChrClasses.dbc](../../dbc/ChrClasses.md). The default is 0 which means all classes are allowed.
