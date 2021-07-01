# quest\_offer\_reward\_locale

**The \`quest\_offer\_reward\_locale\` table**

**Structure**

| Field                           | Type        | Attribute | Key | Null | Default | Extra | Comment |
|---------------------------------|-------------|-----------|-----|------|---------|-------|---------|
| [ID](#id)                       | int(10)     | unsigned  | PRI | NO   | 0       |       |         |
| [locale](#locale)               | varchar(4)  |           | PRI | NO   | NULL    |       |         |
| [RewardText](#rewardtext)       | text        |           |     | YES  | NULL    |       |         |
| [VerifiedBuild](#verifiedbuild) | smallint(6) |           |     | NO   | 0       |       |         |

### ID

See [quest\_template.id](quest_template.md#id)

### locale

The language of the text.
Can have 8 values: deDE, esES, esMX, frFR, koKR, ruRU, zhCN, zhTW

### RewardText

Quest gossip text shown when turning in a quest where no item delivery is involved.

### VerifiedBuild

This field was used to determine whether a template has been verified from WDB files.

If value is 0 then it has not been parsed yet.

If value is above 0 then it has been parsed with WDB files from that specific client build.

If value is -1 then it is just a place holder until proper data are found on WDBs.

If value is -Client Build then it was parsed with WDB files from that specific [client build](../auth/realmlist.md#gamebuild "DB:Auth:realmlist") and manually edited later for some special necessity.
