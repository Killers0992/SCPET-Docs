## `AnimMoveTest`

```csharp
public class VirtualBrightPlayz.SCP_ET.AnimMoveTest
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Animator` | anim |  | 
| `Single` | move |  | 


## `AssetManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.AssetManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<AssetBundle>` | assetBundles |  | 
| `String` | currentAssetName |  | 
| `String` | currentStage |  | 
| `Boolean` | isDone |  | 
| `Single` | progress |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Load() |  | 
| `IEnumerator` | LoadAllAssets(`String` path) |  | 
| `T` | LoadAsset(`String` path) |  | 
| `IEnumerator` | LoadAssetBundle(`String` path, `String` assetname) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AssetManager` | manager |  | 


## `Billboard`

```csharp
public class VirtualBrightPlayz.SCP_ET.Billboard
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | X |  | 
| `Boolean` | Y |  | 
| `Boolean` | Z |  | 


## `Broadcast`

```csharp
public class VirtualBrightPlayz.SCP_ET.Broadcast

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | Duration |  | 
| `String` | Message |  | 


## `BroadcastUI`

```csharp
public class VirtualBrightPlayz.SCP_ET.BroadcastUI
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | displayTimer |  | 
| `Single` | fadeOutWaitTimer |  | 
| `Single` | fadeSpeed |  | 
| `CanvasGroup` | group |  | 
| `Boolean` | isDisplayingBroadcast |  | 
| `Boolean` | isFadingIn |  | 
| `Boolean` | isFadingOut |  | 
| `Single` | progress |  | 
| `Queue<Broadcast>` | queue |  | 
| `TextMeshProUGUI` | text |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clear() |  | 
| `void` | FadeIn() |  | 
| `void` | FadeOut() |  | 
| `void` | QueueMessage(`String` message, `Single` duration) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BroadcastUI` | instance |  | 


## `ChatCommand`

```csharp
public class VirtualBrightPlayz.SCP_ET.ChatCommand
    : Attribute, _Attribute

```

## `CommandResponse`

```csharp
public class VirtualBrightPlayz.SCP_ET.CommandResponse

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isTranslation |  | 
| `String` | message |  | 
| `Boolean` | success |  | 
| `String[]` | translationArgs |  | 
| `TextType` | translationType |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CommandResponse` | Done |  | 
| `CommandResponse` | Fail |  | 
| `CommandResponse` | Success |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `CommandResponse` | Create(`Boolean` success, `String` str) |  | 
| `CommandResponse` | CreateTranslated(`Boolean` success, `String` str) |  | 
| `CommandResponse` | CreateTranslated(`Boolean` success, `String` str, `String[]` args) |  | 


## `ConsoleLogger`

```csharp
public class VirtualBrightPlayz.SCP_ET.ConsoleLogger

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Log(`Object` data) |  | 
| `void` | LogError(`Object` data) |  | 
| `void` | LogException(`Exception` data) |  | 
| `void` | LogWarning(`Object` data) |  | 


## `CustomPlayerSpawner`

```csharp
public class VirtualBrightPlayz.SCP_ET.CustomPlayerSpawner
    : PlayerSpawner

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnServerAddPlayer(`INetworkConnection` conn) |  | 


## `DecalController`

```csharp
public class VirtualBrightPlayz.SCP_ET.DecalController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | fadeTime |  | 
| `Single` | maxFadeTime |  | 
| `DecalType` | type |  | 


## `DecalType`

```csharp
public enum VirtualBrightPlayz.SCP_ET.DecalType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `-1` | None |  | 
| `0` | Blood |  | 
| `1` | Scp106 |  | 
| `2` | Scp173 |  | 


## `Door`

```csharp
public class VirtualBrightPlayz.SCP_ET.Door
    : NetworkBehaviour, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allow049Open |  | 
