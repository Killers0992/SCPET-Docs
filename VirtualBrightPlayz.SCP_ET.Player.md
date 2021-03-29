## `AmbientControl`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.AmbientControl
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AmbientType` | ambient |  | 
| `AudioClip` | ambientGeneric |  | 
| `AudioClip` | ambientGenericEZ |  | 
| `AudioClip` | ambientGenericHCZ |  | 
| `Color` | defaultColor |  | 
| `Boolean` | found |  | 
| `Boolean` | isSource1 |  | 
| `Boolean` | isTemp |  | 
| `AudioSource` | scpSource |  | 
| `AudioSource` | source |  | 
| `AudioSource` | source2 |  | 
| `Single` | speed |  | 
| `Light` | sun |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ChangeTo(`AudioClip` clip) |  | 
| `void` | ScpChangeTo(`AudioClip` clip) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | GetClipTitle(`String` clipName) |  | 


## `AmbientTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.AmbientTrigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AmbientType` | ambient |  | 
| `AudioClip` | clip |  | 


## `AnimationControl`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.AnimationControl
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animSpeed |  | 
| `PlayerController` | ctrl |  | 
| `Boolean` | isDucking |  | 
| `Single` | lerpSpeed |  | 
| `Single` | movement |  | 
| `Single` | sprint |  | 
| `GameObject` | viewmodel |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | NetworkanimSpeed |  | 
| `Boolean` | NetworkisDucking |  | 
| `Single` | Networkmovement |  | 
| `Single` | Networksprint |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdUpdateDucking(`Boolean` duck) |  | 
| `void` | CmdUpdateMove(`Single` move) |  | 
| `void` | CmdUpdateSpeed(`Single` move) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | SetFaceWorldModel(`GameObject` model) |  | 
| `void` | SetHandWorldModel(`GameObject` model) |  | 
| `void` | UserCode_CmdUpdateDucking(`Boolean` duck) |  | 
| `void` | UserCode_CmdUpdateMove(`Single` move) |  | 
| `void` | UserCode_CmdUpdateSpeed(`Single` move) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdUpdateDucking(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdUpdateMove(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdUpdateSpeed(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `CameraFovController`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.CameraFovController
    : MonoBehaviour

```

## `ClassManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.ClassManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<Int32, Class>` | classes |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ClassManager` | singleton |  | 


