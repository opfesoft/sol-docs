TODOs:

| commit       | date       | done | todo / comment |
|--------------|------------|------|----------------|
| sol@12b195e1 | 2021-10-28 |      | verify/rework SQL script / core scripts; also "The Cleaner" should spawn if a second player character is helping; low prio (obsolete quest) |
| sol@26456132 | 2021-10-26 |      | won't take over, improve the CreatureScript instead |
| sol@31dfe4f0 | 2021-10-26 |      | verify/rework SQL script |
| sol@1f603455 | 2021-10-25 |      | verify issue & changes; low Prio (Hallow's End) |
| sol@3cddfb84 | 2021-10-24 |      | verify changes; low prio (minor issue) |
| sol@416e8d2c | 2021-10-24 | X    | won't take over, use SAI instead; done: sol@9336ee8a |
| sol@96441a91 | 2021-10-24 |      | verify changes; low prio (minor issue) |
| sol@a45abcad | 2021-10-24 | X    | take over from TC instead; done: sol@579b350f |
| sol@a98c4122 | 2021-10-24 |      | verify issue & changes; low Prio (Hallow's End) |
| sol@36aced60 | 2021-10-23 |      | take over if needed (the recipes are largely irrelevant for WotLK and were removed in Cataclysm) |
| sol@73a55e02 | 2021-10-22 |      | verify changes; adapt to Sol if taking over parts of the CreatureScript, perhaps improve the SAI instead; low prio (Dungeon: Stratholme) |
| sol@6baf498a | 2021-10-22 |      | won't take over; according to TC issue 15906 the server side spell 30176 has to be implemented which is triggered periodically setting the PvP state; spells 29894 (Alliance) and 29895 (Horde) are used for the slow effect; low prio (PvP) |
| sol@9bcde70d | 2021-10-22 |      | take over if needed (see TC commit ac62d7156f93bf86f57dbad1f24f14031322fd5a for more information) |
| sol@5d69ce82 | 2021-10-22 | X    | verify loot; compare with TC; done: sol@55453d23 |
| sol@c2381a5a | 2021-10-21 | X    | won't take over, just set the respawn time of the GOs to 2 minutes, this should suffice; done: sol@e5f0e902 |
| sol@6798b907 | 2021-10-21 |      | verify changes; low prio (Dungeon: Blackrock Depths) |
| sol@ad73b564 | 2021-10-21 |      | take over if needed |
| sol@2648157a | 2021-10-21 |      | wrong: deletes the existing SAI script; verify the emotes and adjust the existing SAI; low prio (minor issue) |
| sol@7591491b | 2021-10-21 |      | wrong: deletes the existing SAI script which already included reactions to emotes; verify the emotes and adjust the existing SAI; low prio (minor issue) |
| sol@ddb3cb8d | 2021-10-20 |      | verify/rework SQL script; low prio (Hallow's End) |
| sol@aab110c1 | 2021-10-20 | X    | won't take over, rework existing SAI instead; done: sol@1328f2de |
| sol@08db8361 | 2021-10-20 |      | verify changes; low prio (PvP) |
| sol@1fb6830b | 2021-10-20 | X    | wrong: the QuestMoneyReward DBC was not part of the WotLK client, it was introduced later (according to wowdev at least with MoP); implement another solution, e.g. XP * 0.6 copper should suffice; done: sol@55d8984d |
| sol@51161bb7 | 2021-10-20 |      | verify/rework SQL script; low prio (Hallow's End) |
| sol@fb1e750d | 2021-10-20 |      | take over if needed |
| sol@1ec612e6 | 2021-10-20 |      | take over if needed |
| sol@15494554 | 2021-10-19 |      | verify/rework SQL script |
| sol@e8a6c4fa | 2021-10-18 |      | verify/rework SQL script, CreatureScripts and SpellScripts |
| sol@e5321a9b | 2021-10-18 |      | verify/rework SQL script |
| sol@429823a7 | 2021-10-17 | X    | won't take over; there are many other duplicate critters, instead of deleting the duplicates enable random movement for all of them; done: sol@f8d54d6d |
| sol@5fb43be7 | 2021-10-17 |      | take over from TC instead |
| sol@9aab7e8f | 2021-10-17 |      | use other drop chances and also remove item 9361 from the creature loot table |
| sol@60f0fb2e | 2021-10-17 |      | low prio (Localization: esES, esMX) |
| sol@12185d8f | 2021-10-16 |      | verify issue & changes; low prio (Dungeon: Icecrown Citadel) |
| sol@ba719f0f | 2021-10-16 |      | verify changes; low prio (Hallow's End) |
| sol@4a2846f7 | 2021-10-16 |      | verify/rework SQL script |
| sol@191e37ec | 2021-10-16 | X    | verify issues & changes; update: won't take over: even if this was not the case on retail there's no reason to remove the aura if mounted |
| sol@a56f4fe1 | 2021-10-16 |      | verify loot; compare with TC |
| sol@7a828d3c | 2021-10-15 |      | won't take over, rework SAI instead (use SMART\_ACTION\_ADD\_IMMUNITY) |
| sol@0d05970e | 2021-10-14 | X    | verify changes; update: won't take over, keep the prerequisite according to the quest text, no matter how this was handled on retail |
| sol@8b70222a | 2021-10-14 |      | verify changes; low prio (minor issue) |
| sol@ad320d88 | 2021-10-14 |      | verify/rework SQL script |
| sol@476d085a | 2021-10-14 |      | take over if needed |
| sol@c1203874 | 2021-10-14 |      | verify/rework SQL script |
| sol@4c576ebe | 2021-10-14 |      | verify/rework SQL script |
| sol@5d73180c | 2021-10-14 |      | take over if needed |
| sol@3894dfc8 | 2021-10-14 | X    | verify changes; won't take over, not needed; can be accomplished using SMART\_ACTION\_SET\_GO\_STATE or SMART\_ACTION\_GO\_SET\_LOOT\_STATE combined with timers or respawn time of the GO itself; update: some GOs cannot be despawned this way, so implemented the new SAI action type "SMART\_ACTION\_DESPAWN\_GO", see sol@02025b6c |
| sol@a8643f27 | 2021-10-14 | X    | verify position; use UPDATE instead of DELETE/INSERT; done: sol@297e4ba5 |
| sol@b8345a2f | 2021-10-14 |      | take over if needed |
| sol@21e67bae | 2021-10-13 | X    | verify/rework SQL script; done: sol@7e1e0e93 |
| sol@747a2a4f | 2021-10-13 |      | verify changes; low prio (minor issue) |
| sol@b5f8b485 | 2021-10-13 |      | take over if needed |
| sol@4349f076 | 2021-10-13 |      | verify/rework SQL script |
| sol@cd03fd4e | 2021-10-13 |      | verify/rework SQL script |
| sol@13eacaed | 2021-10-12 |      | take over if needed |
| sol@c8ff0bcc | 2021-10-12 |      | verify changes; low prio (Dungeon: Azjol-Nerub) |
| sol@a6e564be | 2021-10-12 |      | wrong: deletes the existing SAI script which already included reactions to emotes; verify the emotes and adjust the existing SAI; low prio (minor issue) |
| sol@cec360b3 | 2021-10-12 | X    | verify/rework SQL script; done: sol@0145f351 |
| sol@57658d82 | 2021-10-12 |      | take over if needed |
| sol@0f5c8887 | 2021-10-12 |      | verify/rework SQL script |
| sol@dd34d7e1 | 2021-10-10 |      | won't take over, improve event script and SAI for Shy-Rotam instead; also add SAI for Sian-Rotam (see TC version) |
| sol@bd727915 | 2021-10-10 | X    | verify loot; compare with TC; done: sol@ddcd0e52 |
| sol@fd7e4ec6 | 2021-10-10 | X    | verify loot; compare with TC; done: sol@ddcd0e52 |
| sol@f8ac4160 | 2021-10-10 | X    | verify position; use UPDATE instead of DELETE/INSERT; done: sol@c7739684 |
| sol@1b3c8c53 | 2021-10-10 |      | verify/rework SQL script |
| sol@d2fd486a | 2021-10-10 |      | verify/rework SQL script |
| sol@4392da3c | 2021-10-10 |      | wrong: the GO was deleted with AC commit sol@0cccdc4a; check the rotation of this GO after sol@0cccdc4a has been processed |
| sol@8826d7de | 2021-10-10 |      | verify/rework SQL script; compare with TC version |
| sol@261cc87e | 2021-10-10 |      | wrong: deletes the existing SAI script; verify the emotes and adjust the existing SAI; low prio (minor issue) |
| sol@1e3f94fa | 2021-10-10 |      | wrong: deletes the existing SAI script which already included reactions to emotes; verify the emotes and adjust the existing SAI; low prio (minor issue) |
| sol@d8e89eeb | 2021-10-10 | X    | verify loot; compare with TC; done: sol@ddcd0e52 |
| sol@3ff389c1 | 2021-10-10 | X    | verify loot; compare with TC; done: sol@ddcd0e52 |
| sol@44545c65 | 2021-10-10 | X    | verify loot; compare with TC; done: sol@ddcd0e52 |
| sol@ae3dc6c7 | 2021-10-10 |      | verify/rework SQL script (also see sol@8605981a) |
| sol@cc892279 | 2021-10-10 |      | verify/rework SQL script |
| sol@3f541b98 | 2021-10-10 |      | verify/rework SQL script; low prio (minor issue) |
| sol@e503afd0 | 2021-10-10 |      | fix SQL script (deletes wrong GUID range); verify new NPCs; low prio (Hallow's End) |
| sol@d9323336 | 2021-10-10 |      | wrong: deletes the existing SAI script which already included reactions to emotes; verify the emotes and adjust the existing SAI; low prio (minor issue) |
| sol@f96b027f | 2021-10-10 |      | take over if needed (also see bugfix sol@db2b380c) |
| sol@0cccdc4a | 2021-10-10 |      | the GOs are also needed for the "Battle for the Undercity" event; keep the ones with lower GUID and adjust their phasemask accordingly (also see sol@4392da3c); same for GUID 265429 (Wrathgate) |
| sol@7cf0ed0a | 2021-10-09 | X    | verify NPC; update: wrong, won't take over, the gossip option was removed during WotLK and there are more than enough NPCs around selling food and drink |
| sol@00e9cf2c | 2021-10-09 |      | verify/rework SQL script; low prio (Dungeon: Stratholme) |
| sol@9dea0ac5 | 2021-10-09 |      | verify GOs; low prio (Harvest Festival) |
| sol@2c7df906 | 2021-10-08 | X    | verify loot; compare with TC; done: sol@98d00d62 |
| sol@49478876 | 2021-10-08 |      | verify changes; low prio (Brewfest) |
| sol@0afe11c5 | 2021-10-08 |      | verify/rework SQL script; low prio (Brewfest) |
| sol@668f519f | 2021-10-08 |      | verify/rework SQL script |
| sol@c6427103 | 2021-10-08 | X    | verify loot; compare with TC; done: sol@ddcd0e52 |
| sol@2c92e965 | 2021-10-08 |      | verify/rework SQL script |
| sol@cb9f3cbf | 2021-10-08 | X    | delete the GUIDs instead and also remove them from game\_event\_gameobject; done: sol@b506cc3c |
| sol@8514eaf9 | 2021-10-07 |      | verify changes; low prio (Dungeon: Blackrock Depths) |
| sol@99cc4285 | 2021-10-07 |      | verify changes, try to find another solution; low prio (minor issue) |
| sol@a5f5568d | 2021-10-07 |      | verify/rework SQL script |
| sol@261d25e9 | 2021-10-07 |      | verify/rework SQL script (also see bugfix sol@4d1a2b2b |
| sol@665760e0 | 2021-10-07 |      | verify/rework SQL script |
| sol@e7a62102 | 2021-10-07 |      | verify/rework SQL script |
| sol@248baf33 | 2021-10-07 |      | verify/rework SQL script |
| sol@c51fb81d | 2021-10-07 |      | verify changes; low prio (Brewfest) |
| sol@78a2f738 | 2021-10-07 |      | take over if needed |
| sol@c4ebfb44 | 2021-10-07 |      | verify changes; low prio (Brewfest) |
| sol@23f55bbd | 2021-10-07 |      | verify/rework SQL script |
| sol@495ca766 | 2021-10-04 |      | take over if needed |
| sol@0d1f72a5 | 2021-10-04 |      | take over if needed |
| sol@de8d0b49 | 2021-10-04 |      | verify issue & changes |
| sol@cdab63c3 | 2021-10-04 |      | verify/rework SQL script |
| sol@4f5d7888 | 2021-10-03 |      | verify/rework SQL script |
| sol@06e50a96 | 2021-10-03 |      | take over if needed (also contains a second PR, see sol@e094c1ae) |
| sol@ecb92f9d | 2021-10-01 | X    | verify changes & loot, compare with TC; done: sol@f8dba2fc |
| sol@77e46769 | 2021-10-01 |      | verify changes; low prio (Dungeon: Uldaman) |
| sol@0c8fb1ea | 2021-10-01 |      | verify changes; low prio (minor issue) |
| sol@46e17796 | 2021-10-01 |      | verify/rework SQL script |
| sol@ac57e6a4 | 2021-10-01 |      | verify/rework SQL script |
| sol@1dd53b17 | 2021-09-27 | X    | verify/rework SQL script; verify AuraScript; implemented another solution: sol@a7b0e74c |
| sol@5f0da005 | 2021-09-27 | X    | verify issue & changes; update: won't take over because those are world drops; the new Classic & TBC is also not a reference for WotLK |
| sol@87a4e493 | 2021-09-25 | X    | verify issue & changes; update: won't take over, cannot reproduce the issue on Sol |
| sol@e6b1201e | 2021-09-24 |      | not needed, but keep as a reference |
| sol@0c2dbfea | 2021-09-24 |      | verify/rework SQL script |
| sol@115f8ce1 | 2021-09-24 |      | verify changes; verify/rework SQL script; low prio (Brewfest) |
| sol@676bf5c4 | 2021-09-23 | X    | Ridge Huntress (GUID: 6947) already fixed (see sol@87262a3a); the other positions are no improvement, one of them still in the ground (btw: vmangos is not a reference for WotLK, and neither is the new Classic or TBC!); fix the positions for the other 2 creatures; done: sol@4755d3cf |
| sol@0cd88d02 | 2021-09-23 |      | improve SAI script instead |
| sol@c3259dab | 2021-09-21 | X    | verify issue & changes; update: cannot reproduce on Sol; update: implemented PROC\_EX\_ONLY\_FIRST\_TICK: sol@6fcd7c50 |
| sol@048025ce | 2021-09-21 |      | verify changes and check if the SAI scripts could be fixed instead; low prio (Dungeon: Zul'Farrak) |
| sol@1bf4f54b | 2021-09-20 |      | verify changes; low prio (minor issue, also see sol@0d411ec2) |
| sol@47bb5cbb | 2021-09-20 |      | verify changes; low prio (Dungeon: Blackrock Depths) |
| sol@ab599911 | 2021-09-20 |      | verify changes; low prio (minor issue) |
| sol@69b81721 | 2021-09-20 |      | verify/rework SQL script |
| sol@f7c0bfc3 | 2021-09-20 |      | verify/rework SQL script; compare with TC version; remove Zeppit spawn |
| sol@251a2c87 | 2021-09-20 |      | verify/rework SQL script |
| sol@1d5d2de0 | 2021-09-19 |      | verify/rework SQL script |
| sol@f76d08f3 | 2021-09-19 | X    | also remove the parameter "noQuestBonus" as it is not used anymore (always "false"); done: sol@ae21f04f |
| sol@424f22f8 | 2021-09-19 |      | take over the TC version instead |
| sol@6673db40 | 2021-09-19 |      | verify/rework SQL script |
| sol@99b3b0de | 2021-09-19 | X    | bugged and obviously wrong: the quests 364 and 3901 clearly address Forsaken and the update statement for quests 3095, 3096, 3097, 3098, 3099 removes all races, even undead; only fix the "Scroll" quests; done: sol@2df4a50e |
| sol@f2abf6b5 | 2021-09-18 |      | verify/rework SQL script |
| sol@36c0d348 | 2021-09-18 |      | verify/rework SQL script |
| sol@6a55feb5 | 2021-09-18 |      | verify/rework SQL script |
| sol@4fb2dc1f | 2021-09-18 |      | take over if needed |
| sol@a02b9ef7 | 2021-09-17 |      | verify/rework SQL script |
| sol@f6f18cb5 | 2021-09-17 | X    | verify changes; update: wrong, won't take over: according to the 2.0.3 patch notes the combo points should not reset until a combo point is applied to a different target; it does not seem that this has been changed until 3.3.5 |
| sol@6632c4bd | 2021-09-17 |      | verify changes; low prio (Dungeon: Blackwing Lair) |
| sol@5a92947e | 2021-09-16 |      | verify changes; probably not necessary as the pet issue is already fixed, see sol@c4c1acee; low prio (Dungeon: Uldaman) |
| sol@cb790b0d | 2021-09-16 |      | verify changes; low prio (Dungeon: Trial of the Crusader) |
| sol@4dc642d5 | 2021-09-16 |      | take over if needed; also see sol@d464ee70 |
| sol@fd229f75 | 2021-09-16 |      | verify changes; low prio (Dungeon: Blackrock Depths) |
| sol@f1e9b674 | 2021-09-16 |      | verify/rework SQL script |
| sol@7406a01a | 2021-09-13 |      | take over parts if needed, also see sol@107658eb, sol@d6118de1, sol@60fb2c38, sol@3aadaa6d, sol@70257303, sol@89f0c42c, sol@a6a85c0d |
| sol@009ba568 | 2021-09-13 |      | verify/rework SQL script |
| sol@15b34616 | 2021-09-13 |      | verify changes; low prio (Dungeon: Blackrock Depths) |
| sol@bb343b48 | 2021-09-13 |      | verify/rework SQL script |
| sol@adab416f | 2021-09-12 |      | verify issue & changes; low prio (Dungeon: Ulduar) |
| sol@1ae8e7ec | 2021-09-12 | X    | wrong: the correct number of dispelled auras is calculated using EffectDieSides and BasePoints; implement another solution; done: sol@9eebf780 |
| sol@e5b8dbeb | 2021-09-11 |      | verify changes; low prio (PvP) |
| sol@3de6ee6c | 2021-09-09 |      | verify/rework SQL script |
| sol@8f47a6da | 2021-09-07 | X    | contains many bugs, e.g. uses creature ID 15642 (Amani Shadowpriest) instead of 15462 (Spitting Scarab) and decreases(!) reputation for killing mobs which is completely wrong in this case; verify all creature IDs and reputation values; update: also see sol@65737d1e; done: sol@083660c9 |
| sol@f07faedc | 2021-09-07 | X    | won't take over, rework the SAI instead and add better comments; done: sol@83d8b3be |
| sol@1f893f97 | 2021-09-07 | X    | rework the whole quest: Yeh'kinya's Bramble should only be usable near a Vale Screecher or Rogue Vale Screecher corpse; set Screecher Spirit active so it will disappear even if no player is near; improve SAI and SAI comments; done: sol@14bcb1bc |
| sol@2e41da54 | 2021-09-07 |      | take over if needed |
| sol@e9be0483 | 2021-09-07 | X    | verify issue; update: Sol does not seem to be affected by this issue |
| sol@8a13fff5 | 2021-09-07 | X    | it is not necessary to create a new pool, just adjust the existing one: remove GO GUID 14999 from the spawns and the pool and add GUID 6248 to the pool instead; done: sol@599e5bb4 |
| sol@7d7eac01 | 2021-09-07 |      | verify/rework SQL script; low prio (Midsummer Fire Festival) |
| sol@55831fab | 2021-09-07 | X    | contains wrong GUIDs in the comments; also use pool template ID 507 instead (501-506 are similar pools); done: sol@b50280d3 |
| sol@52d9f532 | 2021-09-07 | X    | verify/rework SQL script; implemented another solution: sol@b336ba97 |
| sol@02b0b29f | 2021-09-06 |      | verify changes; low prio (minor issue) |
| sol@50991bdc | 2021-09-05 |      | take over if needed; could cause several side effects |
| sol@f5ef1220 | 2021-09-04 | X    | verify changes and check the creatures in the area; done: sol@2307963c |
| sol@6ed71767 | 2021-09-04 |      | keep as reference; take over single values if needed; won't blindly take over such mass updates |
| sol@d8b3df09 | 2021-09-04 |      | low prio (Localization: zhCN) |
| sol@49348256 | 2021-09-03 | X    | verify changes and check the creatures in the area; done: sol@4de06bf3 |
| sol@392319ab | 2021-09-03 | X    | verify quest chain and issue; won't take over, improve the whole quest chain instead: sol@61dd64c8 |
| sol@37c72c17 | 2021-09-03 | X    | wrong: just delete the second Healing Wave because the first one already affects the creature itself; done: sol@dbcdc006 |
| sol@2f9f9522 | 2021-09-02 |      | take over if needed (also see sol@066d2ef8) |
| sol@dd0b964a | 2021-09-01 |      | verify changes; low prio (Midsummer Fire Festival) |
| sol@9d17889b | 2021-09-01 | X    | verify/rework SQL script; compare with TC version; done: sol@f0b97068 |
| sol@332e3e1b | 2021-09-01 |      | verify changes; pooling does not work for instanced maps, handle this via InstanceScript (e.g. similar to sol@95675ffb); low prio (Dungeon: Stratholme) |
| sol@febdb592 | 2021-09-01 | X    | won't take over, just set the drop chances to 5% for all creatures; Ur'dan should not drop the key; done: sol@22347fee |
| sol@568fad6d | 2021-09-01 |      | verify/rework SQL script; low prio (Midsummer Fire Festival) |
| sol@6386acd8 | 2021-09-01 | X    | verify/rework SQL script; done: sol@8bb78824 |
| sol@a0d9cd7f | 2021-09-01 | X    | verify/rework SQL script; done: sol@c81159a5 |
| sol@c27b2391 | 2021-09-01 | X    | only enable random movement (increase radius); also decrease walking speed; done: sol@5cf51ed0 |
| sol@498faf38 | 2021-09-01 |      | verify changes (also see sol@1c77d8a9); low prio (Dungeons) |
| sol@48e09fda | 2021-08-31 |      | verify/rework SQL script |
| sol@bfaa32f2 | 2021-08-31 |      | verify changes; low prio (Dungeons) |
| sol@33b3ea2f | 2021-08-31 | X    | verify/rework SQL script; don't remove text id 3297 for the gossip menu, use a condition to show 2598 only if the quest has not been completed yet; done: sol@c5251554 |
| sol@bf18c770 | 2021-08-30 | X    | verify/rework SQL script; done: sol@72e90723 |
| sol@6978d624 | 2021-08-29 |      | verify changes and adapt to Sol; low prio (GM command) |
| sol@93466e58 | 2021-08-26 | X    | verify changes and check the creatures in the area (including the critters); done: sol@f1c38f92 |
| sol@96addc67 | 2021-08-26 | X    | verify/rework SQL script; done: sol@be258dbb |
| sol@45218224 | 2021-08-26 |      | take over if needed |
| sol@f23d42c0 | 2021-08-26 |      | take over if needed |
| sol@bef68244 | 2021-08-25 | X    | verify/rework SQL script; done: sol@24d334e0 |
| sol@f039ccc3 | 2021-08-25 | X    | verify/rework SQL script; done: sol@75afe154 |
| sol@a8c0a2cc | 2021-08-25 |      | take over if needed (could probably cause performance issues; see also bugfix sol@c1119553) |
| sol@015f8802 | 2021-08-25 |      | won't take over, fix CreatureScript instead (bosses use their own AI); low prio (Dungeon: Lower Blackrock Spire) |
| sol@8c06c1ed | 2021-08-24 | X    | verify/rework SQL script; implemented another solution and improved the quest "Control": sol@b3a6e620 |
| sol@032ca32a | 2021-08-24 |      | does not seem to work, find another solution; low prio (minor issue) |
| sol@940c30a1 | 2021-08-24 | X    | verify changes and check the creatures in the area; done: sol@b1eba7fd |
| sol@ec71301b | 2021-08-24 |      | won't take over; try to find a generic solution as spells like "Rain of Fire" are also affected; low prio as this is just a minor issue |
| sol@7ed0daa9 | 2021-08-24 | X    | verify/rework SQL script; update: won't take over, random movement looks much better; also the WP paths in this commit are basically all the same |
| sol@1b7d3708 | 2021-08-24 |      | verify issue & changes; take over if needed |
| sol@52b78360 | 2021-08-24 | X    | verify/rework SQL script; check every ore location; low prio; done: sol@3ae3f2fa |
| sol@c774899e | 2021-08-24 | X    | use UPDATE instead of DELETE/INSERT; update: won't take over, take over the TC version instead (see TC commit 513cbd289a9b6ac6c120c5f93a5b18f4cc04693e); done: sol@016ef950 |
| sol@1e50a902 | 2021-08-24 | X    | verify/rework SQL script; use GroupId 1 for entry 11497; done: sol@c34de090 |
| sol@690187cb | 2021-08-22 |      | won't take over, fix CreatureScript instead (bosses use their own AI); low prio (Dungeon: Lower Blackrock Spire) |
| sol@5f678053 | 2021-08-22 |      | try to find another solution as this one looks awkward; low prio as this is just a minor issue |
| sol@26cc8c4f | 2021-08-21 | X    | use other position; done: sol@fdaed852 |
| sol@e9f4006e | 2021-08-21 |      | verify changes; low prio (Dungeon: Ulduar) |
| sol@4cc00f54 | 2021-08-20 |      | won't take over, fix CreatureScript instead (bosses use their own AI); low prio (Dungeon: Lower Blackrock Spire) |
| sol@31cc968d | 2021-08-20 | X    | only take over item 16716; done: sol@c7fcdc55 |
| sol@05d0cdd1 | 2021-08-20 | X    | only insert the creature with GUID 3110383; verify position; done: sol@ed844681 |
| sol@c6c3aa55 | 2021-08-19 |      | verify issue & changes; low prio (Dungeon: Deadmines) |
| sol@122fd3ec | 2021-08-19 | X    | verify issue & changes; won't take over: on-use abilities should create threat |
| sol@02da6856 | 2021-08-18 | X    | verify the actual issue; update: keep gossip, even if it was not available on retail |
| sol@06bb81fe | 2021-08-18 | X    | use other position; done: sol@ea6a5f28 |
| sol@f16f8798 | 2021-08-17 | X    | use other positions and random movement; done: sol@e00dcdbc |
| sol@0e6284f2 | 2021-08-17 | X    | use CONDITION\_QUESTSTATE instead; done: sol@3fa719d4 |
| sol@1e84e062 | 2021-08-17 | X    | not needed, just add SPELL\_ATTR3\_NO\_INITIAL\_AGGRO; done: sol@5674a4f9 |
| sol@6b5c3ed0 | 2021-08-17 |      | take over if needed |
| sol@9b7c6bff | 2021-08-17 | X    | wrong: the quest "Gaining Acceptance" is not meant to be repeatable, it should be replaced by "Gaining Even More Acceptance"; currently both quests are visible, this is the only thing which should be fixed; done: sol@3e1cb312 |
| sol@00109650 | 2021-08-16 | X    | wrong: fix spell instead of target type; the creature should use "Frostbolt Volley" (8398), not "Frostbolt" (15043); done: sol@9e4cda7c |
| sol@fcf344b5 | 2021-08-16 | X    | verify/rework SQL script; done: sol@17071ba9 |
| sol@28a76464 | 2021-08-16 | X    | verify issue & changes; won't take over: the part removed here ensures that the boss "Broodlord Lashlayer" is not skipped |
| sol@004af40c | 2021-08-14 |      | take over if needed |
| sol@2ef25c63 | 2021-08-13 | X    | verify changes; verify the creatures in the area; done: sol@04c09b2f |
| sol@0345de19 | 2021-08-12 | X    | verify/rework SQL script; done: sol@0dff0ffa |
| sol@300dc161 | 2021-08-11 |      | too generic, this affects all spells with SPELL\_AURA\_HOVER which probably causes several side effects; better find a specific solution for Levitate; low prio as this is just a minor issue |
| sol@166ccc4f | 2021-08-11 | X    | not needed as the wrong AC commit sol@00111e83 was not taken over; only take over the changes concerning Parasitic Serpent, Vagash and Snort the Heckler; done: sol@2c7be96a (only took over the changes concerning Parasitic Serpent, the other ones are ok, no need to update them) |
| sol@b5f91706 | 2021-08-10 | X    | keep random movement for some of the spawns; disable random movement for other creatures in the camps; done: sol@b10a3ed8 |
| sol@50202844 | 2021-08-09 | X    | wrong: The trainers should only teach riding to players of the same faction; remove the conditions instead as they were taken from TC 4.3.4; update: the conditions are remnants from classic where each faction mount needed a separate riding skill, e.g. "Undead Horsemanship", "Ram Riding" etc.; done: sol@de789b6a |
| sol@2b166d1b | 2021-08-08 | X    | wrong: Shadow Weaving should not be applied with each tick, only on initial cast; find another solution; done: sol@374ea18d |
| sol@80da8284 | 2021-08-08 | X    | choose another position; done: sol@328d27de |
| sol@a81a6197 | 2021-08-07 |      | verify changes; low prio (Dungeon: Ahn'kahet) |
| sol@5b057798 | 2021-08-07 |      | verify issue & changes; low prio (Dungeons) |
| sol@d3d6d0be | 2021-08-07 |      | take over if needed (probably not worth the effort as this is just a minor issue) |
| sol@d8c1ccb6 | 2021-08-06 | X    | rework the SAI script instead; done: sol@aed32846 |
| sol@774abca7 | 2021-08-06 | X    | verify changes; update: won't take over, looks awful with random movement |
| sol@6bb5a885 | 2021-08-06 | X    | verify/rework SQL script; implemented another solution: sol@3a80919d |
| sol@4aed38d7 | 2021-08-06 | X    | verify new spawn; keep old respawn time and idle movement; done: sol@e06016d4 |
| sol@cda264cf | 2021-08-06 | X    | verify new spawns; keep the old respawn time; update: the new spawns use the wrong map, seems like no one is testing this stuff anymore; done: sol@6972a636 |
| sol@31e41890 | 2021-08-06 | X    | does not work correctly, use FilterTargets instead; done: sol@d574136d |
| sol@32650b61 | 2021-08-05 | X    | verify issue and changes; update: won't take over, Deep Wounds should not proc of ranged weapons (even if this might have been the case on retail); also the solution is too generic and could cause several side effects |
| sol@213e53c4 | 2021-08-05 | X    | verify/rework SQL script; update: won't take over, random movement looks much better; also the WP paths in this commit are basically all the same and have far too few points |
| sol@26bf3624 | 2021-08-04 | X    | verify/rework SQL script; done: sol@b2581713 |
| sol@bf84e72d | 2021-08-04 | X    | verify/rework SQL script; done: sol@acb18e14 (the AC commit contained some serious bugs, e.g. wrong map for the spawns, does not seem to have been tested) |
| sol@d56f27ed | 2021-08-03 | X    | verify new position / orientation; done: sol@4aa498d6 |
| sol@b8f6c2a1 | 2021-08-03 | X    | verify/rework SQL script; done: sol@1745c067 |
| sol@9a820e2d | 2021-08-01 | X    | try to implement a solution which touches only the spell script; done: sol@83ca1ea5 |
| sol@80ff915f | 2021-08-01 |      | take over if needed; does not seem to fix anything and the original PR does not contain any information other than that it was copied blindly from TC |
| sol@7f4c5561 | 2021-08-01 |      | take over if needed (the flag is not used anywhere) |
| sol@87b2cd12 | 2021-07-31 |      | take over if needed; does not seem to fix anything and the original PR does not contain any information other than that it was copied blindly from TC |
| sol@19bbe2cd | 2021-07-31 |      | verify changes; low prio (Dungeon: Zul'Gurub) |
| sol@8f5100f3 | 2021-07-30 | X    | verify/rework WP path; keep walking speed as he is bigger than the other Satyrs; set active; update: the WP path has far too few points and some of the points float high above the ground, does not seem to have been tested that much; done: sol@4c878298 |
| sol@2e8301b7 | 2021-07-30 | X    | Sol is not affected by the mentioned issue, but nevertheless verify/rework both WP paths and set the creatures active; done: sol@0bee4c7c |
| sol@00111e83 | 2021-07-30 |      | wrong: the skinning loot template 100003 is used by many other creatures, so don't change the loot template but pick a correct one or create a new one instead; the loot template is used for other high level creatures as well, those should also be fixed; low prio |
| sol@2f63e81a | 2021-07-30 |      | take over if needed |
| sol@1e36a644 | 2021-07-29 | X    | verify/rework SQL script; done: sol@30e98d93 |
| sol@c125f461 | 2021-07-29 | X    | won't take over, properly fix the SAI instead incl. the comments; SMART\_ACTION\_FLEE\_FOR\_ASSIST does not use the target, so changing the target type is useless; done: sol@32423de3 |
| sol@201b3235 | 2021-07-28 | X    | there are other Peacebloom spawns in Redridge Mountains, check the gameobject pool 950 and remove all of them; done: sol@2452b2ac |
| sol@ecf022e8 | 2021-07-28 | X    | verify/rework SQL script; done: sol@a5e10561 |
| sol@f9125f13 | 2021-07-27 |      | probably not needed at all, the elevators were indeed dangerous on retail, e.g. the ones in the Undercity did kill many players |
| sol@e37dba8d | 2021-07-26 |      | probably not needed at all, there are many comments in the internet which state that this was changed later to only be a simple zoom |
| sol@6a5a901a | 2021-07-25 | X    | verify/rework SQL script; update: won't take over, added short WP paths for two of the spawns (not all spawns have to move around): sol@be6dee23 |
| sol@e40ecbda | 2021-07-24 | X    | verify changes; use UPDATE instead of DELETE/INSERT; done: sol@65ced8b0 |
| sol@9343cb51 | 2021-07-24 | X    | won't take over, rework SAI instead; done: sol@e3bc824b |
| sol@b5dfba05 | 2021-07-23 | X    | this is wrong for some of the creatures which are kneeling or lying on the ground; some positions should also be updated; done: sol@5c3a4a66 |
| sol@1919f945 | 2021-07-23 | X    | verify/rework SQL script; done: sol@192d41b3 |
| sol@d6da679e | 2021-07-23 | X    | verify/rework SQL script; done: sol@ca94bffe |
| sol@79f5139d | 2021-07-23 | X    | verify/rework SQL script; done: sol@5789fbef |
| sol@bbe1d4bb | 2021-07-23 | X    | random movement already enabled, see sol@69c6e694; take over the new spawn points and create an appropriate creature pool (this has been forgotten in the AC commit); update: AC added pooling, see commit sol@96a659c6; only take over pooling, not the respawn time; done: sol@f5fba320 |
| sol@9e1c8b3f | 2021-07-23 | X    | verify/rework SQL script; update: the AC commit will disable WP movement for GUID 93615, which is wrong; done: sol@31df2ed5 |
| sol@74edb401 | 2021-07-23 | X    | verify position; update: wrong, won't take over; the new position is from Cataclysm, the old one is correct, so keep the old one |
| sol@e5680dfe | 2021-07-22 |      | verify changes; low prio (Dungeon: Naxxramas) |
| sol@2a4a2f35 | 2021-07-22 |      | wrong: should be a random world drop from level 40-60 mobs; there are already reference loot tables which deal with patterns, designs etc., but they are not really used anywhere: 24700,24701,24702,24703,24704,24705,24706,24707,24708,24709; try to find a better solution; low prio |
| sol@7830ff5b | 2021-07-22 | X    | wrong: those gameobjects serve as spell focus for Mooncloth, it is not possible to use this spell if the objects are deleted; move them into the ground instead; sol@73cd38ff |
| sol@0c318397 | 2021-07-22 | X    | look for a better position as there's another Goldthorn nearby; done: sol@9d711c6f |
| sol@586175ed | 2021-07-22 | X    | verify changes; use UPDATE instead of DELETE/INSERT; applied another solution: sol@c5d7d4a0 |
| sol@1cf7f5c8 | 2021-07-22 | X    | wrong: the NPC needs 2 gossip menu texts (paladin / non-paladin) and the conditions were not updated; a new menu ID is not necessary, just update text ID 10040 with 10044 for menu ID 8111; also adjust positions of Ambassador Sunsorrow and Champion Cyssa Dawnrose as they float in the air because of the stairs; done: sol@a616c042 |
| sol@38f7afea | 2021-07-21 |      | low prio (Localization: zhCN) |
| sol@b226df1e | 2021-07-20 | X    | verify/rework SQL script; done: sol@08afbe51 |
| sol@58b0bca0 | 2021-07-18 | X    | verify/rework SQL script; done: sol@5479fec1 |
| sol@fba9e265 | 2021-07-15 | X    | verify every creature in this area; not all creatures have to move around; also check some of the already wandering creatures and disable random movement; done: sol@90e01fc8 |
| sol@1fa51e51 | 2021-07-12 |      | verify changes; low prio (Dungeon: Ulduar) |
| sol@b5d9b3d5 | 2021-07-12 | X    | verify issue/changes; rework SQL script; update: won't take over, the quest seems to work fine; just increase the effect radius for Plague Strike to 8 yards: sol@55a28f19 |
| sol@2e8a7498 | 2021-07-10 | X    | verify/rework SQL script; implemented another solution, see sol@e4e792a7 & sol@83e97509 |
| sol@a61f7a12 | 2021-07-09 |      | take over if needed |
| sol@b2836769 | 2021-07-08 |      | despite the description the creature pool is not associated with Meshlok, but with two other creatures: Cavern Lurker & Cavern Shambler; obviously they are meant to be replaced with Meshlok, which is probably only possible using an InstanceScript; low prio (Dungeon: Maraudon) |
| sol@06027e32 | 2021-07-08 |      | verify issue; low prio (Dungeon: Utgarde Pinnacle) |
| sol@f8c8e98a | 2021-07-08 |      | take over if needed |
| sol@c7d5080b | 2021-07-08 | X    | take over from TC instead; done: sol@7287e321 |
| sol@6644c651 | 2021-07-08 | X    | verify/rework SQL script; implemented another solution: sol@382f5c58 |
| sol@5eebf892 | 2021-07-07 |      | verify issue; low prio (Dungeon: Icecrown Citadel) |
| sol@3dec029b | 2021-07-07 |      | adapt to Sol; low prio (PvP) |
| sol@b66314b6 | 2021-07-07 | X    | verify/rework SQL script; done: sol@fe86c0cb; note: don't spawn multiple Noxxious Scions because the quest would then become too easy and it also does not match the quest description |
| sol@3b745b06 | 2021-07-07 | X    | take over from TC instead; done: sol@74d9ab80 |
| sol@86860d36 | 2021-07-07 | X    | verify/rework SQL script; done: sol@be4436be |
| sol@9cbd67a3 | 2021-07-07 | X    | verify/rework SQL script; done: sol@a83eb8c4 |
| sol@b062d4a3 | 2021-07-07 | X    | take over TC commit 7182f5ddd1eae074ea96ee457a683453a4f4764b instead; done: sol@af75c29e |
| sol@d3b2d8a5 | 2021-07-07 | X    | take over TC commit 7182f5ddd1eae074ea96ee457a683453a4f4764b instead; done: sol@af75c29e |
| sol@161b052a | 2021-07-06 | X    | verify/rework SQL script; done: sol@f8c3c9ec |
| sol@ab5ce3e3 | 2021-07-04 |      | verify changes; low prio (Dungeon: Molten Core) |
| sol@681e7139 | 2021-07-04 | X    | verify/rework SQL script; done: sol@cf0df16e |
| sol@476dcd3e | 2021-07-04 |      | verify changes; low prio (Dungeon: Molten Core) |
| sol@0cd03311 | 2021-07-03 |      | low prio (Localization: esES, esMX) |
| sol@a2e13dd5 | 2021-07-03 |      | low prio (Localization: esES, esMX) |
| sol@7a7d3d69 | 2021-07-01 |      | low prio (Localization: esMX) |
| sol@c6173e88 | 2021-06-30 |      | take over if needed |
| sol@66cd714a | 2021-06-30 |      | adapt to Sol; low prio (Localization: esES, esMX) |
| sol@6eb6b0bb | 2021-06-29 |      | low prio (Localization: zhCN) |
| sol@b8bd24b4 | 2021-06-28 | X    | verify/rework SQL script; taken from TC instead: sol@43cd762e |
| sol@a23a0c88 | 2021-06-27 | X    | verify/rework SQL script; done: sol@621ea3ca |
| sol@15e44d4d | 2021-06-27 | X    | adapt to Sol; done: sol@8323ba07 |
| sol@c73a5e95 | 2021-06-27 |      | Sol is not affected by the mentioned issue; investigate Deep Freeze nevertheless; also see sol@eff648b3; low prio |
| sol@5b82840e | 2021-06-27 | X    | adjust CreatureScript; done: sol@56fc542e |
| sol@0c22cae7 | 2021-06-26 |      | verify changes; low prio (Stranglethorn Fishing Extravaganza) |
| sol@0b7e74b0 | 2021-06-26 | X    | use SAI to add immunity; done: sol@b2516561 |
| sol@118227a2 | 2021-06-25 | X    | also remove SmartAI from creature template; done: sol@8d48d310 |
| sol@0b8d679f | 2021-06-25 | X    | verify/rework SQL script (also see sol@0eb8a8ed); remove entries in "waypoint\_data" and "waypoint\_scripts"; done: sol@48c4174d |
| sol@d5bce088 | 2021-06-24 | X    | verify/rework SQL script; done: sol@e8c57908 |
| sol@9bf617be | 2021-06-24 | X    | wrong: the quest type is correct, fix the quest itself instead; done: sol@1a58356f |
| sol@1b1378c7 | 2021-06-23 | X    | take over from TC instead; npc text ID 7786 already contains the correct text, no need to create a new one; done: sol@429b8ce2 |
| sol@569e3399 | 2021-06-23 | X    | take over if needed; may cause unforeseen side effects; not really necessary as it is not possible to attack creatures while they are evading; update: was reverted by AC with commit sol@efdb64af |
| sol@b1c5a6c0 | 2021-06-22 | X    | verify/rework SQL script; update: the additional emote text added here is wrong, this was just a text on Wowpedia to describe what the NPC is actually doing in-game; done: sol@e7225db4 |
| sol@b2472cae | 2021-06-22 | X    | use better description; the localized text also has to be updated; done: sol@26c53880 |
| sol@56495763 | 2021-06-20 | X    | verify conditions; add comment if taking over; update: not needed as there's already a condition concerning "Lieutenant's Insignia" which suffices |
| sol@b870fe53 | 2021-06-20 |      | verify & adapt to Sol; low prio (Localization: esES, esMX) |
| sol@64aa901c | 2021-06-20 |      | verify changes; there's at least one bug concerning CONFIG\_START\_HEROIC\_PLAYER\_LEVEL; low prio |
| sol@ff5e4570 | 2021-06-20 | X    | wrong: the gossip options should only be available after the quest "Cache of Mau'ari" is rewarded; also add proper comments; done: sol@9e612aae |
| sol@18a02e9c | 2021-06-18 |      | low prio (Localization: zhCN) |
| sol@ea7f693c | 2021-06-18 | X    | take over TC commit 2fb573150d5c08a5a2fa870f886969d25aee5734 instead; done: sol@80b9fa02 |
| sol@4811a14b | 2021-06-18 | X    | compare changes; check TC implementation; done: sol@3a5ddcb2 |
| sol@8214873e | 2021-06-18 | X    | verify/rework SQL script; implemented another solution: sol@d2f6f12d |
| sol@137c0137 | 2021-06-18 | X    | check if other creatures are using model ID 3680; done: sol@43b3d647 |
| sol@206c4055 | 2021-06-18 | X    | implement other conditions in order to allow the drop even if "The Swarm Grows" is rewarded (otherwise the player is not able to finish the quest later; although this wasn't the case on retail, it provides a better player experience); done: sol@4632de8c |
| sol@efd575fe | 2021-06-18 |      | verify/rework SQL script; low prio (Dungeon: Scholomance) |
| sol@f8c098f3 | 2021-06-18 | X    | wrong: a loot reference cannot be part of a group, so the update changes nothing; find another solution; done: sol@f0b1ca77 |
| sol@3da83cc0 | 2021-06-17 |      | take over if needed |
| sol@0d96866c | 2021-06-14 |      | does not seem to fix the issue, try to find another solution; low prio as it's just a visual bug |
| sol@34da0cda | 2021-06-14 |      | verify changes; low prio (Dungeon: Upper Blackrock Spire) |
| sol@c3bac33e | 2021-06-13 | X    | probably just change the position, not all creatures have to move around randomly; done: sol@12faeaf8 |
| sol@f54c6364 | 2021-06-13 | X    | verify/rework SQL script; use other positions & wander distances; done: sol@60b15a98 (use WP movement instead of random movement) |
| sol@fe2aa2ec | 2021-06-12 |      | verify spell IDs; remove variables; low prio |
| sol@c934b306 | 2021-06-12 | X    | add WP movement instead of random movement; done: sol@cd283a22 |
| sol@9170eadc | 2021-06-11 | X    | verify creatures; not all creatures have to move around randomly, especially not Goreclaw the Ravenous; added WP movement for Goreclaw and two of the Bloodfen raptors: sol@d8c50ca9 |
| sol@85103fd2 | 2021-06-11 | X    | verify/rework SQL script; done: sol@62672290 |
| sol@07ec1ba0 | 2021-06-11 | X    | verify/rework SQL script; done: sol@09de7f9d |
| sol@63359657 | 2021-06-09 | X    | verify/rework SQL script; done: sol@82b0982c |
| sol@0062a81d | 2021-06-09 | X    | verify loot; rework UPDATE statement and remove variables; done: sol@ed27612f |
| sol@3381d0d7 | 2021-06-08 | X    | verify loot; rework DELETE statement and remove variables; done: sol@beda780d |
| sol@6dacfc07 | 2021-06-08 | X    | wrong: only save loot to the DB which the player can actually see (is allowed for the player); implement another solution; done: sol@2ac4d6ff |
| sol@1644e4c0 | 2021.06.07 | X    | use a single DELETE statement instead; done: sol@f6dbc94a |
| sol@752038e2 | 2021-06-05 |      | low prio (Localization: zhCN) |
| sol@c485bab6 | 2021-06-04 | X    | don't use SAI, fix GameObjectScript instead; done: sol@565d1a3f |
| sol@e3fcf1ad | 2021-06-02 | X    | verify/rework SQL script; implemented another solution: sol@d067deae |
| sol@c90a43eb | 2021-06-02 | X    | verify issue; use UPDATE instead of DELETE/INSERT; done: sol@21983c67 |
| sol@8747f965 | 2021-06-02 | X    | verify/rework SQL script; done: sol@363333f4 |
| sol@e7087433 | 2021-06-02 |      | verify/rework SQL script (see also sol@c4185a51); low prio (Dungeon: Wailing Caverns) |
| sol@40a71471 | 2021-06-02 | X    | SAI not necessary, update spell script "spell\_q6124\_6129\_apply\_salve" instead; done: sol@878a1678 |
| sol@ee7d54b7 | 2021-06-01 | X    | verify/rework SQL script; done: sol@b966cffc |
| sol@a7585d61 | 2021-06-01 | X    | verify/rework SQL script; done: sol@5d160109 (many bugfixes were necessary, does not seem this was tested that much) |
| sol@d46a55d9 | 2021-05-31 | X    | verify/rework SQL script; implemented another solution: sol@f6acf6ae |
| sol@11cdb969 | 2021-05-31 | X    | verify issue & changes; done: sol@318ca350 |
| sol@3ac48489 | 2021-05-31 | X    | verify/rework SQL script; update: won't take over as the actual root cause was a bug concerning the assist check for creatures, see sol@37c97766 |
| sol@8dc13a53 | 2021-05-31 | X    | fix the spell script "spell\_gen\_throw\_back" and the spell ID of the throw back spell; done: sol@483c30b9 |
| sol@cedd6363 | 2021-05-30 | X    | verify changes; update: wrong, won't take over; holy resistance is derived from arcane resistance, so the values should stay in the DB |
| sol@107658eb | 2021-05-30 |      | not working; try to find another solution; update: also see sol@7406a01a |
| sol@a355b4d2 | 2021-05-29 |      | verify issue & changes; update: cannot reproduce on Sol; low prio |
| sol@f1b43a89 | 2021-05-27 |      | take over if needed |
| sol@e8181130 | 2021-05-25 |      | verify & adapt to Sol; low prio (Localization: esES, esMX) |
| sol@537798e4 | 2021-05-25 |      | verify & adapt to Sol; low prio (Localization: esES, esMX) |
| sol@2d41cd49 | 2021-05-25 | X    | not working correctly because it uses the wrong WorldMapAreaId; look up the correct one; done: sol@d2c97188 |
| sol@d16605d4 | 2021-05-25 | X    | verify/rework SQL script; verify quest; done: sol@be1a5faa |
| sol@3c09156d | 2021-05-25 | X    | verify/rework SQL script; verify WP path; done: sol@a6557c0a |
| sol@ae66ea08 | 2021-05-25 |      | verify/rework SQL script; low prio (Dungeon: Scholomance) |
| sol@3bc7880d | 2021-05-23 | X    | wrong: don't just switch the broadcast text IDs, fix the conditions instead; done: sol@f0db5f99 |
| sol@556a7b76 | 2021-05-23 |      | adapt to Sol; low prio (Localization: zhCN) |
| sol@07527618 | 2021-05-23 | X    | don't delete the spawn, use Crazed Dragonhawk instead; done: sol@6e417187 |
| sol@b4830948 | 2021-05-23 | X    | not working; try to find another solution; done: sol@37b47c1d |
| sol@0527c17d | 2021-05-22 | X    | verify changes; adapt to Sol; done: sol@e8f70b8f |
| sol@d74832ef | 2021-05-22 | X    | verify/rework SQL script; done: sol@c65e0d34 |
| sol@3f6da615 | 2021-05-21 |      | take over if needed, also see follow-up sol@47f7c46f; update: won't take over, as this does not seem to be correct: only non-spell attacks should have 100% crit on a sitting target; the attack should cause double damage and should be shown as crit in the combat log; the crit must not proc other abilities; implement another solution; very low prio |
| sol@4fff925b | 2021-05-18 | X    | verify/rework SQL script; implemented another solution: sol@d3986026 |
| sol@fc4496ec | 2021-05-18 | X    | verify/rework SQL script; done: sol@6778531e |
| sol@16e04439 | 2021-05-18 | X    | verify/rework SQL script; done: sol@a4b006f9 |
| sol@0ca86925 | 2021-05-15 | X    | verify/rework SQL script; done: sol@c892d7f4 (many bugfixes were necessary, does not seem this was tested that much) |
| sol@16a385d1 | 2021-05-14 | X    | verify/rework SQL script; done: sol@07644142 |
| sol@88071b7e | 2021-05-14 | X    | verify loot chances; update: if every chance in a group is 0 this means that the chances are equal, so this commit is wrong, won't take over |
| sol@fe5aedaa | 2021-05-13 | X    | verify/rework SQL script; done: sol@72093bf3 |
| sol@b14ffdb8 | 2021-05-13 | X    | verify changes; rework SQL script if replacing the CreatureScript with SAI; done: sol@0f10aca0 |
| sol@61325fd4 | 2021-05-11 | X    | verify WP path; set active; rework SQL script; done: sol@9aa4224b |
| sol@ca74d308 | 2021-05-10 | X    | use a single UPDATE statement using the creature IDs instead; done: sol@9094b20d |
| sol@44c45aa2 | 2021-05-10 | X    | the script contains several bugs (e.g. wrong gameobject & map IDs); also don't change the respawn time for gameobjects which are contained in pools; done: sol@168ab5c6 |
| sol@54c18cff | 2021-05-10 | X    | verify/rework SQL script and check WP path; rewrote existing SAI & WP movement: sol@e4e792a7 |
| sol@534ec53b | 2021-05-09 | X    | verify/rework SQL script and compare with original CreatureScript; not taken over, improved CreatureScript and WP path instead: sol@a5f4b19c |
| sol@ea6c2321 | 2021-05-09 | X    | verify/rework SQL script; update: this is buggy, double-check the values (see AC commit sol@6f6234ae); done: sol@edf21d96 |
| sol@44babc3c | 2021-05-08 |      | implement another solution without copy/paste from TC; low prio as the pools are basically working, they just sometimes spawn 1 object less than specified |
| sol@42659f06 | 2021-05-07 | X    | remove associated WP paths; use wander distance 5 instead of 10; done: sol@48b734cd |
| sol@3e1a2024 | 2021-05-06 | X    | verify creature pool; update: wrong, the pool is working correctly; chance 0 for all pool members means equal chance for all |
| sol@926a3103 | 2021-05-06 | X    | don't remove the broadcast text IDs, instead update the broadcast texts themselves; done: sol@e29ab7ec (replaced "Guild Master & Vendor" with "Guild Master", the other texts seem to be ok) |
| sol@64461da3 | 2021-05-06 |      | verify & adapt to Sol; low prio (Localization: esES, esMX) |
| sol@71d5d27e | 2021-05-06 |      | verify changes; low prio (Dungeon: Icecrown Citadel) |
| sol@058f0c94 | 2021-05-06 |      | verify & adapt to Sol; low prio (Localization: esES, esMX) |
| sol@37c3e051 | 2021-05-05 |      | verify & adapt to Sol; low prio (Localization: esES, esMX) |
| sol@ad5ba1a7 | 2021-05-05 | X    | verify/rework SQL script; implemented another solution: sol@e2eaf399 |
| sol@74a54b49 | 2021-05-04 | X    | don't remove the broadcast text ID, instead update the broadcast text itself; done: sol@f04c253c |
| sol@f96c5281 | 2021-05-04 |      | verify & adapt to Sol; low prio (Localization: esES, esMX) |
| sol@1d919f84 | 2021-05-03 | X    | verify position and use UPDATE instead of DELETE/INSERT; done: sol@a4651f4a |
| sol@292439ca | 2021-05-03 | X    | use UPDATE instead of DELETE/INSERT for the position; verify path; done: sol@37248ae7 |
| sol@752595dc | 2021-05-01 | X    | try to find another solution without changing the logic in NearestAttackableUnitInObjectRangeCheck; done: sol@886788e0 |
| sol@5ee7fed0 | 2021-04-30 | X    | verify/rework SQL script; done: sol@36f8d17b |
| sol@6389d2eb | 2021-04-30 | X    | verify/rework SQL script; update: this is wrong, won't take over; the script removes gameobjects, inserts the exact same entries and removes these gameobjects from the appropriate pool; it also adds a bad SAI "fix" for an issue which has another root cause |
| sol@0b87bb0d | 2021-04-30 |      | verify changes; low prio (Dungeon: Deadmines) |
| sol@0372ddc1 | 2021-04-27 | X    | rework SQL script; verify positions; done: sol@ccb0d6a3 |
| sol@28ce1e92 | 2021-04-25 | X    | verify position and use UPDATE instead of DELETE/INSERT; done: sol@3f0f8670 |
| sol@96e0d2ca | 2021-04-25 | X    | verify/rework SQL script; also remove sneak visual effect (UNIT\_FIELD\_BYTES\_1 flag 131072); done: sol@1f7cd054 |
| sol@8ab6c569 | 2021-04-25 | X    | verify/rework SQL script; verify loot; update: this is wrong, won't take over: all reference loot entries have been removed and skinning loot has been added to creature loot; take over creature loot template from TC instead: sol@90ed6260 |
| sol@620eb8e9 | 2021-04-25 |      | verify changes; low prio (Dungeon: Scholomance) |
| sol@eaf90b6b | 2021-04-25 | X    | verify changes (also see sol@83183fea, sol@16a57e57); setting "Attributes" to 8192 (0x00002000) is wrong, correct value is 2097152 (0x00200000); also don't overwrite "Attributes" with a single value, use bitwise OR instead; update: won't take over, as there's no proof that it should not be possible to parry, block or dodge Intercept/Charge |
| sol@98364e43 | 2021-04-25 |      | adapt to Sol; low prio (Localization: zhCN) |
| sol@2e8ef021 | 2021-04-25 |      | verify changes; low prio (Dungeon: Scholomance) |
| sol@472361a0 | 2021-04-25 | X    | verify/rework SQL script; done: sol@b426dde1 |
| sol@c95d1f72 | 2021-04-23 | X    | verify changes; update: find another solution as this one seems to be wrong (removes the check concerning boss encounters); update: taken over anyway: sol@5d15e494 |
| sol@085be43e | 2021-04-19 | X    | verify/rework SQL script; done: sol@e8b31591 |
| sol@6d0ebdfb | 2021-04-18 | X    | wrong; instead of removing the reference from the other creatures remove the item from table "reference\_loot\_template" and add it directly to "creature\_loot\_template"; do the same for Humbert's other items (Pants -> Dun Garok Priest, Chestpiece -> Dun Garok Mountaineer & Tamra Stormpike); done: sol@af3379a9 |
| sol@b5409a18 | 2021-04-18 | X    | verify SQL script; instead of removing the broadcast text ID fix the broadcast text itself; done: sol@c3f52381 |
| sol@9bf10f90 | 2021-04-18 | X    | verify position and use UPDATE instead of DELETE/INSERT; chose another position: sol@2e739a95 |
| sol@53a21ff7 | 2021-04-18 | X    | verify/rework SQL script; done: sol@73545a89 |
| sol@acce0d48 | 2021-04-18 | X    | verify/rework SQL script; done: sol@f9a64aa5 |
| sol@42dde8c7 | 2021-04-16 | X    | verify/rework SQL script; update: this SQL script fixes nothing, it just changes the SAI comments; in fact it introduces new bugs because it deletes broadcast text IDs from creature texts; won't take over, rework the existing SAI instead; done: sol@5c0f9fc9 |
| sol@62635ca5 | 2021-04-13 | X    | only take over the DELETE statements for the duplicates; no need to change the gameobject IDs, instead updates to "gameobject\_template\_locale" should be used to add localized names; done: sol@4bcc98df |
| sol@41e37f2d | 2021-04-11 | X    | only update z position; enable random movement; done: sol@9f908dac |
| sol@91d23c70 | 2021-04-11 | X    | only update z position; done: sol@f334662d |
| sol@d1f4306e | 2021-04-11 | X    | change pool template ID as this one will overwrite "Treasures - Teldrassil" from AC commit sol@74f4ba97; update: not needed anymore as both chests belong to pool template 11655 (see sol@b45d7101) |
| sol@2d020575 | 2021-04-11 | X    | verify/rework SQL script; implemented another solution: sol@fe2d140e |
| sol@40b951fb | 2021-04-11 | X    | only update z position; done: sol@5ecf266c |
| sol@10954b6d | 2021-04-11 | X    | verify drop chances; done: sol@318db455 |
| sol@577bee84 | 2021-04-11 | X    | verify/rework loot chances; seems to be wrong that all are equal; perhaps just add money to the loot instead of changing the chances (check for all junkboxes); done: sol@bb7956f0 |
| sol@372d72fa | 2021-04-11 | X    | verify/rework SQL script; perhaps use summon spell instead of the creature spawns; update: won't take over, instead fixed controlled NPCs to attack if their owner NPC is attacked: sol@5fe208ec |
| sol@70308572 | 2021-04-11 | X    | only update z position; done: sol@d2ceb8ad |
| sol@44cecc82 | 2021-04-11 | X    | only update z position; done: sol@801a6c1f |
| sol@b96a6a13 | 2021-04-11 | X    | verify/rework SQL script; perhaps use summon spell instead of the creature spawns; update: won't take over, instead fixed controlled NPCs to attack if their owner NPC is attacked: sol@5fe208ec |
| sol@d0e9c6ca | 2021-04-08 | X    | verify changes; update: won't take over, Execute should not always hit the target, it should be affected by parry / dodge |
| sol@91dfedd0 | 2021-04-07 |      | take over if needed; does not seem to fix anything and the original PR does not contain any information other than that it was copied blindly from TC |
| sol@88ddc244 | 2021-04-07 |      | take over if needed; does not seem to fix anything and the original PR does not contain any information other than that it was copied blindly from TC |
| sol@042cec82 | 2021-04-06 |      | take over if needed |
| sol@655ccacf | 2021-04-05 |      | don't take over all SQL scripts as there are also several changes to the English localization which seem to be wrong (e.g. quest 5636); low prio (Localization: esES, esMX) |
| sol@0528e0b4 | 2021-04-05 | X    | verify commit and only take over relevant changes from this TC commit: https://github.com/TrinityCore/TrinityCore/commit/8d19fcbc469e0b37a323c876a15097fbe848d884; done: sol@c30b7e25 |
| sol@d8c4795e | 2021-04-04 | X    | verify gameobjects & positions; done: sol@ccb0d6a3 |
| sol@26c30996 | 2021-04-04 |      | verify/rework SQL script; low prio (Dungeon: Naxxramas) |
| sol@7413c17e | 2021-04-04 |      | verify changes & issue (cannot reproduce on Sol); low prio |
| sol@0d8aa2e8 | 2021-04-03 |      | take over if needed |
| sol@6dc4ca85 | 2021-04-02 |      | verify changes; low prio (Dungeon: Naxxramas) |
| sol@1b722dfc | 2021-04-02 | x    | verify/rework SQL script; done: sol@16d6e03c |
| sol@0bbe5fa4 | 2021-04-01 | X    | verify/rework SQL script; implemented another solution: sol@cd296c38 |
| sol@9b9e070c | 2021-04-01 | X    | verify changes; Sol does not seem to be affected by these issues |
| sol@12165b81 | 2021-04-01 | X    | verify/rework SQL script; done: sol@a738b2f1 |
| sol@86f6ec3c | 2021-04-01 | X    | verify/rework SQL script (see also AC commit sol@81c07178); implemented another solution: sol@0d37f7e0 |
| sol@4e112a89 | 2021-04-01 | X    | verify/rework SQL script; implemented another solution: sol@54dee951 |
| sol@f38e63cc | 2021-04-01 | X    | verify/rework SQL script; implemented another solution: sol@dd0d64d4 |
| sol@a9ba546c | 2021-04-01 | X    | verify gameobjects & positions; done: sol@ccb0d6a3 |
| sol@4c0467c5 | 2021-04-01 | X    | verify/rework SQL script (also see sol@4c357c60); update: contains too many bugs and causes side effects (e.g. using the wrong gameobject 180779 which is actually spawned in Northrend); rework the existing script and use the values according to TC's CreatureScript "npc\_demolitionist\_legoso"; completely rewritten: sol@056f733a |
| sol@10c56336 | 2021-04-01 | X    | verify gameobjects & positions; done: sol@ccb0d6a3 |
| sol@c0aa1b88 | 2021-03-29 |      | verify changes; low prio (Love is in the Air) |
| sol@9bf2800c | 2021-03-29 |      | verify changes; low prio (Dungeon: Ulduar) |
| sol@7a5e4be7 | 2021-03-28 |      | verify changes; low prio (Dungeon: Utgarde Keep) |
| sol@2a601a16 | 2021-03-28 | X    | verify changes; taken over with a few improvements: sol@146bf661 |
| sol@01f0020e | 2021-03-27 | X    | verify/rework SQL script; update: won't take over as it's stated multiple times on wowhead that VanCleef summons his allies twice during the fight; the video linked in the original issue is private, also the "new" classic is not the same as 2010 WotLK |
| sol@b1af0192 | 2021-03-24 |      | verify changes; low prio (Dungeon: Vault of Archavon) |
| sol@8ba442bd | 2021-03-23 |      | verify changes (also see bugfixes sol@6745746c, sol@e2dd6b2b); low prio (Dungeon: Naxxramas) |
| sol@485f7e76 | 2021-03-21 | X    | try to find a less intrusive solution instead of taking over all of the TC refactoring; done: sol@75eb56c6, sol@4114a861 |
| sol@9f354db7 | 2021-03-21 | X    | verify changes; update: just another TC refactoring without real benefit; won't take over |
| sol@41ea3394 | 2021-03-20 |      | only take over the Perry Gatner event if there is nothing else to do (the event itself is rather annoying); quest "Stranglethorn Fever" already fixed with commit sol@293d7d38; very low prio |
| sol@3306f925 | 2021-03-20 | X    | verify/rework SQL script; rewrote the whole script: sol@cdecf52f |
| sol@156f7966 | 2021-03-20 | X    | verify/rework SQL script; rewrote the whole script: sol@ad133e7e |
| sol@aea4ce30 | 2021-03-20 |      | verify changes; low prio (Dungeon: Ulduar) |
| sol@45790d18 | 2021-03-19 |      | keep as reference; take over single values if needed; won't blindly take over such mass updates |
| sol@2ec26893 | 2021-03-18 | X    | change pool template ID as this one will overwrite "Minerals - Rolands Doom - Duskwood" from AC commit sol@910106a0; done: sol@d012a9c2 |
| sol@8119bff9 | 2021-03-18 | X    | verify and rework SQL script; also check event script 5991; done: sol@363333f4 |
| sol@79420c86 | 2021-03-17 | X    | position the creature in the water nearby; done: sol@80d13a0b |
| sol@0d19ac43 | 2021-03-17 |      | verify changes; low prio (Dungeon: Ulduar) |
| sol@252f56c0 | 2021-03-17 |      | verify changes; low prio (Dungeon: Ulduar) |
| sol@99c2efe3 | 2021-03-16 | X    | verify issue & solution; not needed, bug was introduced with AC commit sol@0b35a240 which was not taken over by Sol |
| sol@80f665cd | 2021-03-14 | X    | verify new positions; use UPDATE statement; done: sol@bfef495c |
| sol@f8b9a273 | 2021-03-14 | X    | verify new positions; use UPDATE statement; done: sol@cd44de32 |
| sol@3d0192fa | 2021-03-14 | X    | verify changes; update: this is wrong, those creatures are meant as flavor and should not be targetable or killable; correct inhabit type and WP movement was already added with commit sol@88243a8a |
| sol@dd7027dc | 2021-03-14 | X    | verify and rework SQL script; done: sol@818ae884 |
| sol@b514dfb9 | 2021-03-14 | X    | explode visual is not shown; try to find another solution; done: sol@8c3bd5a5 |
| sol@cfadd5a8 | 2021-03-14 | X    | verify and rework SQL script; done: sol@7a1e2ec2 |
| sol@79504214 | 2021-03-14 | X    | verify and rework SQL script (also remove sneak visual as this is added through the spell); done: sol@70558369 |
| sol@30b3d74f | 2021-03-11 | X    | verify and rework SQL script (also see sol@d1fe14ff; perhaps just fix the CreatureScript instead); also don't manipulate the faction template DBC as this is the wrong way to solve the issues (faction is used by multiple creatures and can cause issues with the other ones); use the correct spell to transform to bear form; done: sol@f168b101 |
| sol@7b7dac05 | 2021-03-11 | X    | verify new position; use UPDATE statement; done: sol@0952a39c |
| sol@57c32ec4 | 2021-03-11 | X    | verify and rework SQL script; won't take over, improved the existing SAI instead: sol@582c6a4e |
| sol@3846caab | 2021-03-11 | X    | verify rare creatures, take over and rework only the missing ones and add SAI; update: perhaps implement the rare spawn mechanism using an InstanceScript later, but for now SAI suffices; note: Warder Stilgiss should always spawn despite being a rare mob; done: sol@95675ffb |
| sol@646f6657 | 2021-03-10 | X    | try to find a better solution without manipulating Spell DBC and also addressing the other affected mechanical creatures; done: sol@ef11a791 |
| sol@9e17e139 | 2021-03-09 |      | verify SQL script; low prio (Hallow's End) |
| sol@9d096233 | 2021-03-09 |      | verify SQL script (see also AC commit sol@671c4dc5); low prio (Dungeon: Naxxramas) |
| sol@1e90722a | 2021-03-07 | X    | verify and rework SQL script (see also AC commit sol@bfdfe361); done: sol@8bbe5cc2, sol@f8aac25b, sol@641905b3, sol@7d01d98f |
| sol@53d73416 | 2021-03-07 | X    | broadcast text ID already fixed with commit sol@3e648f34, but the quest does not seem to be working correctly; compare with "official" walkthrough; done: sol@dd4748fd |
| sol@9239f033 | 2021-03-07 | X    | creature IDs 4295 and 4300 should keep their talk actions, but it is necessary to clean up the creature texts and adjust their SAI; done: sol@18cc9039 |
| sol@303ba07b | 2021-03-07 | X    | the spell "New Summon Test" is obviously wrong here, so instead of manipulating the Spell DBC improve the spell script "spell\_q9452\_cast\_net" to directly summon the creature with an appropriate summon type; done: sol@b773b702 |
| sol@bfb6faa2 | 2021-03-06 | X    | wrong; instead of deleting the reference loot ID from creature 16348 remove item 2088 from reference loot ID 24076 and add the item directly to the loot of creature 831 (see TC version); done: sol@3aafe6c3 |
| sol@a269c51d | 2021-03-05 | X    | verify deleted loot and compare with TC version; done: sol@e9c3b4d1; don't remove loot for Farmer Kent (2436) and Xandivious (15623) |
| sol@727590dc | 2021-03-04 | X    | verify and rework SQL script; done: sol@db7dca3a |
| sol@81957089 | 2021-02-28 | X    | implement another solution (remark: the attacking NPCs should not transform to worgen at all; also delete the conditions which were used in the old SAI script to control the transformation according to the Pyrewood Village Event; this has been forgotten in the AC commit and will cause a bug in the SAI execution); done: sol@56d41cf3 |
| sol@41fa30a5 | 2021-02-28 | X    | the quest is working on Sol; the movement bugs described in the AC issue seem to be caused by AC commit sol@c8f43d85 (another good hint to not take this commit over); nevertheless, rework the existing SAI as it seems to be very old and the NPC following the player should indeed fight the enemies; done: sol@330199c6 |
| sol@573a5605 | 2021-02-25 | X    | verify and rework SQL script; update: won't take over, instead fixed controlled NPCs to attack if their owner NPC is attacked: sol@5fe208ec |
| sol@dbd78936 | 2021-02-24 |      | verify and rework SQL script; low prio (Dungeon: Gnomeregan) |
| sol@ae2bd072 | 2021-02-24 |      | verify and rework SQL script; low prio (Dungeon: Gnomeregan) |
| sol@f910d635 | 2021-02-21 | X    | verify and rework SQL script; taken over from TC instead: sol@8dac3d5f |
| sol@922f87e5 | 2021-02-21 | X    | verify and rework SQL script; update: this commit is wrong because it's adding the SAI to **all** firework launchers in the world and doesn't randomly launch rockets, won't take over; implemented a better solution: sol@207d00fe |
| sol@2cd534de | 2021-02-16 | X    | verify and rework SQL script; done: sol@cd3a0535 |
| sol@f6c2c903 | 2021-02-15 | X    | use UPDATE statements with regular expressions; update: the changes are not needed as the placeholders are handled in a case-insensitive way; only fix a wrong name placeholder by replacing $N$N with $B$B, see sol@542ecf4a |
| sol@32e48823 | 2021-02-13 | X    | taken over: sol@6a0df2fa |
| sol@f9d0be8d | 2021-02-09 | X    | verify and rework SQL script (also see bugfix sol@7d46e389); done: sol@30f81211 (only took over the emote state for the Valiance Keep Footman and the increased shooting range for the Valiance Keep Rifleman, the other changes are not needed) |
| sol@0f1633c9 | 2021-02-08 | X    | find a better position; done: sol@9549ab5f |
| sol@d9024111 | 2021-02-07 | X    | verify changes; update: won't take over; according to the 4.2.0 patch notes the Clearcasting buff was increased from 8 to 15 seconds, so 8 seconds is the correct value |
| sol@6e1fb0d5 | 2021-02-03 | X    | take over if needed (additional AC commit: sol@bfcc3c6f); update: "spell\_school\_immune\_mask" won't be taken over; immunities should be handled via scripts |
| sol@c628cd77 | 2021-02-03 |      | verify SQL script; low prio (Lunar Festival) |
| sol@f65cfb6f | 2021-02-02 | X    | verify and rework SQL script; done: sol@5805ce04 |
| sol@911ac12e | 2021-02-01 |      | verify SQL script; low prio (Lunar Festival) |
| sol@9c239d17 | 2021-02-01 |      | verify SQL script; low prio (Lunar Festival) |
| sol@c8f43d85 | 2021-02-01 |      | try to find a better solution for some of the changes if nothing else is left to do (also see bugfixes sol@e7bfbe76, sol@522eb9a7, sol@695a7402, sol@b2f6a36c, sol@1d5cc1fb ....); very low prio as it's not really needed and could cause many unexpected bugs / performance issues; the only interesting changes concerning creature movement are circling the player and going backwards if too close to the player; update: if ever implementing mob fanning use an additional field in creature\_addon to control this behaviour as not all NPCs showed this on retail; also add a config parameter to disable this entirely as it will reduce performance |
| sol@fcad2b56 | 2021-01-31 | X    | only take over name changes for attributes which are actually used in the code; done: sol@c9bae62c |
| sol@6ef73413 | 2021-01-31 |      | verify CreatureScript (and bugfix sol@1a137dad); low prio (Dungeon: Blackwing Lair) |
| sol@d60fbc8e | 2021-01-27 | X    | verify and rework SQL script; done: sol@139c9572 |
| sol@d0c5bee5 | 2021-01-24 | X    | compare with TC version; done: sol@1eb9e027 |
| sol@0a8a7ef1 | 2021-01-22 |      | perhaps take over if nothing else is left to do; not really needed as this was also not the case on retail at the time; low prio |
| sol@f9b836ef | 2021-01-22 | X    | wrong, has to update coordinates in quest\_poi\_points; done: sol@0e6eac8d |
| sol@42244612 | 2021-01-19 | X    | verify and rework SQL script; done: sol@54cb8ce2 |
| sol@eddde219 | 2021-01-18 | X    | take over if needed; update: "INHABIT\_ROOT" won't be taken over; rooting creatures should be handled via scripts, not via inhabit type (often UNIT\_FLAG2\_DISABLE\_TURN is also needed); only fix the issue mentioned in the PR: Webbed Crusader; done: sol@aebf05e9 |
| sol@b2e7f397 | 2021-01-16 | X    | verify and rework SQL script; done: sol@862af8f7 |
| sol@943c1e7a | 2021-01-14 | X    | verify changes; update: won't take over, as this is a bad player experience, even if this probably was the case on retail: setting PvP for these NPCs will cause the player to be flagged with PvP after healing the NPC; UNIT\_FLAG\_PVP\_ATTACKABLE suffices, the color of the NPC's portrait is irrelevant for the quests |
| sol@9c70c6e4 | 2021-01-14 | X    | verify gameobjects and quest; done: sol@bffc89c6 |
| sol@d54a860a | 2021-01-13 | X    | verify and rework SQL script; done: sol@682d0bc1 |
| sol@b9375fff | 2021-01-12 |      | verify and rework SQL script & code changes; low prio (Dungeon: The Oculus) |
| sol@adb877f2 | 2021-01-10 | X    | verify and rework SQL script; done: sol@61bc5bfc |
| sol@7cf097ea | 2021-01-10 | X    | take over if needed; done: sol@2c297364 |
| sol@3fb18944 | 2021-01-09 | X    | deleting the second gossip option is wrong as the SAI triggers different spells depending on the selected option; fixed the broadcast text ID concerning the second option: sol@bb8bbfd4; the bomber missions themselves should be improved, though |
| sol@b1452b5b | 2021-01-09 | X    | verify and rework SQL script; update: won't take over: script is bugged (breaks quest "Re-Cursive"), double quest credit already fixed (see sol@c3976f48), SAI for Fizzcrank Survivor has been improved via sol@d9397bc4 |
| sol@c5fe21fe | 2021-01-08 | X    | verify code and compare with TC; done: sol@8d4ddd4b |
| sol@9592028a | 2021-01-08 | X    | verify text changes; done: sol@2a824c2f |
| sol@2dd6141a | 2021-01-07 | X    | verify changes and take over if needed; done: sol@b5f8d475 |
| sol@ba534cea | 2021-01-07 | X    | verify SAI; not necessary to change the SAI; the actual issue here is that SmartAI does not check if the target is friendly if assisting another unit (fixed with sol@7f6c049a); nevertheless the quest "Ending Their World" should be improved as there are several issues (WP movement, talk texts, IC SAI etc.) |
| sol@8b101654 | 2021-01-07 | X    | verify and rework SQL script; done: sol@3d693c03 |
| sol@9427da06 | 2021-01-06 | X    | verify priest trainer spells; update: won't take over (Exodar is not far away, can use the priest trainer there) |
| sol@f869c17d | 2021-01-06 | X    | use UPDATE instead of DELETE / INSERT; done: sol@ba69b4e0 |
| sol@1a0e4fc6 | 2021-01-05 | X    | changing the walk speed is wrong; adjust CreatureScript instead (also check and improve waypoints); done: sol@14afdbb1 |
| sol@b2761626 | 2021-01-04 | X    | probably find a better solution (AC commit reverted with sol@df600f99, see new solution sol@c8f43d85); very low prio as it's not really needed and could cause many unexpected bugs / performance issues |
| sol@64c686c4 | 2021-01-04 | X    | verify creature spawns; done: sol@214894b7 |
| sol@92881ad1 | 2021-01-04 | X    | verify and rework SQL script; implemented a new solution affecting the whole battle at the supply caravan: sol@7d4ef6a7 |
| sol@0bd7e9dd | 2021-01-03 | X    | verify and rework SQL script; done: sol@cda2e09f |
| sol@1078bf49 | 2021-01-03 | X    | use a better solution; done: sol@9c7d90d6 |
| sol@469d5a8b | 2021-01-02 | X    | verify and rework SQL script; done: sol@e27e4857 |
| sol@1e5e20ab | 2021-01-02 | X    | taken over: sol@039be9ea |
| sol@f366db28 | 2021-01-01 | X    | verify GOs and their associated quests before changing the respawn time; done: sol@a85ca098 |
| sol@106684fb | 2020-12-31 |      | verify SQL script & quest; low prio (Brewfest) |
| sol@0264289f | 2020-12-29 | X    | verify SQL script & texts; done: sol@5fd6cb2a |
| sol@57a4f432 | 2020-12-27 | X    | verify SQL script; done: sol@7f9c41c0 |
| sol@aec0dbb7 | 2020-12-25 |      | verify CreatureScript; low prio (Dungeon: Ulduar) |
| sol@d710057a | 2020-12-25 |      | verify and rework SQL script / CreatureScript (also see sol@0d9bfdea); low prio (Dungeon: Ulduar) |
| sol@1f5babf0 | 2020-12-22 |      | take over if needed |
| sol@dd9d9e0c | 2020-12-15 | X    | verify and rework SQL script (see also AC commit sol@d54a860a); was just taken over from TC without further verification or evaluation (several bugs, script can be simplified and improved at the same time); done: sol@682d0bc1 |
| sol@086ad6c9 | 2020-12-13 | X    | use the already existing broadcast texts; done: sol@1ea51fe0 |
| sol@af53598f | 2020-12-11 |      | verify solution (and bugfixes sol@282966c1, sol@d3aff86c); low prio |
| sol@62cb1f36 | 2020-12-10 | X    | taken over: sol@91d42f37 |
| sol@963553a9 | 2020-12-10 | X    | verify and rework SQL script; done: sol@a3c71145 |
| sol@6d10d075 | 2020-12-09 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@04c245cf | 2020-12-04 | X    | verify and rework SQL script; done: sol@fc68abe6 |
| sol@755e30f9 | 2020-12-04 | X    | verify if this actually fixes anything; the original PR provides no description on the issue and contains no test specification (the attached backtrace is invalid: too old, contains no AC commit and line numbers also don't match); low prio; update: the actual issue here is that multiple threads have access to the player social map, so the access has to be synchronized (the changes in this commit are not needed and won't be taken over); done: sol@b665ca63 |
| sol@5fe10355 | 2020-12-03 | X    | verify SQL script and actual issue; done: sol@27ca9189 |
| sol@0baecd3e | 2020-12-01 | X    | check if this contains something useful; update: won't take over because it breaks creatures following the player throughout the dungeon; fleeing creatures already fixed with commits sol@5d02c61f and sol@4caa8425; done: nothing will be taken over from this commit |
| sol@1c30f878 | 2020-11-29 | X    | verify and rework SQL script; done: sol@5a2fe9dc |
| sol@01fa6257 | 2020-11-28 |      | verify changes and take over if needed; low prio (Dungeon: Obsidian Sanctum) |
| sol@931609d2 | 2020-11-26 | X    | taken over: sol@94f60176 |
| sol@1a8110dc | 2020-11-25 | X    | use a creature pool instead of deleting the second spawn; done: sol@06e0a18a |
| sol@2e39d452 | 2020-11-24 | X    | verify and rework SQL script; done: sol@23fbb3a2 |
| sol@5d3bb608 | 2020-11-23 |      | verify and only take over if actually needed (if so, also take over sol@2788d495); fix PvP flag for the NPCs; low prio |
| sol@fb69db21 | 2020-11-19 | X    | probably find a better solution; done: AC commit reverted with sol@35fb9f49, see new solution sol@af53598f and bugfixes sol@282966c1, sol@d3aff86c |
| sol@9a8aa615 | 2020-11-16 | X    | verify and rework SQL script; done: sol@781df936 |
| sol@17bfcb77 | 2020-11-14 | X    | take over if needed (compare with TC implementation); done: sol@dca0bcd0 |
| sol@2788d495 | 2020-11-14 |      | take over if needed (compare with TC implementation) |
| sol@75ea2170 | 2020-11-13 | X    | verify and rework SQL script; done: sol@78abbe20 |
| sol@5485ef60 | 2020-11-13 | X    | verify and rework SQL script; done: sol@25eb3885 |
| sol@58d4e7e1 | 2020-11-13 | X    | verify and rework SQL script; done: sol@25eb3885 |
| sol@10ef5a16 | 2020-11-13 | X    | verify and rework SQL script; done: sol@d0095140 |
| sol@1cae3835 | 2020-11-13 | X    | verify and rework SQL script; done: sol@5d8d10f3 |
| sol@8ec31ef1 | 2020-11-12 | X    | verify and rework SQL script; done: sol@5d8d10f3 |
| sol@5aafba86 | 2020-11-12 | X    | verify and rework SQL script; done: sol@5d8d10f3 |
| sol@6fd48609 | 2020-11-12 | X    | verify and rework SQL script; done: sol@5d8d10f3 |
| sol@c3368191 | 2020-11-12 | X    | verify and rework SQL script; done: sol@f34ae533 |
| sol@d28688d4 | 2020-11-12 | X    | verify and rework SQL script; done: sol@d7279046 |
| sol@d9b24bf1 | 2020-11-12 | X    | verify and rework SQL script; done: sol@641e8e96 |
| sol@41b5b543 | 2020-11-11 | X    | verify and rework SQL script; done: sol@11fe4f69 |
| sol@c563b3a6 | 2020-11-11 | X    | verify and rework SQL script; done: sol@11fe4f69 |
| sol@8fbbf58c | 2020-11-10 | X    | verify and rework SQL script; done: sol@8ad44364 |
| sol@1cccc8d4 | 2020-11-09 | X    | verify and rework SQL script; done: sol@8ad44364 |
| sol@da4235cc | 2020-11-09 | X    | verify loot and compare with TC version; done: sol@7cff8416 |
| sol@e5fc4fca | 2020-11-08 | X    | verify and rework SQL script; done: sol@8ad44364 |
| sol@9bb6b15c | 2020-11-08 | X    | verify and rework SQL script; done: sol@ee0ca7c5 |
| sol@5254aec6 | 2020-11-07 | X    | verify and compare with TC implementation; done: sol@5b6922da |
| sol@1dc1beb3 | 2020-11-06 | X    | verify and rework SQL script; done: sol@1807c1f4 |
| sol@9763c4f4 | 2020-11-06 | X    | verify and rework SQL script; done: sol@6a23be7c |
| sol@74a34b59 | 2020-11-06 | X    | remove Coilskar Assassins as they should only be spawned during quest "Escape from Coilskar Cistern" (side note: the quest is not scripted correctly and the whole area is also not populated); done: sol@c96a586e |
| sol@f4a5907a | 2020-11-06 | X    | verify WP path; done: sol@4c9388d9 |
| sol@82ee9088 | 2020-11-02 | X    | verify and rework SQL script; done: sol@8bd27087 |
| sol@155e634b | 2020-11-01 | X    | verify and rework SQL script; done: sol@92215744 |
| sol@d2ddf03c | 2020-10-31 | X    | verify and rework SQL script; done: sol@e53d1dc7 |
| sol@cef27317 | 2020-10-31 | X    | verify and rework SQL script; done: sol@e90c034e |
| sol@93c70f5a | 2020-10-30 | X    | verify and rework SQL script; done: sol@8a8fe634 |
| sol@2b47117d | 2020-10-28 | X    | verify and rework SQL script; done: sol@b71f8ef5 |
| sol@00e736e4 | 2020-10-27 | X    | verify and rework SQL script; done: sol@36cd7904 |
| sol@24b9c929 | 2020-10-26 | X    | verify and rework SQL script; done: sol@6e780808 |
| sol@c4ded889 | 2020-10-26 | X    | verify and rework SQL script; done: sol@f35a4d57 |
| sol@5ec25278 | 2020-10-25 | X    | verify and rework SQL script; done: sol@71f51551 |
| sol@d07a34c1 | 2020-10-23 | X    | done: sol@91c47cb4 and sol@c129c06a; AC implementation for AURA\_INTERRUPT\_FLAG\_LEAVE\_COMBAT is at the wrong code place |
| sol@d5bb6ba1 | 2020-10-21 |      | take over if needed; see also follow-up bugfixes sol@b3a967db, sol@a9b2ddba, sol@9c0894ab; could contain several other hidden bugs |
| sol@ab5933ef | 2020-10-17 | X    | take over if needed; done: sol@79964075 |
| sol@24cfa307 | 2020-10-11 | X    | verify and rework SQL script; compare with TC version; low prio (Brewfest) |
| sol@4cca286a | 2020-10-09 | X    | verify and find a better solution as flying creatures respawn on the ground instead of their actual spawn point; done: sol@afa10355 |
| sol@3368e0f8 | 2020-10-08 | X    | verify new creature positions; done: sol@1644948e |
| sol@22f8195c | 2020-10-07 | X    | verify changes and new creature ID; done: sol@733de7ef |
| sol@369d292c | 2020-10-07 | X    | verify SQL script; done: sol@d8fb966d |
| sol@b67c30e2 | 2020-10-03 | X    | verify quest and texts; remove hard-coded gossip; done: sol@cbe3c232 |
| sol@3e81beac | 2020-09-28 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@72025003 | 2020-09-12 | X    | SAI was just taken over from TC without further verification (it is only a small part of the scripts implementing the whole quest chain); Prince Sandoval is not attackable because UNIT\_FLAG\_IMMUNE\_TO\_PC is set; implement a better solution by taking over the TC scripts, verify, rework and adapt them to Sol and get rid of the CreatureScript "npc\_battle\_at\_valhalas"; done: sol@5c12a0bb |
| sol@cc3c2ada | 2020-09-04 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@29f2c2ae | 2020-09-02 |      | create appropriate SAI scripts using SMART\_ACTION\_MUSIC; low prio (Brewfest) |
| sol@a07c2b39 | 2020-09-01 | X    | verify and rework SAI; done: sol@97ab5224 |
| sol@34d9998c | 2020-08-31 | X    | verify and rework SAI; done, script seems to be ok: sol@824a2fcf |
| sol@5fd404de | 2020-08-29 | X    | verify and rework SAI; done: sol@9d5d1a41 |
| sol@6f86643e | 2020-08-29 | X    | verify and rework SAI; done: sol@c2c53ea9 |
| sol@2a6a5e48 | 2020-08-29 | X    | verify and rework SAI; done: sol@5554d209 |
| sol@21fb494d | 2020-08-28 | X    | verify and rework SAI; done: sol@83a8c43a |
| sol@cb860e8e | 2020-08-28 | X    | verify and rework SAI; done: sol@975bb42a |
| sol@fd517414 | 2020-08-28 | X    | verify and rework SAI; done: sol@c56f0d2c |
| sol@68bd9985 | 2020-08-27 | X    | verify and rework SAI; done: sol@cbea7076 |
| sol@e6b49e4a | 2020-08-26 | X    | verify and rework SAI; done: sol@dec28c8f |
| sol@9bf66931 | 2020-08-25 | X    | verify and rework SAI; done: sol@e58260af |
| sol@106f6f94 | 2020-08-19 | X    | Rework SQL script as this one is buggy (e.g. no gameobject GUID specified); also Yor's SAI can be easily improved (no need to write a CreatureScript); done: sol@fc3fd371 |
| sol@f754c008 | 2020-08-15 | X    | verify and rework SAI; done: sol@b143cd27 |
| sol@8b57a3e2 | 2020-08-13 | X    | verify and rework SAI; done: sol@d0ad6250 |
| sol@3ddfb568 | 2020-08-12 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@96dc9fc0 | 2020-08-10 | X    | CreatureScript "npc\_taxi" migrated to SAI: sol@b0398ec4 |
| sol@e949ab27 | 2020-08-02 | X    | rework SQL script (wrong / obsolete texts); done: sol@05d19c1b |
| sol@a6a9cfbb | 2020-07-26 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@e8fa3720 | 2020-07-23 | X    | verify and rework SAI; done: sol@8057cea6 |
| sol@ab01adbb | 2020-07-21 | X    | verify and rework SAI; done: sol@2d7c1d08 |
| sol@8449a0b0 | 2020-07-21 | X    | verify and rework SAI; done: sol@898ca467 |
| sol@a0737047 | 2020-07-14 | X    | verify and rework SAI; done: sol@5045815b |
| sol@26dcedd7 | 2020-07-13 | X    | verify and rework SAI; done: sol@5e04edf1 |
| sol@41c8a116 | 2020-07-12 | X    | verify and rework SAI; done: sol@9b84fd44 |
| sol@6d460c54 | 2020-07-07 | X    | verify and rework SAI; done: sol@7321c904 |
| sol@3dbd0181 | 2020-07-03 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@849edc24 | 2020-07-01 | X    | verify and rework DB script; done: sol@d58e08d5 |
| sol@9410e409 | 2020-06-24 | X    | verify and rework SAI; done: sol@bf97855c |
| sol@255989c1 | 2020-06-23 | X    | verify and rework SAI; done: sol@5d62548b |
| sol@444f691e | 2020-06-17 | X    | verify and rework SAI; done: sol@8d1367d8 |
| sol@82dab24a | 2020-06-16 | X    | verify and rework SAI; done: sol@71f51551 |
| sol@55fde9ca | 2020-06-14 | X    | verify and rework SAI; done: sol@1d7941f5 |
| sol@aee070b8 | 2020-06-08 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@83e46e20 | 2020-06-07 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@88590fe3 | 2020-06-07 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@ac355433 | 2020-06-05 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@9bd47bd5 | 2020-06-04 | X    | verify and collect the SAI in a separate commit; update: won't take over, as "Dazed" is obviously a wrong spell to use here |
| sol@ece33e4c | 2020-06-04 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
