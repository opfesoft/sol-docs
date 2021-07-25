# creature\_questitem

## Structure

| Field                           | Type        | Attributes | Null | Key | Default | Extra | Comment |
|---------------------------------|-------------|------------|------|-----|---------|-------|---------|
| [CreatureEntry](#creatureentry) | int(10)     | unsigned   | NO   | PRI | 0       |       |         |
| [Idx](#idx)                     | int(10)     | unsigned   | NO   | PRI | 0       |       |         |
| [ItemId](#itemid)               | int(10)     | unsigned   | NO   |     | 0       |       |         |
| [VerifiedBuild](#verifiedbuild) | smallint(5) |            | NO   |     | 0       |       |         |

## Description of the fields

### CreatureEntry

Entry ID of a creature that drops quest items when the related quest is active. See [creature_template.entry](creature_template.md#entry)

### Idx

Index

### ItemId

Entry ID of an item that can be looted from the creature when the related quest is active. See [item_template.entry](item_template.md#entry)

### VerifiedBuild

This field was used to determine whether a template has been verified from WDB files.

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is -Client Build then it was parsed with WDB files from that specific [client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist") and manually edited later for some special necessity.
