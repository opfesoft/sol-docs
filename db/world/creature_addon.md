# creature\_addon

The creature\_addon and creature\_template\_addon tables define different things that are applied on creatures when they are loaded. These "different things" can be for example to have the creature be mounted, to have it emote something, to have it display an aura effect, etc. Through the use of the fields in this table, many things can be changed about the outward visual appearance of the creature. The creature\_template\_addon table affects all creatures with that creature template ID while the creature\_addon table affects individually spawned creatures (so that two creatures using the same template can look different).

NOTE: A creature\_addon record will override a creature\_template\_addon record should they overlap on the same creature.

NOTICE: The data for this table is largely incomplete and is mostly just a regurgitation of what the client receives from the server. This article is a WIP as to what all the possible values are.

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
<td><p><a href="#guidentry">guid/entry</a></p></td>
<td><p>int(10)/medumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#path_id">path_id</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#mount">mount</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#bytes1">bytes1</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#bytes2">bytes2</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#emote">emote</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><a href="#addonflags">addonFlags</a></td>
<td>tinyint(1)</td>
<td>unsigned</td>
<td><br />
</td>
<td>NO</td>
<td>0</td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><a href="#maxaggroradius">maxAggroRadius</a></td>
<td>float</td>
<td>unsigned</td>
<td><br />
</td>
<td>YES</td>
<td></td>
<td><br />
</td>
<td><br />
</td>
</tr>
<tr>
<td><p><a href="#auras">auras</a></p></td>
<td><p>text</p></td>
<td><p></p></td>
<td><p><br />
</p></td>
<td><p>YES</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
</tbody>
</table>

## Description of the fields

### guid/entry

For creature\_addon, this field signifies a unique creature guid. It will affect just that creature whose GUID matches the one specified here.
For creature\_template\_addon, this field signifies the [creature\_template.entry](creature_template.md#creature_template-entry). It will affect all spawned creatures using that template entry.

### path\_id

If a creature uses waypoint movement (MovementType 2), this field must contain a valid [waypoint\_data.id](waypoint_data.md#id).

### mount

The model ID of the mount to be used to make the creature appear mounted. The value here overrides the value for the creature's unit field UNIT\_FIELD\_MOUNTDISPLAYID.

### bytes1

The value here overrides the value for the creature's unit field UNIT\_FIELD\_BYTES\_1.

List of known values and what their visual effects on the creature

-   1 = Sitting
-   2 = Sit chair
-   3 = Sleep
-   4 = Sit low chair
-   5 = Sit medium chair
-   6 = Sit high chair
-   7 = Shows health bar as empty (combine with the state dead emote to make a creature look dead)
-   8 = Makes the mob kneel
-   9 = Submerges the creature below the ground
-   131072 = Sneak
-   33554432 = Hover mode
-   50331648 = Hover mode 2

### bytes2

The value here overrides the value for the creature's unit field UNIT\_FIELD\_BYTES\_2.

NOTE: //creatures always have melee weapon ready if any unless specified otherwise

List of few known values and what their visual effects on the creature

-   0 = STATE\_UNARMED (sheathed weapon)
-   1 = STATE\_MELEE (ready melee weapon)
-   2 = STATE\_RANGED (ready ranged weapon, melee weapon is sheathed)

### emote

Emote ID that the creature should continually perform.

List of often used emote IDs and what they do can be found [here](../../dbc/Emotes.md).

### addonFlags

| Flag                                   | Description |
|----------------------------------------|-------------|
| `CREATURE_ADDON_FLAG_IS_LARGE`         | Visibility distance for creatures; if set use maximum visibility distance (250y), otherwise default from worldserver.conf (normally 100y) |
| `CREATURE_ADDON_FLAG_NO_RANDOM_GENDER` | Creature will only use the original gender of the specified DisplayID (see table [creature\_model\_info](creature_model_info.md)) |

### maxAggroRadius

If set the aggro radius is limited to this value.

### auras

This field controls any auras to be applied on the creature (both in effect and visually). To apply multiple auras, you can add more aura entries, separating each entry by a space. Remember that if a spell applies multiple auras.

List of useful aura entries (examples):

-   '16380' - Makes the creature invisible.
-   '18950' - Makes the creature detect other invisible units (players or creatures).
-   '16380 18950' - Both auras above

Important: Do not use temporary auras for spawned creatures, this will lead to a warning in the server log.
