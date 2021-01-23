TODOs:

| commit       | date       | done | todo / comment |
|--------------|------------|------|----------------|
| sol@0a8a7ef1 | 2021-01-22 |      | perhaps take over if nothing else is left to do; not really needed as this was also not the case on retail at the time; low prio |
| sol@f9b836ef | 2021-01-22 | X    | wrong, has to update coordinates in quest\_poi\_points; done: sol@0e6eac8d |
| sol@42244612 | 2021-01-19 |      | verify and rework SQL script |
| sol@eddde219 | 2021-01-18 |      | INHABIT\_ROOT won't be taken over; rooting creatures should be handled via scripts, not via inhabit type; only fix the original issue |
| sol@b2e7f397 | 2021-01-16 |      | verify and rework SQL script |
| sol@943c1e7a | 2021-01-14 |      | verify changes |
| sol@9c70c6e4 | 2021-01-14 |      | verify gameobjects and quest |
| sol@d54a860a | 2021-01-13 |      | verify and rework SQL script |
| sol@b9375fff | 2021-01-12 |      | verify and rework SQL script & code changes |
| sol@adb877f2 | 2021-01-10 |      | verify and rework SQL script |
| sol@7cf097ea | 2021-01-10 |      | take over if needed |
| sol@3fb18944 | 2021-01-09 |      | deleting the second gossip option is wrong as the SAI triggers different spells depending on the selected option; also verify the quest chain, it should not be possible to have both bombing runs at the same time |
| sol@b1452b5b | 2021-01-09 |      | verify and rework SQL script |
| sol@c5fe21fe | 2021-01-08 |      | verify code and compare with TC |
| sol@9592028a | 2021-01-08 |      | verify text changes |
| sol@2dd6141a | 2021-01-07 |      | verify changes and take over if needed |
| sol@ba534cea | 2021-01-07 |      | verify SAI |
| sol@8b101654 | 2021-01-07 |      | verify and rework SQL script |
| sol@9427da06 | 2021-01-06 |      | verify priest trainer spells |
| sol@f869c17d | 2021-01-06 |      | use UPDATE instead of DELETE / INSERT |
| sol@1a0e4fc6 | 2021-01-05 |      | changing the walk speed is wrong; adjust CreatureScript instead (also check and improve waypoints) |
| sol@b2761626 | 2021-01-04 |      | probably find a better solution (AC commit reverted with sol@df600f99); very low prio as it's not really needed and could cause many unexpected bugs |
| sol@64c686c4 | 2021-01-04 |      | verify creature spawns |
| sol@92881ad1 | 2021-01-04 |      | verify and rework SQL script |
| sol@0bd7e9dd | 2021-01-03 |      | verify and rework SQL script |
| sol@1078bf49 | 2021-01-03 | X    | use a better solution; done: sol@9c7d90d6 |
| sol@469d5a8b | 2021-01-02 |      | verify and rework SQL script |
| sol@1e5e20ab | 2021-01-02 |      | verify and rework SQL script |
| sol@f366db28 | 2021-01-01 |      | verify GOs and their associated quests before changing the respawn time |
| sol@106684fb | 2020-12-31 |      | verify SQL script & quest |
| sol@0264289f | 2020-12-29 |      | verify SQL script & texts |
| sol@57a4f432 | 2020-12-27 |      | verify SQL script |
| sol@aec0dbb7 | 2020-12-25 |      | verify CreatureScript |
| sol@d710057a | 2020-12-25 |      | verify and rework SQL script / CreatureScript |
| sol@1f5babf0 | 2020-12-22 |      | take over if needed |
| sol@dd9d9e0c | 2020-12-15 |      | verify and rework SQL script (see also AC commit sol@d54a860a) |
| sol@086ad6c9 | 2020-12-13 |      | use the already existing broadcast texts |
| sol@af53598f | 2020-12-11 |      | verify solution (and bugfixes sol@282966c1, sol@d3aff86c) |
| sol@62cb1f36 | 2020-12-10 |      | verify and rework SQL script |
| sol@963553a9 | 2020-12-10 |      | verify and rework SQL script |
| sol@6d10d075 | 2020-12-09 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@04c245cf | 2020-12-04 |      | verify and rework SQL script |
| sol@755e30f9 | 2020-12-04 |      | verify if this actually fixes anything; the original PR provides no description on the issue and contains no test specification (the attached backtrace is invalid: too old, contains no AC commit and line numbers also don't match) |
| sol@5fe10355 | 2020-12-03 |      | verify SQL script and actual issue |
| sol@0baecd3e | 2020-12-01 |      | check if this contains something useful; don't take over because it breaks the existing behaviour of creatures in dungeons following the player throughout the dungeon; fleeing creatures already fixed with commits sol@5d02c61f and sol@4caa8425 |
| sol@1c30f878 | 2020-11-29 |      | verify and rework SQL script |
| sol@01fa6257 | 2020-11-28 |      | verify changes and take over if needed |
| sol@931609d2 | 2020-11-26 |      | find a better solution (restore the player's phases according to his auras) |
| sol@1a8110dc | 2020-11-25 | X    | use a creature pool instead of deleting the second spawn; done: sol@06e0a18a |
| sol@2e39d452 | 2020-11-24 |      | verify and rework SQL script |
| sol@5d3bb608 | 2020-11-23 |      | verify and only take over if actually needed (if so, also take over sol@2788d495); fix PvP flag for the NPCs |
| sol@fb69db21 | 2020-11-19 |      | probably find a better solution (AC commit reverted with sol@35fb9f49, see new solution sol@af53598f and bugfixes sol@282966c1, sol@d3aff86c) |
| sol@9a8aa615 | 2020-11-16 |      | verify and rework SQL script |
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
| sol@da4235cc | 2020-11-09 |      | verify loot and compare with TC version |
| sol@e5fc4fca | 2020-11-08 | X    | verify and rework SQL script; done: sol@8ad44364 |
| sol@9bb6b15c | 2020-11-08 | X    | verify and rework SQL script; done: sol@ee0ca7c5 |
| sol@5254aec6 | 2020-11-07 |      | verify and compare with TC implementation |
| sol@1dc1beb3 | 2020-11-06 | X    | verify and rework SQL script; done: sol@1807c1f4 |
| sol@9763c4f4 | 2020-11-06 | X    | verify and rework SQL script; done: sol@6a23be7c |
| sol@74a34b59 | 2020-11-06 |      | use correct position above ground, not in the cave |
| sol@f4a5907a | 2020-11-06 |      | verify WP path |
| sol@82ee9088 | 2020-11-02 |      | verify SQL script, compare with TC version |
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
| sol@d5bb6ba1 | 2020-10-21 |      | see also follow-up bugfix sol@b3a967db; could contain several other hidden bugs, so only take over if really needed and double-check the code changes in that case |
| sol@ab5933ef | 2020-10-17 | X    | take over if needed; done: sol@79964075 |
| sol@24cfa307 | 2020-10-11 |      | verify SQL script |
| sol@4cca286a | 2020-10-09 | X    | verify and find a better solution as flying creatures respawn on the ground instead of their actual spawn point; done: sol@afa10355 |
| sol@3368e0f8 | 2020-10-08 |      | verify new creature positions |
| sol@22f8195c | 2020-10-07 |      | verify changes and new creature ID |
| sol@369d292c | 2020-10-07 |      | verify SQL script |
| sol@b67c30e2 | 2020-10-03 | X    | verify quest and texts; remove hard-coded gossip; done: sol@cbe3c232 |
| sol@3e81beac | 2020-09-28 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@72025003 | 2020-09-12 | X    | SAI was just taken over from TC without further verification (it is only a small part of the scripts implementing the whole quest chain); Prince Sandoval is not attackable because UNIT\_FLAG\_IMMUNE\_TO\_PC is set; implement a better solution by taking over the TC scripts, verify, rework and adapt them to Sol and get rid of the CreatureScript "npc\_battle\_at\_valhalas"; done: sol@5c12a0bb |
| sol@cc3c2ada | 2020-09-04 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
| sol@29f2c2ae | 2020-09-02 |      | create appropriate SAI scripts using SMART\_ACTION\_MUSIC; low prio |
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
| sol@9bd47bd5 | 2020-06-04 | X    | verify and collect the SAI in a separate commit; won't take over, as "Dazed" is obviously a wrong spell to use here |
| sol@ece33e4c | 2020-06-04 | X    | verify and collect the SAI in a separate commit; done: sol@0fc62baf |
