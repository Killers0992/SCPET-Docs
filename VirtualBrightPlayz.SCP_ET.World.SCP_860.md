## `SCP860Door`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_860.SCP860Door
    : NetworkBehaviour, ILever, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | box |  | 
| `AudioClip` | entranceClip |  | 
| `Boolean` | gizmo |  | 
| `Double` | lastUsedTime |  | 
| `AudioClip` | lockedClip |  | 
| `AudioClip` | openClip |  | 
| `Outline` | outline |  | 
| `AudioClip` | preUnlockClip |  | 
| `AudioSource` | source |  | 
| `Single` | useTimerCooldown |  | 
| `Single` | useTimerLocal |  | 
| `Single` | useTimerMax |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ExitDim(`PlayerController` player, `Boolean` start) |  | 
| `void` | Highlighted() |  | 
| `void` | OnDoorUsed(`DoorUsedMessage` message, `INetworkConnection` sender = null) |  | 
| `void` | RpcPlayLockedSound() |  | 
| `void` | RpcPlayOpenSound(`Boolean` start) |  | 
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `void` | Update() |  | 
| `Boolean` | UpdateLook(`PlayerController` user, `Vector2` look) |  | 
| `void` | UserCode_OnDoorUsed(`DoorUsedMessage` message, `INetworkConnection` sender) |  | 
| `void` | UserCode_RpcPlayOpenSound(`Boolean` start) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_OnDoorUsed(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayOpenSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP860WP`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_860.SCP860WP
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isStart |  | 
| `GameObject` | pos |  | 
| `AudioSource` | source |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | TeleportServer(`PlayerController` player) |  | 


