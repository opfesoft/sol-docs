# spell\_proc\_event

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

These fields control which spells' family flags can proc the triggered spell. Sometimes also called "SpellClassMask".

### procFlags

A bitmask controlling what events trigger the spell. To combine possible events, add the proc bits together.

| Flag     | Event                                     | Bit        | Comment                                                                            |
|----------|-------------------------------------------|------------|------------------------------------------------------------------------------------|
| 0        | PROC_FLAG_NONE                            | 0x00000000 |                                                                                    |
| 1        | PROC_FLAG_KILLED                          | 0x00000001 | Killed by agressor                                                                 |
| 2        | PROC_FLAG_KILL                            | 0x00000002 | Kill target (in most cases need XP/Honor reward)                                   |
| 4        | PROC_FLAG_DONE_MELEE_AUTO_ATTACK          | 0x00000004 | Done melee auto attack                                                             |
| 8        | PROC_FLAG_TAKEN_MELEE_AUTO_ATTACK         | 0x00000008 | Taken melee auto attack                                                            |
| 16       | PROC_FLAG_DONE_SPELL_MELEE_DMG_CLASS      | 0x00000010 | Done attack by spell that has dmg class melee                                      |
| 32       | PROC_FLAG_TAKEN_SPELL_MELEE_DMG_CLASS     | 0x00000020 | Taken attack by spell that has dmg class melee                                     |
| 64       | PROC_FLAG_DONE_RANGED_AUTO_ATTACK         | 0x00000040 | Done ranged auto attack                                                            |
| 128      | PROC_FLAG_TAKEN_RANGED_AUTO_ATTACK        | 0x00000080 | Taken ranged auto attack                                                           |
| 256      | PROC_FLAG_DONE_SPELL_RANGED_DMG_CLASS     | 0x00000100 | Done attack by spell that has dmg class ranged                                     |
| 512      | PROC_FLAG_TAKEN_SPELL_RANGED_DMG_CLASS    | 0x00000200 | Taken attack by spell that has dmg class ranged                                    |
| 1024     | PROC_FLAG_DONE_SPELL_NONE_DMG_CLASS_POS   | 0x00000400 | Done positive spell that has dmg class none                                        |
| 2048     | PROC_FLAG_TAKEN_SPELL_NONE_DMG_CLASS_POS  | 0x00000800 | Taken positive spell that has dmg class none                                       |
| 4096     | PROC_FLAG_DONE_SPELL_NONE_DMG_CLASS_NEG   | 0x00001000 | Done negative spell that has dmg class none                                        |
| 8192     | PROC_FLAG_TAKEN_SPELL_NONE_DMG_CLASS_NEG  | 0x00002000 | Taken negative spell that has dmg class none                                       |
| 16384    | PROC_FLAG_DONE_SPELL_MAGIC_DMG_CLASS_POS  | 0x00004000 | Done positive spell that has dmg class magic                                       |
| 32768    | PROC_FLAG_TAKEN_SPELL_MAGIC_DMG_CLASS_POS | 0x00008000 | Taken positive spell that has dmg class magic                                      |
| 65536    | PROC_FLAG_DONE_SPELL_MAGIC_DMG_CLASS_NEG  | 0x00010000 | Done negative spell that has dmg class magic                                       |
| 131072   | PROC_FLAG_TAKEN_SPELL_MAGIC_DMG_CLASS_NEG | 0x00020000 | Taken negative spell that has dmg class magic                                      |
| 262144   | PROC_FLAG_DONE_PERIODIC                   | 0x00040000 | Successful do periodic (damage / healing)                                          |
| 524288   | PROC_FLAG_TAKEN_PERIODIC                  | 0x00080000 | Taken spell periodic (damage / healing)                                            |
| 1048576  | PROC_FLAG_TAKEN_DAMAGE                    | 0x00100000 | Taken any damage                                                                   |
| 2097152  | PROC_FLAG_DONE_TRAP_ACTIVATION            | 0x00200000 | On trap activation                                                                 |
| 4194304  | PROC_FLAG_DONE_MAINHAND_ATTACK            | 0x00400000 | Done main-hand melee attacks (spell and autoattack)                                |
| 8388608  | PROC_FLAG_DONE_OFFHAND_ATTACK             | 0x00800000 | Done off-hand melee attacks (spell and autoattack)                                 |
| 16777216 | PROC_FLAG_DEATH                           | 0x01000000 | Died in any way                                                                    |

