# smart\_scripts

## Structure

<table height="400">
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
<td><p><a href="#entryorguid">entryorguid</a></p></td>
<td><p>int(11)</p></td>
<td><p>signed</p></td>
<td><p>PRI</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#source_type">source_type</a></p></td>
<td><p>tinyint(3)</p></td>
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
<td><p><a href="#id">id</a></p></td>
<td><p>smallint(5)</p></td>
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
<td><p><a href="#link">link</a></p></td>
<td><p>smallint(5)</p></td>
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
<td><p><a href="#event_type">event_type</a></p></td>
<td><p>tinyint(3)</p></td>
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
<td><p><a href="#event_phase_mask">event_phase_mask</a></p></td>
<td><p>smallint(5)</p></td>
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
<td><p><a href="#event_chance">event_chance</a></p></td>
<td><p>tinyint(3)</p></td>
<td><p>unsigned</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>100</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p><a href="#event_flags">event_flags</a></p></td>
<td><p>smallint(5)</p></td>
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
<td><p><a href="#event_type">event_param1</a></p></td>
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
<td><p><a href="#event_type">event_param2</a></p></td>
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
<td><p><a href="#event_type">event_param3</a></p></td>
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
<td><p><a href="#event_type">event_param4</a></p></td>
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
<td><p><a href="#event_type">event_param5</a></p></td>
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
<td><p><a href="#action_type">action_type</a></p></td>
<td><p>tinyint(3)</p></td>
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
<td><p><a href="#action_type">action_param1</a></p></td>
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
<td><p><a href="#action_type">action_param2</a></p></td>
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
<td><p><a href="#action_type">action_param3</a></p></td>
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
<td><p><a href="#action_type">action_param4</a></p></td>
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
<td><p><a href="#action_type">action_param5</a></p></td>
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
<td><p><a href="#action_type">action_param6</a></p></td>
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
<td><p><a href="#target_type">target_type</a></p></td>
<td><p>tinyint(3)</p></td>
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
<td><p><a href="#target_type">target_param1</a></p></td>
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
<td><p><a href="#target_type">target_param2</a></p></td>
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
<td><p><a href="#target_type">target_param3</a></p></td>
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
<td><p><a href="#target_type">target_param4</a></p></td>
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
<td><p><a href="#target_type">target_x</a></p></td>
<td><p>float</p></td>
<td><p><br />
</p></td>
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
<td><p><a href="#target_type">target_y</a></p></td>
<td><p>float</p></td>
<td><p><br />
</p></td>
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
<td><p><a href="#target_type">target_z</a></p></td>
<td><p>float</p></td>
<td><p><br />
</p></td>
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
<td><p><a href="#target_type">target_o</a></p></td>
<td><p>float</p></td>
<td><p><br />
</p></td>
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
<td><p><a href="#comment">comment</a></p></td>
<td><p>text</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>NO</p></td>
<td><p>NULL</p></td>
<td><p><br />
</p></td>
<td><p>Event Comment</p></td>
</tr>
</tbody>
</table>

## Description of the fields

### entryorguid

-   EntryOrGuid &gt; 0: entry of the creature / game object / etc.
-   EntryOrGuid &lt; 0: guid of the creature / game object / etc. (overrides existing SAI for entries)
-   Depends on source\_type.

### source\_type

-   Object type: creature, game object, spell. see table below for values

    | Name                                                                | Value |
    |---------------------------------------------------------------------|-------|
    | SMART\_SCRIPT\_TYPE\_CREATURE                                       | 0     |
    | SMART\_SCRIPT\_TYPE\_GAMEOBJECT                                     | 1     |
    | SMART\_SCRIPT\_TYPE\_AREATRIGGER                                    | 2     |
    | SMART\_SCRIPT\_TYPE\_TIMED\_ACTIONLIST                              | 9     |

### id

-   Incremental id *bound* to each entryorguid & source\_type (0, 1, 2, ...).

### link

-   Simple event linking;
-   Example: if id = 0 and link = 1; id 1 will only be able to occur if id = 0 was triggered (id 1 has to use event\_type SMART\_EVENT\_LINK).
-   Smart\_event to be used.

### event\_phase\_mask

When dealing with phases, *phase IDs* have to be used. There are 31 (30+1) different phases: 1, 2, ... 30 and the default 0.

*Example:* The script is in phase 0 by default - If we want it to go to phase 1, we got two choices:

-   SMART\_ACTION\_INC\_PHASE by 1 or SMART\_ACTION\_SET\_PHASE 1

If the script is in phase 0 and want to skip to phase 2:

-   SMART\_ACTION\_INC\_PHASE by 2 or SMART\_ACTION\_SET\_PHASE 2

If the script is in phase 1 and want to skip to phase 2:

-   SMART\_ACTION\_INC\_PHASE by 1 or SMART\_ACTION\_SET\_PHASE 2

| Phase | Flag      | Hex        |
|-------|-----------|------------|
| 1-30  | 0         | 0x00000000 |
| 1     | 1         | 0x00000001 |
| 2     | 2         | 0x00000002 |
| 3     | 4         | 0x00000004 |
| 4     | 8         | 0x00000008 |
| 5     | 16        | 0x00000010 |
| 6     | 32        | 0x00000020 |
| 7     | 64        | 0x00000040 |
| 8     | 128       | 0x00000080 |
| 9     | 256       | 0x00000100 |
| 10    | 512       | 0x00000200 |
| 11    | 1024      | 0x00000400 |
| 12    | 2048      | 0x00000800 |
| 13    | 4096      | 0x00001000 |
| 14    | 8192      | 0x00002000 |
| 15    | 16384     | 0x00004000 |
| 16    | 32768     | 0x00008000 |
| 17    | 65536     | 0x00010000 |
| 18    | 131072    | 0x00020000 |
| 19    | 262144    | 0x00040000 |
| 20    | 524288    | 0x00080000 |
| 21    | 1048576   | 0x00100000 |
| 22    | 2097152   | 0x00200000 |
| 23    | 4194304   | 0x00400000 |
| 24    | 8388608   | 0x00800000 |
| 25    | 16777216  | 0x01000000 |
| 26    | 33554432  | 0x02000000 |
| 27    | 67108864  | 0x04000000 |
| 28    | 134217728 | 0x08000000 |
| 29    | 268435456 | 0x10000000 |
| 30    | 536870912 | 0x20000000 |

- Event will only be able to occur if creature/GO is in this phase.
- Example: If we want an event to only be able to occure in phase 1 and 4, *event\_phase\_mask* = 1+8 = 9
- The event phase is automatically set to 0 on creature reset (this behaviour can be disabled using SMART_ACTION_SET_EVENT_PHASE_RESET)

### event\_chance

This is the probability of the event to occur as a percentage from 0-100. So, if you want the event to occur roughly half of the time, then set this to 50. 

### event\_flags

<table>
<thead>
<tr class="header">
<th><strong>Name</strong></th>
<th>Flag</th>
<th>Hex</th>
<th>Comment</th>
</tr>
</thead>
<tbody>
<tr>
<td><p>SMART_EVENT_FLAG_NOT_REPEATABLE</p></td>
<td><p>1</p></td>
<td><p>0x01</p></td>
<td><p>Event can not repeat</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_FLAG_DIFFICULTY_0</p></td>
<td><p>2</p></td>
<td><p>0x02</p></td>
<td><p>Event only occurs in normal dungeon</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_FLAG_DIFFICULTY_1</p></td>
<td><p>4</p></td>
<td><p>0x04</p></td>
<td><p>Event only occurs in heroic dungeon</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_FLAG_DIFFICULTY_2</p></td>
<td><p>8</p></td>
<td><p>0x08</p></td>
<td><p>Event only occurs in normal raid</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_FLAG_DIFFICULTY_3</p></td>
<td><p>16</p></td>
<td><p>0x10</p></td>
<td><p>Event only occurs in heroic raid</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_FLAG_RESERVED_5</p></td>
<td><p>32</p></td>
<td><p>0x20</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_FLAG_RESERVED_6</p></td>
<td><p>64</p></td>
<td><p>0x40</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_FLAG_DEBUG_ONLY</p></td>
<td><p>128</p></td>
<td><p>0x80</p></td>
<td><p>Event only occurs in debug build</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_FLAG_DONT_RESET</p></td>
<td><p>256</p></td>
<td><p>0x100</p></td>
<td><p>Event will not reset in SmartScript::OnReset()</p></td>
</tr>
</tbody>
</table>

-   Sets if the event should not repeat or should only happen in a given instance/dungeon difficulty (if applicable);

<!-- -->

-   Values can be added together (bitwise math).

### event\_type

