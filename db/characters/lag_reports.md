# lag\_reports

This table stores the lag reports made by players in-game (when they click on "Help Request").

## Structure

| Field                     | Type        | Attributes | Key | Null | Default | Extra          | Comment |
|---------------------------|-------------|------------|-----|------|---------|----------------|---------|
| [reportId](#reportid)     | int(10)     | unsigned   | PRI | NO   |         |auto\_increment |         |
| [guid](#guid)             | int(10)     | unsigned   |     | NO   | 0       |                |         |
| [lagType](#lagtype)       | tinyint(3)  | unsigned   |     | NO   | 0       |                |         |
| [mapId](#mapid)           | smallint(5) | unsigned   |     | NO   | 0       |                |         |
| [posX](#posx)             | float       |            |     | NO   | 0       |                |         |
| [posY](#posy)             | float       |            |     | NO   | 0       |                |         |
| [posZ](#posz)             | float       |            |     | No   | 0       |                |         |
| [latency](#latency)       | int(10)     | unsigned   |     | No   | 0       |                |         |
| [createTime](#createtime) | int(10)     | unsigned   |     | No   | 0       |                |         |

## Description of the fields

### reportId

Report ID

### guid

Player guid. See [characters.guid](characters.md#guid)

### lagType

* 0 = Loot related
* 1 = Auction House related
* 2 = Mail related
* 3 = Chat related
* 4 = Movement related
* 5 = Spells and Abilities related

### mapId

Map where lag was reported. See [Map.dbc](../../dbc/Map.md)

### posX

Position X

### posY

Position Y

### posZ

Position Z

### latency

Latency in ms at the moment of the report.

### createTime

Creation date (Unix time)
