# QuestFactionReward

**QuestFactionReward.dbc**

This DBC contains the most often used values of reputation rewarded by quests. If a quest doesn't have [RewardFactionValueIdOverride](../db/world/quest_template.md#rewardfactionvalueidoverride) filled in, reputation is looked up in QuestFactionReward.dbc. Absolute value X of [RewardFactionValueId](../db/world/quest_template.md#rewardfactionvalueid) gives the RepX column of this DBC. For positive RewardFactionValueId the first line in DBC is used, for negative RewardRepValueId, the second line is used.

**Version is : 3.3.5a**

## Structure

|  Field Nb  |  Name  |  Type  |
| --- | --- | --- |
|  1  |  ID  |  Int  |
|  2  |  Rep0  |  Int  |
|  3  |  Rep1  |  Int  |
|  4  |  Rep2  |  Int  |
|  5  |  Rep3  |  Int  |
|  6  |  Rep4  |  Int  |
|  7  |  Rep5  |  Int  |
|  8  |  Rep6  |  Int  |
|  9  |  Rep7  |  Int  |
|  10  |  Rep8  |  Int  |
|  11  |  Rep9  |  Int  |

## Content

|  Id  |  Rep0  |  Rep1  |  Rep2  |  Rep3  |  Rep4  |  Rep5  |  Rep6  |  Rep7  |  Rep8  |  Rep9  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  1  |  0  |  10  |  25  |  75  |  150  |  250  |  350  |  500  |  1000  |  5  |
|  2  |  0  |  -10  |  -25  |  -75  |  -150  |  -250  |  -350  |  -500  |  -1000  |  -5  |
