# creature\_summon\_groups

This table holds data about temporary summoned creatures. It is possible to group summons and create boss waves of adds etc.

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
<td><p><a href="#summonerid">summonerId</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#summonertype">summonerType</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><a href="#groupid">groupId</a></td>
<td>tinyint(3)</td>
<td>unsigned</td>
<td> </td>
<td>NO</td>
<td>0</td>
<td> </td>
<td> </td>
</tr>
<tr>
<td><a href="#entry">entry</a></td>
<td>mediumint(8)</td>
<td>unsigned</td>
<td> </td>
<td>NO</td>
<td>0</td>
<td> </td>
<td> </td>
</tr>
<tr>
<td><p><a href="#position_x">position_x</a></p></td>
<td><p>float</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#position_y">position_y</a></p></td>
<td><p>float</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td> </td>
</tr>
<tr>
<td><p><a href="#position_z">position_z</a></p></td>
<td><p>float</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td> </td>
</tr>
<tr>
<td><p><a href="#orientation">orientation</a></p></td>
<td><p>float</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><a href="#summontype">summonType</a></td>
<td>tinyint(3)</td>
<td>unsigned</td>
<td> </td>
<td>NO</td>
<td>0</td>
<td> </td>
<td> </td>
</tr>
<tr>
<td><a href="#summontime">summonTime</a></td>
<td>int(10)</td>
<td>unsigned</td>
<td> </td>
<td>NO</td>
<td>0</td>
<td> </td>
<td> </td>
</tr>
</tbody>
</table>

## Description of the fields

### summonerId

Summoner's id depending on summonerType

### summonerType

Summoner's type:

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Value</p></th>
<th><p>Type</p></th>
</tr>
</thead>
<tbody>
<tr>
<td><p>0</p></td>
<td><p>SUMMONER_TYPE_CREATURE</p></td>
</tr>
<tr>
<td><p>1</p></td>
<td><p>SUMMONER_TYPE_GAMEOBJECT</p></td>
</tr>
<tr>
<td><p>2</p></td>
<td><p>SUMMONER_TYPE_MAP</p></td>
</tr>
</tbody>
</table>

### groupId

Group identificator, all creatures with the same groupId will be summoned at once

### entry

Entry of summoned creature from [creature\_template.entry](creature_template.md#entry)

### position\_x

X coordinate of position, where the creature will be spawned

### position\_y

Y coordinate of position, where the creature will be spawned

### position\_z

Z coordinate of position, where the creature will be spawned

### orientation

Orientation the summoned creature will get when spawned

### summonType

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Value</p></th>
<th><p>Name</p></th>
<th><p>Comments</p></th>
</tr>
</thead>
<tbody>
<tr>
<td><p>1</p></td>
<td><p>TEMPSUMMON_TIMED_OR_DEAD_DESPAWN</p></td>
<td><p>Despawns after a specified time (only out of combat) OR when the creature disappears</p></td>
</tr>
<tr>
<td><p>2</p></td>
<td><p>TEMPSUMMON_TIMED_OR_CORPSE_DESPAWN</p></td>
<td><p>Despawns after a specified time (only out of combat) OR when the creature dies</p></td>
</tr>
<tr>
<td><p>3</p></td>
<td><p>TEMPSUMMON_TIMED_DESPAWN</p></td>
<td><p>Despawns after a specified time (no matter if the creature is in combat or not)</p></td>
</tr>
<tr>
<td><p>4</p></td>
<td><p>TEMPSUMMON_TIMED_DESPAWN_OUT_OF_COMBAT</p></td>
<td><p>Despawns after a specified time after the creature is out of combat</p></td>
</tr>
<tr>
<td><p>5</p></td>
<td><p>TEMPSUMMON_CORPSE_DESPAWN</p></td>
<td><p>Despawns instantly after death</p></td>
</tr>
<tr>
<td><p>6</p></td>
<td><p>TEMPSUMMON_CORPSE_TIMED_DESPAWN</p></td>
<td><p>Despawns after a specified time after death</p></td>
</tr>
<tr>
<td><p>7</p></td>
<td><p>TEMPSUMMON_DEAD_DESPAWN</p></td>
<td><p>Despawns when the creature disappears</p></td>
</tr>
<tr>
<td><p>8</p></td>
<td><p>TEMPSUMMON_MANUAL_DESPAWN</p></td>
<td><p>Despawns when UnSummon() is called or other script actions are used, e.g. SMART_ACTION_FORCE_DESPAWN or SCRIPT_COMMAND_DESPAWN_CREATURE</p></td>
</tr>
</tbody>
</table>

### summonTime

Timer linked to summontype (in milliseconds).
