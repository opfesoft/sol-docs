# command

Holds help and security information for commands. This table does NOT create new commands, it only sets / overrides security and provides help.

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
<td><p>name</p></td>
<td><p>varchar(50)</p></td>
<td><p>signed</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
<tr>
<td><p>security</p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p></p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
<tr>
<td><p>help</p></td>
<td><p>longtext</p></td>
<td><p>signed</p></td>
<td><p></p></td>
<td><p>YES</p></td>
<td><p>NULL</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
</tbody>
</table>

## Description of the fields

<h3>name</h3>
<p>The name of the command.</p>

<h3>security</h3>
<p>The security level required to use the command. Corresponds with [account_access.gmlevel](../auth/account_access.md#gmlevel) in the realm database.</p>

<h3>help</h3>
<p>The help text displayed by the .help command.</p>
