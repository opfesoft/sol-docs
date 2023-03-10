# account\_access

This table holds security access level for any realm in [realmlist](realmlist.md) table.

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
<td><p><a href="#id">id</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#gmlevel">gmlevel</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#realmid">RealmID</a></p></td>
<td><p>int(11)</p></td>
<td><p>signed</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><div class="preformatted panel" style="border-width: 1px;">
<div class="preformattedContent panelContent">
<pre><code>-1</code></pre>
</div>
</div></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#comment">comment</a></p></td>
<td><p>varchar(255)</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>YES</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
</tbody>
</table>

## Description of the fields

### id

The [account ID](account.md#id).

### gmlevel

The account security level. Different levels have access to different commands. The individual level required for a command is defined in the [command](command.md) table in each realm.

### RealmID

The [Realm ID](realmlist.md#id).

### comment
