## `SCP049ButtonGenCtrl`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_049_Room.SCP049ButtonGenCtrl
    : NetworkBehaviour, ILever, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | box |  | 
| `AudioClip` | clip |  | 
| `Single` | curRotZ |  | 
| `Boolean` | gizmo |  | 
| `Transform` | leverHandle |  | 
| `String` | missionName |  | 
| `Single` | newRotZ |  | 
| `Outline` | outline |  | 
| `SCP049Room` | scp |  | 
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
| `void` | OnLeverTurn(`GenCtrlLeverMessage` message, `INetworkConnection` sender = null) |  | 
| `void` | RpcSwitchSound() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `Boolean` | UpdateLook(`PlayerController` user, `Vector2` look) |  | 
| `void` | UserCode_OnLeverTurn(`GenCtrlLeverMessage` message, `INetworkConnection` sender) |  | 
| `void` | UserCode_RpcSwitchSound() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_OnLeverTurn(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSwitchSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP049ButtonPowerCtrl`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_049_Room.SCP049ButtonPowerCtrl
    : NetworkBehaviour, ILever, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | box |  | 
| `AudioClip` | clip |  | 
| `Single` | curRotZ |  | 
| `Boolean` | gizmo |  | 
| `Transform` | leverHandle |  | 
| `String` | missionName |  | 
| `Single` | newRotZ |  | 
| `Outline` | outline |  | 
| `SCP049Room` | scp |  | 
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
| `void` | OnLeverTurn(`PowerCtrlLeverMessage` message, `INetworkConnection` sender = null) |  | 
| `void` | RpcSwitchSound() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `Boolean` | UpdateLook(`PlayerController` user, `Vector2` look) |  | 
| `void` | UserCode_OnLeverTurn(`PowerCtrlLeverMessage` message, `INetworkConnection` sender) |  | 
| `void` | UserCode_RpcSwitchSound() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_OnLeverTurn(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSwitchSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP049Room`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_049_Room.SCP049Room
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip` | beginclip |  | 
| `Door` | ContainmentDoor |  | 
| `GameObject` | containmentDoorPrefab |  | 
| `GameObject` | ContainmentDoorSpawn |  | 
| `List<ElevatorController>` | ElevatorControllers |  | 
| `Boolean` | energySubsystemStarted |  | 
| `SCP049ButtonGenCtrl` | genCtrl |  | 
| `Boolean` | geneneratoron |  | 
| `AudioSource` | genSoundSource |  | 
| `Boolean` | isinprogress |  | 
| `AudioClip` | lightsToggleClip |  | 
| `AudioSource` | lightsToggleSource |  | 
| `GameObject` | lowerDoorPrefab |  | 
| `List<Door>` | lowerDoors |  | 
| `List<GameObject>` | lowerDoorSpawns |  | 
| `List<Light>` | lowerLights |  | 
| `MissionInfo` | mission |  | 
| `GameObject` | monitorButton |  | 
| `MonitorInteractController` | monitorController |  | 
| `TMP_Text` | monitorText |  | 
| `SCP049ButtonPowerCtrl` | powerCtrl |  | 
| `Boolean` | powerleveron |  | 
| `List<Light>` | upperLights |  | 
| `List<GameObject>` | zombieSpawns |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | NetworkenergySubsystemStarted |  | 
| `Boolean` | Networkgeneneratoron |  | 
| `Boolean` | Networkisinprogress |  | 
| `Boolean` | Networkpowerleveron |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | btnClick() |  | 
| `void` | CmdClickBtn() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | DisableDoors() |  | 
| `void` | EnableDoors() |  | 
| `void` | EnergySubsystem(`Boolean` old, `Boolean` cur) |  | 
| `void` | LightsCheck(`Boolean` old, `Boolean` cur) |  | 
| `void` | OnTriggerEnter(`Collider` other) |  | 
| `IEnumerator` | openContainment() |  | 
| `void` | RpcUpdateInProgress() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | SetGenLeverOff() |  | 
| `void` | SetGenLeverOn() |  | 
| `IEnumerator` | SetInProgress() |  | 
| `void` | SetPowerLeverOff() |  | 
| `void` | SetPowerLeverOn() |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 
| `void` | UserCode_CmdClickBtn() |  | 
| `void` | UserCode_RpcUpdateInProgress() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdClickBtn(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcUpdateInProgress(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


