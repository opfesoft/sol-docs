# creature\_id\_chance

Can be used to specify multiple alternative creature IDs for a DB creature GUID.

## Structure

| Field             | Type         | Attributes | Null | Key | Default | Extra | Comment |
|-------------------|--------------|------------|------|-----|---------|-------|---------|
| [guid](#guid)     | int(10)      | unsigned   | NO   | PRI | NULL    |       |         |
| [id](#id)         | mediumint(8) | unsigned   | NO   | PRI | NULL    |       |         |
| [chance](#chance) | float        |            | NO   |     | NULL    |       |         |

## Description of the fields

### guid

DB [GUID](creature.md#guid) of the creature.

### id

Alternative [creature ID](creature_template.md#entry).

### chance

Chance to roll this creature ID. Has to be greater than 0 and less than or equal to 100. If no creature ID is rolled the [original ID](creature.md#id) in the "creature" table is used (together with the "[modelid](creature.md#modelid)" to ensure backward compatibility). If all chances for a GUID sum up to 100 the original ID will never be used, so it is best to keep them below 100.

### Additional notes

- The creature ID is rolled before the creature is created and will also override ZoneScript::GetCreatureEntry (take care if using this for instanced maps).
- The creature ID is also rolled on respawn for non-instanced maps.
