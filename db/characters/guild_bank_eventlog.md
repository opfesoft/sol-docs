# guild\_bank\_eventlog

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
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Guild Identificator</p></td>
</tr>
<tr>
<td><p><a href="#logguid">LogGuid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Log record identificator - auxiliary column</p></td>
</tr>
<tr>
<td><p><a href="#tabid">TabID</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Guild bank TabId</p></td>
</tr>
<tr>
<td><p><a href="#eventtype">EventType</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Event type</p></td>
</tr>
<tr>
<td><p><a href="#playerguid">PlayerGuid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#itemormoney">ItemOrMoney</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#itemstackcount">ItemStackCount</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#desttabid">DestTabId</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Destination Tab Id</p></td>
</tr>
<tr>
<td><p><a href="#timestamp">TimeStamp</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
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

### TabId

Source tab ID

### EventType

1 = GUILD\_BANK\_LOG\_DEPOSIT\_ITEM

2 = GUILD\_BANK\_LOG\_WITHDRAW\_ITEM

3 = GUILD\_BANK\_LOG\_MOVE\_ITEM

4 = GUILD\_BANK\_LOG\_DEPOSIT\_MONEY

5 = GUILD\_BANK\_LOG\_WITHDRAW\_MONEY

6 = GUILD\_BANK\_LOG\_REPAIR\_MONEY

7 = GUILD\_BANK\_LOG\_MOVE\_ITEM2

8 = GUILD\_BANK\_LOG\_UNK1

9 = GUILD\_BANK\_LOG\_BUY\_SLOT

### PlayerGuid

GUID of the Player. See [characters.guid](characters.md#guid)

### ItemOrMoney

Either the amount of money or the [item ID](../world/item_template.md#entry).

### ItemStackCount

The stack count of the item.

### DestTabId

Destination tab ID

### TimeStamp

Event UNIX time
