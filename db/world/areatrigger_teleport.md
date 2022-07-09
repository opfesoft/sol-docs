# areatrigger\_teleport

Contains all the teleport triggers definition. This table is used to complete .dbc file information.

## Structure

<table>
<colgroup>
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
<col width="12%" />
</colgroup>
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
<td><p><a href="#id">ID</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Identifier</p></td>
</tr>
<tr>
<td><p><a href="#name">Name</a></p></td>
<td><p>text</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>YES</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#target_map">target_map</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#target_position_x">target_position_x</a></p></td>
<td><p>float</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#target_position_y">target_position_y</a></p></td>
<td><p>float</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#target_position_z">target_position_z</a></p></td>
<td><p>float</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#target_orientation">target_orientation</a></p></td>
<td><p>float</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
</tbody>
</table>

## Description of the fields

### ID

[areatrigger.entry](areatrigger.md#entry)

### Name

Name of the trigger. This can be an arbitrary name, and is for descriptive purposes only.

### target\_map

Target map of the trigger (see Maps.dbc).

### target\_position\_x

X coordinate for the target destination of the trigger

### target\_position\_y

Y coordinate for the target destination of the trigger

### target\_position\_z

Z coordinate for the target destination of the trigger

### target\_orientation

Orientation the player will get when appearing at this location
