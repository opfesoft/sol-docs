# quest\_mail\_sender

**The \`quest\_mail\_sender\` table**

This table contains the quest and creature IDs which are used if a quest reward is sent by mail, see [quest\_template\_addon.RewardMailTemplateID](quest_template_addon.md#rewardmailtemplateid).

**Structure**

| Field                                               | Type   | Attribute | Key | Null | Default | Extra | Comment |
|-----------------------------------------------------|--------|-----------|-----|------|---------|-------|---------|
| [QuestId](quest_template.md#id)                     | int(5) | unsigned  | PRI | NO   | 0       |       |         |
| [RewardMailSenderEntry](creature_template.md#entry) | int(5) | unsigned  |     | NO   | 0       |       |         |
