
Column | Type | Description
--- | --- | ---
[guid](gameobject.md#guid) | int(10) unsigned | 
invisibilityType | tinyint(3) unsigned | 
invisibilityValue | int(10) unsigned | 
useRotation | tinyint(1) unsigned | 

Additional info:
- The invisibility fields are used for special "detect invisibility" spells (the GO is only visible if the player has a specific aura)
- For most GOs only [orientation](gameobject.md#orientation) is used for rotation because of lack of correct rotation data.
- As a workaround another mechanism has been implemented in the core: setting "useRotation = 1" for a GO enables its rotation as it is defined in [gameobject](gameobject.md#rotation0).
