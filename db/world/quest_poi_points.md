# quest\_poi\_points

Comes from sniffs. Visually speaking, this table is used to identify the X and Y coordinates on the map (not the minimap - the main map) where a quest's question mark should appear. Use the ".gps" command where you are standing to find these coordinates. In order to see changes, ".reload quest\_poi", close Wow.exe, then delete your cache folder.

## Structure

<table>
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
<td><p><a href="#questid">questid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unasigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
<tr>
<td><p><a href="#idx1">idx1</a></p></td>
<td><p>int(10)</p></td>
<td><p>unasigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
<tr>
<td><p><a href="#idx2">idx2</a></p></td>
<td><p>int(10)</p></td>
<td><p>unasigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
<tr>
<td><p><a href="#x">x</a></p></td>
<td><p>int(10)</p></td>
<td><p>unasigned</p></td>
<td><p></p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
<tr>
<td><p><a href="#y">y</a></p></td>
<td><p>int(10)</p></td>
<td><p>unasigned</p></td>
<td><p></p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
<tr>
<td><p><a href="#verifiedbuild">VerifiedBuild</a></p></td>
<td><p>smallint</p></td>
<td><p>unasigned</p></td>
<td><p></p></td>
<td><p>YES</p></td>
<td><p>NULL</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
</tbody>
</table>

## Description of the fields

### questid

The Quest Id from [quest\_poi.questid](quest_poi.md#questid)

### idx1

Used to group multiple entries from quest\_poi.id. You must manually increment this value by 1 for each new row in quest\_poi\_point with the same questId (0, 1, 2, 3...).

### idx2

Used to group multiple entries in the quest poi points to draw the polygon for that point of interest. The actual points are the corners of each polygon.

Example quest: Secreat Communication.

<table>
<tbody>
<tr>
<td><p><strong>QuestID</strong></p></td>
<td><p><strong>idx1</strong></p></td>
<td><p><strong>idx2</strong></p></td>
<td><p><strong>x</strong></p></td>
<td><p><strong>y</strong></p></td>
<td><p><strong>VerifiedBuild</strong></p></td>
</tr>
<tr>
<td><p>8318</p></td>
<td><p>3</p></td>
<td><p>0</p></td>
<td><p>-6231</p></td>
<td><p>-51</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p>8318</p></td>
<td><p>3</p></td>
<td><p>1</p></td>
<td><p>-6236</p></td>
<td><p>-19</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p>8318</p></td>
<td><p>3</p></td>
<td><p>2</p></td>
<td><p>-6241</p></td>
<td><p>-52</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p>8318</p></td>
<td><p>3</p></td>
<td><p>3</p></td>
<td><p>-6316</p></td>
<td><p>-282</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p>8318</p></td>
<td><p>3</p></td>
<td><p>4</p></td>
<td><p>-6413</p></td>
<td><p>-282</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p>8318</p></td>
<td><p>3</p></td>
<td><p>5</p></td>
<td><p>-6483</p></td>
<td><p>-250</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p>8318</p></td>
<td><p>3</p></td>
<td><p>6</p></td>
<td><p>-6483</p></td>
<td><p>-217</p></td>
<td><p>0</p></td>
</tr>
<tr>
<td><p>8318</p></td>
<td><p>3</p></td>
<td><p>7</p></td>
<td><p>-6326</p></td>
<td><p>-7</p></td>
<td><p>0</p></td>
</tr>
</tbody>
</table>

### x

The X position of the question mark on the map.

### y

The Y position of the question mark on the map.

### VerifiedBuild

This field is used by the AzerothCore Team to determine whether a template has been verified from WDB files (ADB files for this one).

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is??[-Client Build](../auth/realmlist.md "DB:Auth:realmlist")??then it was parsed with WDB files from that specific??[client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist")??and manually edited later for some special necessity.
