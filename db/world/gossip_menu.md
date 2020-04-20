# gossip\_menu

**The \`gossip\_menu\` table**

This table is used for displaying gossip when a player talks to an NPC with [npcflag](creature_template.md#npcflag) set.

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
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Type</strong></p></td>
<td><p><strong>Attributes</strong></p></td>
<td><p><strong>Key</strong></p></td>
<td><p><strong>Null</strong></p></td>
<td><p><strong>Default</strong></p></td>
<td><p><strong>Extra</strong></p></td>
<td><p><strong>Comment</strong></p></td>
</tr>
<tr class="even">
<td><p><a href="#menuid">MenuID</a></p></td>
<td><p>smallint(6)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr class="odd">
<td><p><a href="#textid">TextID</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
</tbody>
</table>

## Description of the fields

### MenuID

This must match the entry you added to [creature\_template.gossip\_menu\_id](creature_template.md#gossip_menu_id). This also
groups the options from gossip\_menu\_option and displays all options associated with this ID.

**Note:** If adding your own custom menu options please see [Dealing-with-IDs](../../misc/Dealing-with-IDs.md) for appropriate IDs.

### TextID

This links to the [npc\_text.ID](npc_text.md#id) for the gossip you want to be initially displayed. Also this tells the NPC what to say at the top of the options menu when it is displayed.