<table height="400">
<thead>
<tr class="header">
<th><p>Name</p></th>
<th><p>Value</p></th>
<th><p>Param1</p></th>
<th><p>Param2</p></th>
<th><p>Param3</p></th>
<th><p>Param4</p></th>
<th><p>Param5</p></th>
<th>Comment</th>
</tr>
</thead>
<tbody>
<tr>
<td><p>SMART_EVENT_UPDATE_IC</p></td>
<td><p>0</p></td>
<td><p>InitialMin</p></td>
<td><p>InitialMax</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td><p>In combat.</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_UPDATE_OOC</p></td>
<td><p>1</p></td>
<td><p>InitialMin</p></td>
<td><p>InitialMax</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td>Out of combat.</td>
</tr>
<tr>
<td><p>SMART_EVENT_HEALTH_PCT</p></td>
<td><p>2</p></td>
<td><p>HPMin%</p></td>
<td><p>HPMax%</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td><p>Health Percentage</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_MANA_PCT</p></td>
<td><p>3</p></td>
<td><p>ManaMin%</p></td>
<td><p>ManaMax%</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td><p>Mana Percentage</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_AGGRO</p></td>
<td><p>4</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Aggro</td>
</tr>
<tr>
<td><p>SMART_EVENT_KILL</p></td>
<td><p>5</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p>Player only (0/1)</p></td>
<td><p>Creature entry (if param3 is 0)</p></td>
<td><p><br />
</p></td>
<td>On Creature Kill</td>
</tr>
<tr>
<td><p>SMART_EVENT_DEATH</p></td>
<td><p>6</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Death</td>
</tr>
<tr>
<td><p>SMART_EVENT_EVADE</p></td>
<td><p>7</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Evade Attack</td>
</tr>
<tr>
<td><p>SMART_EVENT_SPELLHIT</p></td>
<td><p>8</p></td>
<td><p>SpellID (0: any)</p></td>
<td><p>[SpellSchoolMask](#spell-schools)</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td>On creature/gameobject spell hit. For channeled spells this is triggered on channel start, use SMART_EVENT_CHANNEL_FINISHED_TARGET to handle the event after channeling is finished.</td>
</tr>
<tr>
<td><p>SMART_EVENT_RANGE</p></td>
<td><p>9</p></td>
<td><p>MinDist</p></td>
<td><p>MaxDist</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p>Exact</p></td>
<td>On Target In Range; if "Exact" is 1 will use the exact distance ignoring the size of the units. Useful for range checks concerning combat range (exactly 5 yards).</td>
</tr>
<tr>
<td><p>SMART_EVENT_OOC_LOS</p></td>
<td><p>10</p></td>
<td><p>NoHostile</p></td>
<td><p>MaxRange</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td>0/1 Player Only</td>
<td>On Target In Distance Out of Combat</td>
</tr>
<tr>
<td><p>SMART_EVENT_RESPAWN</p></td>
<td><p>11</p></td>
<td><p>type (None = 0, Map = 1, Area = 2)</p></td>
<td><p>MapId</p></td>
<td><p>ZoneId</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature/Gameobject Respawn</td>
</tr>
<tr>
<td><p>SMART_EVENT_TARGET_HEALTH_PCT</p></td>
<td><p>12</p></td>
<td><p>HPMin%</p></td>
<td><p>HPMax%</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td>On victim health percentage</td>
</tr>
<tr>
<td><p>SMART_EVENT_VICTIM_CASTING</p></td>
<td><p>13</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p>Spell id (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Target Casting Spell</td>
</tr>
<tr>
<td><p>SMART_EVENT_FRIENDLY_HEALTH</p></td>
<td><p>14</p></td>
<td><p>HPDeficit</p></td>
<td><p>Radius</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td>On Friendly Health Deficit</td>
</tr>
<tr>
<td><p>SMART_EVENT_FRIENDLY_IS_CC</p></td>
<td><p>15</p></td>
<td><p>Radius</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_FRIENDLY_MISSING_BUFF</p></td>
<td><p>16</p></td>
<td><p>SpellId</p></td>
<td><p>Radius</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td>On Friendly Lost Buff</td>
</tr>
<tr>
<td><p>SMART_EVENT_SUMMONED_UNIT</p></td>
<td><p>17</p></td>
<td><p><a href="creature_template.md#entry">creature_template.entry</a></p> (0 all)</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature/Gameobject Summoned Unit</td>
</tr>
<tr>
<td><p>SMART_EVENT_TARGET_MANA_PCT</p></td>
<td><p>18</p></td>
<td><p>ManaMin%</p></td>
<td><p>ManaMax%</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td>On Target Mana Percentage</td>
</tr>
<tr>
<td><p>SMART_EVENT_ACCEPTED_QUEST</p></td>
<td><p>19</p></td>
<td><p>QuestID (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Target Accepted Quest</td>
</tr>
<tr>
<td><p>SMART_EVENT_REWARD_QUEST</p></td>
<td><p>20</p></td>
<td><p>QuestID (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Target Rewarded Quest</td>
</tr>
<tr>
<td><p>SMART_EVENT_REACHED_HOME</p></td>
<td><p>21</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Reached Home</td>
</tr>
<tr>
<td><p>SMART_EVENT_RECEIVE_EMOTE</p></td>
<td><p>22</p></td>
<td><p><a href="../../dbc/Emotes.md#slash-commands">Slash Command ID</a></p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p></p></td>
<td><p><br />
</p></td>
<td>On Receive Emote.</td>
</tr>
<tr>
<td><p>SMART_EVENT_HAS_AURA</p></td>
<td><p>23</p></td>
<td><p>SpellID</p></td>
<td><p>Stacks</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td>On Creature Has Aura</td>
</tr>
<tr>
<td><p>SMART_EVENT_TARGET_BUFFED</p></td>
<td><p>24</p></td>
<td><p>SpellID</p></td>
<td><p>Stacks</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td>On Target Buffed With Spell</td>
</tr>
<tr>
<td><p>SMART_EVENT_RESET</p></td>
<td><p>25</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>After Combat, On Respawn or Spawn</td>
</tr>
<tr>
<td><p>SMART_EVENT_IC_LOS</p></td>
<td><p>26</p></td>
<td><p>NoHostile</p></td>
<td><p>MaxRange</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td>0/1 Player Only</td>
<td>On Target In Distance In Combat</td>
</tr>
<tr>
<td><p>SMART_EVENT_PASSENGER_BOARDED</p></td>
<td><p>27</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p>seatId (0: all seats; 1: seat 0; 2: seat 1 etc.)</p></td>
<td><p>playerOnly (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_PASSENGER_REMOVED</p></td>
<td><p>28</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p>seatId (0: all seats; 1: seat 0; 2: seat 1 etc.)</p></td>
<td><p>playerOnly (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_CHARMED</p></td>
<td><p>29</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Charmed</td>
</tr>
<tr>
<td><p>SMART_EVENT_CHARMED_TARGET</p></td>
<td><p>30</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Target Charmed</td>
</tr>
<tr>
<td><p>SMART_EVENT_SPELLHIT_TARGET</p></td>
<td><p>31</p></td>
<td><p>SpellId (0: any)</p></td>
<td><p>[SpellSchoolMask](#spell-schools)</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td>On Target Spell Hit</td>
</tr>
<tr>
<td><p>SMART_EVENT_DAMAGED</p></td>
<td><p>32</p></td>
<td><p>MinDmg</p></td>
<td><p>MaxDmg (if 0 any damage which is greater than MinDmg)</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td>On Creature Damaged</td>
</tr>
<tr>
<td><p>SMART_EVENT_DAMAGED_TARGET</p></td>
<td><p>33</p></td>
<td><p>MinDmg</p></td>
<td><p>MaxDmg (if 0 any damage which is greater than MinDmg)</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p><br />
</p></td>
<td>On Target Damaged</td>
</tr>
<tr>
<td><p>SMART_EVENT_MOVEMENTINFORM</p></td>
<td><p>34</p></td>
<td><p>MovementType (0=any)</p></td>
<td><p>PointID (if 0 will trigger on any point)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>ESCORT_MOTION_TYPE = 17, POINT_MOTION_TYPE = 8, WAYPOINT_MOTION_TYPE = 2</td>
</tr>
<tr>
<td><p>SMART_EVENT_SUMMON_DESPAWNED</p></td>
<td><p>35</p></td>
<td><p>Entry</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Summoned Unit Despawned</td>
</tr>
<tr>
<td><p>SMART_EVENT_CORPSE_REMOVED</p></td>
<td><p>36</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On creature corpse removed or creature despawned</td>
</tr>
<tr>
<td><p>SMART_EVENT_AI_INIT</p></td>
<td><p>37</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_DATA_SET</p></td>
<td><p>38</p></td>
<td><p>Field</p></td>
<td><p>Value</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td>On Creature/Gameobject Data Set, Can be used with SMART_ACTION_SET_DATA</td>
</tr>
<tr>
<td><p>SMART_EVENT_WAYPOINT_START</p></td>
<td><p>39</p></td>
<td><p>PointId (0 any)</p></td>
<td><p>pathId (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Waypoint ID Started</td>
</tr>
<tr>
<td><p>SMART_EVENT_WAYPOINT_REACHED</p></td>
<td><p>40</p></td>
<td><p>PointId (0 any)</p></td>
<td><p>pathId (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Waypoint ID Reached</td>
</tr>
<tr>
<td><p>SMART_EVENT_AREATRIGGER_ONTRIGGER</p></td>
<td><p>46</p></td>
<td><p>TriggerId (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_TEXT_OVER</p></td>
<td><p>52</p></td>
<td><p><a href="creature_text.md#groupid">creature_text.GroupID</a></p></td>
<td><p><a href="creature.md#id">creature.id</a> (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On TEXT_OVER Event Triggered After SMART_ACTION_TALK</td>
</tr>
<tr>
<td><p>SMART_EVENT_RECEIVE_HEAL</p></td>
<td><p>53</p></td>
<td><p>MinHeal</p></td>
<td><p>MaxHeal (if 0 any heal which is greater than MinHeal)</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td>On Creature Received Healing</td>
</tr>
<tr>
<td><p>SMART_EVENT_JUST_SUMMONED</p></td>
<td><p>54</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Just spawned</td>
</tr>
<tr>
<td><p>SMART_EVENT_WAYPOINT_PAUSED</p></td>
<td><p>55</p></td>
<td><p>PointId (0 any)</p></td>
<td><p>pathID (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Paused at Waypoint ID</td>
</tr>
<tr>
<td><p>SMART_EVENT_WAYPOINT_RESUMED</p></td>
<td><p>56</p></td>
<td><p>PointId (0 any)</p></td>
<td><p>pathID (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Resumed after Waypoint ID</td>
</tr>
<tr>
<td><p>SMART_EVENT_WAYPOINT_STOPPED</p></td>
<td><p>57</p></td>
<td><p>PointId (0 any)</p></td>
<td><p>pathID (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Stopped On Waypoint ID</td>
</tr>
<tr>
<td><p>SMART_EVENT_WAYPOINT_ENDED</p></td>
<td><p>58</p></td>
<td><p>PointId (0 any)</p></td>
<td><p>pathID (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature Waypoint Path Ended</td>
</tr>
<tr>
<td><p>SMART_EVENT_TIMED_EVENT_TRIGGERED</p></td>
<td><p>59</p></td>
<td><p>Id</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_UPDATE</p></td>
<td><p>60</p></td>
<td><p>InitialMin</p></td>
<td><p>InitialMax</p></td>
<td><p>RepeatMin</p></td>
<td><p>RepeatMax</p></td>
<td><p>spawnedGOonly (0/1)</p></td>
<td><p>If "spawnedGOonly" is set and the script owner is a gameobject the event is only triggered if the GO is currently spawned.</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_LINK</p></td>
<td><p>61</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>Used to link together multiple events as a chain of events.</td>
</tr>
<tr>
<td><p>SMART_EVENT_GOSSIP_SELECT</p></td>
<td><p>62</p></td>
<td><p><a href="gossip_menu_option.md#menuid">gossip_menu_option.MenuID</a></p></td>
<td><p><a href="gossip_menu_option.md#optionid">gossip_menu_option.OptionID</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On gossip clicked (<a href="gossip_menu_option.md">gossip_menu_option</a>).</td>
</tr>
<tr>
<td><p>SMART_EVENT_GOSSIP_HELLO</p></td>
<td><p>64</p></td>
<td><p>filter (0/1/2)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Right-Click Creature/Gameobject that have gossip enabled. The parameter "filter" is only used for GOs: execute action according to the value: 0: always, 1: only on GossipHello, 2: only on ReportUse</td>
</tr>
<tr>
<td><p>SMART_EVENT_FOLLOW_COMPLETED</p></td>
<td><p>65</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><div class="content-wrapper">
<p>SMART_EVENT_UNUSED_66</p>
</div></td>
<td><p>66</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>UNUSED</td>
</tr>
<tr>
<td><p>SMART_EVENT_IS_BEHIND_TARGET</p></td>
<td><p>67</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On Creature is behind target.</td>
</tr>
<tr>
<td><p>SMART_EVENT_GAME_EVENT_START</p></td>
<td><p>68</p></td>
<td><p><a href="game_event.md#evententry">game_event.eventEntry</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On <a href="game_event.md">game_event</a> started. Do not use directly with "summon" actions, use timed action lists instead.</td>
</tr>
<tr>
<td><p>SMART_EVENT_GAME_EVENT_END</p></td>
<td><p>69</p></td>
<td><p><a href="game_event.md#evententry">game_event.eventEntry</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On <a href="game_event.md">game_event</a> ended. Do not use directly with "summon" actions, use timed action lists instead.</td>
</tr>
<tr>
<td><p>SMART_EVENT_GO_STATE_CHANGED</p></td>
<td><p>70</p></td>
<td><p>State (0 - GO_NOT_READY, 1 - GO_READY, 2 - GO_ACTIVATED, 3 - GO_JUST_DEACTIVATED)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_GO_EVENT_INFORM</p></td>
<td><p>71</p></td>
<td><p>EventId</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_EVENT_ACTION_DONE</p></td>
<td><p>72</p></td>
<td><p>EventId</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td>SMART_EVENT_ON_SPELLCLICK</td>
<td>73</td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td>SMART_EVENT_FRIENDLY_HEALTH_PCT</td>
<td>74</td>
<td><p>minHpPct</p></td>
<td><p>maxHpPct</p></td>
<td><p>repeatMin</p></td>
<td><p>repeatMax</p></td>
<td><p>radius</p></td>
<td><p>The parameter "radius" is only used if the target type is "SMART_TARGET_ACTION_INVOKER". Otherwise the health of all specified targets will be checked for the event to occur (the triggered action will use all specified targets).</p></td>
</tr>
<tr>
<td>SMART_EVENT_DISTANCE_CREATURE</td>
<td>75</td>
<td>database guid</td>
<td>database entry</td>
<td>distance</td>
<td>repeat interval (ms)</td>
<td><p>alive state (0 - Ignore alive state, 1 - Alive, 2 - Dead)</p></td>
<td><p>On creature guid OR any instance of creature entry is within distance.</p></td>
</tr>
<tr>
<td>SMART_EVENT_DISTANCE_GAMEOBJECT</td>
<td>76</td>
<td>database guid</td>
<td>database entry</td>
<td>distance</td>
<td>repeat interval (ms)</td>
<td><p>GO state (0 - Ignore GO state, 1 - Active, 2 - Ready, 3 - Active alternative)</p></td>
<td><p>On gameobject guid OR any instance of gameobject entry is within distance.</p></td>
</tr>
<tr>
<td>SMART_EVENT_COUNTER_SET</td>
<td>77</td>
<td>counterID</td>
<td>value</td>
<td>cooldownMin</td>
<td>cooldownMax</td>
<td><p><br />
</p></td>
<td>If the value of specified counterID is equal to a specified value</td>
</tr>
<tr>
<td>SMART_EVENT_FOLLOW_TARGET_LOST</td>
<td>231</td>
<td>range (0: unlimited, just check if target exists on the map)</td>
<td>heartbeat in ms (if 0 use 5000)</td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On follow target out of range or not on the map anymore; heartbeat determines how often the check is made (default every 5 seconds)</td>
</tr>
<tr>
<td>SMART_EVENT_KILL_DELAY_STARTED</td>
<td>232</td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On kill delay started (see SMART_ACTION_SET_KILL_DELAY).</td>
</tr>
<tr>
<td><p>SMART_EVENT_SPELL_CAST</p></td>
<td><p>233</p></td>
<td><p>SpellID (0: any)</p></td>
<td><p>[SpellSchoolMask](#spell-schools)</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td>On creature spell casting finished.</td>
</tr>
<tr>
<td><p>SMART_EVENT_SPELL_FAILED</p></td>
<td><p>234</p></td>
<td><p>SpellID (0: any)</p></td>
<td><p>[SpellSchoolMask](#spell-schools)</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td>On creature spell casting failed.</td>
</tr>
<tr>
<td><p>SMART_EVENT_SPELL_START</p></td>
<td><p>235</p></td>
<td><p>SpellID (0: any)</p></td>
<td><p>[SpellSchoolMask](#spell-schools)</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td>On creature spell casting started.</td>
</tr>
<tr>
<td><p>SMART_EVENT_CHANNEL_FINISHED</p></td>
<td><p>236</p></td>
<td><p>SpellID (0: any)</p></td>
<td><p>[SpellSchoolMask](#spell-schools)</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td>On creature spell channeling finished.</td>
</tr>
<tr>
<td><p>SMART_EVENT_FLEE_FINISHED</p></td>
<td><p>237</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>On creature finishes fleeing (e.g. caused by spell, SMART_ACTION_FLEE_FOR_ASSIST or SMART_ACTION_FLEE).</td>
</tr>
<tr>
<td><p>SMART_EVENT_CHANNEL_FINISHED_TARGET</p></td>
<td><p>238</p></td>
<td><p>SpellID (0: any)</p></td>
<td><p>[SpellSchoolMask](#spell-schools)</p></td>
<td><p>CooldownMin</p></td>
<td><p>CooldownMax</p></td>
<td><p><br />
</p></td>
<td>On spell channeling finished on this creature as target (caster is used as invoker here).</td>
</tr>
</tbody>
</table>

### action\_type

<table height="400">
<thead>
<tr class="header">
<th><p>Name</p></th>
<th><p>Value</p></th>
<th><p>Param1</p></th>
<th><p>Param2</p></th>
<th><p>Param3</p></th>
<th><p>Param4</p></th>
<th><p>Param5</p></th>
<th><p>Param6</p></th>
<th><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr>
<td><p>SMART_ACTION_NONE</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Do nothing</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_TALK</p></td>
<td><p>1</p></td>
<td><p><a href="creature_text.md#groupid">creature_text.GroupID</a></p></td>
<td><p>Duration to wait before SMART_EVENT_TEXT_OVER is triggered.</p></td>
<td>0 It will try to trigger talk of the target
<p>1 Set target as talk target (used for $vars in texts and whisper target)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Param2 in Milliseconds.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_FACTION</p></td>
<td><p>2</p></td>
<td><p><a href="../../dbc/FactionTemplate.md">FactionID</a> (or 0 for default)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Sets a faction for creature. The faction is automatically reset on respawn.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_MORPH_TO_ENTRY_OR_MODEL</p></td>
<td><p>3</p></td>
<td><p><a href="creature_template.md#entry">creature_template.entry</a>(param1)</p></td>
<td><p><a href="creature_template.md#modelidx">creature_template.modelidx</a>(param2)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Take DisplayID of creature (param1) OR Turn to DisplayID (param2) OR Both = 0 for Demorph</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SOUND</p></td>
<td><p>4</p></td>
<td><p>SoundId</p></td>
<td><p>onlySelf (1: only sends the sound to targeted players, 0: sends the sound to everyone in visibility range of the target)</p></td>
<td><p>distance (1: the sound fades with increasing distance to the target, 0: the sound is played at full volume no matter the distance)</p></td>
<td><p>type</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Play Sound. Type can be one of these values:<br />
0: Play sound for the specified target(s)<br />
1: Play sound for all players in the entire zone<br />
2: Play sound for all players in the area</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_PLAY_EMOTE</p></td>
<td><p>5</p></td>
<td><p><a href="../../dbc/Emotes.md">EmoteId</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Play Emote</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_FAIL_QUEST</p></td>
<td><p>6</p></td>
<td><p>QuestID</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Fail Quest of Target</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_OFFER_QUEST</p></td>
<td><p>7</p></td>
<td><p><a href="quest_template.md#id">quest_template.id</a></p></td>
<td><p>directAdd (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Add Quest to Target</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_REACT_STATE</p></td>
<td><p>8</p></td>
<td><p><a href="#react-states">ReactState</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>React State. Can be Passive (0), Defensive (1), Aggressive (2).</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ACTIVATE_GOBJECT</p></td>
<td><p>9</p></td>
<td><p>alternative (0/1)</p></td>
<td><p>use instead of activate (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Activate object. If "use" is 1 the GO is used by the creature (e.g. sitting on a chair). If "alternative" is 1 set GO_STATE_ACTIVE_ALTERNATIVE instead of GO_STATE_ACTIVE (only if "use" is 0).</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RANDOM_EMOTE</p></td>
<td><p>10</p></td>
<td><p><a href="../../dbc/Emotes.md">EmoteId1</a></p></td>
<td><p><a href="../../dbc/Emotes.md">EmoteId2</a></p></td>
<td><p><a href="../../dbc/Emotes.md">EmoteId3</a></p></td>
<td><p><a href="../../dbc/Emotes.md">EmoteId4</a></p></td>
<td><p><a href="../../dbc/Emotes.md">EmoteId5</a></p></td>
<td><p><a href="../../dbc/Emotes.md">EmoteId6</a></p></td>
<td><p>Play Random Emote</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CAST</p></td>
<td><p>11</p></td>
<td><p>SpellId</p></td>
<td><p><a href="#cast-flags">castFlags</a></p></td>
<td><p>limitTargets (0 = all targets)</p></td>
<td><p>forceRepeatOnRangeFail</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Cast Spell ID at Target(s); if "forceRepeatOnRangeFail" is set to 1 recalculate the event timer if the spell fails due to the range check (repeat 500ms later until the range check is successful); only works for events with timers, e.g. "SMART_EVENT_UPDATE_IC"</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SUMMON_CREATURE</p></td>
<td><p>12</p></td>
<td><p>creature_template.entry</p></td>
<td><p><a href="#summon-types">Summon type</a></p></td>
<td><p>duration in ms</p></td>
<td><p>attackType (0/1/2/3)</p></td>
<td><p>randomMinDist</p></td>
<td><p>randomMaxDist</p></td>
<td><p>Summon creature; attackType 1: attack target, 2: attack invoker, 3: attack script owner; if an entity is specified as target and also coordinates are set (target x,y,z) those coordinates are handled as offset from the target's position (the z offset is set to terrain height if not specified); if randomMaxDist is specified, calculate a random point within randomMinDist and randomMaxDist from the target to summon the creature</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_THREAT_SINGLE_PCT</p></td>
<td><p>13</p></td>
<td><p>Threat% inc</p></td>
<td><p>Threat% dec</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Change threat percentage for the specified targets</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_THREAT_ALL_PCT</p></td>
<td><p>14</p></td>
<td><p>Threat% inc</p></td>
<td><p>Threat% dec</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Change threat percentage for all creatures on the current threat list</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CALL_AREAEXPLOREDOREVENTHAPPENS</p></td>
<td><p>15</p></td>
<td><p><a href="quest_template.md#id">quest_template.id</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Complete the specified quest for all targeted players</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_EMOTE_STATE</p></td>
<td><p>17</p></td>
<td><p><a href="../../dbc/Emotes.md">EmoteId</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Play Emote Continuously</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_UNIT_FLAG</p></td>
<td><p>18</p></td>
<td><p>(may be more than one field OR'd together)</p></td>
<td><p>type</p>
<p>If false set <a href="creature_template.md#unit_flags">creature_template.unit_flags</a></p>
<p>If true set <a href="creature_template.md#unit_flags2">creature_template.unit_flags2</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Can set Multi-able flags at once</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_UNIT_FLAG</p></td>
<td><p>19</p></td>
<td><p>(may be more than one field OR'd together)</p></td>
<td><p>type</p>
<p>If false set  <a href="creature_template.md#unit_flags">creature_template.unit_flags</a></p>
<p>If true set <a href="creature_template.md#unit_flags2">creature_template.unit_flags2</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Can Remove Multi-able flags at once</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_AUTO_ATTACK</p></td>
<td><p>20</p></td>
<td><p>AllowAttackState (0 = Stop attack, anything else means continue attacking)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Stop or Continue Automatic Attack.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ALLOW_COMBAT_MOVEMENT</p></td>
<td><p>21</p></td>
<td><p>AllowCombatMovement (0 = Stop combat based movement, anything else continue attacking)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Allow or Disable Combat Movement</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_EVENT_PHASE</p></td>
<td><p>22</p></td>
<td><p><a href="#event_phase_mask">event_phase_mask</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Set event phase 0-12; the event phase is set to 0 on reset of the script owner (e.g. after combat, can be disabled using SMART_ACTION_SET_EVENT_PHASE_RESET)</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_INC_EVENT_PHASE</p></td>
<td><p>23</p></td>
<td><p>Increment</p></td>
<td><p>Decrement</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Set param1 OR param2 (not both); Value 0 has no effect; the event phase is set to 0 on reset (can be disabled using SMART_ACTION_SET_EVENT_PHASE_RESET)</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_EVADE</p></td>
<td><p>24</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Evade Incoming Attack</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_FLEE_FOR_ASSIST</p></td>
<td><p>25</p></td>
<td><p>talk</p></td>
<td><p>radius (0: use default)</p></td>
<td><p>call assist radius (0: use default)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If you want the fleeing NPC to say '%s attempts to run away in fear', use 1 as "talk" parameter, 0 for no message. If >1 subtract 2 and use the result as <a href="creature_text.md#groupid">creature_text.GroupID</a>.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CALL_GROUPEVENTHAPPENS</p></td>
<td><p>26</p></td>
<td><p><a href="quest_template.md#id">quest_template.id</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Complete the specified quest for all targeted players and their groups</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_COMBAT_STOP</p></td>
<td><p>27</p></td>
<td><p>DeleteThreatList (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVEAURASFROMSPELL</p></td>
<td><p>28</p></td>
<td><p>Spellid (0 removes all auras)</p></td>
<td><p>charges (0 removes aura)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_FOLLOW</p></td>
<td><p>29</p></td>
<td><p>Distance</p></td>
<td><p>Angle</p></td>
<td><p>End NPC <a href="creature_template.md#entry">creature_template.entry</a></p></td>
<td><p>credit</p></td>
<td><p>creditType (0 monsterkill, 1 event)</p></td>
<td><p>aliveState End NPC (0: alive, 1: dead)</p></td>
<td><p>Follow the target; stop following if target is SMART_TARGET_NONE or SMART_TARGET_SELF; angle is counter-clockwise, 0 means in front of the target; if lower or equal to 6 use as radian, otherwise use as degrees; as only integer values are allowed if specified as radian the degrees would be as follows:<br />
1: ca. 57.3 degrees<br />
2: ca. 114.6 degrees<br />
3: ca. 171.9 degrees<br />
4: ca. 229.2 degrees<br />
5: ca. 286.5 degrees<br />
6: ca. 343.8 degrees<br />
Important note: Ensure that the home position is saved regularly while following the target (use "SMART_ACTION_SET_HOME_POS" for this) or else the creature won't fight correctly as it conflicts with its evade mode.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RANDOM_PHASE</p></td>
<td><p>30</p></td>
<td><p><a href="#event_phase_mask">event_phase_mask</a> 1</p></td>
<td><p><a href="#event_phase_mask">event_phase_mask</a> 2</p></td>
<td><p><a href="#event_phase_mask">event_phase_mask</a> 3</p></td>
<td><p><a href="#event_phase_mask">event_phase_mask</a> 4</p></td>
<td><p><a href="#event_phase_mask">event_phase_mask</a> 5</p></td>
<td><p><a href="#event_phase_mask">event_phase_mask</a> 6</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RANDOM_PHASE_RANGE</p></td>
<td><p>31</p></td>
<td><p><a href="#event_phase_mask">event_phase_mask</a> minimum</p></td>
<td><p><a href="#event_phase_mask">event_phase_mask</a> maximum</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RESET_GOBJECT</p></td>
<td><p>32</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Reset Gameobject</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CALL_KILLEDMONSTER</p></td>
<td><p>33</p></td>
<td><p><a href="creature_template.md#entry">creature_template.entry</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>This is the ID from <a href="quest_template.md#requirednpcorgo">quest_template.RequiredNpcOrGo</a></p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_INST_DATA</p></td>
<td><p>34</p></td>
<td><p>Field</p></td>
<td><p>Data</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Set Instance Data</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_INST_DATA64</p></td>
<td><p>35</p></td>
<td><p>Field</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Set Instance Data uint64</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_UPDATE_TEMPLATE</p></td>
<td><p>36</p></td>
<td><p><a href="creature_template.md#entry">creature_template.entry</a></p></td>
<td><p>Update Level</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Updates creature_template to given entry (the AI will stay the same, but stats, creature texts etc. are taken from the new entry)</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_DIE</p></td>
<td><p>37</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Kill Target</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_IN_COMBAT_WITH_ZONE</p></td>
<td><p>38</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CALL_FOR_HELP</p></td>
<td><p>39</p></td>
<td><p>Radius in yards that other creatures must be to acknowledge the call for help.</p></td>
<td><p>0/1 (say "calls for help" text)</p></td>
<td><p>0/1 (force assistance from neutral / defensive NPCs nearby)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If you want the NPC to say '%s calls for help!' use 1 on param2, 0 for no message.<br />
If param3 is set to 1 the call forces neutral / defensive NPCs nearby to also attack the player;
if set to 0 only aggressive / hostile NPCs attack</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_SHEATH</p></td>
<td><p>40</p></td>
<td><p>Sheath (0-unarmed, 1-melee, 2-ranged)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_FORCE_DESPAWN</p></td>
<td><p>41</p></td>
<td><p>Despawn timer &quot;ms&quot;</p></td>
<td><p>despawnMinionId</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Despawn the target after the specified time in ms if it is a creature (this overrides any previous despawn action). If the target is a gameobject it is deleted at once, the timer is ignored in this case. If despawnMinionId > 0 despawns all minions of the target with the specified creature_template.entry.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_INVINCIBILITY_HP_LEVEL</p></td>
<td><p>42</p></td>
<td><p>flat hp value</p></td>
<td><p>percent hp value</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If you use both params, only percent will be used.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_MOUNT_TO_ENTRY_OR_MODEL</p></td>
<td><p>43</p></td>
<td><p>creature_template.entry</p></td>
<td><p><a href="creature_template.md#modelidx">creature_template.modelidx</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Mount to Creature Entry (param1) OR Mount to Creature Display (param2) Or both = 0 for Unmount</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_INGAME_PHASE_MASK</p></td>
<td><p>44</p></td>
<td><p><a href="creature.md#phasemask">creature.phaseMask</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_DATA</p></td>
<td><p>45</p></td>
<td><p>Field</p></td>
<td><p>Data</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Set Data For Target, can be used with SMART_EVENT_DATA_SET</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_MOVE_FORWARD</p></td>
<td><p>46</p></td>
<td><p>distance</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>move self forward for the specified distance (point movement)</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_VISIBILITY</p></td>
<td><p>47</p></td>
<td><p>0/1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Makes creature Visible = 1  or  Invisible = 0</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_ACTIVE</p></td>
<td><p>48</p></td>
<td><p>0/1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If a creature or GO is set active it will stay active even if no player is near. Take care, though, as it needs additional ressources (CPU/RAM) to keep them active (other objects/creatures nearby stay active). If a creature dies the active state is automatically turned off; it can be turned on again using the event SMART_EVENT_DEATH if the corpse should also stay active, e.g. to trigger actions via SMART_EVENT_CORPSE_REMOVED. If the active state is turned on using the events SMART_EVENT_RESPAWN and SMART_EVENT_DEATH the creature will stay active forever.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ATTACK_START</p></td>
<td><p>49</p></td>
<td><p>targetType</p></td>
<td><p>targetParam1</p></td>
<td><p>targetParam2</p></td>
<td><p>targetParam3</p></td>
<td><p>targetParam4</p></td>
<td><p><br />
</p></td>
<td><p>Start attacking the target. If more than one target exists attack a random one. If targetType >0 the action is executed for each selected target instead of the script owner.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SUMMON_GO</p></td>
<td><p>50</p></td>
<td><p><a href="gameobject_template.md#entry">gameobject_template.entry</a></p></td>
<td><p>De-spawn time in seconds.</p></td>
<td><p>targetSummon (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Spawns Gameobject, use target_type to set spawn position; if an entity is specified as target and also coordinates are set (target x,y,z) those coordinates are handled as offset from the target's position; if targetSummon is 1 then the target will summon the GO on the position of the actor</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_KILL_UNIT</p></td>
<td><p>51</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Kills Creature.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ACTIVATE_TAXI</p></td>
<td><p>52</p></td>
<td><p>TaxiID</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Sends player to flight path. You have to be close to Flight Master, which gives Taxi ID you need.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_WP_START</p></td>
<td><p>53</p></td>
<td><p>0 = walk / 1 = run</p></td>
<td><p><a href="waypoints.md#entry">waypoints.entry</a></p></td>
<td><p>canRepeat</p></td>
<td><p><a href="quest_template.md#id">quest_template.id</a></p></td>
<td><p>despawntime</p></td>
<td><p><a href="#react-states">reactState</a></p></td>
<td><p>Creature starts Waypoint Movement. Use <a href="waypoints.md#entry">waypoints</a> table to create movement. Uses the target as escort if it consists of players (stored in the reserved target list SMART_ESCORT_TARGETS).</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_WP_PAUSE</p></td>
<td><p>54</p></td>
<td><p>time (in ms)</p></td>
<td><p>onlyOOC (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Creature pauses its waypoint movement for the given time. If onlyOOC is set the pause timer is only updated if the creature is OOC. If the movement is already paused the pause timer is updated.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_WP_STOP</p></td>
<td><p>55</p></td>
<td><p>despawnTime</p></td>
<td><p><a href="quest_template.md#id">quest_template.id</a></p></td>
<td><p>fail (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Creature stops its Waypoint Movement.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ADD_ITEM</p></td>
<td><p>56</p></td>
<td><p><a href="item_template.md#entry">item_template.entry</a></p></td>
<td><p>count</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Adds item(s) to player.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_ITEM</p></td>
<td><p>57</p></td>
<td><p><a href="item_template.md#entry">item_template.entry</a></p></td>
<td><p>count</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Removes item(s) from player.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_RUN</p></td>
<td><p>59</p></td>
<td><p>0 = Off / 1 = On</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_FLY</p></td>
<td><p>60</p></td>
<td><p>fly (0/1)</p></td>
<td><p>speed</p></td>
<td><p>disable gravity (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Only works for creatures with inhabit air or the flag "CREATURE_FLAG_EXTRA_NO_MOVE_FLAGS_UPDATE"</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_SWIM</p></td>
<td><p>61</p></td>
<td><p>0 = Off / 1 = On</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_TELEPORT</p></td>
<td><p>62</p></td>
<td><p><a href="../../dbc/Map.md">MapID</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Continue this action with the TARGET_TYPE column. Use any target_type (except 0), and use target_x, target_y, target_z, target_o as the coordinates</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_COUNTER</p></td>
<td><p>63</p></td>
<td><p>counterID</p></td>
<td><p>value</p></td>
<td><p>reset (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If reset is 0 the counter with the specified ID is increased by the given value; if reset is 1 the counter is set to the value; the counters are cleared on reset of the script owner (e.g. after combat, can be disabled using SMART_ACTION_SET_COUNTER_RESET)</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_STORE_TARGET_LIST</p></td>
<td><p>64</p></td>
<td><p>varID</p></td>
<td><p>varID range</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Stores the targets in a list with the specified "varID". If "varID range" is set each of the targets will be stored in a separate "varID", beginning with "varID" until (and including) "varID range". The ID 16777215 reserved for SMART_ESCORT_TARGETS (see SMART_ACTION_WP_START)  and not allowed to be used here.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_WP_RESUME</p></td>
<td><p>65</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Creature continues in its Waypoint Movement.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_ORIENTATION</p></td>
<td><p>66</p></td>
<td><p>quickChange</p></td>
<td><p>targetType</p></td>
<td><p>targetParam1</p></td>
<td><p>targetParam2</p></td>
<td><p>targetParam3</p></td>
<td><p>targetParam4</p></td>
<td><p>Depends on the script target. If SMART_TARGET_SELF, facing will be the same as in HomePosition, For SMART_TARGET_POSITION you need to set target_o : 0 = North, West = 1.5, South = 3, East = 4.5<br><br>
quickChange 1 forces the creature to quickly change its orientation (useful if this smart action is combined with SMART_ACTION_WP_PAUSE)<br><br>
If targetType >0 the action is executed for each selected target instead of the script owner.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CREATE_TIMED_EVENT</p></td>
<td><p>67</p></td>
<td><p>id</p></td>
<td><p>InitialMin</p></td>
<td><p>InitialMax</p></td>
<td><p>RepeatMin(only if it repeats)</p></td>
<td><p>RepeatMax(only if it repeats)</p></td>
<td><p>chance</p></td>
<td><p>It is possible to create multiple timed events with the same ID, but to remove all of them it is necessary to call SMART_ACTION_REMOVE_TIMED_EVENT multiple times. Important: The timer will persist even after respawn.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_PLAYMOVIE</p></td>
<td><p>68</p></td>
<td><p>entry</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_MOVE_TO_POS</p></td>
<td><p>69</p></td>
<td><p>PointId</p></td>
<td><p>isTransport (0 or 1)</p></td>
<td><p>controlled (0 or 1)</p></td>
<td><p>ContactDistance</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>PointId is called by SMART_EVENT_MOVEMENTINFORM. Continue this action with the TARGET_TYPE column. Use any target_type, and use target_x, target_y, target_z as the coordinates; if an entity is specified as target and also coordinates are set (target x,y,z) those coordinates are handled as offset from the target's position (max. 50 absolute offset allowed). If ContactDistance > 0 and also target_o is set use target_o as distance, otherwise just use ContactDistance.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RESPAWN_TARGET</p></td>
<td><p>70</p></td>
<td><p>Despawntime in seconds (only for GOs which start despawned; for creature: 0: respawn only if dead; >0: force respawn even if alive)</p></td>
<td><p>saveRespawnTime (creatures only; 0: ignore, just respawn target; 1/2: just enable/disable save respawn time, target is not respawned)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>The respawn time is not saved for normal creatures, only elite, boss etc.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_EQUIP</p></td>
<td><p>71</p></td>
<td><p><a href="creature_equip_template.md#id">creature_equip_template.ID</a></p></td>
<td><p>Slotmask</p></td>
<td><p>Slot1 (<a href="item_template.md#entry">item_template.entry</a>)</p></td>
<td><p>Slot2 (<a href="item_template.md#entry">item_template.entry</a>)</p></td>
<td><p>Slot3 (<a href="item_template.md#entry">item_template.entry</a>)</p></td>
<td><p><br />
</p></td>
<td><p>only slots with mask set will be sent to client, bits are 1, 2, 4, leaving mask 0 is defaulted to mask 7 (send all), Slots1-3 are only used if no Param1 is set</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CLOSE_GOSSIP</p></td>
<td><p>72</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>Closes gossip window.</td>
</tr>
<tr>
<td><p>SMART_ACTION_TRIGGER_TIMED_EVENT</p></td>
<td><p>73</p></td>
<td><p>id</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>It is not necessary to create the timed event beforehand.</td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_TIMED_EVENT</p></td>
<td><p>74</p></td>
<td><p>id</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ADD_AURA</p></td>
<td><p>75</p></td>
<td><p>SpellId</p></td>
<td><p>stacks (if 0 just apply the aura once)</p></td>
<td><p>notPresent</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Adds aura to unit(s). Use e.g. target_type 17 to make AoE aura. If "notPresent" is set the aura is not applied if it is already present on the target.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_OVERRIDE_SCRIPT_BASE_OBJECT</p></td>
<td><p>76</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>WARNING: CAN CRASH CORE, do not use if you dont know what you are doing</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RESET_SCRIPT_BASE_OBJECT</p></td>
<td><p>77</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CALL_SCRIPT_RESET</p></td>
<td><p>78</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_RANGED_MOVEMENT</p></td>
<td><p>79</p></td>
<td><p>attackDistance</p></td>
<td><p>attackAngle</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Sets movement to follow at a specific range to the target.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CALL_TIMED_ACTIONLIST</p></td>
<td><p>80</p></td>
<td><p>EntryOrGuid * 100 (<a href="#entryorguid">entryorguid</a> with 00 added after the entry, or 01, 02, 03 etc. for multiple action lists)</p></td>
<td><p>timer update type(0 OOC, 1 IC, 2 ALWAYS)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If an action list is already running it is overwritten with the new one. It is not possible to call a timed action list from within a timed action list. A running action list is cancelled on death.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_NPC_FLAG</p></td>
<td><p>81</p></td>
<td><p><a href="creature_template.md#npcflag">creature_template.npcflag</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Set NPC flags, overwriting the existing value. The NPC flags are reset automatically on respawn.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ADD_NPC_FLAG</p></td>
<td><p>82</p></td>
<td><p><a href="creature_template.md#npcflag">creature_template.npcflag</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>Add NPC flags to the existing value. If value 0 is used the NPC flags are reset to the value specified in the creature template. The NPC flags are reset automatically on respawn.</td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_NPC_FLAG</p></td>
<td><p>83</p></td>
<td><p><a href="creature_template.md#npcflag">creature_template.npcflag</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>Remove NPC flags from the existing value. If value 0 is used all NPC flags are removed. The NPC flags are reset automatically on respawn.</td>
</tr>
<tr>
<td><p>SMART_ACTION_SIMPLE_TALK</p></td>
<td><p>84</p></td>
<td><p><a href="creature_text.md#groupid">creature_text.GroupID</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Makes a player say text. SMART_EVENT_TEXT_OVER is not triggered and whispers can not be used.</p></td>
</tr>
<tr>
<td>SMART_ACTION_INVOKER_CAST</td>
<td><p>85</p></td>
<td><p>SpellID</p></td>
<td><p><a href="#cast-flags">castFlags</a></p></td>
<td><p>limitTargets (0 = all targets)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>if avaliable, last used invoker will cast spellId with castFlags on targets (warning: TC 3.3.5 uses another action here: SMART_ACTION_SELF_CAST)</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CROSS_CAST</p></td>
<td><p>86</p></td>
<td><p>SpellID</p></td>
<td><p><a href="#cast-flags">castFlags</a></p></td>
<td><p>CasterTargetType (caster is selected here, use it as target_type)</p></td>
<td><p>CasterTarget (target_param1)</p></td>
<td><p>CasterTarget (target_param2)</p></td>
<td><p>CasterTarget (target_param3)</p></td>
<td><p>This action is used to make selected caster (in CasterTargetType) to cast spell. Actual target is entered in target_type as normally.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CALL_RANDOM_TIMED_ACTIONLIST</p></td>
<td><p>87</p></td>
<td><p>EntryOrGuid 1 (<a href="#entryorguid">entryorguid</a> * 100 + n)</p></td>
<td><p>EntryOrGuid 2 (<a href="#entryorguid">entryorguid</a> * 100 + n)</p></td>
<td><p>EntryOrGuid 3 (<a href="#entryorguid">entryorguid</a> * 100 + n)</p></td>
<td><p>EntryOrGuid 4 (<a href="#entryorguid">entryorguid</a> * 100 + n)</p></td>
<td><p>EntryOrGuid 5 (<a href="#entryorguid">entryorguid</a> * 100 + n)</p></td>
<td><p>EntryOrGuid 6 (<a href="#entryorguid">entryorguid</a> * 100 + n)</p></td>
<td><p>Will select one entry from the ones provided. 0 is ignored. The timer will update IC and OOC. If an action list is already running it is overwritten with the new one. It is not possible to call a timed action list from within a timed action list.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CALL_RANDOM_RANGE_TIMED_ACTIONLIST</p></td>
<td><p>88</p></td>
<td><p>EntryOrGuid 1 (<a href="#entryorguid">entryorguid</a> * 100 + n)</p></td>
<td><p>EntryOrGuid 2 (<a href="#entryorguid">entryorguid</a> * 100 + n)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>0 is ignored. The timer will update IC and OOC. If an action list is already running it is overwritten with the new one. It is not possible to call a timed action list from within a timed action list.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RANDOM_MOVE</p></td>
<td><p>89</p></td>
<td><p>Radius</p></td>
<td><p>MinMoveTime</p></td>
<td><p>MaxMoveTime</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Enables random movement for the targeted creatures using the specified radius. If radius is 0 disables random movement. The target will use walk speed if not explicitly overridden using SMART_ACTION_SET_RUN. If MinMoveTime is set and less than or equal MaxMoveTime the creature is forced to stop for the specified time at each random point.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_UNIT_FIELD_BYTES_1</p></td>
<td><p>90</p></td>
<td><p><a href="https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Entities/Unit/Unit.h#L138">Flag/Value</a></p></td>
<td><p><a href="https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Entities/Unit/Unit.h#L138">Type</a></p></td>
<td><p>setValue (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If "setValue" is 1 set the byte value instead of the flag.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_UNIT_FIELD_BYTES_1</p></td>
<td><p>91</p></td>
<td><p><a href="https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Entities/Unit/Unit.h#L138">Flag</a></p></td>
<td><p><a href="https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Entities/Unit/Unit.h#L138">Type</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_INTERRUPT_SPELL</p></td>
<td><p>92</p></td>
<td><p>With delay (0/1)</p></td>
<td><p>SpellId</p></td>
<td><p>Instant (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>This action allows you to interrupt the current spell being cast. If you do not set the spellId, the core will find the current spell depending on the withDelay and the withInstant values.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SEND_GO_CUSTOM_ANIM</p></td>
<td><p>93</p></td>
<td><p>animprogress (0-255)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_DYNAMIC_FLAG</p></td>
<td><p>94</p></td>
<td><p><a href="creature_template.md#dynamicflags">creature_template.dynamicflags</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ADD_DYNAMIC_FLAG</p></td>
<td><p>95</p></td>
<td><p><a href="creature_template.md#dynamicflags">creature_template.dynamicflags</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_DYNAMIC_FLAG</p></td>
<td><p>96</p></td>
<td><p><a href="creature_template.md#dynamicflags">creature_template.dynamicflags</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_JUMP_TO_POS</p></td>
<td><p>97</p></td>
<td><p>Speed XY (if 0 calculate automatically)</p></td>
<td><p>Speed Z</p></td>
<td><p>selfJump (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If selfJump is 1 the actor will jump to the target (you can add an offset from the target's position by also specifying target coordinates); if selfJump is 0 the targeted creature will jump to the target coordinates</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SEND_GOSSIP_MENU</p></td>
<td><p>98</p></td>
<td><p><a href="gossip_menu.md#menuid">gossip_menu.MenuID</a></p></td>
<td><p><a href="gossip_menu.md#textid">gossip_menu.TextID</a><br />
(same value as <a href="npc_text.md#id">npc_text.ID</a>)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Can be used together with 'SMART_EVENT_GOSSIP_HELLO' to set custom gossip.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_GO_SET_LOOT_STATE</p></td>
<td><p>99</p></td>
<td><p>LootState (0 - Not ready, 1 - Ready, 2 - Activated, 3 - Just deactivated)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SEND_TARGET_TO_TARGET</p></td>
<td><p>100</p></td>
<td><p>Id</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Send targets previously stored with SMART_ACTION_STORE_TARGET, to another npc/go, the other npc/go can then access them as if it was its own stored list</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_HOME_POS</p></td>
<td><p>101</p></td>
<td><p>0: if the target is a creature, set it's current position as it's new home position; if the target is SMART_TARGET_POSITION, use this position as new home position for the actor</p>
<p>1: if the target is a creature, reset it's home position to the one from the DB; if the target is SMART_TARGET_POSITION, reset the actor's home position to the one from the DB (the actual values of the target position are ignored)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_HEALTH_REGEN</p></td>
<td><p>102</p></td>
<td><p>0/1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Sets the current creatures health regen on or off.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_ROOT</p></td>
<td><p>103</p></td>
<td><p>0/1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Enables or disables creature movement</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_GO_FLAG</p></td>
<td><p>104</p></td>
<td><p><a href="gameobject_template_addon.md#flags">gameobject_template_addon.flags</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>oldFlag = newFlag</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ADD_GO_FLAG</p></td>
<td><p>105</p></td>
<td><p><a href="gameobject_template_addon.md#flags">gameobject_template_addon.flags</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>oldFlag |= newFlag</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_GO_FLAG</p></td>
<td><p>106</p></td>
<td><p><a href="gameobject_template_addon.md#flags">gameobject_template_addon.flags</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>oldFlag &amp;= ~newFlag</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SUMMON_CREATURE_GROUP</p></td>
<td><p>107</p></td>
<td><p><a href="creature_summon_groups.md#groupid">creature_summon_groups.groupId</a></p></td>
<td><p>attackInvoker (0/1)</p></td>
<td><p>attackScriptOwner (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Use creature_summon_groups table. SAI target has no effect, use 0</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_POWER</p></td>
<td><p>108</p></td>
<td><p><a href="https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Miscellaneous/SharedDefines.h#L169">Power type</a></p></td>
<td><p>New power</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ADD_POWER</p></td>
<td><p>109</p></td>
<td><p><a href="https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Miscellaneous/SharedDefines.h#L169">Power type</a></p></td>
<td><p>Power to add</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_POWER</p></td>
<td><p>110</p></td>
<td><p><a href="https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Miscellaneous/SharedDefines.h#L169">Power type</a></p></td>
<td><p>Power to remove</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_GAME_EVENT_STOP</p></td>
<td><p>111</p></td>
<td><p><a href="game_event.md#evententry">game_event.eventEntry</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_GAME_EVENT_START</p></td>
<td><p>112</p></td>
<td><p><a href="game_event.md#evententry">game_event.eventEntry</a></p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_START_CLOSEST_WAYPOINT</p></td>
<td><p>113</p></td>
<td><p>wp1</p></td>
<td><p>wp2</p></td>
<td><p>wp3</p></td>
<td><p>wp4</p></td>
<td><p>wp5</p></td>
<td><p>wp6</p></td>
<td><p>Make target follow closest waypoint to its location</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RISE_UP</p></td>
<td><p>114</p></td>
<td><p>distance</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>move up for the specified distance (warning: TC 3.3.5 uses another action here: SMART_ACTION_MOVE_OFFSET)</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RANDOM_SOUND</p></td>
<td><p>115</p></td>
<td><p>soundId1</p></td>
<td><p>soundId2</p></td>
<td><p>soundId3</p></td>
<td><p>soundId4</p></td>
<td><p>onlySelf (1: only sends the sound to targeted players, 0: sends the sound to everyone in visibility range of the target)</p></td>
<td><p>distance (1: the sound fades with increasing distance to the target, 0: the sound is played at full volume no matter the distance)</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_CORPSE_DELAY</p></td>
<td><p>116</p></td>
<td><p>delay (in seconds)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_DISABLE_EVADE</p></td>
<td><p>117</p></td>
<td><p>0/1 (1 = disabled, 0 = enabled)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Take care if using this action. Disabling evasion is dangerous (e.g. the creature won't reset anymore).</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_SIGHT_DIST</p></td>
<td><p>121</p></td>
<td><p>SightDistance</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_FLEE</p></td>
<td><p>122</p></td>
<td><p>FleeTime (ms)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ADD_THREAT</p></td>
<td><p>123</p></td>
<td><p>+threat</p></td>
<td><p>-threat</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Add/remove threat directly to all specified targets</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_LOAD_EQUIPMENT</p></td>
<td><p>124</p></td>
<td><p>Id</p></td>
<td><p>force</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_TRIGGER_RANDOM_RANGE_TIMED_EVENT</p></td>
<td><p>125</p></td>
<td><p>id min range</p></td>
<td><p>id max range</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>It is not necessary to create the timed events beforehand.</td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_ALL_GAMEOBJECTS</p></td>
<td><p>126</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Remove all GOs associated with the targeted unit(s).</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_MOVE_TO_POS_TARGET</p></td>
<td><p>201</p></td>
<td><p>pointId</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Target has to be one or more creatures; move them to the specified position (target x,y,z)</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_GO_STATE</p></td>
<td><p>202</p></td>
<td><p>State (0 - GO_STATE_ACTIVE, 1 - GO_STATE_READY, 2 - GO_STATE_ACTIVE_ALTERNATIVE)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_EXIT_VEHICLE</p></td>
<td><p>203</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_UNIT_MOVEMENT_FLAGS</p></td>
<td><p>204</p></td>
<td><p>flags</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_COMBAT_DISTANCE</p></td>
<td><p>205</p></td>
<td><p>combatDistance</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_CASTER_COMBAT_DIST</p></td>
<td><p>206</p></td>
<td><p>followDistance</p></td>
<td><p>resetToMax</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_HOVER</p></td>
<td><p>207</p></td>
<td><p>0/1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ADD_IMMUNITY</p></td>
<td><p>208</p></td>
<td><p>type<br />
0 IMMUNITY_EFFECT (enum SpellEffects)<br />
1 IMMUNITY_STATE (enum AuraType)<br />
2 IMMUNITY_SCHOOL (enum [SpellSchoolMask](#spell-schools))<br />
3 IMMUNITY_DAMAGE (enum [SpellSchoolMask](#spell-schools))<br />
4 IMMUNITY_DISPEL (enum DispelType)<br />
5 IMMUNITY_MECHANIC (enum Mechanics)<br />
6 IMMUNITY_ID (NPC is immune to the spell ID specified in "value")<br />
7 IMMUNITY_ALLOW_ID (NPC is immune to everything except for the spell ID specified in "value")</p></td>
<td><p>id (normally the spell from which the immunity originates, for script purposes use 0)</p></td>
<td><p>value<br />
depends on "type", e.g. for type "IMMUNITY_SCHOOL" or "IMMUNITY_DAMAGE" it's a bit mask, see [Spell Schools](#spell-schools) below or [SharedDefines.h](https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Miscellaneous/SharedDefines.h).</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_REMOVE_IMMUNITY</p></td>
<td><p>209</p></td>
<td><p>type</p></td>
<td><p>id</p></td>
<td><p>value</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_FALL</p></td>
<td><p>210</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_EVENT_PHASE_RESET</p></td>
<td><p>211</p></td>
<td><p>0: Keep event phase on creature reset; 1: Event phase will be set to 0 on creature reset (default behaviour)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_STOP_MOTION</p></td>
<td><p>212</p></td>
<td><p>stopMoving</p></td>
<td><p>movementExpired</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_NO_ENVIRONMENT_UPDATE</p></td>
<td><p>213</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_ZONE_UNDER_ATTACK</p></td>
<td><p>214</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_LOAD_GRID</p></td>
<td><p>215</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Use target x/y values to load the respective grid</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_MUSIC</p></td>
<td><p>216</p></td>
<td><p>SoundId</p></td>
<td><p>onlySelf (1: only sends music to targeted players, 0: sends music to everyone in visibility range of the target)</p></td>
<td><p>type</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Plays the specified sound file as music. Type can be one of these values:<br />
0: Play music for the specified target(s)<br />
1: Play music for all players in the entire zone<br />
2: Play music for all players in the area</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_RANDOM_MUSIC</p></td>
<td><p>217</p></td>
<td><p>SoundId1</p></td>
<td><p>SoundId2</p></td>
<td><p>SoundId3</p></td>
<td><p>SoundId4</p></td>
<td><p>onlySelf (1: only sends music to targeted players, 0: sends music to everyone in visibility range of the target)</p></td>
<td><p>type</p></td>
<td><p>Plays randomly one of the specified sound files as music. Type can be one of these values:<br />
0: Play music for the specified target(s)<br />
1: Play music for all players in the entire zone<br />
2: Play music for all players in the area</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CYCLIC_MOVE</p></td>
<td><p>231</p></td>
<td><p>type (0 stop cyclic movement, 1 circle clockwise, 2 circle counterclockwise, >2 <a href="waypoints.md#entry">waypoints.entry</a>)</p></td>
<td><p>stepCount (only for circle)</p></td>
<td><p>centerSelf (only for circle)</p></td>
<td><p>speed (if 0 use default speed)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Start cyclic movement using a circle with target_o as radius or a <a href="waypoints.md#entry">waypoints.entry</a>. If "centerSelf" is set to 1 the specified target creatures will start circling the script owner.<br />
If the start position distance is far away the circle movement speed will be decreased following the second circle (this is the behaviour of the client which is reflected by the server)</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_HEALTH</p></td>
<td><p>232</p></td>
<td><p>use percentage (0/1)</p></td>
<td><p>copy from target (0/1)</p></td>
<td><p>health</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If "health" is greater than 0 set the health on the target(s). Otherwise copy health, either from the first target to the script owner if "copy from target" is set to 1 or from the script owner to all targets if set to 0. Use percentage if "use percentage" is set to 1, otherwise the actual health amount.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_DESPAWN_GO</p></td>
<td><p>233</p></td>
<td><p>respawnTime in s</p></td>
<td><p>playDespawnAnim (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Despawns the targeted GOs and respawn after "respawnTime" seconds (important: if >0 this overrides [gameobject.spawntimesecs](gameobject.md#spawntimesecs)!). If the GO starts despawned (spawntimesecs is negative) the "respawnTime" value is ignored. If "playDespawnAnim" is 1 the GO is playing its despawn animation.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CUSTOM_TALK</p></td>
<td><p>234</p></td>
<td><p>[broadcast_text.id](broadcast_text.md#id)</p></td>
<td><p>talkType (0: say, 1: yell, 2: text emote, 3: boss emote, 4: whisper, 5: boss whisper)</p></td>
<td><p>talker (0: action target, 1: self, 2: invoker)</p></td>
<td><p>talkTarget (0: action target, 1: self, 2: invoker)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_COUNTER_RESET</p></td>
<td><p>235</p></td>
<td><p>0: Keep counters on creature reset; 1: Counters will be cleared on creature reset (default behaviour)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CALL_EVENT_SCRIPT</p></td>
<td><p>236</p></td>
<td><p>[event_scripts](event_scripts.md) ID</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_CREATURE_FORMATION</p></td>
<td><p>237</p></td>
<td><p>[creature_formations.groupAI](creature_formations.md#groupai)</p></td>
<td><p>update formation (0: create, 1: leave, 2: update formation info)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Add the creature to the target's [creature formation](creature_formations.md). If the creature formation does not exist, create a new one with the target as leader. If multiple targets are specified, only the first one is picked. Use target z as distance and target o as angle. The default movement type is set to "idle", keep this in mind if leaving the formation.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_LOAD_WP_PATH</p></td>
<td><p>238</p></td>
<td><p>[waypoint_data.id](waypoint_data.md#id)</p></td>
<td><p>unload path (0/1)</p></td>
<td><p>nextPathPoint</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Start WP movement using [waypoint_data](waypoint_data.md) which is better suited for formations than SMART_ACTION_FOLLOW. The default movement type is set to "idle", keep this in mind if unloading the path. If "nextPathPoint" is set continue with the specified point.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_STOP_WP_PATH</p></td>
<td><p>239</p></td>
<td><p>duration in ms</p></td>
<td><p>resetLastPlayerInteraction (0 / 1 - clear / 2 - set to current time)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Stop WP movement using [waypoint_data](waypoint_data.md) for the specified duration.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_OWNER_DEATH_DESPAWN</p></td>
<td><p>240</p></td>
<td><p>disable (0/1)</p></td>
<td><p><a href="#summon-types">Summon type</a></p></td>
<td><p>duration in ms</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>If "disable" is set to 1 prevent the despawn of minions if their owner dies. If summon type is 0, use 4 as default (TEMPSUMMON_TIMED_DESPAWN_OUT_OF_COMBAT). If duration is 0 use 5000 as default.</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_KILL_DELAY</p></td>
<td><p>241</p></td>
<td><p>delay (in ms)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Can be used to delay the kill of a creature, e.g. to show spell visuals before the creature dies. Use SMART_EVENT_KILL_DELAY_STARTED to trigger actions, for example to disable combat using SMART_ACTION_AUTO_ATTACK and SMART_ACTION_ALLOW_COMBAT_MOVEMENT.
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SCALE</p></td>
<td><p>242</p></td>
<td><p>percent</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Scale the targeted unit or gameobject. If 0 percent is used the scaling is reset (either 100% or to the value specified in [creature_template.scale](creature_template.md#scale) or [gameobject_template.size](gameobject_template.md#size)).
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_SET_LOOT_DISABLED</p></td>
<td><p>243</p></td>
<td><p>0/1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Disable loot; currently only implemented for GOs.
</p></td>
</tr>
<tr>
<td><p>SMART_ACTION_TRIGGER_RANDOM_TIMED_EVENT</p></td>
<td><p>244</p></td>
<td><p>id1</p></td>
<td><p>id2</p></td>
<td><p>id3</p></td>
<td><p>id4</p></td>
<td><p>id5</p></td>
<td><p>id6</p></td>
<td>It is not necessary to create the timed events beforehand.</td>
</tr>
</tbody>
</table>

### target\_type

<table height="400">
<thead>
<tr class="header">
<th><p>Name</p></th>
<th><p>Value</p></th>
<th><p>target_param1</p></th>
<th><p>target_param2</p></th>
<th><p>target_param3</p></th>
<th><p>target_param4</p></th>
<th><p>target_x</p></th>
<th><p>target_y</p></th>
<th><p>target_z</p></th>
<th><p>target_o</p></th>
<th><p>Comment</p></th>
</tr>
</thead>
<tbody>
<tr>
<td><p>SMART_TARGET_NONE</p></td>
<td><p>0</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>None.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_SELF</p></td>
<td><p>1</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Self cast.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_VICTIM</p></td>
<td><p>2</p></td>
<td><p>maxDist3D</p></td>
<td><p>restrictType - bitmask:<br />
1 - player only<br />
2 - threat list size <= restrictValue<br />
4 - threat list size >= restrictValue</p></td>
<td><p>powerType</p></td>
<td><p>restrictValue</p></td>
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Our current target. (ie: highest aggro). Power type: 1 - Mana, 2 - Rage, 3 - Focus, 4 - Energy, 5 - Happiness, 6 - Rune, 7 - Runic Power</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_HOSTILE_SECOND_AGGRO</p></td>
<td><p>3</p></td>
<td><p>maxDist3D</p></td>
<td><p>restrictType (see above)</p></td>
<td><p>powerType</p></td>
<td><p>restrictValue</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Second highest aggro. Power type: see above</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_HOSTILE_LAST_AGGRO</p></td>
<td><p>4</p></td>
<td><p>maxDist3D</p></td>
<td><p>restrictType (see above)</p></td>
<td><p>powerType</p></td>
<td><p>restrictValue</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Dead last on aggro. Power type: see above</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_HOSTILE_RANDOM</p></td>
<td><p>5</p></td>
<td><p>maxDist3D</p></td>
<td><p>restrictType (see above)</p></td>
<td><p>powerType</p></td>
<td><p>restrictValue</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Just any random target on our threat list. Power type: see above</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_HOSTILE_RANDOM_NOT_TOP</p></td>
<td><p>6</p></td>
<td><p>maxDist3D</p></td>
<td><p>restrictType (see above)</p></td>
<td><p>powerType</p></td>
<td><p>restrictValue</p></td>
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Any random target except top threat. Power type: see above</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_ACTION_INVOKER</p></td>
<td><p>7</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Unit who caused this Event to occur.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_POSITION</p></td>
<td><p>8</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>x</p></td>
<td><p>y</p></td>
<td><p>z</p></td>
<td><p>o</p></td>
<td><p>Use xyz from event params.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_CREATURE_RANGE</p></td>
<td><p>9</p></td>
<td><p><a href="creature_template.md#entry">creature_template.entry</a> (0 any)</p></td>
<td><p>minDist2D</p></td>
<td><p>maxDist2D</p></td>
<td><p>alive state (1 alive, 2 dead, 0 both)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>All creatures with the specified ID within the specified range and the specified alive state (the script owner will never be included here).</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_CREATURE_GUID</p></td>
<td><p>10</p></td>
<td><p><a href="creature.md#guid">creature.guid</a></p></td>
<td><p><a href="creature_template.md#entry">creature_template.entry</a></p></td>
<td><p>getFromHashMap (0/1, this does not work in instances!)</p></td>
<td><p>alive state (1 alive, 2 dead, 0 both)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Creature with specified GUID and/or specified creature template ID and the specified alive state.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_CREATURE_DISTANCE</p></td>
<td><p>11</p></td>
<td><p><a href="creature_template.md#entry">creature_template.entry</a> (0 any)</p></td>
<td><p>maxDist2D</p></td>
<td><p>alive state (1 alive, 2 dead, 0 both)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>All creatures with the specified ID within the specified distance and the specified alive state (the script owner will never be included here).</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_STORED</p></td>
<td><p>12</p></td>
<td><p>id</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Uses pre-stored target(list). Can also be ID 16777215 which is reserved for SMART_ESCORT_TARGETS (see SMART_ACTION_WP_START).</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_GAMEOBJECT_RANGE</p></td>
<td><p>13</p></td>
<td><p><a href="gameobject_template.md#entry">gameobject_template.entry</a> (0 any)</p></td>
<td><p>minDist2D</p></td>
<td><p>maxDist2D</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>All game objects with the specified ID within the specified range (the script owner will never be included here).</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_GAMEOBJECT_GUID</p></td>
<td><p>14</p></td>
<td><p><a href="gameobject.md#guid">gameobject.guid</a></p></td>
<td><p><a href="gameobject_template.md#entry">gameobject_template.entry</a></p></td>
<td><p>getFromHashMap (0/1, this does not work in instances!)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Object with specified GUID and/or specified game object template ID.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_GAMEOBJECT_DISTANCE</p></td>
<td><p>15</p></td>
<td><p><a href="gameobject_template.md#entry">gameobject_template.entry</a> (0 any)</p></td>
<td><p>maxDist2D</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>All objects with the specified ID within the specified distance (the script owner will never be included here).</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_INVOKER_PARTY</p></td>
<td><p>16</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Invoker's party members</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_PLAYER_RANGE</p></td>
<td><p>17</p></td>
<td><p>minDist2D</p></td>
<td><p>maxDist2D</p></td>
<td><p>maxCount</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>All players up to maxCount within the specified range.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_PLAYER_DISTANCE</p></td>
<td><p>18</p></td>
<td><p>maxDist2D</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>All players within the specified distance.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_CLOSEST_CREATURE</p></td>
<td><p>19</p></td>
<td><p><a href="creature_template.md#entry">creature_template.entry</a> (0 any)</p></td>
<td><p>maxDist3D (Can be from 1-100 yards, if 0 then 100 yards will be used)</p></td>
<td><p>dead? (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Closest creature with the specified ID within the specified range. If maxDist is 0 then 100 yards will be used.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_CLOSEST_GAMEOBJECT</p></td>
<td><p>20</p></td>
<td><p><a href="gameobject_template.md#entry">gameobject_template.entry</a> (0 any)</p></td>
<td><p>maxDist3D (Can be from 1-100 yards, if 0 then 100 yards will be used)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Closest object with specified ID within specified range. If maxDist is 0 then 100 yards will be used.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_CLOSEST_PLAYER</p></td>
<td><p>21</p></td>
<td><p>maxDist3D</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Closest player within specified range.</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_ACTION_INVOKER_VEHICLE</p></td>
<td><p>22</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Unit's vehicle who caused this Event to occur</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_OWNER_OR_SUMMONER</p></td>
<td><p>23</p></td>
<td><p>use owner of owner (0/1)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Unit's owner or summoner</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_THREAT_LIST</p></td>
<td><p>24</p></td>
<td><p>maxDist (0 any)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>All units on creature's threat list within the specified distance if maxDist > 0</p></td>
</tr>
<tr>
<td>SMART_TARGET_CLOSEST_ENEMY</td>
<td>25</td>
<td>maxDist3D</td>
<td>playerOnly (0/1)</td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>Any attackable target (creature or player) within maxDist</td>
</tr>
<tr>
<td>SMART_TARGET_CLOSEST_FRIENDLY</td>
<td>26</td>
<td>maxDist3D</td>
<td>playerOnly (0/1)</td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td>Any friendly unit (creature, player or pet) within maxDist</td>
</tr>
<tr>
<td>SMART_TARGET_FARTHEST</td>
<td>28</td>
<td>maxDist</td>
<td>playerOnly (0/1)</td>
<td>isInLos (0/1)</td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Farthest unit on the threat list</p></td>
</tr>
<tr>
<td>SMART_TARGET_VEHICLE_PASSENGER</td>
<td>29</td>
<td>seatMask</td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Target units identified by the specified seat bit mask; 0 means all seats;<br />
combine bits 1 (seat 0), 2 (seat 1), 4 (seat 2), 8 (seat 3) etc. if targeting multiple seats, example:<br />
seat mask 9 means seat 0 and 3 (bit 1 + 8)</p></td>
</tr>
<tr>
<td>SMART_TARGET_CREATURE_FORMATION</td>
<td>231</td>
<td>memberType (0 - members only, 1 - leader only, 2 - leader and members)</td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>Target alive members of the [creature formation](creature_formations.md).</p></td>
</tr>
<tr>
<td><p>SMART_TARGET_MINION</p></td>
<td><p>232</p></td>
<td><p><a href="creature_template.md#entry">creature_template.entry</a></p></td>
<td><p>alive state (1 alive, 2 dead, 0 both)</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p><br />
</p></td>
<td><p>All minions with the specified creature entry.</p></td>
</tr>
</tbody>
</table>

### comment

Commenting on SAI uses a template which is the following: (with an example)

"Creature name - Event - Action"

"Minion of Gurok - On spawn - Set Random Movement"

**Quick notes:**

-   Always update creature\_template, gameobject\_template or areatrigger\_scripts with:

```sql
UPDATE `creature_template` SET `AIName` = 'SmartAI' WHERE `entry` = y;

UPDATE `gameobject_template` SET `AIName` = 'SmartGameObjectAI' WHERE `entry` = y;

INSERT INTO `areatrigger_scripts` (`entry`, `ScriptName`) VALUES (y, 'SmartTrigger');
```

-   If the creature or GO is inside a dungeon, set event\_flags accordingly to the instance difficulty (heroic, 25 man, etc.).

In case of doubt about an Event, Action or Target, check source code (src/server/game/AI/SmartScripts files; mainly SmartScript.cpp)

### Cast Flags

| Name                                                           | Flag | Hex    | Comment                                                                                  |
|----------------------------------------------------------------|------|--------|------------------------------------------------------------------------------------------|
| SMARTCAST\_INTERRUPT\_PREVIOUS                                 | 1    | 0x0001 | Interrupt any spell casting                                                              |
| SMARTCAST\_TRIGGERED                                           | 2    | 0x0002 | Triggered (this makes spell cost zero mana and have no cast time)                        |
| SMARTCAST\_AURA\_NOT\_PRESENT                                  | 32   | 0x0020 | Only casts the spell if the target does not have an aura from the spell                  |
| SMARTCAST\_COMBAT\_MOVE                                        | 64   | 0x0040 | Prevent combat movement on cast, allow on fail range, mana, LOS                          |
| SMARTCAST\_AURA\_NOT\_PRESENT\_UNIT                            | 4096 | 0x1000 | Only casts the spell if the target does not have an aura from the spell cast by the unit |

### React States

| Name              | Value | Comment                                                       |
|-------------------|-------|---------------------------------------------------------------|
| REACT\_PASSIVE    | 0     | Does not defend or attack at all. Does nothing.               |
| REACT\_DEFENSIVE  | 1     | Only attacks back when attacked.                              |
| REACT\_AGGRESSIVE | 2     | Will attack if on threat list and in threat radius. (default) |

### Summon Types

| Name                                        | Value | Comment                                                                               |
|---------------------------------------------|-------|---------------------------------------------------------------------------------------|
| TEMPSUMMON\_TIMED\_OR\_DEAD\_DESPAWN        | 1     | Despawns after a specified time (only out of combat) OR when the creature disappears. |
| TEMPSUMMON\_TIMED\_OR\_CORPSE\_DESPAWN      | 2     | Despawns after a specified time (only out of combat) OR when the creature dies.       |
| TEMPSUMMON\_TIMED\_DESPAWN                  | 3     | Despawns after a specified time (no matter if the creature is in combat or not).      |
| TEMPSUMMON\_TIMED\_DESPAWN\_OUT\_OF\_COMBAT | 4     | Despawns after a specified time after the creature is out of combat.                  |
| TEMPSUMMON\_CORPSE\_DESPAWN                 | 5     | Despawns instantly after death.                                                       |
| TEMPSUMMON\_CORPSE\_TIMED\_DESPAWN          | 6     | Despawns after a specified time after death.                                          |
| TEMPSUMMON\_DEAD\_DESPAWN                   | 7     | Despawns when the creature disappears.                                                |
| TEMPSUMMON\_MANUAL\_DESPAWN                 | 8     | Despawns when UnSummon() (or Force Despawn action) is called.                         |

### Spell Schools

| Bit | Name     |
|-----|----------|
| 1   | Physical |
| 2   | Holy     |
| 4   | Fire     |
| 8   | Nature   |
| 16  | Frost    |
| 32  | Shadow   |
| 64  | Arcane   |

### Invoker:

Actions like SMART\_ACTION\_INVOKER\_CAST and targets like SMART\_TARGET\_ACTION\_INVOKER will work only if the event is in this list:

SMART\_EVENT\_AGGRO

SMART\_EVENT\_DEATH

SMART\_EVENT\_KILL

SMART\_EVENT\_SUMMONED\_UNIT

SMART\_EVENT\_SPELLHIT

SMART\_EVENT\_SPELLHIT\_TARGET

SMART\_EVENT\_DAMAGED

SMART\_EVENT\_RECEIVE\_HEAL

SMART\_EVENT\_RECEIVE\_EMOTE

SMART\_EVENT\_JUST\_SUMMONED

SMART\_EVENT\_DAMAGED\_TARGET

SMART\_EVENT\_SUMMON\_DESPAWNED

SMART\_EVENT\_PASSENGER\_BOARDED

SMART\_EVENT\_PASSENGER\_REMOVED

SMART\_EVENT\_GOSSIP\_HELLO

SMART\_EVENT\_GOSSIP\_SELECT

SMART\_EVENT\_ACCEPTED\_QUEST

SMART\_EVENT\_REWARD\_QUEST

SMART\_EVENT\_FOLLOW\_COMPLETED

SMART\_EVENT\_ON\_SPELLCLICK

SMART\_EVENT\_AREATRIGGER\_ONTRIGGER

SMART\_EVENT\_IC\_LOS

SMART\_EVENT\_OOC\_LOS

SMART\_EVENT\_DISTANCE\_CREATURE

SMART\_EVENT\_FRIENDLY\_HEALTH

SMART\_EVENT\_FRIENDLY\_HEALTH\_PCT

SMART\_EVENT\_FRIENDLY\_IS\_CC

SMART\_EVENT\_FRIENDLY\_MISSING\_BUFF

SMART\_EVENT\_ACTION\_DONE

SMART\_EVENT\_TARGET\_HEALTH\_PCT

SMART\_EVENT\_TARGET\_MANA\_PCT

SMART\_EVENT\_RANGE

SMART\_EVENT\_VICTIM\_CASTING

SMART\_EVENT\_TARGET\_BUFFED

SMART\_EVENT\_IS\_BEHIND\_TARGET

SMART\_EVENT\_INSTANCE\_PLAYER\_ENTER

SMART\_EVENT\_TRANSPORT\_ADDCREATURE

SMART\_EVENT\_DATA\_SET

SMART\_EVENT\_CHANNEL\_FINISHED\_TARGET
