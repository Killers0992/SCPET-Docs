## `NetworkedRigidbody`

```csharp
public class ClientSidePrediction.RB.NetworkedRigidbody
    : NetworkedClient<RigidbodyInput, RigidbodyState>, INetworkedClient

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ProcessInput(`RigidbodyInput` input) |  | 
| `RigidbodyState` | RecordState(`UInt32` lastProcessedInputTick) |  | 
| `void` | SetState(`RigidbodyState` state) |  | 


## `NetworkedRigidbodyGUI`

```csharp
public class ClientSidePrediction.RB.NetworkedRigidbodyGUI
    : NetworkedClientGUI

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DrawStats() |  | 
| `void` | SetPhantomState(`GameObject` phantom, `INetworkedClientState` state) |  | 


## `NetworkedRigidbodyMessenger`

```csharp
public class ClientSidePrediction.RB.NetworkedRigidbodyMessenger
    : NetworkBehaviour, INetworkedClientMessenger<RigidbodyInput, RigidbodyState>

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `RigidbodyState` | LatestServerState |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `Action<RigidbodyInput>` | OnInputReceived |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SendInput(`RigidbodyInput` input) |  | 
| `void` | SendState(`RigidbodyState` state) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdSendInput(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSendState(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `RigidbodyInput`

```csharp
public struct ClientSidePrediction.RB.RigidbodyInput
    : INetworkedClientInput

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | deltaTime |  | 
| `Vector2` | movement |  | 
| `UInt32` | tick |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | DeltaTime |  | 
| `UInt32` | Tick |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ToString() |  | 


## `RigidbodyPrediction`

```csharp
public class ClientSidePrediction.RB.RigidbodyPrediction
    : ClientPrediction<RigidbodyInput, RigidbodyState>

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `RigidbodyInput` | GetInput(`Single` deltaTime, `UInt32` currentTick) |  | 


## `RigidbodyState`

```csharp
public struct ClientSidePrediction.RB.RigidbodyState
    : IEquatable<RigidbodyState>, INetworkedClientState, IEquatable<INetworkedClientState>

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | angularVelocity |  | 
| `UInt32` | lastProcessedInputTick |  | 
| `Vector3` | position |  | 
| `Quaternion` | rotation |  | 
| `Vector3` | velocity |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `UInt32` | LastProcessedInputTick |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Equals(`RigidbodyState` other) |  | 
| `Boolean` | Equals(`INetworkedClientState` other) |  | 
| `String` | ToString() |  | 


