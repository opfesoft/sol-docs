# creature\_formations

This table allows to group mobs. Members of group will follow others, and attack their targets.

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
<td><p><a href="#leaderguid">leaderGUID</a></p></td>
<td><p>int(11)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#memberguid">memberGUID</a></p></td>
<td><p>int(11)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#dist">dist</a></p></td>
<td><p>float</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#angle">angle</a></p></td>
<td><p>float</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><a href="#groupai">groupAI</a></td>
<td>int(11)</td>
<td>unsigned</td>
<td> </td>
<td>NO</td>
<td>NULL</td>
<td> </td>
<td> </td>
</tr>
</tbody>
</table>

## Description of the fields

### leaderGUID

[GUID](creature.md#guid) of group leader

### memberGUID

[GUID](creature.md#guid) of group member

### dist

Maximum distance between group leader and member

### angle

Angle between leader and member<br>
Note: Only degrees are used! Values should be between 0 and 360:

| degrees | position in relation to the leader |
|---------|------------------------------------|
| 180     | front                              |
| 270     | left                               |
| 0       | behind                             |
| 90      | right                              |

The core will automatically switch the position of the members if the leader takes a turn greater than 90 degrees. This prevents crossover movement of the members. Examples:

- 90 degrees becomes 270 degrees (and vice versa)
- 220 degrees becomes 140 degrees (and vice versa)
- 30 degrees becomes 330 degrees (and vice versa)

### groupAI

Sets group member behaviours, values are:

| Value | Behaviour                                                        |
|-------|------------------------------------------------------------------|
| 0     | If any creature from the group is attacked, members won't assist |
| 1     | Group members will assist only their leader if attacked.         |
| >1    | Group members will assist all group members                      |
| 5     | Group members won't follow the leader                            |

### Additional notes

- Formations are currently only moved via random and waypoint movement generators (see table "[waypoint\_data](waypoint_data.md)" for the latter).
- By default the formation members use pathfinding to reach the next point, this can be disabled for waypoint movement using [waypoint\_data.pathfinding](waypoint_data.md#pathfinding).
