# spell\_threat

This table holds threat values on all spells that should either give or take away threat.

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
<td><p><a href="#entry">entry</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#threat">Threat</a></p></td>
<td><p>smallint(6)</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
</tbody>
</table>

## Description of the fields

### entry

The spell ID. See Spell.dbc.

### Threat

The threat value that this spells should add to the caster (or take away if it is negative).
