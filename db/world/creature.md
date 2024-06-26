# creature

Contains individual creature spawn data for each individual spawn of each individual creature in the game world.

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
<td><p><a href="#guid">guid</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p>Auto Increment</p></td>
<td><p>Global Unique Identifier</p></td>
</tr>
<tr>
<td><p><a href="#id">id</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Creature Identifier</p></td>
</tr>
<tr>
<td><p><a href="#map">map</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Map Identifier</p></td>
</tr>
<tr>
<td><p><a href="#zoneid">zoneId</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Zone Identifier (filled by the core, see worldserver parameter Calculate.Creature.Zone.Area.Data)</p></td>
</tr>
<tr>
<td><p><a href="#areaid">areaId</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Area Identifier (filled by the core, see worldserver parameter Calculate.Creature.Zone.Area.Data)</p></td>
</tr>
<tr>
<td><p><a href="#spawnmask">spawnMask</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>1</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#phasemask">phaseMask</a></p></td>
<td><p>smallint(5)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>1</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#modelid">modelid</a></p></td>
<td><p>mediumint(8)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>0 core determined random model or model_id to prevent random model selection by core.</p></td>
</tr>
<tr>
<td><p><a href="#equipment_id">equipment_id</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>1</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#position_x">position_x</a></p></td>
<td><p>float</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#position_y">position_y</a></p></td>
<td><p>float</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#position_z">position_z</a></p></td>
<td><p>float</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#orientation">orientation</a></p></td>
<td><p>float</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#spawntimesecs">spawntimesecs</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>120</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#wander_distance">wander_distance</a></p></td>
<td><p>float</p></td>
<td><p>signed</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>5</p></td>
<td><p> </p></td>
<td><p>Dist in yards for random movement.</p></td>
</tr>
<tr>
<td><p><a href="#curhealth">curhealth</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>1</p></td>
<td><p> </p></td>
<td><p>Only used if [creature\_template.regenhealth](creature_template.md#regenhealth) is 0.</p></td>
</tr>
<tr>
<td><p><a href="#curmana">curmana</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>Only used if [creature\_template.regenhealth](creature_template.md#regenhealth) is 0.</p></td>
</tr>
<tr>
<td><p><a href="#movementtype">MovementType</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p>0 No movement, 1 random, 2 path</p></td>
</tr>
<tr>
<td><p><a href="#npcflag">npcflag</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#unit_flags">unit_flags</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr>
<td><p><a href="#dynamicflags">dynamicflags</a></p></td>
<td><p>int(10)</p></td>
<td><p>unsigned</p></td>
<td><p> </p></td>
<td><p>NO</p></td>
<td><p>0</p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
</tbody>
</table>

## Description of the fields

### guid

A unique identifier given to each creature to distinguish one creature from another. Two creatures can NOT have same GUID.

### id

The ID of the [template](creature_template.md#entry) that is used when instantiating this creature.

### map

The ID of the [map](../../dbc/Map.md) that the creature is spawned on.

### zoneId

The ID of the zone that the creature is spawned on. Useful for debugging and filled by the core if worldserver parameter "Calculate.Creature.Zone.Area.Data" is set to 1.

### areaId

The ID of the area that the creature is spawned on. Useful for debugging and filled by the core if worldserver parameter "Calculate.Creature.Zone.Area.Data" is set to 1.

### spawnMask

Controls under which difficulties the creature is spawned. The values are bit-masked, so you can add them together to combine the effects of two or more values.

Example:

4 + 8 = 12

The creature will spawn in only the 10 and 25 man heroic versions of the map that the creature is spawned on.


 

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Value</p></th>
<th><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr>
<td><p>0</p></td>
<td><p>Not spawned</p></td>
</tr>
<tr>
<td><p>1</p></td>
<td><p>Spawned only in 10-man-normal versions of maps (includes maps without a heroic mode)</p></td>
</tr>
<tr>
<td><p>2</p></td>
<td><p>Spawned only in 25-man-normal versions of maps (or heroics pre 3.2)</p></td>
</tr>
<tr>
<td><p>4</p></td>
<td><p>Spawned only in 10-man heroic versions of maps</p></td>
</tr>
<tr>
<td><p>8</p></td>
<td><p>Spawned only in 25-man-heroic versions of maps</p></td>
</tr>
<tr>
<td><p>15</p></td>
<td><p>Spawned in all versions of maps</p></td>
</tr>
</tbody>
</table>

### phaseMask

This is a bit-mask field that describes all the phases that a creature will appear in. Aura 261 determines the phase you can see. For example, if you had this aura <http://www.wowhead.com/?spell=55782>, you would be able to see creatures in phase 2. If you wanted the creature to be visible in both phase 1 and phase 2, you would set the phase-mask to 3.

### modelid

The model ID associated with the creature. Note that two creatures that use the same template can have different models. See [creature\_model\_info](creature_model_info.md) for more information on model-specific characteristics.

Note:

This can be left at 0 and a random model from its assigned models in [creature\_template](creature_template.md) will be assigned by the core.

### equipment\_id

The ID as defined within [creature\_equip\_template](creature_equip_template.md) corresponding to the [entry](creature_template.md). The value essential defines the equip:

-   **-1**: A random equip from the set of equips in [creature\_equip\_template](creature_equip_template.md) will be chosen.
-   **0**: No equipment defined.
-   **1+**: The individual id within creature\_equip\_template.

The equipment ID specified here is only used for the initial spawn. If the equipment is changed via scripts the creature will keep the new equipment on respawn.

If a creature is spawned via GM command `.npc add`, then this value will be set automatically (0 if no equip specified in creature\_equip\_template, otherwise the equipment with [id](creature_equip_template.md#id) 1).

### position\_x

The X position of the creatures spawn point.

### position\_y

The Y position of the creatures spawn point.

### position\_z

The Z position of the creatures spawn point.

### orientation

The orientation of the creatures spawn point. (North = 0.0; South = pi (3.14159))

### spawntimesecs

The respawn time, in seconds, of the creature.

Using a negative value will result in the creature starting out by being dead until a script will respawn it.

### wander\_distance

The maximum distance that the creature may wander from its spawn point. If greater than 0 its [MovementType](#movementtype) has to be 1.

### curhealth

The health that the creature will spawn with. Only used if [creature\_template.regenhealth](creature_template.md#regenhealth) is 0.

### curmana

The mana that the creature will spawn with. Only used if [creature\_template.regenhealth](creature_template.md#regenhealth) is 0.

### MovementType

The movement type associated with the creature. Usually the same as its [MovementType](creature_template.md#movementtype), but it can be different.

### npcflag

Same as [creature\_template.npcflag](creature_template.md#npcflag).

NOTE: A creature.npcflag record will override a [creature\_template.npcflag](creature_template.md#npcflag) record.

### unit\_flags

Same as creature\_template.unit\_flags.

Note:

A creature.unit\_flags record will override a [creature\_template.unit\_flags](creature_template.md#unit_flags) record.

### dynamicflags

Same as creature\_template.dynamicflags.

Note:

A creature.dynamicflags record will override a [creature\_template.dynamicflags](creature_template.md#dynamicflags) record.
