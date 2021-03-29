## `CleanRoomController`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.CleanRoom.CleanRoomController
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Door` | _aDoor |  | 
| `Door` | _bDoor |  | 
| `GameObject` | aDoorSpawn |  | 
| `AudioSource` | audioSource |  | 
| `GameObject` | bDoorSpawn |  | 
| `Single` | CooldownTime |  | 
| `IEnumerator` | coroutine |  | 
| `GameObject` | defaultDoor |  | 
| `AudioClip` | hiss |  | 
| `ParticleSystem[]` | particles |  | 
| `Light` | redLight |  | 
| `Single` | timer |  | 
| `AudioClip` | warn |  | 
| `Light` | whiteLight |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | RpcChangeLight(`Boolean` state) |  | 
| `void` | RpcWarnSound(`Int32` id) |  | 
| `void` | Start() |  | 
| `void` | Trigger() |  | 
| `void` | Update() |  | 
| `void` | UserCode_RpcChangeLight(`Boolean` state) |  | 
| `void` | UserCode_RpcWarnSound(`Int32` id) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcChangeLight(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcWarnSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `CleanRoomTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.CleanRoom.CleanRoomTrigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CleanRoomController` | ctrl |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnTriggerEnter(`Collider` other) |  | 


