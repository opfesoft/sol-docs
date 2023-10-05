# spell\_threat

This table holds threat values on all spells that should either give or take away threat.

## Structure

| Field    | Type         | Attributes | Key | Null | Default | Extra | Comment |
|----------|--------------|------------|-----|------|---------|-------|---------|
| entry    | mediumint(8) | unsigned   | PRI | NO   | NULL    |       | Spell ID |
| flatMod  | int(11)      |            |     | YES  | NULL    |       | Flat threat value that this spell should add to the caster (or take away if it is negative) |
| pctMod   | float        |            |     | NO   | 1       |       | Threat multiplier for damage/healing |
| apPctMod | float        |            |     | NO   | 0       |       | Additional threat bonus from attack power |

