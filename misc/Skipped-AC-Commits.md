Skipped AC commits (just as a reminder and documentation; not counting the pending SQL imports which follow each SQL update):<br>
(2020-09-09: Stopped tracking all commits, as Sol follows its own development path and also too many bugs make their way into AC; only track interesting commits as "[TODOs](TODO.md)" which have to be further verified or reworked)

| commit       | date       | comment |
|--------------|------------|---------|
| sol@438cde6a | 2020-09-08 | already fixed: sol@0a9f517a |
| sol@2ed607e5 | 2020-09-08 | docs |
| sol@4a9476bb | 2020-09-08 | ACE removal not needed |
| sol@156b0e41 | 2020-09-07 | not needed as AC commit sol@833611f1 was not taken over by Sol |
| sol@4dd9b927 | 2020-09-07 | ACE removal not needed |
| sol@879f3c0c | 2020-09-07 | not needed |
| sol@b164fea2 | 2020-09-06 | not needed |
| sol@cceb9086 | 2020-09-06 | GitHub |
| sol@b95c14f9 | 2020-09-06 | already fixed: sol@0a9f517a |
| sol@af2ada0d | 2020-09-06 | not needed |
| sol@07a3f93c | 2020-09-05 | not needed |
| sol@f6763549 | 2020-09-05 | wrong: only need to hide the heroic attempt message on normal difficulty, otherwise this will also hide the Blood Quickening Timer; fixed: sol@86d1a532 |
| sol@e68962f5 | 2020-09-05 | not needed |
| sol@9d381fa0 | 2020-09-05 | already fixed: sol@0a9f517a |
| sol@92d2c4c6 | 2020-09-04 | not needed |
| sol@fa6f814e | 2020-09-04 | already fixed: sol@0a9f517a |
| sol@0c2dce03 | 2020-09-04 | GitHub |
| sol@cc3c2ada | 2020-09-04 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@e9c805a7 | 2020-09-04 | not needed |
| sol@7a4a409c | 2020-09-04 | not needed, works correctly on Sol (various bugs were introduced with AC commit sol@fe1815d4 which was not taken over by Sol; Sol fix: sol@fa480f63) |
| sol@1e2ebb3f | 2020-09-03 | CI |
| sol@29410b53 | 2020-09-03 | not needed |
| sol@c6b2b4c3 | 2020-09-03 | CI |
| sol@5244b8d7 | 2020-09-03 | not needed |
| sol@a51c865a | 2020-09-03 | GitHub |
| sol@e06dd5b1 | 2020-09-02 | CI |
| sol@29f2c2ae | 2020-09-02 | not needed, can be accomplished using SAI (see SMART\_ACTION\_MUSIC); TODO: create appropriate SAI scripts |
| sol@2fc95675 | 2020-09-02 | not needed, see [comment](#dmg_boss) below |
| sol@d0958c76 | 2020-09-02 | docker |
| sol@41abcfbe | 2020-09-02 | docs |
| sol@37248474 | 2020-09-01 | docs |
| sol@a07c2b39 | 2020-09-01 | TODO: verify and rework SAI |
| sol@34d9998c | 2020-08-31 | TODO: verify and rework SAI |
| sol@bbb4af34 | 2020-08-31 | CI |
| sol@0ff3f84f | 2020-08-31 | CI |
| sol@f11ddc65 | 2020-08-31 | CI |
| sol@1f89282b | 2020-08-31 | not needed |
| sol@38903b5d | 2020-08-31 | docs |
| sol@3a56cdbd | 2020-08-30 | replacing the creature ID leads to several bugs (e.g. cannot turn in the quest "Muradin's Lament" anymore); fixed in sol@3e1253b2 |
| sol@5fd404de | 2020-08-29 | TODO: verify and rework SAI |
| sol@6f86643e | 2020-08-29 | TODO: verify and rework SAI |
| sol@2a6a5e48 | 2020-08-29 | TODO: verify and rework SAI |
| sol@21fb494d | 2020-08-28 | TODO: verify and rework SAI |
| sol@cb860e8e | 2020-08-28 | TODO: verify and rework SAI |
| sol@fd517414 | 2020-08-28 | TODO: verify and rework SAI |
| sol@d7a758e3 | 2020-08-27 | CI |
| sol@68bd9985 | 2020-08-27 | TODO: verify and rework SAI |
| sol@e6b49e4a | 2020-08-26 | TODO: verify and rework SAI |
| sol@d8ad0c52 | 2020-08-26 | wrong: the ability to refresh "Living Bomb" was introduced with patch 4.0.1 |
| sol@9d5bbaf2 | 2020-08-26 | not needed, see [comment](#dmg_boss) below |
| sol@a9b90c9a | 2020-08-25 | ACE removal not needed |
| sol@9bf66931 | 2020-08-25 | TODO: verify and rework SAI |
| sol@c79a4757 | 2020-08-24 | wrong, see [comment](#combat_with_zone) below |
| sol@78a02c8f | 2020-08-23 | better solution implemented, see sol@5aa37a16 |
| sol@5bac46bb | 2020-08-23 | not needed (there is nothing wrong with Boahn's loot) |
| sol@77b7a20f | 2020-08-22 | not needed (the bug was introduced with AC commit sol@833611f1 which was not taken over by Sol) |
| sol@a5c301a2 | 2020-08-22 | wrong, as the SQL script updates on 'guid' instead of 'id'; fixed in sol@caff0d30 |
| sol@1dd9965d | 2020-08-21 | CI |
| sol@2ad98c57 | 2020-08-21 | CI |
| sol@ed8ed175 | 2020-08-21 | not needed |
| sol@70bdba83 | 2020-08-20 | not needed |
| sol@73d72531 | 2020-08-20 | not needed |
| sol@5d284f02 | 2020-08-20 | not needed |
| sol@07c9debb | 2020-08-19 | CI |
| sol@2bc832ef | 2020-08-19 | not needed; clang warnings already fixed, see sol@37244e4d, sol@206577b8 |
| sol@3f8abc6b | 2020-08-19 | no need to move SAI to CreatureScript; the CreatureScript is also not using the correct Heroic spells (the TC version taken over here is very old) |
| sol@fae5753f | 2020-08-19 | not needed |
| sol@106f6f94 | 2020-08-19 | TODO: Rework SQL script as this one is buggy (e.g. no gameobject GUID specified); also Yor's SAI can be easily improved (no need to write a CreatureScript) |
| sol@1854a3a3 | 2020-08-18 | CI |
| sol@9e5c3f78 | 2020-08-18 | unit tests |
| sol@da61bf3a | 2020-08-17 | unit tests |
| sol@da1725cf | 2020-08-17 | unit tests |
| sol@408366f3 | 2020-08-17 | not needed |
| sol@8b9cec62 | 2020-08-16 | not needed |
| sol@95dff359 | 2020-08-15 | CI / docker |
| sol@c2b40b12 | 2020-08-15 | unit tests not needed |
| sol@f754c008 | 2020-08-15 | TODO: verify and rework SAI |
| sol@8b57a3e2 | 2020-08-13 | TODO: verify and rework SAI |
| sol@d2cc3fcb | 2020-08-13 | Docker not needed; other improvements already implemented, see sol@206577b8 |
| sol@3ddfb568 | 2020-08-12 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@0e1713d1 | 2020-08-11 | already fixed, see sol@206577b8 |
| sol@96dc9fc0 | 2020-08-10 | TODO: use gossip menu ids in the "npc\_taxi" CreatureScript, no need to move the logic into the DB |
| sol@f398fd22 | 2020-08-09 | not needed, see [comment](#dmg_boss) below |
| sol@455ce5f0 | 2020-08-09 | not needed |
| sol@ca8dbc39 | 2020-08-08 | not needed, see [comment](#dmg_boss) below |
| sol@cdb49996 | 2020-08-06 | not needed |
| sol@ad6ad094 | 2020-08-06 | not needed |
| sol@a37ea1b6 | 2020-08-05 | Sol uses 80 as default GM.StartLevel (see sol@2c6e5432) |
| sol@4e764850 | 2020-08-03 | wrong, "amount" has to stay signed integer: amount -1 means that the item is removed from the inventory, so if deleting the DB entry for item 40582 it will actually be added to the inventory because it is contained in the DBC |
| sol@e949ab27 | 2020-08-02 | TODO: rework SQL script (wrong / obsolete texts) |
| sol@fcaf91b8 | 2020-07-30 | already implemented, see sol@dc6a4411 |
| sol@91bbbf08 | 2020-07-28 | not needed |
| sol@a6a9cfbb | 2020-07-26 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@049299ca | 2020-07-25 | not needed, see [comment](#dmg_boss) below |
| sol@3b911f7f | 2020-07-24 | not needed, see [comment](#dmg_boss) below |
| sol@e8fa3720 | 2020-07-23 | TODO: verify and rework SAI |
| sol@833611f1 | 2020-07-22 | not needed |
| sol@ab01adbb | 2020-07-21 | TODO: verify and rework SAI |
| sol@8449a0b0 | 2020-07-21 | TODO: verify and rework SAI |
| sol@d735e225 | 2020-07-20 | macOS |
| sol@39f2d13f | 2020-07-19 | wrong, see [comment](#combat_with_zone) below |
| sol@a62f29fe | 2020-07-17 | wrong, see [comment](#combat_with_zone) below |
| sol@6bf93eb8 | 2020-07-16 | readme |
| sol@f73bd8b2 | 2020-07-15 | already fixed, see sol@037c5762 |
| sol@a0737047 | 2020-07-14 | TODO: verify and rework SAI |
| sol@26dcedd7 | 2020-07-13 | TODO: verify and rework SAI |
| sol@41c8a116 | 2020-07-12 | TODO: verify and rework SAI |
| sol@6d460c54 | 2020-07-07 | TODO: verify and rework SAI |
| sol@b9adeba2 | 2020-07-07 | not needed |
| sol@f9d6711b | 2020-07-06 | not needed |
| sol@12c00e91 | 2020-07-06 | Windows |
| sol@3dbd0181 | 2020-07-03 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@b5004b31 | 2020-07-02 | not needed, see [comment](#dmg_boss) below |
| sol@d7afa142 | 2020-07-01 | not needed, see [comment](#dmg_boss) below |
| sol@849edc24 | 2020-07-01 | TODO: verify and rework DB script |
| sol@ce7fa544 | 2020-06-29 | not needed, see [comment](#dmg_boss) below |
| sol@7d54d191 | 2020-06-27 | not needed, see [comment](#dmg_boss) below |
| sol@3fe41b1d | 2020-06-27 | not needed, see [comment](#dmg_boss) below |
| sol@f1b266f4 | 2020-06-25 | not needed, see [comment](#dmg_boss) below |
| sol@9410e409 | 2020-06-24 | TODO: verify and rework SAI |
| sol@255989c1 | 2020-06-23 | TODO: verify and rework SAI |
| sol@039fe10a | 2020-06-22 | GitHub issue template |
| sol@0b35a240 | 2020-06-19 | not needed, see sol@53e48938 |
| sol@444f691e | 2020-06-17 | TODO: verify and rework SAI |
| sol@82dab24a | 2020-06-16 | TODO: verify and rework SAI; also reducing the respawn time for rares to 10 minutes is wrong (doesn't make them rare anymore) |
| sol@a12e58b1 | 2020-06-15 | not needed, see sol@206577b8 |
| sol@55fde9ca | 2020-06-14 | TODO: verify and rework SAI |
| sol@d3e5b5bb | 2020-06-13 | SQL script has been reworked, see sol@d11b6f2e |
| sol@8ab818d9 | 2020-06-12 | SQL script has been reworked, see sol@75818b14 |
| sol@74ce78b2 | 2020-06-12 | not needed, see [comment](#dmg_boss) below |
| sol@d08d3b22 | 2020-06-11 | not needed, see [comment](#dmg_boss) below |
| sol@d4293f52 | 2020-06-10 | not needed, see [comment](#dmg_boss) below |
| sol@46123a38 | 2020-06-09 | not needed, see [comment](#dmg_boss) below |
| sol@aee070b8 | 2020-06-08 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@83e46e20 | 2020-06-07 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@88590fe3 | 2020-06-07 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@2fc109a1 | 2020-06-06 | not needed, see [comment](#dmg_boss) below |
| sol@3ed778df | 2020-06-06 | not needed, see [comment](#dmg_boss) below |
| sol@ac355433 | 2020-06-05 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@9bd47bd5 | 2020-06-04 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@ece33e4c | 2020-06-04 | not needed, see [comment](#dmg_boss) below; TODO: verify and collect the SAI in a separate commit |
| sol@6c727805 | 2020-06-04 | not needed, see [comment](#dmg_boss) below |
| sol@c208a121 | 2020-06-03 | CI |
| sol@3526d3af | 2020-06-02 | CI |
| sol@7c0cc3cf | 2020-06-02 | not needed, see sol@206577b8 |
| sol@5fb235ff | 2020-06-01 | Sol doesn't support Eluna |
| sol@7c1da6c5 | 2020-06-01 | CI |
| sol@fa805a29 | 2020-06-01 | not needed, see [comment](#dmg_boss) below |
| sol@468398d5 | 2020-05-31 | MySQL / Windows |
| sol@50484427 | 2020-05-31 | not needed, see [comment](#dmg_boss) below |
| sol@2e597c06 | 2020-05-30 | MySQL |
| sol@86f5c914 | 2020-05-29 | MySQL |
| sol@00ce59d2 | 2020-05-29 | not needed, see [comment](#dmg_boss) below |
| sol@027c42fd | 2020-05-28 | not needed, "tele" command is good enough |
| sol@428133dc | 2020-05-26 | MySQL |
| sol@72614dd0 | 2020-05-26 | docker |
| sol@c50131fa | 2020-05-25 | not needed (<a name="dmg_boss"></a>Sol uses another damage calculation, see sol@d41fae5c; type\_flag "CREATURE\_TYPEFLAGS\_BOSS" is wrong here, it is meant for raid bosses as can be seen in old videos) |
| sol@8e2e27d3 | 2020-05-25 | docker |
| sol@1fc82e7f | 2020-05-24 | docker |
| sol@f7278844 | 2020-05-24 | docker |
| sol@c7f4204d | 2020-05-23 | already fixed, see sol@1d0de3ec |
| sol@2c4ffc19 | 2020-05-22 | not needed, see sol@d579b3f4 and sol@b9a142c6 |
| sol@dca4fd3d | 2020-05-22 | MySQL |
| sol@a1644ed8 | 2020-05-21 | SQL script has been reworked, see sol@7c23067c |
| sol@275c6e79 | 2020-05-20 | not needed, see sol@c0b30b28 |
| sol@fecba9f2 | 2020-05-17 | not needed as MySQL is not supported by Sol |
| sol@dca02598 | 2020-05-16 | installer script |
| sol@807005ae | 2020-05-14 | no need to rename the GM command "explorecheat" |
| sol@7d7cedd1 | 2020-05-14 | the quest chain is already broken because quest 6804 (Poisoned Water) is missing in "creature\_queststarter", no need to remove the whole quest chain |
| sol@74e0f002 | 2020-05-13 | not needed and on top of that takes away the option to create "hidden" quests (quests without quest marker); even if it is not used on retail it can be used for custom content |
| sol@db45f79c | 2020-05-12 | not needed |
| sol@4266d1f7 | 2020-05-07 | CI |
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
| sol@2abde9bd | 2020-04-08 | SQL script has been reworked, see sol@83b99ab9 and sol@0c893298 |
| sol@f821b0c7 | 2020-04-05 | SQL script has been reworked, see sol@3568b8f6 |
| sol@d22251bc | 2020-04-04 | split into 2 commits: 1. contains the actual change, 2. contains sol@ea709de5 and its fix; see sol@bc224cdb and sol@1db927b3 |
| sol@378cd6fe | 2020-04-04 | spell "Silenced - You can only chat with GMs." not needed (could also use GM command "mute") |
| sol@9d0ebcd8 | 2020-04-02 | unnecessary change to table "battleground\_template" |
| sol@cfdbf00a | 2020-04-01 | only needed for mod-learn-spells |
| sol@ea709de5 | 2020-03-31 | bugged (SQL scripts getting added multiple times) |
| sol@ccb1d813 | 2020-03-29 | SQL script has been reworked, see sol@54318d8f |
| sol@b868f0ad | 2020-03-24 | revert sol@0521a314 |
| sol@0521a314 | 2020-03-21 | bugged |
| sol@2eeab4c7 | 2020-03-08 | git-tools update |
| sol@ed4d95f9 | 2020-03-06 | readme update |
| sol@7aad1743 | 2020-03-05 | readme update |
| sol@857e7992 | 2020-03-01 | unnecessary change to the old "demorph" GM command |
