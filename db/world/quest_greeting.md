# quest\_greeting

This table holds greeting texts shown for quest giver NPCs or gameobjects. Concerning NPCs they are only shown if UNIT\_NPC\_FLAG\_QUESTGIVER is set and UNIT\_NPC\_FLAG\_GOSSIP is **not set** (see [creature\_template.npcflag](creature_template.md#npcflag)).

## Structure

| Field                               | Type         | Attributes | Null | Key | Default | Extra | Comment |
|-------------------------------------|--------------|------------|------|-----|---------|-------|---------|
| [ID](#id)                           | mediumint(8) | unsigned   | NO   | PRI | 0       |       |         |
| [Type](#type)                       | tinyint(3)   | unsigned   | NO   | PRI | 0       |       |         |
| [GreetEmoteType](#greetemotetype)   | smallint(5)  | unsigned   | NO   |     | 0       |       |         |
| [GreetEmoteDelay](#greetemotedelay) | int(10)      | unsigned   | NO   |     | 0       |       |         |
| [Greeting](#greeting)               | text         |            | NO   |     | NULL    |       |         |

## Description of the fields

### id

[creature ID](creature_template.md#entry) or [gameobject ID](gameobject_template.md#entry).

### type

- 0: creature (use [creature ID](creature_template.md#entry) as ID)
- 1: gameobject (use [gameobject ID](gameobject_template.md#entry) as ID)

### greetemotetype

The NPC emote, see [Emotes.dbc](../../dbc/Emotes.md).

### greetemotedelay

The emote delay in milliseconds.

### greeting

The greeting text.