### procEx

| Flag     | Name                        | Bit       | Comment                                                                               |
|----------|-----------------------------|-----------|---------------------------------------------------------------------------------------|
| 0        | PROC_EX_NONE                | 0x0000000 | If none can trigger on Hit/Crit only (passive spells MUST defined by SpellFamily flag) |
| 1        | PROC_EX_NORMAL_HIT          | 0x0000001 | If set only from normal hit (only damage spells)                                      |
| 2        | PROC_EX_CRITICAL_HIT        | 0x0000002 |                                                                                       |
| 4        | PROC_EX_MISS                | 0x0000004 |                                                                                       |
| 8        | PROC_EX_RESIST              | 0x0000008 |                                                                                       |
| 16       | PROC_EX_DODGE               | 0x0000010 |                                                                                       |
| 32       | PROC_EX_PARRY               | 0x0000020 |                                                                                       |
| 64       | PROC_EX_BLOCK               | 0x0000040 |                                                                                       |
| 128      | PROC_EX_EVADE               | 0x0000080 |                                                                                       |
| 256      | PROC_EX_IMMUNE              | 0x0000100 |                                                                                       |
| 512      | PROC_EX_DEFLECT             | 0x0000200 |                                                                                       |
| 1024     | PROC_EX_ABSORB              | 0x0000400 |                                                                                       |
| 2048     | PROC_EX_REFLECT             | 0x0000800 |                                                                                       |
| 4096     | PROC_EX_INTERRUPT           | 0x0001000 | Melee hit result can be Interrupt (not used)                                          |
| 8192     | PROC_EX_FULL_BLOCK          | 0x0002000 | Block all attack damage                                                               |
| 16384    | PROC_EX_RESERVED2           | 0x0004000 |                                                                                       |
| 32768    | PROC_EX_NOT_ACTIVE_SPELL    | 0x0008000 | Spell mustn't do damage/heal to proc                                                  |
| 65536    | PROC_EX_EX_TRIGGER_ALWAYS   | 0x0010000 | If set trigger always (no matter of hit result) used for drop charges                 |
| 131072   | PROC_EX_ONLY_ON_PLAYER_CAST | 0x0020000 | If set trigger only once on player cast (ignores all other procEx-flags)              |
| 262144   | PROC_EX_ONLY_ACTIVE_SPELL   | 0x0040000 | Spell has to do damage/heal to proc                                                   |
| 524288   | PROC_EX_NO_OVERHEAL         | 0x0080000 | Proc if heal did some work                                                            |
| 1048576  | PROC_EX_NO_AURA_REFRESH     | 0x0100000 | Proc if aura was not refreshed                                                        |
| 2097152  | PROC_EX_ONLY_FIRST_TICK     | 0x0200000 | Proc only on first tick (in case of periodic spells)                                  |

### ppmRate

This field controls the times per minute that the spell should proc. If zero, then the value is taken from the DBC entry.

As ppmRate is a rate it will not be guaranteed to proc X amount of times per minute. The ppm is calculated by this formula:

```
((WeaponSpeed * PPM) / 600.0f);   // result is chance in percent (Probability = SpeedInSec * (PPM / 60))
```

### CustomChance

Custom chance for triggering, given in percentage.

### Cooldown

Define hidden cooldowns on the spell, given in milliseconds. Also known as the proc's internal cooldown, or ICD.
