# spell\_group

Table used to group spells for varius checks in the core. One spell may be added to many groups, but can occur in one group only once.

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
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#spell_id">spell_id</a></p></td>
<td><p>int(11)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#special_flag">special_flag</a></p></td>
<td><p>int(11)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
</tbody>
</table>

## Description of the fields

### id

Group identifier
Rules of assigning id:

-   if group is going to be used in core code, use first avalible entry below 1000 and add enum value to SpellGroup enum in SpellMgr.h
-   if group is not going to be used in core code, use lowest avalible entry higher than 1000

### spell\_id

SpellId from Spell.dbc. If spell is added to spell\_ranks, spell\_id has to be first rank of that spell.

### special\_flag

| Flag                                         | Value  |
|----------------------------------------------|--------|
| SPELL_GROUP_SPECIAL_FLAG_NONE                | 0x000  |
| SPELL_GROUP_SPECIAL_FLAG_ELIXIR_BATTLE       | 0x001  |
| SPELL_GROUP_SPECIAL_FLAG_ELIXIR_GUARDIAN     | 0x002  |
| SPELL_GROUP_SPECIAL_FLAG_ELIXIR_UNSTABLE     | 0x004  |
| SPELL_GROUP_SPECIAL_FLAG_ELIXIR_SHATTRATH    | 0x008  |
| SPELL_GROUP_SPECIAL_FLAG_FORCED_STRONGEST    | 0x010  |
| SPELL_GROUP_SPECIAL_FLAG_SKIP_STRONGER_CHECK | 0x020  |
| SPELL_GROUP_SPECIAL_FLAG_BASE_AMOUNT_CHECK   | 0x040  |
| SPELL_GROUP_SPECIAL_FLAG_PRIORITY1           | 0x100  |
| SPELL_GROUP_SPECIAL_FLAG_PRIORITY2           | 0x200  |
| SPELL_GROUP_SPECIAL_FLAG_PRIORITY3           | 0x400  |
| SPELL_GROUP_SPECIAL_FLAG_PRIORITY4           | 0x800  |
