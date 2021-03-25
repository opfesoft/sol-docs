# spell\_proc\_event

**The \`spell\_proc\_event\` table**

This table holds information on what events (or procs) certain spells are activated. All spells in this table must have applied a SPELL_AURA_PROC_TRIGGER_SPELL (42) aura. Any entries in this table will overwrite the existing proc settings in the spell's DBC entry.

## Structure

| Field                                | Type         | Attributes | Key | Null | Default | Extra | Comment |
|--------------------------------------|--------------|------------|-----|------|---------|-------|---------|
| [entry](#entry)                      | mediumint(8) |            | PRI | NO   | 0       |       |         |
| [SchoolMask](#schoolmask)            | tinyint(4)   |            |     | NO   | 0       |       |         |
| [SpellFamilyName](#spellfamilyname)   | smallint(5)  | unsigned   |     | NO   | 0       |       |         |
| [SpellFamilyMask0](#spellfamilymaskx) | int(10)      | unsigned   |     | NO   | 0       |       |         |
| [SpellFamilyMask1](#spellfamilymaskx) | int(10)      | unsigned   |     | NO   | 0       |       |         |
| [SpellFamilyMask2](#spellfamilymaskx) | int(10)      | unsigned   |     | NO   | 0       |       |         |
| [procFlags](#procflags)               | int(10)      | unsigned   |     | NO   | 0       |       |         |
| [procEx](#procex)                     | int(10)      | unsigned   |     | NO   | 0       |       |         |
| [ppmRate](#ppmrate)                   | float        |            |     | NO   | 0       |       |         |
| [CustomChance](#customchance)         | float        |            |     | NO   | 0       |       |         |
| [Cooldown](#cooldown)                 | int(10)      | unsigned   |     | NO   | 0       |       |         |

## Description of the fields

### entry

The spell ID that is capable to proc on an event (can use negative spellId for ranked spells).

### SchoolMask

This field contains a bitmask that controls on what types of spell damage the proc can be triggered, e.g. if an aura procs only when the unit it is cast upon is hit by shadow spells (spell 34914). To combine spell schools, just add the bit values.

| School ID | Bit | Name     |
|-----------|-----|----------|
| 0         | 1   | Physical |
| 1         | 2   | Holy     |
| 2         | 4   | Fire     |
| 3         | 8   | Nature   |
| 4         | 16  | Frost    |
| 5         | 32  | Shadow   |
| 6         | 64  | Arcane   |

### SpellFamilyName

This field controls which family name spells can proc the triggered spell.

| ID | Family Name  |
|----|--------------|
| 0  | Generic      |
| 3  | Mage         |
| 4  | Warrior      |
| 5  | Warlock      |
| 6  | Priest       |
| 7  | Druid        |
| 8  | Rogue        |
| 9  | Hunter       |
| 10 | Paladin      |
| 11 | Shaman       |
| 13 | Potion       |
| 15 | Death Knight |

### SpellFamilyMaskX

These fields control which spells' family flags can proc the triggered spell. 

### procFlags

A bitmask controlling what events trigger the spell. To combine possible events, add the proc bits together.

| Event                                   | Bit        | Comment                                                                            |
|-----------------------------------------|------------|------------------------------------------------------------------------------------|
| PROC_FLAG_NONE                          | 0x00000000 |                                                                                    |
| PROC_FLAG_KILLED                        | 0x00000001 | Killed by agressor                                                                 |
| PROC_FLAG_KILL_AND_GET_XP               | 0x00000002 | Kill that yields experience or honor                                               |
| PROC_FLAG_SUCCESSFUL_MELEE_HIT          | 0x00000004 | Successful melee attack                                                            |
| PROC_FLAG_TAKEN_MELEE_HIT               | 0x00000008 | Taken damage from melee strike hit                                                 |
| PROC_FLAG_SUCCESSFUL_MELEE_SPELL_HIT    | 0x00000010 | Successful attack by Spell that use melee weapon                                   |
| PROC_FLAG_TAKEN_MELEE_SPELL_HIT         | 0x00000020 | Taken damage by Spell that use melee weapon                                        |
| PROC_FLAG_SUCCESSFUL_RANGED_HIT         | 0x00000040 | Successful Ranged attack (all ranged attack deal as spell so newer set :( )        |
| PROC_FLAG_TAKEN_RANGED_HIT              | 0x00000080 | Taken damage from ranged attack (all ranged attack deal as spell so newer set :( ) |
| PROC_FLAG_SUCCESSFUL_RANGED_SPELL_HIT   | 0x00000100 | Successful Ranged attack by Spell that use ranged weapon                           |
| PROC_FLAG_TAKEN_RANGED_SPELL_HIT        | 0x00000200 | Taken damage by Spell that use ranged weapon                                       |
| PROC_FLAG_SUCCESSFUL_POSITIVE_AOE_HIT   | 0x00000400 | Successful AoE (not 100% sure unused)                                              |
| PROC_FLAG_TAKEN_POSITIVE_AOE            | 0x00000800 | Taken AoE      (not 100% sure unused)                                              |
| PROC_FLAG_SUCCESSFUL_AOE_SPELL_HIT      | 0x00001000 | Successful AoE damage spell hit (not 100% sure unused)                             |
| PROC_FLAG_TAKEN_AOE_SPELL_HIT           | 0x00002000 | Taken AoE damage spell hit      (not 100% sure unused)                             |
| PROC_FLAG_SUCCESSFUL_POSITIVE_SPELL     | 0x00004000 | Successful cast positive spell (by default only on healing)                        |
| PROC_FLAG_TAKEN_POSITIVE_SPELL          | 0x00008000 | Taken positive spell hit (by default only on healing)                              |
| PROC_FLAG_SUCCESSFUL_NEGATIVE_SPELL_HIT | 0x00010000 | Successful negative spell cast (by default only on damage)                         |
| PROC_FLAG_TAKEN_NEGATIVE_SPELL_HIT      | 0x00020000 | Taken negative spell (by default only on damage)                                   |
| PROC_FLAG_ON_DO_PERIODIC                | 0x00040000 | Successful do periodic (damage / healing determined from 14-17 flags)              |
| PROC_FLAG_ON_TAKE_PERIODIC              | 0x00080000 | Taken spell periodic (damage / healing determined from 14-17 flags)                |
| PROC_FLAG_TAKEN_ANY_DAMAGE              | 0x00100000 | Taken any damage                                                                   |
| PROC_FLAG_ON_TRAP_ACTIVATION            | 0x00200000 | On trap activation                                                                 |
| PROC_FLAG_TAKEN_OFFHAND_HIT             | 0x00400000 | Taken off-hand melee attacks(not used)                                             |
| PROC_FLAG_SUCCESSFUL_OFFHAND_HIT        | 0x00800000 | Successful off-hand melee attacks                                                  |
| PROC_FLAG_DEATH                         | 0x01000000 | Died in any way                                                                    |

### procEx

| Name                        | Bit       | Comment                                                                               |
|-----------------------------|-----------|---------------------------------------------------------------------------------------|
| PROC_EX_NONE                | 0x0000000 | If none can tigger on Hit/Crit only (passive spells MUST defined by SpellFamily flag) |
| PROC_EX_NORMAL_HIT          | 0x0000001 | If set only from normal hit (only damage spells)                                      |
| PROC_EX_CRITICAL_HIT        | 0x0000002 |                                                                                       |
| PROC_EX_MISS                | 0x0000004 |                                                                                       |
| PROC_EX_RESIST              | 0x0000008 |                                                                                       |
| PROC_EX_DODGE               | 0x0000010 |                                                                                       |
| PROC_EX_PARRY               | 0x0000020 |                                                                                       |
| PROC_EX_BLOCK               | 0x0000040 |                                                                                       |
| PROC_EX_EVADE               | 0x0000080 |                                                                                       |
| PROC_EX_IMMUNE              | 0x0000100 |                                                                                       |
| PROC_EX_DEFLECT             | 0x0000200 |                                                                                       |
| PROC_EX_ABSORB              | 0x0000400 |                                                                                       |
| PROC_EX_REFLECT             | 0x0000800 |                                                                                       |
| PROC_EX_INTERRUPT           | 0x0001000 | Melee hit result can be Interrupt (not used)                                          |
| PROC_EX_FULL_BLOCK          | 0x0002000 | Block all attack damage                                                               |
| PROC_EX_RESERVED2           | 0x0004000 |                                                                                       |
| PROC_EX_NOT_ACTIVE_SPELL    | 0x0008000 |                                                                                       |
| PROC_EX_EX_TRIGGER_ALWAYS   | 0x0010000 | If set trigger always ( no matter another flags) used for drop charges                |
| PROC_EX_EX_ONE_TIME_TRIGGER | 0x0020000 | If set trigger always but only one time                                               |
| PROC_EX_ONLY_ACTIVE_SPELL   | 0x0040000 | Spell has to do damage/heal to proc                                                   |
| PROC_EX_NO_OVERHEAL         | 0x0080000 | Proc if heal did some work                                                            |
| PROC_EX_NO_AURA_REFRESH     | 0x0100000 | Proc if aura was not refreshed                                                        |

### ppmRate

This field controls the times per minute that the spell should proc. If zero, then the value is taken from the DBC entry.

### CustomChance

Custom chance for triggering, given in percentage.

### Cooldown

Define hidden cooldowns on the spell, given in milliseconds. Also known as the proc's internal cooldown, or ICD.
