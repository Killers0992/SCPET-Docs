## `CharacterControllerInput`

```csharp
public struct ClientSidePrediction.CC.CharacterControllerInput
    : INetworkedClientInput

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | deltaTime |  | 
| `Vector2` | input |  | 
| `UInt32` | tick |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | DeltaTime |  | 
| `UInt32` | Tick |  | 


## `CharacterControllerMessenger`

```csharp
public class ClientSidePrediction.CC.CharacterControllerMessenger
    : NetworkBehaviour, INetworkedClientMessenger<CharacterControllerInput, CharacterControllerState>

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `CharacterControllerState` | LatestServerState |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `Action<CharacterControllerInput>` | OnInputReceived |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SendInput(`CharacterControllerInput` input) |  | 
| `void` | SendState(`CharacterControllerState` state) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdSendInput(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSendState(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `CharacterControllerPrediction`

```csharp
public class ClientSidePrediction.CC.CharacterControllerPrediction
    : ClientPrediction<CharacterControllerInput, CharacterControllerState>

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `CharacterControllerInput` | GetInput(`Single` deltaTime, `UInt32` currentTick) |  | 


## `CharacterControllerState`

```csharp
public struct ClientSidePrediction.CC.CharacterControllerState
    : IEquatable<CharacterControllerState>, INetworkedClientState, IEquatable<INetworkedClientState>

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `UInt32` | lastProcessedInput |  | 
| `Vector3` | position |  | 
| `Single` | verticalVelocity |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `UInt32` | LastProcessedInputTick |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Equals(`CharacterControllerState` other) |  | 
| `Boolean` | Equals(`INetworkedClientState` other) |  | 


## `NetworkedCharacterController`

```csharp
public class ClientSidePrediction.CC.NetworkedCharacterController
    : NetworkedClient<CharacterControllerInput, CharacterControllerState>, INetworkedClient

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ProcessInput(`CharacterControllerInput` input) |  | 
| `CharacterControllerState` | RecordState(`UInt32` lastProcessedInputTick) |  | 
| `void` | SetState(`CharacterControllerState` state) |  | 


## `NetworkedCharacterControllerGUI`

```csharp
public class ClientSidePrediction.CC.NetworkedCharacterControllerGUI
    : NetworkedClientGUI

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DrawStats() |  | 
| `void` | SetPhantomState(`GameObject` phantom, `INetworkedClientState` state) |  | 


