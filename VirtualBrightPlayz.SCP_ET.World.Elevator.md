## `ElevatorButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Elevator.ElevatorButton
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `ElevatorController` | elevator |  | 
| `ElevatorNetwork` | elevatorNet |  | 
| `Int32` | ElevatorNetworkId |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Int32` | NetworkElevatorNetworkId |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Highlighted() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `ElevatorController`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Elevator.ElevatorController
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioSource` | bAudio |  | 
| `BoxCollider` | bcollider |  | 
| `GameObject` | bDoor |  | 
| `GameObject` | bDoorPos |  | 
| `AudioClip` | beepAudio |  | 
| `GameObject` | doorprefab |  | 
| `String` | elevatorRefId |  | 
| `Boolean` | isblackedout |  | 
| `Boolean` | islocked |  | 
| `Boolean` | isMoving |  | 
| `LayerMask` | mask |  | 
| `AudioClip` | movingAudio |  | 
| `ElevatorNetwork` | network |  | 
| `Int32` | networkId |  | 
| `Boolean` | onTopLevel |  | 
| `NetworkIdentitySyncvar` | otherRef |  | 
| `AudioSource` | tAudio |  | 
| `BoxCollider` | tcollider |  | 
| `GameObject` | tDoor |  | 
| `GameObject` | tDoorPos |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `NetworkIdentity` | NetworkotherRef |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Beep() |  | 
| `IEnumerator` | ChangeFloor(`Single` time) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | LoadComplete() |  | 
| `void` | MoveAudio() |  | 
| `void` | QueueChangeFloor() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 


## `ElevatorDoor`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Elevator.ElevatorDoor
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allow096Open |  | 
| `Boolean` | allow173Open |  | 
| `Boolean` | allow939Open |  | 
| `GameObject[]` | closePos |  | 
| `AudioClip[]` | closeSounds |  | 
| `ElevatorController` | elevator |  | 
| `AudioClip` | forceClose |  | 
| `Boolean` | isElevator |  | 
| `Boolean` | isLocked |  | 
| `Boolean` | IsMoving |  | 
| `Single` | maxTimeOpen |  | 
| `GameObject[]` | modelPos |  | 
| `Boolean` | open |  | 
| `AudioClip` | open096 |  | 
| `AudioClip` | open173 |  | 
| `AudioClip` | open939 |  | 
| `GameObject[]` | openPos |  | 
| `AudioClip[]` | openSounds |  | 
| `Single` | openTimer |  | 
| `Single` | speed |  | 
| `AudioClip` | timeWarnClip |  | 
| `Boolean` | useTimeOpen |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsOpen |  | 
| `Boolean` | NetworkisLocked |  | 
| `Boolean` | Networkopen |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdClose() |  | 
| `void` | CmdForceClose() |  | 
| `void` | CmdOpen() |  | 
| `void` | CmdOpen096() |  | 
| `void` | CmdOpen173() |  | 
| `void` | CmdOpen939() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
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


## `ElevatorLink`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Elevator.ElevatorLink
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ElevatorController` | controller |  | 


## `ElevatorNetwork`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Elevator.ElevatorNetwork
    : NetworkBehaviour, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | bDoorSave |  | 
| `ElevatorController[]` | controllers |  | 
| `Boolean[]` | isMoving |  | 
| `Boolean[]` | isOnTop |  | 
| `String[]` | tDoorSave |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Guid |  | 
| `String` | PrefabGuid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | LoadComplete() |  | 
| `void` | RpcStartMove(`Int32` id) |  | 
| `void` | RpcStopMove(`Int32` id) |  | 
| `void` | StartMove(`Int32` id) |  | 
| `void` | StopMove(`Int32` id) |  | 
| `void` | UserCode_RpcStartMove(`Int32` id) |  | 
| `void` | UserCode_RpcStopMove(`Int32` id) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcStartMove(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcStopMove(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `ElevatorRef`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Elevator.ElevatorRef
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioSource` | bAudio |  | 
| `BoxCollider` | bcollider |  | 
| `GameObject` | bDoorPos |  | 
| `NetworkIdentitySyncvar` | elevator |  | 
| `String` | elevatorId |  | 
| `Int32` | id |  | 
| `Boolean` | used |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `NetworkIdentity` | Networkelevator |  | 
| `Int32` | Networkid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | GenGUID() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 


