# Emotes

**Emotes.dbc**

This DBC contains emotes which can be used by NPCs.

**Version is : 3.3.5a**

## Structure

| Column     | Type     | Comment                                                                                                               |
|------------|----------|-----------------------------------------------------------------------------------------------------------------------|
| 1          | long     | An ID for the emote. Must be unique.                                                                                  |
| 2          | str      | A descriptive name for the emote.                                                                                     |
| 3          | long     | Refers to an ID in [AnimationData](AnimationData.md). This is the ID of the animation to play.                        |
| 4          | flags    |                                                                                                                       |
| 5          | flags    |                                                                                                                       |
| 6          | long     |                                                                                                                       |
| 7          | long     | Refers to an ID in [SoundEntries](SoundEntries.md). This is the ID of the sound to play when the animation is played. |

## Content

When testing the NPC emotes listed below using the *.npc playemote \#* command, the NPC generally continuously plays the specified emote. When playing the emote through, for example, and SAI script, the NPC may use the emote differently.

| EmoteID | Emote Name |
|---------|------------|
| 0 | ONESHOT_NONE |
| 1 | ONESHOT_TALK(DNR) |
| 2 | ONESHOT_BOW |
| 3 | ONESHOT_WAVE(DNR) |
| 4 | ONESHOT_CHEER(DNR) |
| 5 | ONESHOT_EXCLAMATION(DNR) |
| 6 | ONESHOT_QUESTION |
| 7 | ONESHOT_EAT |
| 10 | STATE_DANCE |
| 11 | ONESHOT_LAUGH |
| 12 | STATE_SLEEP |
| 13 | STATE_SIT |
| 14 | ONESHOT_RUDE(DNR) |
| 15 | ONESHOT_ROAR(DNR) |
| 16 | ONESHOT_KNEEL |
| 17 | ONESHOT_KISS |
| 18 | ONESHOT_CRY |
| 19 | ONESHOT_CHICKEN |
| 20 | ONESHOT_BEG |
| 21 | ONESHOT_APPLAUD |
| 22 | ONESHOT_SHOUT(DNR) |
| 23 | ONESHOT_FLEX |
| 24 | ONESHOT_SHY(DNR) |
| 25 | ONESHOT_POINT(DNR) |
| 26 | STATE_STAND |
| 27 | STATE_READYUNARMED |
| 28 | STATE_WORK_SHEATHED |
| 29 | STATE_POINT(DNR) |
| 30 | STATE_NONE |
| 33 | ONESHOT_WOUND |
| 34 | ONESHOT_WOUNDCRITICAL |
| 35 | ONESHOT_ATTACKUNARMED |
| 36 | ONESHOT_ATTACK1H |
| 37 | ONESHOT_ATTACK2HTIGHT |
| 38 | ONESHOT_ATTACK2HLOOSE |
| 39 | ONESHOT_PARRYUNARMED |
| 43 | ONESHOT_PARRYSHIELD |
| 44 | ONESHOT_READYUNARMED |
| 45 | ONESHOT_READY1H |
| 48 | ONESHOT_READYBOW |
| 50 | ONESHOT_SPELLPRECAST |
| 51 | ONESHOT_SPELLCAST |
| 53 | ONESHOT_BATTLEROAR |
| 54 | ONESHOT_SPECIALATTACK1H |
| 60 | ONESHOT_KICK |
| 61 | ONESHOT_ATTACKTHROWN |
| 64 | STATE_STUN |
| 65 | STATE_DEAD |
| 66 | ONESHOT_SALUTE |
| 68 | STATE_KNEEL |
| 69 | STATE_USESTANDING |
| 70 | ONESHOT_WAVE_NOSHEATHE |
| 71 | ONESHOT_CHEER_NOSHEATHE |
| 92 | ONESHOT_EAT_NOSHEATHE403 ONESHOT_CUSTOMSPELL02 |
| 93 | STATE_STUN_NOSHEATHE404 ONESHOT_CUSTOMSPELL03 |
| 94 | ONESHOT_DANCE405 ONESHOT_CUSTOMSPELL04 |
| 113 | ONESHOT_SALUTE_NOSHEATH406 ONESHOT_CUSTOMSPELL05 |
| 133 | STATE_USESTANDING_NOSHEATHE407 ONESHOT_CUSTOMSPELL06 |
| 153 | ONESHOT_LAUGH_NOSHEATHE408 ONESHOT_CUSTOMSPELL07 |
| 173 | STATE_WORK409 ONESHOT_CUSTOMSPELL08 |
| 193 | STATE_SPELLPRECAST410 ONESHOT_CUSTOMSPELL09 |
| 213 | ONESHOT_READYRIFLE411 ONESHOT_CUSTOMSPELL10 |
| 214 | STATE_READYRIFLE412 STATE_EXCLAIM |
| 233 | STATE_WORK_MINING413 STATE_DANCE_CUSTOM |
| 234 | STATE_WORK_CHOPWOOD415 STATE_SIT_CHAIR_MED |
| 253 | STATE_APPLAUD416 STATE_CUSTOM_SPELL_01 |
| 254 | ONESHOT_LIFTOFF417 STATE_CUSTOM_SPELL_02 |
| 273 | ONESHOT_YES(DNR)418 STATE_EAT |
| 274 | ONESHOT_NO(DNR)419 STATE_CUSTOM_SPELL_04 |
| 275 | ONESHOT_TRAIN(DNR)420 STATE_CUSTOM_SPELL_03 |
| 293 | ONESHOT_LAND421 STATE_CUSTOM_SPELL_05 |
| 313 | STATE_AT_EASE422 STATE_SPELLEFFECT_HOLD |
| 333 | STATE_READY1H423 STATE_EAT_NO_SHEATHE |
| 353 | STATE_SPELLKNEELSTART424 STATE_MOUNT |
| 373 | STAND_STATE_SUBMERGED425 STATE_READY2HL |
| 374 | ONESHOT_SUBMERGE426 STATE_SIT_CHAIR_HIGH |
| 375 | STATE_READY2H427 STATE_FALL |
| 376 | STATE_READYBOW428 STATE_LOOT |
| 377 | ONESHOT_MOUNTSPECIAL429 STATE_SUBMERGED |
| 378 | STATE_TALK430 ONESHOT_COWER(DNR) |
| 379 | STATE_FISHING431 STATE_COWER |
| 380 | ONESHOT_FISHING432 ONESHOT_USESTANDING |
| 381 | ONESHOT_LOOT433 STATE_STEALTH_STAND |
| 382 | STATE_WHIRLWIND434 ONESHOT_OMNICAST_GHOUL (W/SOUND |
| 383 | STATE_DROWNED435 ONESHOT_ATTACKBOW |
| 384 | STATE_HOLD_BOW436 ONESHOT_ATTACKRIFLE |
| 385 | STATE_HOLD_RIFLE437 STATE_SWIM_IDLE |
| 386 | STATE_HOLD_THROWN438 STATE_ATTACK_UNARMED |
| 387 | ONESHOT_DROWN439 ONESHOT_SPELLCAST (W/SOUND) |
| 388 | ONESHOT_STOMP440 ONESHOT_DODGE |
| 389 | ONESHOT_ATTACKOFF441 ONESHOT_PARRY1H |
| 390 | ONESHOT_ATTACKOFFPIERCE442 ONESHOT_PARRY2H |
| 391 | STATE_ROAR443 ONESHOT_PARRY2HL |
| 392 | STATE_LAUGH444 STATE_FLYFALL |
| 393 | ONESHOT_CREATURE_SPECIAL445 ONESHOT_FLYDEATH |
| 394 | ONESHOT_JUMPLANDRUN446 STATE_FLY_FALL |
| 395 | ONESHOT_JUMPEND447 ONESHOT_FLY_SIT_GROUND_DOWN |
| 396 | ONESHOT_TALK_NOSHEATHE448 ONESHOT_FLY_SIT_GROUND_UP |
| 397 | ONESHOT_POINT_NOSHEATHE449 ONESHOT_EMERGE |
| 398 | STATE_CANNIBALIZE450 ONESHOT_DRAGONSPIT |
| 399 | ONESHOT_JUMPSTART451 STATE_SPECIALUNARMED |
| 400 | STATE_DANCESPECIAL452 ONESHOT_FLYGRAB |
| 401 | ONESHOT_DANCESPECIAL453 STATE_FLYGRABCLOSED |
| 402 | ONESHOT_CUSTOMSPELL01454 ONESHOT_FLYGRABTHROWN |
| 455 | STATE_FLY_SIT_GROUND |
| 456 | STATE_WALKBACKWARDS |
| 457 | ONESHOT_FLYTALK |
| 458 | ONESHOT_FLYATTACK1H |
| 459 | STATE_CUSTOMSPELL08 |
| 460 | ONESHOT_FLY_DRAGONSPIT |
| 461 | STATE_SIT_CHAIR_LOW |
| 462 | ONE_SHOT_STUN |
| 463 | ONESHOT_SPELLCAST_OMNI |
| 465 | STATE_READYTHROWN |
| 466 | ONESHOT_WORK_CHOPWOOD |
| 467 | ONESHOT_WORK_MINING |
| 468 | STATE_SPELL_CHANNEL_OMNI |
| 469 | STATE_SPELL_CHANNEL_DIRECTED |
| 470 | STAND_STATE_NONE |
| 471 | STATE_READYJOUST |
| 473 | STATE_STRANGULATE |
| 474 | STATE_READYSPELLOMNI |
| 475 | STATE_HOLD_JOUST |
| 476 | ONESHOT_CRY (JAINA PROUDMOORE ONLY) |

## Slash Commands

The IDs here are important to identify the correct player emote (e.g. for SAI event "SMART_EVENT_RECEIVE_EMOTE", see [smart_scripts.event_type](../db/world/smart_scripts.md#event_type))

| ID | Slash Command Name | EmoteID |
|----|--------------------|---------|
| 1 | AGREE | 0 |
| 2 | AMAZE | 0 |
| 3 | ANGRY | 14 |
| 4 | APOLOGIZE | 0 |
| 5 | APPLAUD | 21 |
| 6 | BASHFUL | 24 |
| 7 | BECKON | 0 |
| 8 | BEG | 20 |
| 9 | BITE | 0 |
| 10 | BLEED | 0 |
| 11 | BLINK | 0 |
| 12 | BLUSH | 24 |
| 13 | BONK | 0 |
| 14 | BORED | 0 |
| 15 | BOUNCE | 0 |
| 16 | BRB | 0 |
| 17 | BOW | 2 |
| 18 | BURP | 0 |
| 19 | BYE | 3 |
| 20 | CACKLE | 11 |
| 21 | CHEER | 4 |
| 22 | CHICKEN | 19 |
| 23 | CHUCKLE | 11 |
| 24 | CLAP | 21 |
| 25 | CONFUSED | 6 |
| 26 | CONGRATULATE | 5 |
| 27 | COUGH | 0 |
| 28 | COWER | 431 |
| 29 | CRACK | 0 |
| 30 | CRINGE | 0 |
| 31 | CRY | 18 |
| 32 | CURIOUS | 6 |
| 33 | CURTSEY | 2 |
| 34 | DANCE | 10 |
| 35 | DRINK | 7 |
| 36 | DROOL | 0 |
| 37 | EAT | 7 |
| 38 | EYE | 0 |
| 39 | FART | 0 |
| 40 | FIDGET | 0 |
| 41 | FLEX | 23 |
| 42 | FROWN | 0 |
| 43 | GASP | 5 |
| 44 | GAZE | 0 |
| 45 | GIGGLE | 11 |
| 46 | GLARE | 0 |
| 47 | GLOAT | 11 |
| 48 | GREET | 3 |
| 49 | GRIN | 0 |
| 50 | GROAN | 0 |
| 51 | GROVEL | 20 |
| 52 | GUFFAW | 11 |
| 53 | HAIL | 3 |
| 54 | HAPPY | 0 |
| 55 | HELLO | 3 |
| 56 | HUG | 0 |
| 57 | HUNGRY | 0 |
| 58 | KISS | 17 |
| 59 | KNEEL | 68 |
| 60 | LAUGH | 11 |
| 61 | LAYDOWN | 12 |
| 62 | MASSAGE | 0 |
| 63 | MOAN | 0 |
| 64 | MOON | 0 |
| 65 | MOURN | 18 |
| 66 | NO | 274 |
| 67 | NOD | 273 |
| 68 | NOSEPICK | 0 |
| 69 | PANIC | 0 |
| 70 | PEER | 0 |
| 71 | PLEAD | 20 |
| 72 | POINT | 25 |
| 73 | POKE | 0 |
| 74 | PRAY | 16 |
| 75 | ROAR | 15 |
| 76 | ROFL | 11 |
| 77 | RUDE | 14 |
| 78 | SALUTE | 66 |
| 79 | SCRATCH | 0 |
| 80 | SEXY | 0 |
| 81 | SHAKE | 0 |
| 82 | SHOUT | 22 |
| 83 | SHRUG | 6 |
| 84 | SHY | 24 |
| 85 | SIGH | 0 |
| 86 | SIT | 13 |
| 87 | SLEEP | 12 |
| 88 | SNARL | 0 |
| 89 | SPIT | 0 |
| 90 | STARE | 0 |
| 91 | SURPRISED | 0 |
| 92 | SURRENDER | 20 |
| 93 | TALK | 1 |
| 94 | TALKEX | 5 |
| 95 | TALKQ | 6 |
| 96 | TAP | 0 |
| 97 | THANK | 1 |
| 98 | THREATEN | 0 |
| 99 | TIRED | 0 |
| 100 | VICTORY | 4 |
| 101 | WAVE | 3 |
| 102 | WELCOME | 3 |
| 103 | WHINE | 0 |
| 104 | WHISTLE | 0 |
| 105 | WORK | 0 |
| 106 | YAWN | 0 |
| 107 | BOGGLE | 6 |
| 108 | CALM | 0 |
| 109 | COLD | 0 |
| 110 | COMFORT | 0 |
| 111 | CUDDLE | 0 |
| 112 | DUCK | 0 |
| 113 | INSULT | 14 |
| 114 | INTRODUCE | 0 |
| 115 | JK | 0 |
| 116 | LICK | 0 |
| 117 | LISTEN | 0 |
| 118 | LOST | 6 |
| 119 | MOCK | 0 |
| 120 | PONDER | 6 |
| 121 | POUNCE | 0 |
| 122 | PRAISE | 0 |
| 123 | PURR | 0 |
| 124 | PUZZLE | 6 |
| 125 | RAISE | 0 |
| 126 | READY | 0 |
| 127 | SHIMMY | 0 |
| 128 | SHIVER | 0 |
| 129 | SHOO | 0 |
| 130 | SLAP | 0 |
| 131 | SMIRK | 0 |
| 132 | SNIFF | 0 |
| 133 | SNUB | 0 |
| 134 | SOOTHE | 0 |
| 135 | STINK | 0 |
| 136 | TAUNT | 19 |
| 137 | TEASE | 0 |
| 138 | THIRSTY | 0 |
| 139 | VETO | 0 |
| 140 | SNICKER | 0 |
| 141 | STAND | 26 |
| 142 | TICKLE | 0 |
| 143 | VIOLIN | 18 |
| 163 | SMILE | 0 |
| 183 | RASP | 14 |
| 203 | PITY | 0 |
| 204 | GROWL | 15 |
| 205 | BARK | 0 |
| 223 | SCARED | 430 |
| 224 | FLOP | 0 |
| 225 | LOVE | 0 |
| 226 | MOO | 0 |
| 243 | COMMEND | 21 |
| 264 | TRAIN | 275 |
| 303 | HELPME | 22 |
| 304 | INCOMING | 25 |
| 305 | CHARGE | 25 |
| 306 | FLEE | 22 |
| 307 | ATTACKMYTARGET | 15 |
| 323 | OOM | 1 |
| 324 | FOLLOW | 1 |
| 325 | WAIT | 1 |
| 326 | HEALME | 1 |
| 327 | OPENFIRE | 25 |
| 328 | FLIRT | 24 |
| 329 | JOKE | 1 |
| 343 | GOLFCLAP | 21 |
| 363 | WINK | 0 |
| 364 | PAT | 0 |
| 365 | SERIOUS | 0 |
| 366 | MOUNTSPECIAL | 377 |
| 367 | GOODLUCK | 0 |
| 368 | BLAME | 25 |
| 369 | BLANK | 0 |
| 370 | BRANDISH | 0 |
| 371 | BREATH | 0 |
| 372 | DISAGREE | 274 |
| 373 | DOUBT | 274 |
| 374 | EMBARRASS | 0 |
| 375 | ENCOURAGE | 0 |
| 376 | ENEMY | 0 |
| 377 | EYEBROW | 0 |
| 378 | TOAST | 7 |
| 379 | FAIL | 18 |
| 380 | HIGHFIVE | 0 |
| 381 | ABSENT | 0 |
| 382 | ARM | 0 |
| 383 | AWE | 0 |
| 384 | BACKPACK | 0 |
| 385 | BADFEELING | 0 |
| 386 | CHALLENGE | 0 |
| 387 | CHUG | 0 |
| 389 | DING | 0 |
| 390 | FACEPALM | 0 |
| 391 | FAINT | 0 |
| 392 | GO | 0 |
| 393 | GOING | 0 |
| 394 | GLOWER | 0 |
| 395 | HEADACHE | 0 |
| 396 | HICCUP | 0 |
| 398 | HISS | 0 |
| 399 | HOLDHAND | 0 |
| 401 | HURRY | 0 |
| 402 | IDEA | 0 |
| 403 | JEALOUS | 0 |
| 404 | LUCK | 0 |
| 405 | MAP | 0 |
| 406 | MERCY | 20 |
| 407 | MUTTER | 0 |
| 408 | NERVOUS | 0 |
| 409 | OFFER | 0 |
| 410 | PET | 0 |
| 411 | PINCH | 0 |
| 413 | PROUD | 0 |
| 414 | PROMISE | 0 |
| 415 | PULSE | 0 |
| 416 | PUNCH | 0 |
| 417 | POUT | 0 |
| 418 | REGRET | 0 |
| 420 | REVENGE | 0 |
| 421 | ROLLEYES | 0 |
| 422 | RUFFLE | 0 |
| 423 | SAD | 0 |
| 424 | SCOFF | 0 |
| 425 | SCOLD | 0 |
| 426 | SCOWL | 0 |
| 427 | SEARCH | 0 |
| 428 | SHAKEFIST | 0 |
| 429 | SHIFTY | 0 |
| 430 | SHUDDER | 0 |
| 431 | SIGNAL | 0 |
| 432 | SILENCE | 0 |
| 433 | SING | 1 |
| 434 | SMACK | 0 |
| 435 | SNEAK | 0 |
| 436 | SNEEZE | 0 |
| 437 | SNORT | 0 |
| 438 | SQUEAL | 0 |
| 439 | STOPATTACK | 0 |
| 440 | SUSPICIOUS | 0 |
| 441 | THINK | 0 |
| 442 | TRUCE | 0 |
| 443 | TWIDDLE | 0 |
| 444 | WARN | 0 |
| 445 | SNAP | 0 |
| 446 | CHARM | 0 |
| 447 | COVEREARS | 0 |
| 448 | CROSSARMS | 0 |
| 449 | LOOK | 0 |
| 450 | OBJECT | 25 |
| 451 | SWEAT | 0 |
| 453 | YW | 1 |
