# guild\_eventlog

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
<td><p><a href="#guildid">guildid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p>Guild Identificator</p></td>
</tr>
<tr>
<td><p><a href="#logguid">LogGuid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p>Log record identificator - auxiliary column</p></td>
</tr>
<tr>
<td><p><a href="#eventtype">EventType</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p>Event type</p></td>
</tr>
<tr>
<td><p><a href="#playerguid1">PlayerGuid1</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p>Player 1</p></td>
</tr>
<tr>
<td><p><a href="#playerguid2">PlayerGuid2</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p>Player 2</p></td>
</tr>
<tr>
<td><p><a href="#newrank">NewRank</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p>New rank (in case promotion/demotion)</p></td>
</tr>
<tr>
<td><p><a href="#timestamp">TimeStamp</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p>Event UNIX time</p></td>
</tr>
</tbody>
</table>

## Description of the fields

### guildid

Guild Identificator, see [guild.guildid](guild.md#guildid)

### LogGuid

Log record identificator - auxiliary column

### EventType

1 = GUILD\_EVENT\_LOG\_INVITE\_PLAYER

2 = GUILD\_EVENT\_LOG\_JOIN\_GUILD

3 = GUILD\_EVENT\_LOG\_PROMOTE\_PLAYER

4 = GUILD\_EVENT\_LOG\_DEMOTE\_PLAYER

5 = GUILD\_EVENT\_LOG\_UNINVITE\_PLAYER

6 = GUILD\_EVENT\_LOG\_LEAVE\_GUILD

### PlayerGuid1

GUID of Player 1, see [characters.guid](characters.md#guid)

### PlayerGuid2

GUID of Player 2, see [characters.guid](characters.md#guid)

### NewRank

New rank (in case of promotion/demotion), see [guild\_rank.rid](guild_rank.md#rid)

### TimeStamp

Event UNIX time