## `DeadBodyFall`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.DeadBodyFall
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Animator` | anim |  | 
| `GameObject` | body |  | 
| `Single` | bodyDecayTime |  | 
| `GameObject` | bodyMesh |  | 
| `String` | playerTextureIndex |  | 
| `Boolean` | shouldDecay |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | NetworkplayerTextureIndex |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 


## `DisconnectMessage`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.DisconnectMessage

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | code |  | 
| `String` | message |  | 
| `Boolean` | translated |  | 
| `Int32` | translationType |  | 


## `InteractController`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.InteractController
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerController` | controller |  | 
| `IInteractable` | prevInteractable |  | 
| `Boolean` | wasInteractingLastFrame |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckInteract(`Vector2` look, `Boolean` state) |  | 
| `IInteractable` | GetValidInteract() |  | 
| `void` | ShowStatus(`TextType` type, `String` status, `Boolean` isLocal) |  | 
| `void` | Start() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdInteract(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `MissionInfo`

```csharp
public struct VirtualBrightPlayz.SCP_ET.Player.MissionInfo

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Complete |  | 
| `String` | Description |  | 
| `Int32` | Favor |  | 
| `Int32` | FavorRequired |  | 
| `Boolean` | GlobalTask |  | 
| `String` | IDofCompleter |  | 
| `String` | InitialGivenToID |  | 
| `String` | MissionGiver |  | 
| `String` | MissionName |  | 
| `Boolean` | PlayerCanStealReward |  | 
| `Boolean` | Started |  | 


## `MouseCursorController`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.MouseCursorController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | canLook |  | 
| `PlayerController` | ctrl |  | 
| `DebugLogManager` | dbgmgr |  | 
| `Boolean` | hideUI |  | 
| `Boolean` | InVR |  | 
| `Boolean` | roundStarted |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MouseCursorController` | cursorController |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsOverUI() |  | 
| `Boolean` | IsTextInput() |  | 


## `PlayerController`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.PlayerController
    : NetworkBehaviour, IHuman, ICanTakeDamage, IEntity, ICanTriggerTesla

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | _godMode |  | 
| `GameObject` | _rot |  | 
| `AchievementController` | achievementController |  | 
| `AdminMenu` | adminmenuScript |  | 
| `Single` | airTime |  | 
| `Single` | aliveTime |  | 
| `AudioClip[]` | allowSounds |  | 
| `GameObject` | ambient |  | 
| `AmbientControl` | ambientControl |  | 
| `AnimationControl` | animctrl |  | 
| `Quaternion` | BaseRotation |  | 
| `AudioClip[]` | bleedingSounds |  | 
| `AudioSource` | bleedSoundSource |  | 
| `Camera` | cam |  | 
| `Boolean` | camLock |  | 
| `Class` | classPlayer |  | 
| `Double` | clientoldnettime |  | 
| `Single` | commonFov |  | 
| `Vector3` | commonPos |  | 
| `Single` | crouchSpeed |  | 
| `CharacterController` | ctrl |  | 
| `Int32` | CurrentInvItem |  | 
| `AudioClip[]` | denySounds |  | 
| `Vector3` | duckPos |  | 
| `PlayerHealthEffectsController` | effectsHP |  | 
| `AudioClip` | fallDamageSound |  | 
| `AudioSource` | footstepSource |  | 
| `AudioSource` | genericSource |  | 
| `List<GlobalGroupData>` | globalGroups |  | 
| `AudioClip[]` | grassFootSounds |  | 
| `Single` | gravity |  | 
| `Single` | groundDistance |  | 
| `LayerMask` | groundMask |  | 
| `AudioSource` | gunSoundSource |  | 
| `Single` | HeadRotation |  | 
| `PlayerHealthController` | healthController |  | 
| `Single` | heightMod |  | 
| `Boolean` | infAmmo |  | 
| `Boolean` | inputAllowed |  | 
| `GameObject` | InvContentUI |  | 
| `GameObject` | InventoryUI |  | 
| `GameObject` | InvItemIconPrefab |  | 
| `Boolean` | InvOpen |  | 
| `Boolean` | invr |  | 
| `Boolean` | isDucking |  | 
| `Boolean` | isFly |  | 
| `Boolean` | isMoving |  | 
| `Boolean` | isReloading |  | 
| `Boolean` | isSprinting |  | 
| `LayerMask` | itemMask |  | 
| `Single` | jumpHeight |  | 
| `Vector3` | leftHand |  | 
| `Boolean` | lockBlink |  | 
| `Single` | loneTime |  | 
| `Single` | lowFallHeight |  | 
| `Int32` | MaxInvItems |  | 
| `GameObject` | medkitPrefab |  | 
| `Boolean` | menu |  | 
| `AudioClip[]` | metalFootSounds |  | 
| `AudioClip[]` | metalFootSoundsSprint |  | 
| `AudioClip[]` | metalGrateFootSounds |  | 
| `AudioClip[]` | metalGrateFootSoundsSprint |  | 
| `Single` | mouseSenseX |  | 
| `Single` | mouseSenseY |  | 
| `Single` | moveAnimTimer |  | 
| `PlayerMovementController` | movementController |  | 
| `Single` | movementFootstepTimer |  | 
| `Camera` | navCam |  | 
| `GameObject` | navigatorMesh |  | 
| `Vector3` | newPosCache |  | 
| `Quaternion` | newRotCache |  | 
| `Single` | noclipExcludeTimer |  | 
| `Boolean` | noSee |  | 
| `Boolean` | noTarget |  | 
| `Single` | peakFallHeight |  | 
| `AudioClip[]` | pickupSounds |  | 
| `String` | playerGroup |  | 
| `String` | playerGroupColor |  | 
| `Boolean` | playerGroupIsDefault |  | 
| `Int32` | playerId |  | 
| `PlayerList` | playerlistScript |  | 
| `String` | playerName |  | 
| `String` | playerRole |  | 
| `GameObject` | playersList |  | 
| `PlayerMissionManager` | pms |  | 
| `Vector3` | Position |  | 
| `AudioClip` | pullOutGunSound |  | 
| `Single` | radiusMod |  | 
| `Boolean` | readyToPlay |  | 
| `AudioClip` | reloadEndSound |  | 
| `AudioClip` | reloadMidSound |  | 
| `AudioClip` | reloadStartSound |  | 
| `Single` | reloadTimer |  | 
| `Vector3` | rightHand |  | 
| `Single` | scareFov |  | 
| `AudioClip[]` | scp1499Sounds |  | 
| `Boolean` | serverIsVr |  | 
| `Double` | serveroldnettime |  | 
| `Single` | shootCooldown |  | 
| `Camera` | speccam |  | 
| `Single` | speed |  | 
| `Single` | sprintFov |  | 
| `Single` | sprintSpeed |  | 
| `PlayerStats` | stats |  | 
| `UInt64` | steamId |  | 
| `Boolean` | step |  | 
| `AudioClip[]` | stoneFootSounds |  | 
| `AudioClip[]` | stoneFootSoundsSprint |  | 
| `GameObject` | textChat |  | 
| `TextChat` | textChatScript |  | 
| `Boolean` | thirdPerson |  | 
| `Single` | updateXFormTimer |  | 
| `Boolean` | useCache |  | 
| `Vector3` | vel |  | 
| `Single` | viewBobMax |  | 
| `VoiceChatV2` | voiceChatScript |  | 
| `Single` | walkSoundSpeed |  | 
| `Single` | walkSpeed |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | ClassId |  | 
| `DimensionType` | CurrentDimension |  | 
| `Boolean` | godMode |  | 
| `Boolean` | HasRing |  | 
| `Boolean` | IsBlinking |  | 
| `Single` | IsMakingSound |  | 
| `Boolean` | isValidTarget |  | 
| `Boolean` | Network_godMode |  | 
| `Single` | NetworkcrouchSpeed |  | 
| `Single` | Networkgravity |  | 
| `Boolean` | NetworkisFly |  | 
| `Single` | NetworkjumpHeight |  | 
| `Single` | NetworkloneTime |  | 
| `Boolean` | NetworknoSee |  | 
| `Boolean` | NetworknoTarget |  | 
| `String` | NetworkplayerGroup |  | 
| `Int32` | NetworkplayerId |  | 
| `String` | NetworkplayerName |  | 
| `Single` | NetworksprintSpeed |  | 
| `UInt64` | NetworksteamId |  | 
| `Boolean` | NetworkthirdPerson |  | 
| `Single` | NetworkwalkSpeed |  | 
| `GameObject` | rot |  | 
| `String` | Zone |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AccessSound(`Int32` id) |  | 
| `void` | AddHint(`String` message, `Color` color, `Single` duration, `HintType` type) |  | 
| `void` | AddTranslatedHint(`String` message, `Color` color, `Single` duration, `HintType` type) |  | 
| `void` | AddTranslatedHint(`String` message, `Color` color, `Single` duration, `HintType` type, `String[]` args) |  | 
| `void` | Awake() |  | 
| `void` | Broadcast(`String` message, `Single` duration = 5) |  | 
| `void` | CheckLoneliness(`Single` oldValue, `Single` newValue) |  | 
| `void` | ClearBroadcasts() |  | 
| `void` | ClearInv() |  | 
| `void` | CmdBlink() |  | 
| `void` | CmdReload() |  | 
| `void` | CmdRequestTag(`String` sid, `String` token, `Boolean` hidetag) |  | 
| `void` | CmdScare(`Single` time) |  | 
| `void` | CmdSetVr(`Boolean` vr) |  | 
| `void` | CmdShoot() |  | 
| `void` | CmdStoneFootstep(`Int32` idx) |  | 
| `void` | CmdTeleportXForm(`Vector3` pos, `Quaternion` baserot, `Single` rot) |  | 
| `IEnumerator` | DelayedDisconnect(`INetworkConnection` conn, `Single` waitTime) |  | 
| `void` | DenyAccessSound(`Int32` id) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Disconnect(`String` message, `Boolean` isTranslated = False, `TextType` translationType = Common) |  | 
| `void` | DropAllInv() |  | 
| `void` | FadeScreen(`Single` alpha, `Single` speed) |  | 
| `void` | Kill(`DeathTypes` type, `GameObject` go) |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | PickupSound() |  | 
| `IEnumerator` | RequestBadgeToken() |  | 
| `void` | RpcAccessSound(`Int32` id) |  | 
| `void` | RpcBleedDamageSound() |  | 
| `void` | RpcDenyAccessSound(`Int32` id) |  | 
| `void` | RpcFallDamage() |  | 
| `void` | RpcPickupSound() |  | 
| `void` | RpcStoneFootstep(`Int32` idx) |  | 
| `void` | RpcUpdateInv() |  | 
| `void` | Scare(`GameObject` scareobj) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | ServerUpdateXForm(`INetworkConnection` connection, `Vector3` pos, `Quaternion` baserot, `Single` rot) |  | 
| `void` | ShowStatus(`String` status) |  | 
| `void` | SwitchSpecCam() |  | 
| `void` | TakeDamage(`Single` f, `GameObject` go, `DeathTypes` type) |  | 
| `void` | TargetDisconnect(`INetworkConnection` conn, `DisconnectMessage` msg) |  | 
| `void` | TargetRpcAddHint(`INetworkConnection` conn, `String` message, `Color` color, `Single` duration, `Int32` type) |  | 
| `void` | TargetRpcAddTranslatedHint(`INetworkConnection` conn, `String` message, `Color` color, `Single` duration, `Int32` type) |  | 
| `void` | TargetRpcAddTranslatedHintWithArgs(`INetworkConnection` conn, `String` message, `Color` color, `Single` duration, `Int32` type, `String[]` args) |  | 
| `void` | TargetRpcAwardAchievement(`INetworkConnection` connection, `String` achievement) |  | 
| `void` | TargetRpcBroadcast(`INetworkConnection` conn, `String` message, `Single` duration) |  | 
| `void` | TargetRpcClearBroadcasts(`INetworkConnection` conn) |  | 
| `void` | TargetRpcFadeScreen(`INetworkConnection` connection, `Single` alpha, `Single` speed) |  | 
| `void` | TargetShowStatus(`INetworkConnection` connection, `String` status) |  | 
| `void` | TargetUpdate1499(`INetworkConnection` conn, `Boolean` isIn) |  | 
| `void` | TargetUpdateXForm(`INetworkConnection` connection, `Vector3` pos, `Quaternion` baserot, `Single` rot) |  | 
| `void` | UpdateFPSChar() |  | 
| `void` | UpdateInvUI() |  | 
| `void` | UserCode_CmdBlink() |  | 
| `void` | UserCode_CmdReload() |  | 
| `void` | UserCode_CmdRequestTag(`String` sid, `String` token, `Boolean` hidetag) |  | 
| `void` | UserCode_CmdScare(`Single` time) |  | 
| `void` | UserCode_CmdShoot() |  | 
| `void` | UserCode_CmdStoneFootstep(`Int32` idx) |  | 
| `void` | UserCode_CmdTeleportXForm(`Vector3` pos, `Quaternion` baserot, `Single` rot) |  | 
| `void` | UserCode_RpcAccessSound(`Int32` id) |  | 
| `void` | UserCode_RpcBleedDamageSound() |  | 
| `void` | UserCode_RpcDenyAccessSound(`Int32` id) |  | 
| `void` | UserCode_RpcFallDamage() |  | 
| `void` | UserCode_RpcPickupSound() |  | 
| `void` | UserCode_RpcStoneFootstep(`Int32` idx) |  | 
| `void` | UserCode_RpcUpdateInv() |  | 
| `void` | UserCode_TargetDisconnect(`INetworkConnection` conn, `DisconnectMessage` msg) |  | 
| `void` | UserCode_TargetRpcAddHint(`INetworkConnection` conn, `String` message, `Color` color, `Single` duration, `Int32` type) |  | 
| `void` | UserCode_TargetRpcAddTranslatedHint(`INetworkConnection` conn, `String` message, `Color` color, `Single` duration, `Int32` type) |  | 
| `void` | UserCode_TargetRpcAddTranslatedHintWithArgs(`INetworkConnection` conn, `String` message, `Color` color, `Single` duration, `Int32` type, `String[]` args) |  | 
| `void` | UserCode_TargetRpcAwardAchievement(`INetworkConnection` connection, `String` achievement) |  | 
| `void` | UserCode_TargetRpcBroadcast(`INetworkConnection` conn, `String` message, `Single` duration) |  | 
| `void` | UserCode_TargetRpcClearBroadcasts(`INetworkConnection` conn) |  | 
| `void` | UserCode_TargetRpcFadeScreen(`INetworkConnection` connection, `Single` alpha, `Single` speed) |  | 
| `void` | UserCode_TargetShowStatus(`INetworkConnection` connection, `String` status) |  | 
| `void` | UserCode_TargetUpdate1499(`INetworkConnection` conn, `Boolean` isIn) |  | 
| `void` | UserCode_TargetUpdateXForm(`INetworkConnection` connection, `Vector3` pos, `Quaternion` baserot, `Single` rot) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerController` | localPlayer |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdBlink(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdChangeName(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdReload(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdRequestTag(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdScare(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdShoot(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdStoneFootstep(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdTeleportXForm(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcAccessSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcBleedDamageSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcDenyAccessSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcFallDamage(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPickupSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcStoneFootstep(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcUpdateInv(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetDisconnect(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcAddHint(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcAddTranslatedHint(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcAddTranslatedHintWithArgs(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcAwardAchievement(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcBroadcast(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcClearBroadcasts(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcFadeScreen(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetShowStatus(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetUpdate1499(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetUpdateXForm(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `PlayerHealthController`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.PlayerHealthController
    : NetworkBehaviour, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip[]` | bleedSounds |  | 
| `AudioSource` | bleedSource |  | 
| `Single` | bloodCooldown |  | 
| `PlayerController` | ctrl |  | 
| `GameObject[]` | decalPrefabs |  | 
| `GameObject` | decalSource |  | 
| `DreamFX4` | dreamfx |  | 
| `Single` | Health |  | 
| `Single` | maxBloodCooldown |  | 
| `Boolean` | ScrambleOthersMessages |  | 
| `Boolean` | ScrambleSentMessages |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Guid |  | 
| `Single` | NetworkHealth |  | 
| `Boolean` | NetworkScrambleOthersMessages |  | 
| `String` | PrefabGuid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | LoadComplete() |  | 
| `void` | PlrDamage(`Single` damage, `GameObject` attacker, `DeathTypes` DamageType = Unknown) |  | 
| `void` | PlrHeal(`Single` heals, `Single` maxHealth) |  | 
| `void` | RpcBleedsound() |  | 
| `void` | RpcPlaceDecal(`Int32` type, `Vector3` position, `Single` size) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | ServerPlaceDecal(`DecalType` decal, `Single` size, `Boolean` sound = True) |  | 
| `void` | UserCode_RpcBleedsound() |  | 
| `void` | UserCode_RpcPlaceDecal(`Int32` type, `Vector3` position, `Single` size) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcBleedsound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlaceDecal(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `PlayerHealthEffectsController`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.PlayerHealthEffectsController
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SyncList<IEffect>` | effects |  | 
| `PlayerHealthController` | healthController |  | 
| `PlayerStats` | stats |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddEffect(`IEffect` effect, `Boolean` stack = True) |  | 
| `void` | EffectAddClient(`IEffect` effect) |  | 
| `void` | EffectRemoveClient(`IEffect` effect) |  | 
| `Boolean` | HasEffect(`String` id) |  | 
| `void` | RemoveAllEffects() |  | 
| `Boolean` | RemoveEffect(`String` id) |  | 


## `PlayerList`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.PlayerList
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | defaultPlayer |  | 
| `Int32` | gameModeId |  | 
| `Dictionary<PlayerController, String>` | groups |  | 
| `Text` | headerT |  | 
| `GameObject` | list |  | 
| `Dictionary<PlayerController, PlayerListElement>` | players |  | 
| `Single` | timer |  | 
| `String` | title |  | 
| `Text` | titleT |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | NetworkgameModeId |  | 
| `String` | Networktitle |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddObject(`PlayerController` instance) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | DestroyObject(`PlayerController` instance) |  | 
| `void` | RpcPlayerListCalculate() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | ServerPlayerListCalculate() |  | 
| `void` | UserCode_RpcPlayerListCalculate() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerList` | List |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPlayerListCalculate(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `PlayerListSetup`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.PlayerListSetup
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | defaultPlayer |  | 
| `Text` | headerT |  | 
| `Text` | titleT |  | 


## `PlayerMissionManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.PlayerMissionManager
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SyncMissionInfo` | localPlayerMissions |  | 
| `AudioClip` | missionClip |  | 
| `PlayerStats` | stats |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddMissionServer(`Nullable<MissionInfo>` mission, `Boolean` Completed) |  | 
| `Int32` | GetIndex(`String` missionName) |  | 
| `MissionInfo` | GetMission(`String` missionName, `MissionInfo` replace) |  | 
| `void` | RemoveMissionServer(`Int32` index) |  | 
| `void` | TargetNewMission(`INetworkConnection` conn, `String` text) |  | 
| `void` | TargetNewMissionKey(`INetworkConnection` conn, `TranslationKeySet` keySet) |  | 
| `void` | TargetPlayAudio(`INetworkConnection` conn) |  | 
| `void` | UserCode_TargetNewMission(`INetworkConnection` conn, `String` text) |  | 
| `void` | UserCode_TargetNewMissionKey(`INetworkConnection` conn, `TranslationKeySet` keySet) |  | 
| `void` | UserCode_TargetPlayAudio(`INetworkConnection` conn) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_TargetNewMission(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetNewMissionKey(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetPlayAudio(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `PlayerMovementController`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.PlayerMovementController
    : NetworkBehaviour, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | AsthmaSpeedValue |  | 
| `CapsuleCollider` | capsule |  | 
| `Single` | clientMovementSync |  | 
| `Vector3` | clientPositionCache |  | 
| `Quaternion` | clientRotationCache |  | 
| `Single` | clientSyncTimer |  | 
| `PlayerController` | ctrl |  | 
| `InteractController` | interact |  | 
| `Boolean` | isGrounded |  | 
| `Boolean` | isMoving |  | 
| `Single` | lerpSpeed |  | 
| `Single` | moveLerpSpeed |  | 
| `Vector3` | movementOverride |  | 
| `PlayerPredict` | predict |  | 
| `UInt64` | prevServerMoveTime |  | 
| `Rigidbody` | rb |  | 
| `Vector4` | rotationOverride |  | 
| `JSONVector` | savePos |  | 
| `JSONVector` | saveRot |  | 
| `Single` | saveRot2 |  | 
| `Vector2` | serverMoveCache |  | 
| `Single` | serverMovementSync |  | 
| `Vector2` | serverMoveRotCache |  | 
| `UInt64` | serverMoveTime |  | 
| `Single` | serverSyncTimer |  | 
| `Single` | soundCrouchLevel |  | 
| `Single` | soundSprintLevel |  | 
| `Single` | soundWalkLevel |  | 
| `Single` | speedMulti |  | 
| `Boolean` | syncIsDucking |  | 
| `Boolean` | syncIsJump |  | 
| `Boolean` | syncIsSprinting |  | 
| `UInt64` | TimeTickerClient |  | 
| `UInt64` | TimeTickerServer |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Guid |  | 
| `Single` | NetworkAsthmaSpeedValue |  | 
| `Vector3` | NetworkmovementOverride |  | 
| `Vector4` | NetworkrotationOverride |  | 
| `Single` | NetworkspeedMulti |  | 
| `Boolean` | NetworksyncIsDucking |  | 
| `Boolean` | NetworksyncIsJump |  | 
| `Boolean` | NetworksyncIsSprinting |  | 
| `String` | PrefabGuid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdSpectate() |  | 
| `void` | CmdUpdate(`Vector3` pos, `Quaternion` rot, `Vector3` vel, `Single` rot2, `Boolean` sprint, `Boolean` crouch, `Boolean` jump, `UInt64` time) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | ForceSetPos(`Vector3` pos) |  | 
| `void` | LoadComplete() |  | 
| `void` | OnGUI() |  | 
| `void` | RpcTeleport(`Vector3` pos, `Quaternion` rot, `Single` rot2) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 
| `void` | UpdateControllerServer(`Boolean` forceFreecam, `Vector3` pos, `Quaternion` rot, `Single` rot2, `Boolean` sprint, `Boolean` crouch, `Boolean` jump, `Single` timestep, `Boolean` skip, `Boolean` calcGravity, `Single` movemulti) |  | 
| `void` | UpdateLook(`Vector2` look) |  | 
| `void` | UpdateMouse() |  | 
| `void` | UserCode_CmdSpectate() |  | 
| `void` | UserCode_RpcTeleport(`Vector3` pos, `Quaternion` rot, `Single` rot2) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `UInt64` | LerpD(`UInt64` a, `UInt64` b, `Single` t) |  | 
| `void` | Skeleton_CmdSpectate(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcTeleport(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `PlayerSave`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.PlayerSave
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerController` | ctrl |  | 
| `String` | Guid |  | 
| `String` | PrefabGuid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetSaveData() |  | 
| `void` | SetSaveData(`Object` data) |  | 


## `PlayerStats`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.PlayerStats
    : NetworkBehaviour, ISavable, IPlayer, IEntity

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AnalogGlitch` | analogGlitch |  | 
| `Single` | blinkDuration |  | 
| `Single` | blinkTimer |  | 
| `AudioClip[]` | breatheGasmaskClips |  | 
| `AudioClip` | breatheGasmaskEnd |  | 
| `AudioClip[]` | breatheNormalClips |  | 
| `AudioClip` | breatheNormalEnd |  | 
| `AudioSource` | breathSource |  | 
| `AudioSource` | breathSourceGasmask |  | 
| `PostTest` | bvPost |  | 
| `Int32` | ClassId |  | 
| `GameObject` | classMesh |  | 
| `GameObject` | classMeshParent |  | 
| `ClassPrefab` | classMeshPrefab |  | 
| `AudioClip[]` | coughClips |  | 
| `AudioSource` | coughSrc |  | 
| `PlayerController` | ctrl |  | 
| `Int32` | curWeaponAmmo |  | 
| `GameObject` | deadBody |  | 
| `DimensionType` | dimension |  | 
| `Single` | dreamDelay |  | 
| `DreamFX2` | dreamfx |  | 
| `Single` | dreamTimer |  | 
| `PlayerHealthEffectsController` | effectsHP |  | 
| `Boolean` | gasmask |  | 
| `Image` | gasMaskOverlay |  | 
| `GameObject` | gunPos |  | 
| `Boolean` | hasCheatsEnabled |  | 
| `Boolean` | hasRing |  | 
| `Boolean` | hasSpawned |  | 
| `AudioClip` | heartbeat |  | 
| `Single` | heartbeatCooldown |  | 
| `AudioSource` | heartbeatSrc |  | 
| `Inventory` | inv |  | 
| `Boolean` | isBlinking |  | 
| `Boolean` | isBlinkingDisabled |  | 
| `Boolean` | isInfRun |  | 
| `PostTest` | ivPost |  | 
| `Boolean` | manualBlink |  | 
| `Single` | maxBlink |  | 
| `Single` | MaxHealth |  | 
| `Single` | maxSprint |  | 
| `AnimationCurve` | moveUpDownCurve |  | 
| `GameObject` | muzzleLight |  | 
| `GameObject` | nvGogglesLight |  | 
| `PostTest` | nvPost |  | 
| `PlayerMissionManager` | playerMissionManager |  | 
| `String` | playerTextureIndex |  | 
| `RenderTexture` | renderTexture |  | 
| `Int32` | reserveAmmo |  | 
| `Single` | rotationOffset |  | 
| `Camera` | specCam |  | 
| `Single` | sprintAmount |  | 
| `Boolean` | sprintIsRecovering |  | 
| `Single` | sprintRecoverDelay |  | 
| `Single` | SprintRecoverMultiplier |  | 
| `Single` | sprintSoundCooldown |  | 
| `Single` | sprintSoundCooldownMax |  | 
| `AnimationCurve` | turnLeftRightCurve |  | 
| `Transform` | usernameText |  | 
| `TextMeshProUGUI` | usernameTextMesh |  | 
| `Single` | viewBobOffset |  | 
| `Single` | viewBobRot |  | 
| `Single` | viewBobTime |  | 
| `String` | zone |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | blueVision |  | 
| `DimensionType` | CurrentDimension |  | 
| `String` | Guid |  | 
| `Single` | Health |  | 
| `Boolean` | infraVision |  | 
| `Single` | NetworkblinkTimer |  | 
| `Int32` | NetworkClassId |  | 
| `Int32` | NetworkcurWeaponAmmo |  | 
| `DimensionType` | Networkdimension |  | 
| `Boolean` | NetworkhasSpawned |  | 
| `Boolean` | NetworkisBlinking |  | 
| `Single` | NetworkmaxBlink |  | 
| `Single` | NetworkMaxHealth |  | 
| `Single` | NetworkmaxSprint |  | 
| `String` | NetworkplayerTextureIndex |  | 
| `Int32` | NetworkreserveAmmo |  | 
| `Single` | NetworksprintAmount |  | 
| `String` | Networkzone |  | 
| `Boolean` | nightVision |  | 
| `PlayerController` | PlayerController |  | 
| `String` | PlayerName |  | 
| `String` | PrefabGuid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClientChangeClass(`Int32` old, `Int32` id) |  | 
| `void` | Cough() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Heal(`Single` heals, `Single` maxHealth) |  | 
| `void` | KillPlayer() |  | 
| `void` | KillPlayer(`DeathTypes` death, `GameObject` killer) |  | 
| `void` | LoadComplete() |  | 
| `void` | RpcBreathe() |  | 
| `void` | RpcBreatheEnd() |  | 
| `void` | RpcCough() |  | 
| `void` | SendPlayerChatMessage(`String` message) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | SetBlinkTimer(`Single` setTime) |  | 
| `void` | SetPosition() |  | 
| `void` | TakeDamage(`Single` damage, `GameObject` damager, `DeathTypes` death = Unknown) |  | 
| `void` | TargetSetManualBlink(`INetworkConnection` conn, `Boolean` value) |  | 
| `void` | UserCode_RpcBreathe() |  | 
| `void` | UserCode_RpcBreatheEnd() |  | 
| `void` | UserCode_RpcCough() |  | 
| `void` | UserCode_TargetSetManualBlink(`INetworkConnection` conn, `Boolean` value) |  | 
| `void` | UseSprint(`Single` multi = 2, `Single` recoverMulti = 2, `Single` maxCutoff = 0, `Single` min = 0, `Boolean` hasgasmask = False) |  | 
| `void` | ViewBob(`Single` mag, `Single` max, `Boolean` isFlying) |  | 
| `void` | ViewBob(`Double` time, `Boolean` isFlying) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | DeathToTranslation(`PlayerController` ctrl, `DeathTypes` death) |  | 
| `void` | Skeleton_RpcBreathe(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcBreatheEnd(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcCough(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetSetManualBlink(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SyncMissionInfo`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.SyncMissionInfo
    : SyncList<MissionInfo>, IList<MissionInfo>, ICollection<MissionInfo>, IEnumerable<MissionInfo>, IEnumerable, IReadOnlyList<MissionInfo>, IReadOnlyCollection<MissionInfo>, ISyncObject

```

## `TextChatDelete`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.TextChatDelete
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CanvasGroup` | canvasGroup |  | 
| `AnimationCurve` | createCurve |  | 
| `Single` | creationTimer |  | 
| `AnimationCurve` | fadeCurve |  | 
| `Single` | hideTimer |  | 
| `Single` | timeAlive |  | 
| `Single` | timeToStartDecay |  | 
| `Text` | txt |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | chatOpen |  | 


## `VoiceChat`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.VoiceChat
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip` | BackClip |  | 
| `BinaryReader` | breader |  | 
| `AudioClip` | clip |  | 
| `Single` | interval |  | 
| `AudioSource` | src |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdSetVoice(`Single[]` arr) |  | 
| `void` | CmdSetVoiceSeq(`Int32` seq, `Single[]` arr) |  | 
| `Single[]` | GetVoice(`Int32` len = 12000, `Int32` offset = 0) |  | 
| `void` | RpcSetVoice(`Single[]` arr) |  | 
| `void` | RpcSetVoiceSeq(`Int32` seq, `Single[]` arr) |  | 
| `void` | UserCode_CmdSetVoice(`Single[]` arr) |  | 
| `void` | UserCode_CmdSetVoiceSeq(`Int32` seq, `Single[]` arr) |  | 
| `void` | UserCode_RpcSetVoice(`Single[]` arr) |  | 
| `void` | UserCode_RpcSetVoiceSeq(`Int32` seq, `Single[]` arr) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | bitRate |  | 
| `Int32` | frequency |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdSetVoice(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdSetVoiceSeq(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSetVoice(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSetVoiceSeq(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


