# linked\_respawn

This table links trash mobs to bosses so that if you kill the boss, the trash do not respawn before the instance is reset.
Gameobjects can be linked too!

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
<td><p><a href="#guid">guid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>Dependent Creature</p></td>
</tr>
<tr>
<td><p><a href="#linkedguid">linkedGuid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>Master Creature</p></td>
</tr>
<tr>
<td><p><a href="#linktype">linkType</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
</tbody>
</table>

## Description of the fields

### guid

This is the guid of the [creature](creature.md#guid) or [gameobject](gameobject.md#guid) you want to link.

### linkedGuid

This is the guid of the [creature](creature.md#guid) or [gameobject](gameobject.md#guid) (boss most likely) that you want to link to.

### linkedType

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr>
<td><p><strong>Value</strong></p></td>
<td><p><strong>Dependent</strong></p></td>
<td><p><strong>Master</strong></p></td>
</tr>
<tr>
<td><p>0</p></td>
<td><p>creature</p></td>
<td><p>creature</p></td>
</tr>
<tr>
<td><p>1</p></td>
<td><p>creature</p></td>
<td><p>gameobject</p></td>
</tr>
<tr>
<td><p>2</p></td>
<td><p>gameobject</p></td>
<td><p>gameobject</p></td>
</tr>
<tr>
<td><p>3</p></td>
<td><p>gameobject</p></td>
<td><p>creature</p></td>
</tr>
</tbody>
</table>


