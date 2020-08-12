Skipped AC commits (just as a reminder and documentation):

| commit       | date       | comment |
|--------------|------------|---------|
| sol@c83c53e7 | 2020-08-12 | follow-up sol@3ddfb568 |
| sol@3ddfb568 | 2020-08-12 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@0e1713d1 | 2020-08-11 | already fixed, see sol@206577b8 |
| sol@d5079353 | 2020-08-10 | follow-up sol@96dc9fc0 |
| sol@96dc9fc0 | 2020-08-10 | TODO: use gossip menu ids in the "npc\_taxi" CreatureScript, no need to move the logic into the DB |
| sol@e00ae680 | 2020-08-09 | follow-up sol@f398fd22 |
| sol@f398fd22 | 2020-08-09 | not needed, see [comment](#dmg_boss) below |
| sol@205409ec | 2020-08-09 | follow-up sol@455ce5f0 |
| sol@455ce5f0 | 2020-08-09 | not needed |
| sol@0580ac08 | 2020-08-08 | follow-up sol@ca8dbc39 |
| sol@ca8dbc39 | 2020-08-08 | not needed, see [comment](#dmg_boss) below |
| sol@cdb49996 | 2020-08-06 | not needed |
| sol@ad6ad094 | 2020-08-06 | not needed |
| sol@a37ea1b6 | 2020-08-05 | Sol uses 80 as default GM.StartLevel (see sol@2c6e5432) |
| sol@83d5d9dc | 2020-08-03 | follow-up sol@4e764850 |
| sol@4e764850 | 2020-08-03 | wrong, "amount" has to stay signed integer: amount -1 means that the item is removed from the inventory, so if deleting the DB entry for item 40582 it will actually be added to the inventory because it is contained in the DBC |
| sol@3f1adefb | 2020-08-02 | follow-up sol@e949ab27 |
| sol@e949ab27 | 2020-08-02 | TODO: rework SQL script (wrong / obsolete texts) |
| sol@fcaf91b8 | 2020-07-30 | already implemented, see sol@dc6a4411 |
| sol@91bbbf08 | 2020-07-28 | not needed |
| sol@e3a81ad1 | 2020-07-26 | follow-up sol@a6a9cfbb |
| sol@a6a9cfbb | 2020-07-26 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@b9ff7eb0 | 2020-07-25 | follow-up sol@049299ca |
| sol@049299ca | 2020-07-25 | not needed, see [comment](#dmg_boss) below |
| sol@99dd2689 | 2020-07-24 | follow-up sol@3b911f7f |
| sol@3b911f7f | 2020-07-24 | not needed, see [comment](#dmg_boss) below |
| sol@16c20c96 | 2020-07-23 | follow-up sol@e8fa3720 |
| sol@e8fa3720 | 2020-07-23 | TODO: verify and rework SAI |
| sol@e428f0d6 | 2020-07-22 | follow-up sol@833611f1 |
| sol@833611f1 | 2020-07-22 | not needed |
| sol@3cce4446 | 2020-07-21 | follow-up sol@ab01adbb |
| sol@ab01adbb | 2020-07-21 | TODO: verify and rework SAI |
| sol@24e7e8cf | 2020-07-21 | follow-up sol@8449a0b0 |
| sol@8449a0b0 | 2020-07-21 | TODO: verify and rework SAI |
| sol@d735e225 | 2020-07-20 | macOS |
| sol@39f2d13f | 2020-07-19 | wrong, see [comment](#combat_with_zone) below |
| sol@49e4ae7e | 2020-07-17 | follow-up sol@a62f29fe |
| sol@a62f29fe | 2020-07-17 | wrong, see [comment](#combat_with_zone) below |
| sol@6bf93eb8 | 2020-07-16 | readme |
| sol@abb2d99b | 2020-07-15 | follow-up sol@f73bd8b2 |
| sol@f73bd8b2 | 2020-07-15 | already fixed, see sol@037c5762 |
| sol@0d9e52d8 | 2020-07-14 | follow-up sol@a0737047 |
| sol@a0737047 | 2020-07-14 | TODO: verify and rework SAI |
| sol@e359cb00 | 2020-07-13 | follow-up sol@26dcedd7 |
| sol@26dcedd7 | 2020-07-13 | TODO: verify and rework SAI |
| sol@2fb9985a | 2020-07-12 | follow-up sol@41c8a116 |
| sol@41c8a116 | 2020-07-12 | TODO: verify and rework SAI |
| sol@a0b00be5 | 2020-07-07 | follow-up sol@6d460c54 |
| sol@6d460c54 | 2020-07-07 | TODO: verify and rework SAI |
| sol@b9adeba2 | 2020-07-07 | not needed |
| sol@f9d6711b | 2020-07-06 | not needed |
| sol@12c00e91 | 2020-07-06 | Windows |
| sol@aeab506f | 2020-07-03 | follow-up sol@3dbd0181 |
| sol@3dbd0181 | 2020-07-03 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@e225ba26 | 2020-07-02 | follow-up sol@b5004b31 |
| sol@b5004b31 | 2020-07-02 | not needed, see [comment](#dmg_boss) below |
| sol@df637282 | 2020-07-01 | follow-up sol@d7afa142 |
| sol@d7afa142 | 2020-07-01 | not needed, see [comment](#dmg_boss) below |
| sol@8968039a | 2020-07-01 | follow-up sol@849edc24 |
| sol@849edc24 | 2020-07-01 | TODO: verify and rework DB script |
| sol@94a62654 | 2020-06-29 | follow-up sol@ce7fa544 |
| sol@ce7fa544 | 2020-06-29 | not needed, see [comment](#dmg_boss) below |
| sol@6332fd95 | 2020-06-27 | follow-up sol@7d54d191 |
| sol@7d54d191 | 2020-06-27 | not needed, see [comment](#dmg_boss) below |
| sol@7b56b2bb | 2020-06-27 | follow-up sol@3fe41b1d |
| sol@3fe41b1d | 2020-06-27 | not needed, see [comment](#dmg_boss) below |
| sol@64dbdd96 | 2020-06-25 | follow-up sol@f1b266f4 |
| sol@f1b266f4 | 2020-06-25 | not needed, see [comment](#dmg_boss) below |
| sol@257a5308 | 2020-06-24 | follow-up sol@9410e409 |
| sol@9410e409 | 2020-06-24 | TODO: verify and rework SAI |
| sol@20c7da23 | 2020-06-23 | follow-up sol@255989c1 |
| sol@255989c1 | 2020-06-23 | TODO: verify and rework SAI |
| sol@039fe10a | 2020-06-22 | GitHub issue template |
| sol@cae81a95 | 2020-06-19 | follow-up sol@0b35a240 |
| sol@0b35a240 | 2020-06-19 | not needed, see sol@53e48938 |
| sol@fb9eb95f | 2020-06-17 | follow-up sol@444f691e |
| sol@444f691e | 2020-06-17 | TODO: verify and rework SAI |
| sol@383a95f9 | 2020-06-16 | follow-up sol@82dab24a |
| sol@82dab24a | 2020-06-16 | TODO: verify and rework SAI; also reducing the respawn time for rares to 10 minutes is wrong (doesn't make them rare anymore) |
| sol@a12e58b1 | 2020-06-15 | not needed, see sol@206577b8 |
| sol@cccdb0a6 | 2020-06-14 | follow-up sol@55fde9ca |
| sol@55fde9ca | 2020-06-14 | TODO: verify and rework SAI |
| sol@74247183 | 2020-06-13 | follow-up sol@d3e5b5bb |
| sol@d3e5b5bb | 2020-06-13 | SQL script has been reworked, see sol@d11b6f2e |
| sol@49c6a815 | 2020-06-12 | follow-up sol@8ab818d9 |
| sol@8ab818d9 | 2020-06-12 | SQL script has been reworked, see sol@75818b14 |
| sol@bf74a3a0 | 2020-06-12 | follow-up sol@74ce78b2 |
| sol@74ce78b2 | 2020-06-12 | not needed, see [comment](#dmg_boss) below |
| sol@b5e1d93d | 2020-06-11 | follow-up sol@d08d3b22 |
| sol@d08d3b22 | 2020-06-11 | not needed, see [comment](#dmg_boss) below |
| sol@a8658f24 | 2020-06-10 | follow-up sol@d4293f52 |
| sol@d4293f52 | 2020-06-10 | not needed, see [comment](#dmg_boss) below |
| sol@80fd8226 | 2020-06-09 | follow-up sol@46123a38 |
| sol@46123a38 | 2020-06-09 | not needed, see [comment](#dmg_boss) below |
| sol@f860d49d | 2020-06-08 | follow-up sol@aee070b8 |
| sol@aee070b8 | 2020-06-08 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@441c02a4 | 2020-06-07 | follow-up sol@83e46e20 |
| sol@83e46e20 | 2020-06-07 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@3282ae8e | 2020-06-07 | follow-up sol@88590fe3 |
| sol@88590fe3 | 2020-06-07 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@78995f97 | 2020-06-06 | follow-up sol@2fc109a1 |
| sol@2fc109a1 | 2020-06-06 | not needed, see [comment](#dmg_boss) below |
| sol@a67dd974 | 2020-06-06 | follow-up sol@3ed778df |
| sol@3ed778df | 2020-06-06 | not needed, see [comment](#dmg_boss) below |
| sol@0550a8d5 | 2020-06-05 | follow-up sol@ac355433 |
| sol@ac355433 | 2020-06-05 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@c98c6452 | 2020-06-04 | follow-up sol@9bd47bd5 |
| sol@9bd47bd5 | 2020-06-04 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@f4953cc1 | 2020-06-04 | follow-up sol@ece33e4c |
| sol@ece33e4c | 2020-06-04 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@bdd1c331 | 2020-06-04 | follow-up sol@6c727805 |
| sol@6c727805 | 2020-06-04 | not needed, see [comment](#dmg_boss) below |
| sol@c208a121 | 2020-06-03 | CI |
| sol@5a0a12c6 | 2020-06-02 | could be dangerous because some scripted spells could cause issues if used in the wrong context (even crashing the server) |
| sol@3526d3af | 2020-06-02 | CI |
| sol@7c0cc3cf | 2020-06-02 | not needed, see sol@206577b8 |
| sol@5fb235ff | 2020-06-01 | Sol doesn't support Eluna |
| sol@7c1da6c5 | 2020-06-01 | CI |
| sol@b64e20c8 | 2020-06-01 | follow-up sol@fa805a29 |
| sol@fa805a29 | 2020-06-01 | not needed, see [comment](#dmg_boss) below |
| sol@468398d5 | 2020-05-31 | MySQL / Windows |
| sol@c92d9b92 | 2020-05-31 | follow-up sol@50484427 |
| sol@50484427 | 2020-05-31 | not needed, see [comment](#dmg_boss) below |
| sol@2e597c06 | 2020-05-30 | MySQL |
| sol@86f5c914 | 2020-05-29 | MySQL |
| sol@408a5152 | 2020-05-29 | follow-up sol@00ce59d2 |
| sol@00ce59d2 | 2020-05-29 | not needed, see [comment](#dmg_boss) below |
| sol@d1e83f6e | 2020-05-28 | follow-up sol@027c42fd |
| sol@027c42fd | 2020-05-28 | not needed, "tele" command is good enough |
| sol@428133dc | 2020-05-26 | MySQL |
| sol@72614dd0 | 2020-05-26 | docker |
| sol@6c7184b2 | 2020-05-25 | follow-up sol@c50131fa |
| sol@c50131fa | 2020-05-25 | not needed (<a name="dmg_boss"></a>Sol uses another damage calculation, see sol@d41fae5c; type\_flag "CREATURE\_TYPEFLAGS\_BOSS" is wrong here, it is meant for raid bosses as can be seen in old videos) |
| sol@8e2e27d3 | 2020-05-25 | docker |
| sol@1fc82e7f | 2020-05-24 | docker |
| sol@f7278844 | 2020-05-24 | docker |
| sol@c7f4204d | 2020-05-23 | already fixed, see sol@1d0de3ec |
| sol@92442cfb | 2020-05-22 | follow-up sol@2c4ffc19 |
| sol@2c4ffc19 | 2020-05-22 | not needed, see sol@d579b3f4 and sol@b9a142c6 |
| sol@dca4fd3d | 2020-05-22 | MySQL |
| sol@9745fc52 | 2020-05-21 | follow-up sol@a1644ed8 |
| sol@a1644ed8 | 2020-05-21 | SQL script has been reworked, see sol@7c23067c |
| sol@8b7530b9 | 2020-05-20 | follow-up sol@275c6e79 |
| sol@275c6e79 | 2020-05-20 | not needed, see sol@c0b30b28 |
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
| sol@2514f8fc | 2020-04-18 | not needed, may be taken over later if it is actually used anywhere (double-check for bugs!) |
| sol@f381bd47 | 2020-04-17 | not needed and also uses a <a name="combat_with_zone"></a>wrong logic: "SMART\_ACTION\_SET\_IN\_COMBAT\_WITH\_ZONE" is meant to be used with targeted creatures, not with the script holder |
| sol@6a410efa | 2020-04-17 | not needed, may be taken over later if it is actually used anywhere (double-check for bugs!) |
| sol@8aa80eef | 2020-04-16 | not needed, may be taken over later if it is actually used anywhere (double-check for bugs!) |
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
