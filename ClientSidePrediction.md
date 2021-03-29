## `ClientPrediction<TClientInput, TClientState>`

```csharp
public abstract class ClientSidePrediction.ClientPrediction<TClientInput, TClientState>
    : MonoBehaviour

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `NetworkedClient<TClientInput, TClientState>` | Client |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `TClientInput` | GetInput(`Single` deltaTime, `UInt32` currentTick) |  | 
| `void` | HandleTick(`Single` deltaTime, `UInt32` currentTick, `TClientState` latestServerState) |  | 


## `INetworkedClient`

```csharp
public interface ClientSidePrediction.INetworkedClient

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `UInt32` | CurrentTick |  | 
| `INetworkedClientState` | LatestServerState |  | 


## `INetworkedClientInput`

```csharp
public interface ClientSidePrediction.INetworkedClientInput

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | DeltaTime |  | 
| `UInt32` | Tick |  | 


## `INetworkedClientMessenger<TClientInput, TClientState>`

```csharp
public interface ClientSidePrediction.INetworkedClientMessenger<TClientInput, TClientState>

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `TClientState` | LatestServerState |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `Action<TClientInput>` | OnInputReceived |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SendInput(`TClientInput` input) |  | 
| `void` | SendState(`TClientState` state) |  | 


## `INetworkedClientState`

```csharp
public interface ClientSidePrediction.INetworkedClientState
    : IEquatable<INetworkedClientState>

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `UInt32` | LastProcessedInputTick |  | 


## `MainMenu`

```csharp
public class ClientSidePrediction.MainMenu
    : MonoBehaviour

```

## `NetworkedClient<TClientInput, TClientState>`

```csharp
public abstract class ClientSidePrediction.NetworkedClient<TClientInput, TClientState>
    : MonoBehaviour, INetworkedClient

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | networkUpdateInterval |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `UInt32` | CurrentTick |  | 
| `INetworkedClientState` | LatestServerState |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | HandleOtherPlayerState(`TClientState` state) |  | 
| `void` | LogInputQueue() |  | 
| `void` | LogState() |  | 
| `void` | ProcessInput(`TClientInput` input) |  | 
| `TClientState` | RecordState(`UInt32` lastProcessedInputTick) |  | 
| `void` | SendClientInput(`TClientInput` input) |  | 
| `void` | SetState(`TClientState` state) |  | 


## `NetworkedClientGUI`

```csharp
public abstract class ClientSidePrediction.NetworkedClientGUI
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DrawStats() |  | 
| `void` | SetPhantomState(`GameObject` phantom, `INetworkedClientState` state) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | ServerTickRate |  | 


