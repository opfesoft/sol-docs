# creature\_guid\_chance

Can be used to apply a specific creature ID to one randomly chosen GUID from a list of creature GUIDs.

## Structure

| Field             | Type         | Attributes | Null | Key | Default | Extra | Comment |
|-------------------|--------------|------------|------|-----|---------|-------|---------|
| [id](#id)         | mediumint(8) | unsigned   | NO   | PRI | NULL    |       |         |
| [guid](#guid)     | int(10)      | unsigned   | NO   | PRI | NULL    |       | unique  |
| [chance](#chance) | float        |            | NO   |     | NULL    |       |         |

## Description of the fields

### id

Alternative [creature ID](creature_template.md#entry).

### guid

DB [GUID](creature.md#guid) of the creature.

### chance

Chance to roll this creature GUID. Has to be greater than 0 and less than or equal to 100.

### Additional notes

- This is meant to apply the creature ID of a single rare mob to a bunch of creature GUIDs.
- This will override any GUIDs specified in [creature\_id\_chance](creature_id_chance.md).
- Don't mix creature GUIDs from instanced with non-instanced maps or multiple instanced maps, this will not work correctly.
- It is possible to mix GUIDs from multiple non-instanced maps.
- The creature ID is applied before the creature is created and will also override ZoneScript::GetCreatureEntry (take care if using this for instanced maps).
- Concerning instanced maps the creature ID is only applied once during creation of the instance, not on respawn.