| `Boolean` | allow096Open |  | 
| `Boolean` | allow173Open |  | 
| `Boolean` | allow939Open |  | 
| `GameObject[]` | closePos |  | 
| `AudioClip[]` | closeSounds |  | 
| `String` | doorName |  | 
| `DoorType` | doorType |  | 
| `ParticleSystem[]` | dust |  | 
| `ElevatorController` | elevator |  | 
| `AudioClip` | forceClose |  | 
| `Boolean` | isElevator |  | 
| `Boolean` | IsForcedMoving |  | 
| `Boolean` | isLocked |  | 
| `Boolean` | IsMoving |  | 
| `Single` | maxTimeOpen |  | 
| `GameObject[]` | modelPos |  | 
| `UnityEvent` | OnClosed |  | 
| `UnityEvent` | OnOpened |  | 
| `Boolean` | open |  | 
| `AudioClip` | open096 |  | 
| `AudioClip` | open173 |  | 
| `AudioClip` | open939 |  | 
| `Single` | openedByScpTimer |  | 
| `Boolean` | openedByScpWarning |  | 
| `GameObject[]` | openPos |  | 
| `AudioClip[]` | openSounds |  | 
| `Single` | openTimer |  | 
| `Boolean` | rotateDoor |  | 
| `ParticleSystem` | sparks |  | 
| `Single` | speed |  | 
| `AudioClip` | timeWarnClip |  | 
| `Boolean` | useTimeOpen |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Guid |  | 
| `Boolean` | IsOpen |  | 
| `String` | NetworkdoorName |  | 
| `Boolean` | NetworkisLocked |  | 
| `Boolean` | Networkopen |  | 
| `String` | PrefabGuid |  | 
| `JSONVector` | savePos |  | 
| `JSONVector` | saveRot |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdClose() |  | 
| `void` | CmdForceClose() |  | 
| `void` | CmdOpen() |  | 
| `void` | CmdOpen049() |  | 
| `void` | CmdOpen096(`Boolean` force) |  | 
| `void` | CmdOpen173() |  | 
| `void` | CmdOpen939() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | DisplayCaption(`String` message) |  | 
| `void` | LoadComplete() |  | 
| `void` | RpcCloseSound() |  | 
| `void` | RpcForceCloseSound() |  | 
| `void` | RpcOnOpenClose(`Boolean` isopen) |  | 
| `void` | RpcOpenSound() |  | 
| `void` | RpcOpenSound096() |  | 
| `void` | RpcOpenSound173() |  | 
| `void` | RpcOpenSound939() |  | 
| `void` | RpcWarnSound() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | Update() |  | 
| `void` | UserCode_RpcCloseSound() |  | 
| `void` | UserCode_RpcForceCloseSound() |  | 
| `void` | UserCode_RpcOnOpenClose(`Boolean` isopen) |  | 
| `void` | UserCode_RpcOpenSound() |  | 
| `void` | UserCode_RpcOpenSound096() |  | 
| `void` | UserCode_RpcOpenSound173() |  | 
| `void` | UserCode_RpcOpenSound939() |  | 
| `void` | UserCode_RpcWarnSound() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcCloseSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcForceCloseSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcOnOpenClose(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcOpenSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcOpenSound096(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcOpenSound173(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcOpenSound939(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcWarnSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `DoorType`

```csharp
public enum VirtualBrightPlayz.SCP_ET.DoorType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Default |  | 
| `1` | OfficeDoor |  | 
| `2` | Hcz |  | 
| `3` | ContainmentDoor |  | 
| `4` | Checkpoint |  | 
| `5` | CleanRoom |  | 
| `6` | Airlock |  | 
| `7` | Lockroom |  | 
| `8` | Elevator |  | 


## `EditorMenuButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.EditorMenuButton
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OpenMapEditor() |  | 


## `Embed`

```csharp
public class VirtualBrightPlayz.SCP_ET.Embed
    : IEmbedUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `EmbedAuthor` | Author |  | 
| `Int32` | Color |  | 
| `String` | Description |  | 
| `List<EmbedField>` | Fields |  | 
| `EmbedFooter` | Footer |  | 
| `EmbedImage` | Image |  | 
| `EmbedProvider` | Provider |  | 
| `EmbedThumbnail` | Thumbnail |  | 
| `Nullable<DateTimeOffset>` | TimeStamp |  | 
| `String` | Title |  | 
| `String` | Type |  | 
| `String` | Url |  | 
| `EmbedVideo` | Video |  | 


## `EmbedAuthor`

```csharp
public class VirtualBrightPlayz.SCP_ET.EmbedAuthor
    : EmbedUrl, IEmbedUrl, IEmbedIconUrl, IEmbedIconProxyUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | IconUrl |  | 
| `String` | Name |  | 
| `String` | ProxyIconUrl |  | 


## `EmbedField`

```csharp
public class VirtualBrightPlayz.SCP_ET.EmbedField

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Inline |  | 
| `String` | Name |  | 
| `String` | Value |  | 


## `EmbedFooter`

```csharp
public class VirtualBrightPlayz.SCP_ET.EmbedFooter
    : IEmbedIconUrl, IEmbedIconProxyUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | IconUrl |  | 
| `String` | ProxyIconUrl |  | 
| `String` | Text |  | 


## `EmbedImage`

```csharp
public class VirtualBrightPlayz.SCP_ET.EmbedImage
    : EmbedProxyUrl, IEmbedUrl, IEmbedProxyUrl, IEmbedDimension

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | Height |  | 
| `Int32` | Width |  | 


## `EmbedProvider`

```csharp
public class VirtualBrightPlayz.SCP_ET.EmbedProvider
    : EmbedUrl, IEmbedUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Name |  | 


## `EmbedProxyUrl`

```csharp
public abstract class VirtualBrightPlayz.SCP_ET.EmbedProxyUrl
    : EmbedUrl, IEmbedUrl, IEmbedProxyUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ProxyUrl |  | 


## `EmbedThumbnail`

```csharp
public class VirtualBrightPlayz.SCP_ET.EmbedThumbnail
    : EmbedProxyUrl, IEmbedUrl, IEmbedProxyUrl, IEmbedDimension

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | Height |  | 
| `Int32` | Width |  | 


## `EmbedUrl`

```csharp
public abstract class VirtualBrightPlayz.SCP_ET.EmbedUrl
    : IEmbedUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Url |  | 


## `EmbedVideo`

```csharp
public class VirtualBrightPlayz.SCP_ET.EmbedVideo
    : EmbedUrl, IEmbedUrl, IEmbedDimension

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | Height |  | 
| `Int32` | Width |  | 


## `GameSceneLoader`

```csharp
public class VirtualBrightPlayz.SCP_ET.GameSceneLoader
    : MonoBehaviour

```

Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | hasRun |  | 


## `GameSceneManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.GameSceneManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Animator` | animator |  | 
| `Boolean` | done |  | 
| `Boolean` | enableVR |  | 
| `Boolean` | isServer |  | 
| `TextMeshProUGUI` | lHeader |  | 
| `GameObject` | loadingMask |  | 
| `GameObject` | loadingRoot |  | 
| `TextMeshProUGUI` | lSub |  | 
| `String` | networkSceneToLoad |  | 
| `Boolean` | shouldCapture |  | 
| `GameObject` | vrplayer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DirectConnect(`String` serverIp) |  | 
| `IEnumerator` | Loaded() |  | 
| `void` | SetProgress() |  | 
| `void` | StartHost(`String` serverName, `String` mapName, `Int32` hostType, `String` port, `Int32` maxPlayers) |  | 
| `void` | StartServer() |  | 
| `IEnumerator` | Wait() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameSceneManager` | singleton |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | GetArg(`String` argname) |  | 


## `HintController`

```csharp
public class VirtualBrightPlayz.SCP_ET.HintController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | fadeSpeed |  | 
| `Boolean` | isFadingIn |  | 
| `Boolean` | isFadingOut |  | 
| `Single` | length |  | 


## `HintType`

```csharp
public enum VirtualBrightPlayz.SCP_ET.HintType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | IgnoreSettings |  | 
| `1` | Speech |  | 
| `2` | All |  | 


## `HintUI`

```csharp
public class VirtualBrightPlayz.SCP_ET.HintUI
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | text |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddMessage(`String` message, `Color` color, `Single` duration, `HintType` type) |  | 
| `void` | AddTranslatedMessage(`String` message, `Color` color, `Single` duration, `HintType` type) |  | 
| `void` | AddTranslatedMessage(`String` message, `Color` color, `Single` duration, `HintType` type, `String[]` args) |  | 
| `Boolean` | CanShowHint(`HintType` hint) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `HintUI` | instance |  | 


## `IEmbedDimension`

```csharp
public interface VirtualBrightPlayz.SCP_ET.IEmbedDimension

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | Height |  | 
| `Int32` | Width |  | 


## `IEmbedIconProxyUrl`

```csharp
public interface VirtualBrightPlayz.SCP_ET.IEmbedIconProxyUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ProxyIconUrl |  | 


## `IEmbedIconUrl`

```csharp
public interface VirtualBrightPlayz.SCP_ET.IEmbedIconUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | IconUrl |  | 


## `IEmbedProxyUrl`

```csharp
public interface VirtualBrightPlayz.SCP_ET.IEmbedProxyUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ProxyUrl |  | 


## `IEmbedUrl`

```csharp
public interface VirtualBrightPlayz.SCP_ET.IEmbedUrl

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Url |  | 


## `IGMenu`

```csharp
public class VirtualBrightPlayz.SCP_ET.IGMenu
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | allHideUI |  | 
| `Image` | ammoBar |  | 
| `Image` | ammoBG1 |  | 
| `Image` | ammoBG2 |  | 
| `Text` | ammoTxt |  | 
| `Image` | blinkBar |  | 
| `GameObject` | blinkOverlay |  | 
| `Text` | blinkTxt |  | 
| `GameObject` | classSelectMenu |  | 
| `Boolean` | closeInteractBar |  | 
| `GameObject` | crossHair |  | 
| `RawImage` | curItem |  | 
| `RawImage` | curWornItem |  | 
| `GameObject` | defaultText |  | 
| `RawImage` | DocViewer |  | 
| `TMP_Text` | endtext |  | 
| `GameObject` | fadeScreen |  | 
| `FadeScreen` | fadeScreenComponent |  | 
| `Single` | fps |  | 
| `Single` | fpsTimer |  | 
| `GameObject` | gameMenu |  | 
| `RawImage` | gasMaskOverlay |  | 
| `Text` | headerText |  | 
| `Text` | healthTxt |  | 
| `Image` | hpBar |  | 
| `Image` | interactBar |  | 
| `RawImage` | interactImage |  | 
| `GameObject` | InvContentUI |  | 
| `GameObject` | InvCurHandItemBorder |  | 
| `GameObject` | InvCurWornItemBorder |  | 
| `GameObject` | InventoryUI |  | 
| `GameObject` | InvScrollOverBorder |  | 
| `Text` | InvScrollOverText |  | 
| `GameObject` | loadingOverlay |  | 
| `GameObject` | menu |  | 
| `GameObject` | MicUI |  | 
| `TMP_Text` | nextroundin |  | 
| `Text` | pingTxt |  | 
| `GameObject` | plyStatsOverlay |  | 
| `Image` | reloadBar |  | 
| `Image` | reloadBG1 |  | 
| `Image` | reloadBG2 |  | 
| `TMP_Text` | roundendtext |  | 
| `GameObject` | roundendui |  | 
| `GameObject` | roundStartButton |  | 
| `GameObject` | roundStartScreen |  | 
| `Canvas` | screenWorldUI |  | 
| `GameObject` | settingsMenu |  | 
| `Image` | sprintBar |  | 
| `Text` | sprintTxt |  | 
| `Text` | status |  | 
| `RawImage` | tc_bg |  | 
| `InputField` | tc_input |  | 
| `Image` | tc_scrollbar |  | 
| `GameObject` | textChat |  | 
| `GameObject` | tmpcamera |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Disconnect() |  | 
| `void` | PlayerStatsShowHide(`Int32` ClassID) |  | 
| `void` | SettingsMenu() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `IGMenu` | singleton |  | 


## `JSONVector`

```csharp
public struct VirtualBrightPlayz.SCP_ET.JSONVector

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | x |  | 
| `Single` | y |  | 
| `Single` | z |  | 


## `JSONVector2`

```csharp
public class VirtualBrightPlayz.SCP_ET.JSONVector2

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | x |  | 
| `Single` | y |  | 


## `JSONVector2Extend`

```csharp
public static class VirtualBrightPlayz.SCP_ET.JSONVector2Extend

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `JSONVector2` | GetJSONVector(this `Vector2` v3) |  | 
| `Vector2` | GetVector2(this `JSONVector2` v3) |  | 


## `JSONVector3Extend`

```csharp
public static class VirtualBrightPlayz.SCP_ET.JSONVector3Extend

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `JSONVector` | GetJSONVector(this `Vector3` v3) |  | 
| `Vector3` | GetVector3(this `JSONVector` v3) |  | 


## `KeybindListing`

```csharp
public class VirtualBrightPlayz.SCP_ET.KeybindListing
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `InputAction` | action |  | 
| `InputActionMap` | actionMap |  | 
| `InputBinding` | binding |  | 
| `InputControl` | control |  | 
| `TextMeshProUGUI` | KeybindKey |  | 
| `TextMeshProUGUI` | KeybindName |  | 
| `Button` | KeybindRe |  | 
| `Button` | KeybindReset |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDestroy() |  | 
| `void` | Rebind() |  | 
| `void` | Reset() |  | 
| `void` | Start() |  | 


## `KeybindManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.KeybindManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | content |  | 
| `GameObject` | defaultPrefab |  | 


## `LCZChkptDoor`

```csharp
public class VirtualBrightPlayz.SCP_ET.LCZChkptDoor
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Door` | d |  | 


## `LightData`

```csharp
public class VirtualBrightPlayz.SCP_ET.LightData

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | LightColor |  | 


## `LoadingScript`

```csharp
public class VirtualBrightPlayz.SCP_ET.LoadingScript
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RawImage` | background |  | 
| `GameObject` | image |  | 
| `Texture[]` | images |  | 
| `GameObject` | innerImage |  | 
| `GameSceneManager` | k |  | 
| `GameObject` | OuterImage |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | tipCount |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | getRandomTip() |  | 


## `MapData`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapData

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<ObjectData>` | Objects |  | 
| `List<RoomData>` | Rooms |  | 


## `MapGenV1Door`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGenV1Door
    : MonoBehaviour, IMapDoor

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | door |  | 
| `String` | zone |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsNotSpawned |  | 
| `GameObject` | Prefab |  | 
| `String` | Zone |  | 


## `MapGenV1Spawn`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGenV1Spawn
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject[]` | roomPrefab |  | 


## `MaterialData`

```csharp
public class VirtualBrightPlayz.SCP_ET.MaterialData

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | MaterialColor |  | 
| `JSONVector2` | Offset |  | 
| `JSONVector2` | Tiling |  | 
| `String` | WebURL |  | 


## `MaterialDownloader`

```csharp
public class VirtualBrightPlayz.SCP_ET.MaterialDownloader
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | acceptedDownloadExternalContent |  | 
| `GameObject` | bar |  | 
| `Image` | barFillImage |  | 
| `Text` | barHeaderText |  | 
| `Text` | barText |  | 
| `GameObject` | confirmPanel |  | 
| `Button` | confirmPanelButton |  | 
| `Text` | confirmPanelText |  | 
| `Boolean` | isDownloading |  | 
| `Queue<MatData>` | matsQueue |  | 
| `Dictionary<String, Material>` | texturesDatabase |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddToQueue(`GameObject` obj, `String` WebURL, `Vector2` tiling, `Vector2` offset) |  | 
| `void` | CloseConfirmPanel() |  | 
| `IEnumerator` | DownloadHandler() |  | 
| `void` | OpenConfirmPanel(`String` confirmText, `UnityAction` act) |  | 
| `IEnumerator` | WaitForDownloadingEnd(`GameObject` obj, `String` url, `Vector2` tiling, `Vector2` offset) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MaterialDownloader` | singleton |  | 


## `MenuImageRandomizer`

```csharp
public class VirtualBrightPlayz.SCP_ET.MenuImageRandomizer
    : MonoBehaviour

```

## `MenuRooms`

```csharp
public class VirtualBrightPlayz.SCP_ET.MenuRooms
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CameraBobEnabled |  | 
| `Single` | CameraBobSpeed |  | 
| `Single` | CameraBobStrength |  | 
| `GameObject[]` | cameras |  | 
| `Single` | CameraSwitchTime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SwitchCamera() |  | 


## `ModPackage`

```csharp
public class VirtualBrightPlayz.SCP_ET.ModPackage
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<AssetBundle>` | assetBundles |  | 
| `List<GameObject>` | clusters |  | 
| `List<GameObject>` | doors |  | 
| `List<String>` | extraModDirs |  | 
| `List<String>` | hashes |  | 
| `Dictionary<String, String>` | linkedHashes |  | 
| `Dictionary<String, ModInfo>` | mods |  | 
| `List<GameObject>` | rooms |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `ModInfo` | GetModInfoFromHash(`String` hash) |  | 
| `UniTask` | LoadModDir(`String` package) |  | 
| `UniTask` | LoadMods() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ModPackage` | instance |  | 


## `NetManCache`

```csharp
public class VirtualBrightPlayz.SCP_ET.NetManCache
    : MonoBehaviour

```

Static Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `NetManCache` | Cache |  | 
| `NetworkManager` | Manager |  | 


## `ObjectData`

```csharp
public class VirtualBrightPlayz.SCP_ET.ObjectData

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | Data |  | 
| `String` | ObjectID |  | 
| `JSONVector` | Position |  | 
| `JSONVector` | Rotation |  | 
| `JSONVector` | Scale |  | 


## `ObjectsDB`

```csharp
public class VirtualBrightPlayz.SCP_ET.ObjectsDB
    : MonoBehaviour, IObjectDatabase

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, GameObject>` | ObjectDB |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IDictionary<String, Object>` | Database |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | GetId(`Object` obj) |  | 
| `void` | RegisterNetwork() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ObjectsDB` | db |  | 


## `PlayerRT`

```csharp
public class VirtualBrightPlayz.SCP_ET.PlayerRT
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Camera` | cam |  | 
| `RawImage` | image |  | 
| `RenderTexture` | targetTexture |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | Scale |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | RedrawTex() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerRT` | rT |  | 


## `PluginLoader`

```csharp
public class VirtualBrightPlayz.SCP_ET.PluginLoader
    : MonoBehaviour, IGameGlobals

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PluginSystem` | pluginSystem |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Reload() |  | 
| `void` | SendAdminCommand(`String` command, `IPlayer` player) |  | 
| `void` | SendChatCommand(`String` command, `IPlayer` player) |  | 
| `void` | SendGlobalChatMessage(`String` message) |  | 
| `void` | SpawnNpc(`String` id, `Vector3` position) |  | 


## `PluginLogger`

```csharp
public class VirtualBrightPlayz.SCP_ET.PluginLogger
    : Logger

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Debug(`String` tag, `String` message) |  | 
| `void` | Error(`String` tag, `String` message) |  | 
| `void` | Info(`String` tag, `String` message) |  | 
| `void` | Warn(`String` tag, `String` message) |  | 


## `QuitGameButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.QuitGameButton
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | QuitGame() |  | 


## `RoomData`

```csharp
public class VirtualBrightPlayz.SCP_ET.RoomData

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `JSONVector` | Position |  | 
| `String` | RoomName |  | 
| `JSONVector` | Rotation |  | 
| `JSONVector` | Scale |  | 


## `RoundEnd`

```csharp
public class VirtualBrightPlayz.SCP_ET.RoundEnd
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | introScene |  | 
| `Boolean` | roundEnded |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `IEnumerator` | Counter(`String` endMessage, `Single` time) |  | 
| `void` | EndRound(`String` endMessage, `Single` timeToEnd) |  | 
| `void` | ResetMap() |  | 
| `void` | RpcHideEndScreen() |  | 
| `void` | RpcShowEndScreen(`String` endMessage, `Single` timeToEnd) |  | 
| `void` | Update() |  | 
| `void` | UserCode_RpcHideEndScreen() |  | 
| `void` | UserCode_RpcShowEndScreen(`String` endMessage, `Single` timeToEnd) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcHideEndScreen(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcShowEndScreen(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `RoundStart`

```csharp
public class VirtualBrightPlayz.SCP_ET.RoundStart
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isRoundstarted |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | NetworkisRoundstarted |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | OnHostRoundStart() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `IEnumerator` | StartRoundLate() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | EscapeText |  | 


## `SCP1123_Door`

```csharp
public class VirtualBrightPlayz.SCP_ET.SCP1123_Door
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | closeAng |  | 
| `GameObject` | door |  | 
| `Boolean` | IsMoving |  | 
| `Single` | maxTimeOpen |  | 
| `Boolean` | open |  | 
| `Vector3` | openAng |  | 
| `AudioClip` | openSound |  | 
| `Single` | speed |  | 
| `AudioClip` | timeWarnClip |  | 
| `Boolean` | useTimeOpen |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsOpen |  | 
| `Boolean` | Networkopen |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdClose() |  | 
| `void` | CmdOpen() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | RpcOnOpenClose(`Boolean` isopen) |  | 
| `void` | RpcOpenSound() |  | 
| `void` | RpcWarnSound() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | UserCode_RpcOnOpenClose(`Boolean` isopen) |  | 
| `void` | UserCode_RpcOpenSound() |  | 
| `void` | UserCode_RpcWarnSound() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcOnOpenClose(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcOpenSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcWarnSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `ServerListingModel`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerListingModel

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Address |  | 
| `Boolean` | IsDedicated |  | 
| `Boolean` | IsVerified |  | 
| `String` | LastUpdated |  | 
| `String` | MapName |  | 
| `Int32` | MaxPlayers |  | 
| `String` | Name |  | 
| `Boolean` | Official |  | 
| `String` | PastebinId |  | 
| `Int32` | PlayerCount |  | 
| `String` | Version |  | 


## `ServerListModel`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerListModel

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Address |  | 
| `Boolean` | IsDedicated |  | 
| `String` | MapName |  | 
| `Int32` | MaxPlayers |  | 
| `String` | Name |  | 
| `String` | PastebinId |  | 
| `Int32` | PlayerCount |  | 
| `String` | UniqueToken |  | 
| `List<UInt64>` | Users |  | 
| `String` | Version |  | 


## `TextChat`

```csharp
public class VirtualBrightPlayz.SCP_ET.TextChat
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RawImage` | bg |  | 
| `String` | chatChannel |  | 
| `PlayerController` | controller |  | 
| `GameObject` | defaultText |  | 
| `InputField` | input |  | 
| `Boolean` | isTextChatOpened |  | 
| `String` | lastMessage |  | 
| `Int32` | maxMessages |  | 
| `List<GameObject>` | objects |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | NetworkchatChannel |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddMessage(`String` Message) |  | 
| `void` | CmdSendMessage(`String` Message) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `String` | GetChatColor(`PlayerController` ctrl) |  | 
| `void` | RpcAddMessage(`String` Message, `String` Color) |  | 
| `void` | RpcAddTranslatedMessage(`String` Message, `String` Color, `Int32` TextType) |  | 
| `void` | RpcAddTranslatedMessageWithArgs(`String` Message, `String` Color, `Int32` TextType, `String` ArgString) |  | 
| `void` | SendTextMessage(`String` str) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | TargetRpcAddMessage(`INetworkConnection` connection, `String` Message, `String` Color) |  | 
| `void` | TargetRpcAddTranslatedMessage(`INetworkConnection` connection, `String` Message, `String` Color, `Int32` TextType) |  | 
| `void` | TargetRpcAddTranslatedMessageWithArgs(`INetworkConnection` connection, `String` Message, `String` Color, `Int32` TextType, `String` ArgString) |  | 
| `void` | UserCode_CmdSendMessage(`String` Message) |  | 
| `void` | UserCode_RpcAddMessage(`String` Message, `String` Color) |  | 
| `void` | UserCode_RpcAddTranslatedMessage(`String` Message, `String` Color, `Int32` TextType) |  | 
| `void` | UserCode_RpcAddTranslatedMessageWithArgs(`String` Message, `String` Color, `Int32` TextType, `String` ArgString) |  | 
| `void` | UserCode_TargetRpcAddMessage(`INetworkConnection` connection, `String` Message, `String` Color) |  | 
| `void` | UserCode_TargetRpcAddTranslatedMessage(`INetworkConnection` connection, `String` Message, `String` Color, `Int32` TextType) |  | 
| `void` | UserCode_TargetRpcAddTranslatedMessageWithArgs(`INetworkConnection` connection, `String` Message, `String` Color, `Int32` TextType, `String` ArgString) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, IChatCommand>` | commands |  | 
| `String` | defaultColor |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdSendMessage(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcAddMessage(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcAddTranslatedMessage(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcAddTranslatedMessageWithArgs(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcAddMessage(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcAddTranslatedMessage(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcAddTranslatedMessageWithArgs(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `TextData`

```csharp
public class VirtualBrightPlayz.SCP_ET.TextData

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Message |  | 


## `VideoPlayerData`

```csharp
public class VirtualBrightPlayz.SCP_ET.VideoPlayerData

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `JSONVector` | ScreenPosition |  | 
| `JSONVector` | ScreenRotation |  | 
| `JSONVector` | ScreenScale |  | 


## `Webhook`

```csharp
public class VirtualBrightPlayz.SCP_ET.Webhook

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | AvatarUrl |  | 
| `String` | Content |  | 
| `List<Embed>` | Embeds |  | 
| `Boolean` | IsTTS |  | 
| `String` | Username |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Task<HttpResponseMessage>` | Send(`String` content, `String` username = null, `String` avatarUrl = null, `Boolean` isTTS = False, `IEnumerable<Embed>` embeds = null) |  | 


