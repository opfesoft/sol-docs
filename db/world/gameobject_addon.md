# gameobject\_addon

## Structure

| Field                                   | Type       | Attributes | Null | Key | Default | Extra | Comment |
|-----------------------------------------|------------|------------|------|-----|---------|-------|---------|
| [guid](#guid)                           | int(10)    | unsigned   | NO   | PRI | 0       |       |         |
| [invisibilityType](#invisibilitytype)   | tinyint(3) | unsigned   | NO   |     | 0       |       |         |
| [invisibilityValue](#invisibilityvalue) | int(10)    | unsigned   | NO   |     | 0       |       |         |
| [useRotation](#userotation)             | tinyint(1) | unsigned   | NO   |     | 0       |       |         |

## Description of the fields

### guid

Gameobject GUID. See [gameobject.guid](gameobject.md#guid)

### invisibilityType

### invisibilityValue

The invisibility fields are used for special "detect invisibility" spells (the GO is only visible if the player has a specific aura)

### useRotation

For most GOs only [orientation](gameobject.md#orientation) is used for rotation because of lack of correct rotation data. As a workaround another mechanism has been implemented in the core: setting "useRotation = 1" for a GO enables its rotation as it is defined in [gameobject](gameobject.md#rotation0).
