## `FemurBreakerButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.FemurBreaker.FemurBreakerButton
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `FemurBreakerControl` | control |  | 
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
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `FemurBreakerControl`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.FemurBreaker.FemurBreakerControl
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<AudioClip>` | clips |  | 
| `GameObject` | containmentCube |  | 
| `List<Camera>` | monitorCams |  | 
| `Scp106RecontainmentMonitor[]` | monitors |  | 
| `Scp106RecontainmentStatus` | recontainmentStatus |  | 
| `GameObject` | spawnpoint |  | 
| `BoxCollider` | whoPressButtonBox |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Scp106RecontainmentStatus` | NetworkrecontainmentStatus |  | 
| `Boolean` | recontained |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | BreakFemur() |  | 
| `IEnumerator` | Contain() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | MoveCubeUp() |  | 
| `void` | RpcMoveCubeUp() |  | 
| `void` | RpcPlayClip(`Int32` id) |  | 
| `void` | RpcStopCams() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | Start() |  | 
| `void` | StopCams() |  | 
| `void` | TargetRpcRecontain106Achievement(`INetworkConnection` connection) |  | 
| `void` | UserCode_RpcMoveCubeUp() |  | 
| `void` | UserCode_RpcPlayClip(`Int32` id) |  | 
| `void` | UserCode_RpcStopCams() |  | 
| `void` | UserCode_TargetRpcRecontain106Achievement(`INetworkConnection` connection) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcMoveCubeUp(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayClip(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcStopCams(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRpcRecontain106Achievement(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `Scp106RecontainmentStatus`

```csharp
public enum VirtualBrightPlayz.SCP_ET.World.FemurBreaker.Scp106RecontainmentStatus
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `-1` | Unknown |  | 
| `0` | Uncontained |  | 
| `1` | ActivatingBreaker |  | 
| `2` | BreakingFemur |  | 
| `3` | InBox |  | 
| `4` | Contained |  | 


