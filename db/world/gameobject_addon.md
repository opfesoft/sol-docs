
Column | Type | Description
--- | --- | ---
Guid | int(10) unsigned | 
InvisibilityType | tinyint(3) unsigned | 
InvisibilityValue | int(10) unsigned | 

Additional info:
- For most GOs only orientation is used for rotation because of lack of correct rotation data.
- As a workaround another mechanism has been implemented in the core: setting both invisibility type and value to 0 for a GO enables its rotation as it is defined in [gameobject](gameobject.md).

see [src/server/game/Entities/GameObject/GameObject.cpp](https://gitlab.com/opfesoft/sol/-/blob/master/src/server/game/Entities/GameObject/GameObject.cpp):
```cpp
// xinef: hackfix - but make it possible to use original WorldRotation (using special gameobject addon data)
// pussywizard: temporarily calculate WorldRotation from orientation, do so until values in db are correct
if (addon && addon->invisibilityType == INVISIBILITY_GENERAL && addon->InvisibilityValue == 0)
    SetWorldRotation(rotation);
else
    SetWorldRotationAngles(NormalizeOrientation(GetOrientation()), 0.0f, 0.0f);
break;
```
