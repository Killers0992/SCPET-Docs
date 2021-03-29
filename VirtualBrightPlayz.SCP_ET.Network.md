## `CustomLobby`

```csharp
public class VirtualBrightPlayz.SCP_ET.Network.CustomLobby
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | gameScene |  | 
| `Int32` | index |  | 
| `GameObject` | leaveButton |  | 
| `GameObject` | lobbyStartRoot |  | 
| `GameObject` | manualStartScreen |  | 
| `Texture2D` | mutedIcon |  | 
| `GameObject` | playerlistContent |  | 
| `GameObject` | playerlistDefault |  | 
| `String` | serverMaxPlayers |  | 
| `TextMeshProUGUI` | serverMaxPlayersText |  | 
| `String` | serverName |  | 
| `TextMeshProUGUI` | serverNameText |  | 
| `Transform[]` | spawns |  | 
| `GameObject` | startButton |  | 
| `LobbyStartTypes` | startType |  | 
| `String` | text |  | 
| `GameObject` | timerStartScreen |  | 
| `Texture2D` | unmutedIcon |  | 
| `Int32` | voteCount |  | 
| `Boolean` | voted |  | 
| `GameObject` | voteStartScreen |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | NetworkserverMaxPlayers |  | 
| `String` | NetworkserverName |  | 
| `LobbyStartTypes` | NetworkstartType |  | 
| `String` | Networktext |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `Transform` | GetNextPlayerSpawn() |  | 
| `IEnumerator` | RoundCountDownTimer() |  | 
| `void` | RpcOpenLoadingBox() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | StartGame() |  | 
| `void` | StopGame() |  | 
| `void` | UpdateMaxPlayers(`String` old, `String` cur) |  | 
| `void` | UpdateName(`String` old, `String` cur) |  | 
| `void` | UpdatePlrList() |  | 
| `void` | UpdateText(`String` old, `String` cur) |  | 
| `void` | UserCode_RpcOpenLoadingBox() |  | 
| `void` | Vote() |  | 
| `IEnumerator` | VoteStartScreen() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcOpenLoadingBox(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `CustomLobbyPlayer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Network.CustomLobbyPlayer
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CustomLobby` | lobby |  | 
| `String` | playerName |  | 
| `TextMeshProUGUI` | text |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | NetworkplayerName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdChangeName(`String` plrname) |  | 
| `void` | CmdRequestStartPerm() |  | 
| `void` | CmdTryStart() |  | 
| `void` | CmdVote(`Boolean` value) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | OnDestroy() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | SetName(`String` old, `String` cur) |  | 
| `IEnumerator` | Start() |  | 
| `void` | TargetSetStartPerm(`INetworkConnection` identity, `Boolean` value) |  | 
| `void` | TargetVoteResponse(`INetworkConnection` identity, `Boolean` val) |  | 
| `void` | Update() |  | 
| `void` | UserCode_CmdChangeName(`String` plrname) |  | 
| `void` | UserCode_CmdRequestStartPerm() |  | 
| `void` | UserCode_CmdTryStart() |  | 
| `void` | UserCode_CmdVote(`Boolean` value) |  | 
| `void` | UserCode_TargetSetStartPerm(`INetworkConnection` identity, `Boolean` value) |  | 
| `void` | UserCode_TargetVoteResponse(`INetworkConnection` identity, `Boolean` val) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdChangeName(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdRequestStartPerm(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdTryStart(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdVote(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetSetStartPerm(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetVoteResponse(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `DatabaseClientObjectManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.Network.DatabaseClientObjectManager
    : ClientObjectManager

```

