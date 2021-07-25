# transports

This table contains all type 15 transports (ships, zeppelins etc.). All other transport types have their frame time read from TransportAnimation.dbc.

**Note:** Transports have their own [map](../../dbc/Map.md)

## Structure

| Field                   | Type         | Attribute | Key | Null | Default | Extra           | Comment |
|-------------------------|--------------|-----------|-----|------|---------|-----------------|---------|
[guid](#guid)             | int(10)      | unsigned  | PRI | NO   | NULL    | auto\_increment |         |
[entry](#entry)           | mediumint(8) | unsigned  | UNI | NO   | 0       |                 |         |
[name](#name)             | text         |           |     | YES  | NULL    |                 |         |
[ScriptName](#scriptname) | char(64)     |           |     | NO   |         |                 |         |

## Description of the fields

### guid

A unique identifier for the transport. Normally just incremented by 1 for each new entry.

### entry

[gameobject\_template.entry](gameobject_template.md#entry) to be used for this transport. It must be a type 15 gameobject.

### name

An arbitrary name to describe the transport entry.

### ScriptName
