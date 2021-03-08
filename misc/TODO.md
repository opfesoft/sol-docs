TODOs:

| commit       | date       | done | todo / comment |
|--------------|------------|------|----------------|
| sol@1e90722a | 2021-03-07 |      | verify and rework SQL script |
| sol@53d73416 | 2021-03-07 |      | broadcast text ID already fixed with commit sol@3e648f34, but the quest does not seem to be working correctly; compare with "official" walkthrough |
| sol@9239f033 | 2021-03-07 |      | creature IDs 4295 and 4300 should keep their talk actions, but it is necessary to clean up the creature texts and adjust their SAI |
| sol@303ba07b | 2021-03-07 |      | the spell "New Summon Test" is obviously wrong here, so instead of manipulating the Spell DBC improve the spell script "spell\_q9452\_cast\_net" to directly summon the creature with an appropriate summon type |
| sol@bfb6faa2 | 2021-03-06 |      | wrong; instead of deleting the reference loot ID from creature 16348 remove item 2088 from reference loot ID 24076 and add the item directly to the loot of creature 831 (see TC version) |
| sol@a269c51d | 2021-03-05 |      | verify deleted loot and compare with TC version |
| sol@727590dc | 2021-03-04 |      | verify and rework SQL script |
| sol@81957089 | 2021-02-28 |      | implement another solution (remark: the attacking NPCs should not transform to worgen at all; also delete the conditions which were used in the old SAI script to control the transformation according to the Pyrewood Village Event; this has been forgotten in the AC commit and will cause a bug in the SAI execution) |
| sol@41fa30a5 | 2021-02-28 |      | the quest is working on Sol; the movement bugs described in the AC issue seem to be caused by AC commit sol@c8f43d85 (another good hint to not take this commit over); nevertheless, rework the existing SAI as it seems to be very old and the NPC following the player should indeed fight the enemies |
| sol@573a5605 | 2021-02-25 |      | verify and rework SQL script |
| sol@dbd78936 | 2021-02-24 |      | verify and rework SQL script; low prio (Dungeon: Gnomeregan) |
| sol@ae2bd072 | 2021-02-24 |      | verify and rework SQL script; low prio (Dungeon: Gnomeregan) |
| sol@f910d635 | 2021-02-21 |      | verify and rework SQL script |
| sol@922f87e5 | 2021-02-21 |      | verify and rework SQL script |
| sol@2cd534de | 2021-02-16 |      | verify and rework SQL script |
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
| sol@c8f43d85 | 2021-02-01 |      | perhaps try to find a better solution for some of the changes if nothing else is left to do (also see bugfixes sol@e7bfbe76, sol@522eb9a7, sol@695a7402); very low prio as it's not really needed and could cause many unexpected bugs / performance issues |
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
| sol@d710057a | 2020-12-25 |      | verify and rework SQL script / CreatureScript; low prio (Dungeon: Ulduar) |
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
| sol@d5bb6ba1 | 2020-10-21 |      | see also follow-up bugfix sol@b3a967db; could contain several other hidden bugs, so only take over if really needed and double-check the code changes in that case; low prio |
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
