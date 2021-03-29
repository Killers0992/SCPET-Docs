## `GameSettings`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.GameSettings
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioMixer` | mixer |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, String>` | DisabledMods |  | 
| `Int32` | latestServerConfigVersion |  | 
| `AudioMixer` | mixerAsset |  | 
| `JsonServerSettings` | serverSettings |  | 
| `JsonGameSettings` | settings |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ApplyAudio() |  | 
| `void` | ApplyWidthHeight() |  | 
| `Boolean` | GetCheatSetting() |  | 
| `Boolean` | GetFullScreen() |  | 
| `Boolean` | GetHeadBob() |  | 
| `Int32` | GetHeight() |  | 
| `Single` | GetMouseSenseX() |  | 
| `Single` | GetMouseSenseY() |  | 
| `Int32` | GetQuality() |  | 
| `LightShadows` | GetShadows() |  | 
| `Int32` | GetTextureQuality() |  | 
| `Int32` | GetWidth() |  | 
| `void` | LoadDisabledMods() |  | 
| `void` | LoadServerSettings() |  | 
| `void` | LoadSettings() |  | 
| `void` | ReadAudio() |  | 
| `void` | SaveDisabledMods() |  | 
| `void` | SaveSettings() |  | 
| `void` | SetFullScreen(`Boolean` value) |  | 
| `void` | SetHeight(`Int32` value) |  | 
| `void` | SetMouseSenseX(`Single` sense) |  | 
| `void` | SetMouseSenseY(`Single` sense) |  | 
| `void` | SetQuality(`Int32` qual) |  | 
| `void` | SetShadows(`LightShadows` shadows) |  | 
| `void` | SetTextureQuality(`Int32` qual) |  | 
| `void` | SetWidth(`Int32` value) |  | 


Static Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `SettingsUpdated` | OnSettingsSaved |  | 


## `HolidayController`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.HolidayController

```

Static Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `HolidayUpdate` | activeHoliday |  | 
| `Boolean` | isHolidayActive |  | 


## `HolidaySpawner`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.HolidaySpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject[]` | objects |  | 
| `HolidayUpdate` | update |  | 


## `HolidayUpdate`

```csharp
public enum VirtualBrightPlayz.SCP_ET.Misc.HolidayUpdate
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `-1` | None |  | 
| `0` | SCPETBirthday |  | 
| `1` | AprilFools |  | 
| `2` | Halloween |  | 
| `3` | Christmas |  | 


## `InputManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.InputManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `InputActionAsset` | input |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | LoadBinds() |  | 
| `void` | SaveBinds() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `InputManager` | manager |  | 


## `LanguageDropdown`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.LanguageDropdown
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dropdown` | dropdown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetLanguage(`Int32` LanguageIndex) |  | 
| `IEnumerator` | Start() |  | 


## `PrefabLightmapData`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.PrefabLightmapData
    : MonoBehaviour

```

## `QMapImporter`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.QMapImporter
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | className |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Light` | GetLight() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ImportMap(`Stream` stream) |  | 


## `RandomAmbient`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.RandomAmbient
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip[]` | clips |  | 
| `AudioClip[]` | clips106 |  | 
| `PlayerController` | ctrl |  | 
| `DimensionType` | dimension |  | 
| `LayerMask` | mask |  | 
| `Single` | maxTimer |  | 
| `Single` | minTimer |  | 
| `Boolean` | raycast |  | 
| `AudioSource` | source |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip[]` | GetValidClips() |  | 


## `Resolution_Dropdown`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.Resolution_Dropdown
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetResolution(`Int32` resoltionIndex) |  | 


## `RLCChild`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.RLCChild
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RoomLightController` | rlc |  | 


## `RoomLightController`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.RoomLightController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider[]` | cols |  | 
| `PlayerController` | ctrl |  | 
| `Boolean` | isPhysicsOn |  | 
| `Boolean` | isVisible |  | 
| `Light[]` | lights |  | 
| `List<MeshCollider>` | mColliders |  | 
| `List<GameObject>` | pViewers |  | 
| `GameObject` | root |  | 
| `List<GameObject>` | viewers |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Disable() |  | 
| `IEnumerator` | DisableLate() |  | 
| `void` | DisablePhysics() |  | 
| `void` | Enable() |  | 
| `void` | EnablePhysics() |  | 


## `Scp008Settings`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.Scp008Settings

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | maxDamage |  | 
| `Int32` | minDamage |  | 


## `Scp106Settings`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.Scp106Settings

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | enableFemurBreaker |  | 
| `Int32` | followTimer |  | 
| `Int32` | grabDamage |  | 
| `Int32` | maxSpawnTimer |  | 
| `Int32` | minSpawnTimer |  | 


## `Scp173Settings`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.Scp173Settings

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | openDoors |  | 
| `Single` | spawnTimer |  | 


## `Scp914Settings`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.Scp914Settings

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | affectPlayers |  | 
| `List<String>` | recipeOverrides |  | 


## `Scp939Settings`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.Scp939Settings

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | baseDamagePerBite |  | 
| `Single` | randomDamage |  | 


## `ToggleTimer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.ToggleTimer
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject[]` | objects |  | 
| `Single` | progress |  | 
| `Single` | timer |  | 


## `VMouse`

```csharp
public class VirtualBrightPlayz.SCP_ET.Misc.VMouse
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Canvas` | canvas |  | 
| `Single` | minMove |  | 
| `Single` | speed |  | 
| `Single` | timeout |  | 
| `RectTransform` | xform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | Start() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `VMouse` | instance |  | 


