## `NetPlayerMove`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Movement.NetPlayerMove
    : NetworkedClient<PlayerInput, PlayerState>, INetworkedClient

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | footTick |  | 
| `Single` | networkSyncInterval |  | 
| `Double` | time |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | ProcessInput(`PlayerInput` input) |  | 
| `PlayerState` | RecordState(`UInt32` lastProcessedInputTick) |  | 
| `void` | SetState(`PlayerState` state) |  | 


## `PlayerInput`

```csharp
public struct VirtualBrightPlayz.SCP_ET.Player.Movement.PlayerInput
    : INetworkedClientInput

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | crouching |  | 
| `Single` | deltaTime |  | 
| `Vector2` | input |  | 
| `Vector2` | inputRotation |  | 
| `Boolean` | jumping |  | 
| `Boolean` | sprinting |  | 
| `UInt32` | tick |  | 
| `UInt32` | viewBobTime |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | DeltaTime |  | 
| `UInt32` | Tick |  | 


## `PlayerMoveMessage`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Movement.PlayerMoveMessage
    : NetworkBehaviour, INetworkedClientMessenger<PlayerInput, PlayerState>

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | maxInputs |  | 
| `Int32` | maxStates |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerState` | LatestServerState |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `Action<PlayerInput>` | OnInputReceived |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SendInput(`PlayerInput` input) |  | 
| `void` | SendState(`PlayerState` state) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdSendInput(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSendState(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `PlayerPredict`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Movement.PlayerPredict
    : ClientPrediction<PlayerInput, PlayerState>

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector2` | input |  | 
| `Boolean` | jump |  | 
| `Vector2` | look |  | 
| `UInt32` | viewTick |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `PlayerInput` | GetInput(`Single` deltaTime, `UInt32` currentTick) |  | 
| `void` | Update() |  | 


## `PlayerState`

```csharp
public struct VirtualBrightPlayz.SCP_ET.Player.Movement.PlayerState
    : IEquatable<PlayerState>, INetworkedClientState, IEquatable<INetworkedClientState>

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isGrounded |  | 
| `UInt32` | lastProcessedInput |  | 
| `Vector3` | position |  | 
| `Quaternion` | rotation |  | 
| `Double` | time |  | 
| `Single` | verticalVelocity |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `UInt32` | LastProcessedInputTick |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Equals(`PlayerState` other) |  | 
| `Boolean` | Equals(`INetworkedClientState` other) |  | 


