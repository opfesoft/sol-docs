Skipped AC commits (just as a reminder and documentation):

| commit       | date       | comment |
|--------------|------------|---------|
| sol@fecba9f2 | 2020-05-17 | not needed as MySQL is not supported by Sol |
| sol@dca02598 | 2020-05-16 | installer script |
| sol@4a402d6d | 2020-05-14 | follow-up sol@807005ae |
| sol@807005ae | 2020-05-14 | no need to rename the GM command "explorecheat" |
| sol@6e70b962 | 2020-05-14 | follow-up sol@7d7cedd1 |
| sol@7d7cedd1 | 2020-05-14 | the quest chain is already broken because quest 6804 (Poisoned Water) is missing in "creature\_queststarter", no need to remove the whole quest chain |
| sol@1aab9b1b | 2020-05-13 | follow-up sol@ee81b7c8 |
| sol@ee81b7c8 | 2020-05-13 | follow-up sol@74e0f002 |
| sol@74e0f002 | 2020-05-13 | not needed and on top of that takes away the option to create "hidden" quests (quests without quest marker); even if it is not used on retail it can be used for custom content |
| sol@db45f79c | 2020-05-12 | not needed |
| sol@fede473a | 2020-05-11 | follow-up sol@397c5d91 |
| sol@4266d1f7 | 2020-05-07 | CI |
| sol@49cff4ab | 2020-04-26 | follow-up sol@fe1815d4 |
| sol@fe1815d4 | 2020-04-26 | SQL script has been reworked, see sol@fa480f63; the original script will delete existing NPCs on other maps and also contains many other bugs |
| sol@5f2f68c5 | 2020-04-23 | CI |
| sol@9cc5bcc1 | 2020-04-23 | CI |
| sol@cee55da4 | 2020-04-22 | CI |
| sol@fe5b46f3 | 2020-04-21 | not needed, the Ragefire Shaman is working correctly; actually this commit is a regression: Lightning Bolt does not prevent combat movement anymore and is not interrupted by Healing Wave |
| sol@13979719 | 2020-04-19 | CI |
| sol@2514f8fc | 2020-04-18 | not needed, may be taken over later if it is actually used anywhere |
| sol@f381bd47 | 2020-04-17 | not needed, may be taken over later if it is actually used anywhere |
| sol@6a410efa | 2020-04-17 | not needed, may be taken over later if it is actually used anywhere |
| sol@8aa80eef | 2020-04-16 | not needed, may be taken over later if it is actually used anywhere |
| sol@9174e1eb | 2020-04-08 | follow-up sol@2abde9bd |
| sol@2abde9bd | 2020-04-08 | SQL script has been reworked, see sol@83b99ab9 and sol@0c893298 |
| sol@44c3bef1 | 2020-04-05 | follow-up sol@f821b0c7 |
| sol@f821b0c7 | 2020-04-05 | SQL script has been reworked, see sol@3568b8f6 |
| sol@d22251bc | 2020-04-04 | split into 2 commits: 1. contains the actual change, 2. contains sol@ea709de5 and its fix; see sol@bc224cdb and sol@1db927b3 |
| sol@378cd6fe | 2020-04-04 | spell "Silenced - You can only chat with GMs." not needed (could also use GM command "mute") |
| sol@397c5d91 | 2020-04-02 | follow-up sol@9d0ebcd8 |
| sol@9d0ebcd8 | 2020-04-02 | unnecessary change to table "battleground\_template" |
| sol@cfdbf00a | 2020-04-01 | only needed for mod-learn-spells |
| sol@ea709de5 | 2020-03-31 | bugged (SQL scripts getting added multiple times) |
| sol@f9f3efe0 | 2020-03-29 | follow-up sol@ccb1d813 |
| sol@ccb1d813 | 2020-03-29 | SQL script has been reworked, see sol@54318d8f |
| sol@b868f0ad | 2020-03-24 | revert sol@0521a314 |
| sol@0521a314 | 2020-03-21 | bugged |
| sol@2eeab4c7 | 2020-03-08 | git-tools update |
| sol@ed4d95f9 | 2020-03-06 | readme update |
| sol@7aad1743 | 2020-03-05 | readme update |
| sol@59e00ad1 | 2020-03-01 | follow-up sol@857e7992 |
| sol@857e7992 | 2020-03-01 | unnecessary change to the old "demorph" GM command |
