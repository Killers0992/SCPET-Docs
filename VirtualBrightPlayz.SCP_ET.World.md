## `AssetModelLoader`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.AssetModelLoader
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | localObj |  | 
| `String` | path |  | 


## `ButtonErrorType`

```csharp
public enum VirtualBrightPlayz.SCP_ET.World.ButtonErrorType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | NoSound |  | 
| `1` | Click |  | 
| `2` | ErrClick |  | 
| `3` | KeyClick |  | 
| `4` | ErrKeyClick |  | 
| `5` | ErrOfficeDoor |  | 
| `6` | ItemPickup0 |  | 


## `ButtonLCZCtrl`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.ButtonLCZCtrl
    : NetworkBehaviour, ILever, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | box |  | 
| `AudioClip` | clip |  | 
| `Single` | curRotZ |  | 
| `Boolean` | gizmo |  | 
| `LayerMask` | ItemMask |  | 
| `Transform` | leverHandle |  | 
| `String` | missionName |  | 
| `Single` | newRotZ |  | 
| `Outline` | outline |  | 
| `AudioSource` | source |  | 
| `Single` | syncTimer |  | 
| `Single` | turnMulti |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Single` | NetworkcurRotZ |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Highlighted() |  | 
| `void` | OnLeverTurn(`LCZCtrlLeverMessage` message, `INetworkConnection` sender = null) |  | 
| `void` | RpcSwitchSound() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `Boolean` | UpdateLook(`PlayerController` user, `Vector2` look) |  | 
| `void` | UserCode_OnLeverTurn(`LCZCtrlLeverMessage` message, `INetworkConnection` sender) |  | 
| `void` | UserCode_RpcSwitchSound() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_OnLeverTurn(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSwitchSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `CameraFix`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.CameraFix
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | dist |  | 
| `Boolean` | shouldRender |  | 


## `CustomModelLoader`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.CustomModelLoader
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | filename |  | 
| `GameObject` | localObj |  | 
| `String` | path |  | 


## `DoorEvent`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.DoorEvent
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | type |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DoorOpen() |  | 
| `void` | Start() |  | 


## `EmitGas`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.EmitGas
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | damage |  | 
| `Single` | eyeDamage |  | 


## `EventButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.EventButton
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Highlighted() |  | 
| `void` | Start() |  | 
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `void` | TriggerEvent(`PlayerController` plr, `Boolean` isLocal) |  | 
| `void` | Update() |  | 


## `FanController`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.FanController
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | axis |  | 
| `Transform` | fan |  | 
| `ParticleSystemForceField` | field |  | 
| `Single` | maxSpeed |  | 
| `Single` | maxTimer |  | 
| `Single` | minTimer |  | 
| `AudioSource` | newaudio |  | 
| `AudioClip` | runningClip |  | 
| `Single` | speed |  | 
| `Boolean` | spinning |  | 
| `AudioClip` | windDownClip |  | 
| `AudioClip` | windUpClip |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Networkspinning |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | WindDown() |  | 
| `void` | WindUp() |  | 


## `FlickeringLight`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.FlickeringLight
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | alwaysOn |  | 
| `AudioClip[]` | flickerSounds |  | 
| `Single` | maxTimeout |  | 
| `Single` | minTimeout |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | EndFlicker() |  | 
| `void` | Flicker() |  | 


## `HeightmapMesh`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.HeightmapMesh
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | addNewVerts |  | 
| `AnimationCurve` | curve2 |  | 
| `FractalType` | fractalType |  | 
| `Single` | frequency |  | 
| `Single` | frequency2 |  | 
| `Boolean` | genTexture |  | 
| `Int32` | iterations |  | 
| `MeshRenderer` | meshRenderer |  | 
| `Single` | meshScale |  | 
| `FastNoiseLite` | noise |  | 
| `FastNoiseLite` | noise2 |  | 
| `NoiseType` | noiseType |  | 
| `Vector2` | offset |  | 
| `Single` | offsetScale |  | 
| `Single` | scale |  | 
| `Single` | scale2 |  | 
| `Int32` | seed |  | 
| `Vector2Int` | size |  | 
| `Vector2Int` | texSize |  | 
| `Texture2D` | texture |  | 
| `Vector2` | uvSize |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ResetupMesh() |  | 
| `void` | SetupMesh() |  | 
| `void` | Start() |  | 


## `IDimension`

```csharp
public interface VirtualBrightPlayz.SCP_ET.World.IDimension

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | DimId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ExitDim(`PlayerController` player) |  | 
| `void` | TeleportPlayer(`PlayerController` player) |  | 


## `InteractableButton`

```csharp
public abstract class VirtualBrightPlayz.SCP_ET.World.InteractableButton
    : NetworkBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GizmoDraw() |  | 
| `Boolean` | Use(`GameObject` plr, `String&` status, `ButtonErrorType&` errorType) |  | 


## `KillTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.KillTrigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `DeathTypes` | deathType |  | 
| `AudioClip` | killSound |  | 
| `AudioSource` | source |  | 


## `LCZMissionControl`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.LCZMissionControl
    : NetworkBehaviour, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | checkpointsUnlocked |  | 
| `String` | lockdownText |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Guid |  | 
| `Boolean` | NetworkcheckpointsUnlocked |  | 
| `String` | PrefabGuid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | FixedUpdate() |  | 
| `void` | LoadComplete() |  | 
| `IEnumerator` | RegisterMonitors() |  | 
| `void` | RpcUpdateLockdownState(`String` text, `Boolean` sound) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | UserCode_RpcUpdateLockdownState(`String` text, `Boolean` sound) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LCZMissionControl` | control |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcUpdateLockdownState(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `MapDB`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.MapDB
    : MonoBehaviour, IObjectDatabase

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, GameObject>` | Prefabs |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IDictionary<String, Object>` | Database |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | GetId(`Object` obj) |  | 
| `IEnumerator` | LoadRooms() |  | 
| `void` | RegisterNetwork() |  | 
| `GameObject` | Spawn(`Vector3` pos, `Guid` guid) |  | 
| `void` | UnSpawn(`GameObject` spawned) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MapDB` | db |  | 


## `MapGenV2`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.MapGenV2
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MapGenV2Room[]` | genericRooms |  | 
| `Cell[,]` | map |  | 
| `MapGenV2Room[]` | requiredRooms |  | 
| `Random` | rng |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GenMap(`Int32` seed, `Int32` xsize, `Int32` zsize, `Int32` spacing, `Int32` roomspacing) |  | 


## `MapGenV2Room`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.MapGenV2Room
    : MonoBehaviour, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanReplace |  | 
| `BoxCollider` | dimensions |  | 
| `Boolean` | ISCheckpoint |  | 
| `Boolean` | IsRequired |  | 
| `Boolean` | IsSublevelChange |  | 
| `Int32` | Layer |  | 
| `Int32` | maxTimesToBeSpawned |  | 
| `Boolean` | Network |  | 
| `Single` | RLCmultiply |  | 
| `GameObject` | roomLighting |  | 
| `String` | RoomName |  | 
| `CellType` | RoomType |  | 
| `Boolean` | SpawnRLC |  | 
| `Boolean` | StatusChange |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Guid |  | 
| `String` | PrefabGuid |  | 
| `String` | roomid |  | 
| `JSONVector` | savePos |  | 
| `JSONVector` | saveRot |  | 
| `JSONVector` | saveScl |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | LoadComplete() |  | 


## `MapInit2`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.MapInit2
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | mapgen2 |  | 


## `MonitorCamera2`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.MonitorCamera2
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Camera` | cam |  | 
| `MeshRenderer` | render |  | 
| `RenderTexture` | tex |  | 


## `NaziController`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.NaziController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Animator` | anim |  | 
| `GameObject` | BigRoomPos |  | 
| `AudioClip` | FinalSpeech |  | 
| `AudioClip` | GetOut_1 |  | 
| `AudioClip` | GetOut_2 |  | 
| `AudioSource` | NaziAudioSource |  | 
| `GameObject` | OutsideCellPos |  | 
| `GameObject` | SmallRoomPos |  | 


## `NetworkRoomLight`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.NetworkRoomLight
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | lightsOn |  | 
| `RoomLightController` | rlc |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | NetworklightsOn |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | DisableLights(`Boolean` old, `Boolean` cur) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 


## `NetworkSpawnDocument`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.NetworkSpawnDocument
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Document |  | 
| `GameObject` | prefab |  | 


## `NetworkSpawnDoor`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.NetworkSpawnDoor
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3[]` | ButtonPosOffset |  | 
| `GameObject` | buttonPrefab |  | 
| `Vector3[]` | ButtonRotOffset |  | 
| `Boolean` | defaultLock |  | 
| `String` | doorName |  | 
| `Int32` | eventId |  | 
| `Boolean` | hasEvent |  | 
| `Boolean` | lczChkpt |  | 
| `GameObject` | prefab |  | 
| `String[]` | ReqAccess |  | 
| `Int32` | ReqLevel |  | 
| `Boolean` | RequireKeyCard |  | 
| `Boolean` | RequireKeyCardId |  | 


## `NetworkSpawnMe`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.NetworkSpawnMe
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | Chance |  | 
| `GameObject` | prefab |  | 


## `PlayerView_1123`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.PlayerView_1123
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Camera` | cam |  | 
| `CharacterController` | ctrl |  | 
| `Boolean` | Enabled |  | 
| `Boolean` | isMoving |  | 
| `GameObject` | rotation |  | 
| `SCP_1123` | scp |  | 
| `Single` | speed |  | 
| `Single` | walkSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetEnable(`Boolean` enable) |  | 


## `PropDoor`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.PropDoor
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioSource` | audioSrc |  | 
| `GameObject` | close |  | 
| `AudioClip[]` | closeClip |  | 
| `Boolean` | isOpen |  | 
| `GameObject` | open |  | 
| `AudioClip[]` | openClip |  | 
| `Single` | progress |  | 
| `Single` | speed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Close() |  | 
| `void` | Open() |  | 


## `RLCSpawner`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.RLCSpawner
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | dimensions |  | 
| `GameObject` | roomLighting |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Start() |  | 


## `RoomNav`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.RoomNav
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3[]` | data |  | 
| `Dictionary<Vector3, Int32>` | values |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | GetClosestPoint(`Vector3` pos, `Single` dist) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RoomNav` | nav |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | GetClosestPoint(`Vector3[]` arr, `Vector3` pos, `Single` dist) |  | 
| `Vector3` | GetClosestPoint(`Vector3[]` arr, `Vector3` pos, `Single` dist, `Vector3` exclude, `Single` excludeDist) |  | 


## `RoomNavData`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.RoomNavData
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3[]` | data |  | 
| `Single` | globalGridSize |  | 
| `LayerMask` | mask |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GenMap() |  | 


## `RoomPhysicsCull`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.RoomPhysicsCull
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | radius |  | 


## `SCP_1123`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_1123
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `FSMManager` | ai2 |  | 
| `SCP1123_Door` | bigRoomDoor |  | 
| `SCP1123_Door` | cellDoor |  | 
| `Single` | complienceTimer |  | 
| `SCP1123_Entity` | ent |  | 
| `AudioClip` | GunshotSound |  | 
| `AudioClip` | HorrorSound |  | 
| `SCP1123_Door` | lilRoomDoor |  | 
| `GameObject` | Nazi |  | 
| `NaziController` | naziManager |  | 
| `Single` | oldWalkSpeed |  | 
| `Boolean` | outsideCellTrigger |  | 
| `Boolean` | outsideTop1123Room |  | 
| `PlayerController` | player |  | 
| `PlayerView_1123` | playerView |  | 
| `GameObject` | PlyObject |  | 
| `Single` | sayGetOutTimer |  | 
| `Boolean` | smoothTp |  | 
| `Single` | smoothTpTimer |  | 
| `Int32` | stage |  | 
| `Door` | topContainmentDoor |  | 
| `AudioClip` | TouchSound |  | 
| `GameObject` | tpBigRoomPos |  | 
| `GameObject` | tpBottomHallPos |  | 
| `GameObject` | tpCellPos |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdDoorForce(`Int32` id) |  | 
| `void` | RpcPlaySound(`Int32` id) |  | 
| `void` | RpcSetStage(`Int32` stg) |  | 
| `void` | TpToCell(`Boolean` force = False) |  | 
| `void` | UserCode_RpcPlaySound(`Int32` id) |  | 
| `void` | UserCode_RpcSetStage(`Int32` stg) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPlaySound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSetStage(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP_1123_fake`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_1123_fake
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 
| `SCP_1123` | scp |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Highlighted() |  | 
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `SCP_1123_real`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_1123_real
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 
| `SCP_1123` | scp |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Highlighted() |  | 
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `SCP_1123_Trigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_1123_Trigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SCP_1123` | scp |  | 


## `SCP1123_DoorButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP1123_DoorButton
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `SCP1123_Door` | door |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | locked |  | 
| `Boolean` | open |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Highlighted() |  | 
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `SCP1123_DoorSpawn`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP1123_DoorSpawn
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | prefab |  | 
| `SCP_1123` | scp |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | ShouldDestroyOnLoad() |  | 
| `IEnumerator` | Start() |  | 


## `SCP1123_Entity`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP1123_Entity
    : MonoBehaviour, IEntity, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `FSMManager` | ai2 |  | 
| `String` | ai2State |  | 
| `PlayerController` | player |  | 
| `Quaternion` | plyOGAng |  | 
| `Single` | plyOGHeadRotation |  | 
| `Vector3` | plyOGPos |  | 
| `SCP_1123` | scp |  | 
| `Int32` | stage |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `DimensionType` | CurrentDimension |  | 
| `String` | Guid |  | 
| `String` | PrefabGuid |  | 
| `JSONVector` | savePos |  | 
| `JSONVector` | saveRot |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | LoadComplete() |  | 
| `IEnumerator` | LoadLate(`String` state) |  | 


## `SCP1123Fake`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP1123Fake
    : FSMState

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP1123Flashback`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP1123Flashback
    : FSMState

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP1123Idle`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP1123Idle
    : FSMState

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP1123Intro`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP1123Intro
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | complyTime |  | 
| `Single` | doorOpenTime |  | 
| `String` | noneStateName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP914`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP914
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioSource` | audioSrc |  | 
| `Scp914Setting` | curMode |  | 
| `Scp914Setting` | curModeTo |  | 
| `PropDoor[]` | Doors |  | 
| `SCP914Gear[]` | gears |  | 
| `BoxCollider` | input |  | 
| `Boolean` | isModeSelectTurning |  | 
| `Boolean` | isRefining |  | 
| `SCP914Key` | key |  | 
| `SCP914Knob` | knob |  | 
| `Single` | maxRefineTimer |  | 
| `Single[]` | ModeAngles |  | 
| `GameObject` | ModeSelect |  | 
| `Single` | ModeSelectSpeed |  | 
| `BoxCollider` | output |  | 
| `List<SCP914Recipe>` | RecipeOverrides |  | 
| `SCP914RecipeObject[]` | Recipes |  | 
| `List<SCP914Recipe>` | RecipeTypes |  | 
| `AudioClip` | refineAudio |  | 
| `Double` | refineTime |  | 
| `Single` | refineTimer |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Scp914Setting` | NetworkcurMode |  | 
| `Scp914Setting` | NetworkcurModeTo |  | 
| `Boolean` | NetworkisRefining |  | 
| `Double` | NetworkrefineTime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `SCP914Recipe[]` | GetItemOverrides(`WorldItemBase` worldItem, `Scp914Setting` setting) |  | 
| `SCP914Recipe[]` | GetItemRecipes(`WorldItemBase` worldItem, `Scp914Setting` setting) |  | 
| `void` | Refine() |  | 
| `void` | RefineChange(`Boolean` old, `Boolean` refine) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | GetTypeFromStr(`String` str) |  | 


## `SCP914Gear`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP914Gear
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AnimationCurve` | curve |  | 
| `Single` | speed |  | 


## `SCP914Key`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP914Key
    : NetworkBehaviour, ILever, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | box |  | 
| `Single` | curRotZ |  | 
| `Boolean` | gizmo |  | 
| `Single` | newRotZ |  | 
| `Outline` | outline |  | 
| `SCP914` | scp |  | 
| `Single` | syncTimer |  | 
| `Single` | turnMulti |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Single` | NetworkcurRotZ |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Highlighted() |  | 
| `void` | OnKeyTurn(`SCP914KeyMessage` message, `INetworkConnection` sender = null) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `Boolean` | UpdateLook(`PlayerController` user, `Vector2` look) |  | 
| `void` | UserCode_OnKeyTurn(`SCP914KeyMessage` message, `INetworkConnection` sender) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_OnKeyTurn(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP914Knob`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP914Knob
    : NetworkBehaviour, ILever, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Single` | curRotZ |  | 
| `Boolean` | gizmo |  | 
| `Scp914Setting` | newMode |  | 
| `Single` | newRotZ |  | 
| `Outline` | outline |  | 
| `SCP914` | scp |  | 
| `Single` | turnMulti |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Single` | NetworkcurRotZ |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Highlighted() |  | 
| `void` | OnKnobTurn(`SCP914KnobMessage` message, `INetworkConnection` sender = null) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `Boolean` | UpdateLook(`PlayerController` user, `Vector2` look) |  | 
| `void` | UserCode_OnKnobTurn(`SCP914KnobMessage` message, `INetworkConnection` sender) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_OnKnobTurn(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP914RecipeObject`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP914RecipeObject
    : ScriptableObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Enabled |  | 
| `String` | InputItem |  | 
| `String` | OutputItem |  | 
| `Scp914Setting` | Setting |  | 


## `Scp914Setting`

```csharp
public enum VirtualBrightPlayz.SCP_ET.World.Scp914Setting
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Rough |  | 
| `1` | Coarse |  | 
| `2` | OneToOne |  | 
| `3` | Fine |  | 
| `4` | VeryFine |  | 


## `SettingsLight`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SettingsLight
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | followSettings |  | 
| `Light` | myLight |  | 
| `Boolean` | spawnWorldLight |  | 
| `Single` | timer |  | 


## `SpectateCam`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SpectateCam
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | expandAmount |  | 
| `Boolean` | isUsing |  | 
| `Single` | maxViewDist |  | 
| `Single` | radius |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsVisible(`Collider` other) |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | MaxColliders |  | 


## `TeslaGate`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.TeslaGate
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | active |  | 
| `ParticleSystem` | activeParticle |  | 
| `AudioClip` | chargeSound |  | 
| `Single` | chargeTimer |  | 
| `Single` | cooldownTimer |  | 
| `ParticleSystem` | idleParticle |  | 
| `ParticleSystem` | idleParticleTwo |  | 
| `AudioClip` | idleSound |  | 
| `Boolean` | isCharging |  | 
| `Boolean` | isShocking |  | 
| `MonitorController[]` | monitors |  | 
| `AudioClip` | shockSound |  | 
| `AudioSource` | source |  | 
| `TeslaGateCollider` | teslaCollider |  | 
| `String` | textActive |  | 
| `String` | textInactive |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Charge(`Single` time = 0,7) |  | 
| `void` | PlayIdleSound() |  | 
| `void` | RpcPlayChargeSound() |  | 
| `void` | RpcPlayShockSound() |  | 
| `void` | UserCode_RpcPlayChargeSound() |  | 
| `void` | UserCode_RpcPlayShockSound() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPlayChargeSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayShockSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `TeslaGateCollider`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.TeslaGateCollider
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `TeslaGate` | parent |  | 


## `TeslaShock`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.TeslaShock
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `TeslaGate` | parent |  | 


## `TVSpawn`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.TVSpawn
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | tv |  | 


## `WorldAmbientTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.WorldAmbientTrigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | boxcollider |  | 
| `AudioClip` | clip |  | 
| `Color` | color |  | 
| `Single` | farClip |  | 
| `Boolean` | fog |  | 
| `Boolean` | isExiting |  | 
| `Material` | sky |  | 
| `Transform` | sun |  | 
| `Color` | sunColor |  | 
| `Boolean` | sunLocal |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Start() |  | 
| `void` | Update() |  | 


## `WorldLight`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.WorldLight
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `FlickeringLight` | _flicker |  | 
| `Light` | _light |  | 
| `Camera` | active |  | 
| `MeshRenderer` | quad |  | 


## `WorldParticleSystem`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.WorldParticleSystem
    : MonoBehaviour

```

