# achievement\_reward

This table describes the reward that you will receive when you obtain a given achievement.

## Structure

<table>
<colgroup>
<col width="14%" />
<col width="14%" />
<col width="14%" />
<col width="14%" />
<col width="14%" />
<col width="14%" />
<col width="14%" />
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
</tr>
<tr>
<td><p><a href="#id">ID</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#titlea">TitleA</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#titleh">TitleH</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#itemid">ItemID</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#sender">Sender</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#subject">Subject</a></p></td>
<td><p>varchar(255)</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>YES</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#body">Body</a></p></td>
<td><p>text</p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p>YES</p></td>
<td><p>NULL</p></td>
<td><p> </p></td>
</tr>
<tr>
<td><a href="#mailtemplateid">MailTemplateID</a></td>
<td>mediumint(8)</td>
<td>unsigned</td>
<td> </td>
<td>YES</td>
<td>0</td>
<td> </td>
</tr>
</tbody>
</table>

## Description of the fields

### ID

This is the ID of the achievement taken from the DBC `Achievement.dbc`.

### TitleA

This is the ID of the title for Alliance from `CharTitles.dbc` if the achievement rewards a title.

### TitleH

This is the ID of the title for Horde from `CharTitles.dbc` if the achievement rewards a title.

### ItemID

This is the item that that the player will receive if the achievement rewards an item. The player will get this item in a mail.

### Sender

This is the sender of the mail that the player will receive.

### Subject

This is the subject of the mail that the player will receive.

### Body

This is the body (text) of the mail that the player will receive.

### MailTemplateID

Id of the MailTemplate from `MailTemplate.dbc` of that mail that the player will receive. To use this column, `Subject` and `Body` must be empty as they are loaded from the DBC file.
