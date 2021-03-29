## `CustomNetworkManager`

```csharp
public class Assets.MirrorEXT.CustomNetworkManager
    : NetworkManager

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | currentServerAddress |  | 
| `GameObject` | lobbyPrefab |  | 
| `String` | lobbyScene |  | 
| `Int32` | maxPlayers |  | 
| `String` | menuScene |  | 
| `GameObject` | playerPrefab |  | 
| `List<NetworkConnection>` | QueuedPlayers |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `Boolean` | BoxCallback(`Int32` code) |  | 
| `void` | CommonServerHostStart() |  | 
| `IEnumerator` | GetServerAddress() |  | 
| `IEnumerator` | HostGame() |  | 
| `IEnumerator` | JoinSteamRelayLobby(`Lobby` lobby1, `SteamId` id1) |  | 
| `void` | LobbyInvited(`Friend` friend, `Lobby` lobby1) |  | 
| `void` | LobbyJoined(`Lobby` lobby1, `SteamId` id1) |  | 
| `void` | LobbyJoined(`Lobby` lobby1) |  | 
| `void` | OnClientDisconnect() |  | 
| `void` | OnDestroy() |  | 
| `void` | OnServerDisconnect(`INetworkConnection` conn) |  | 
| `void` | OnServerReady(`INetworkConnection` conn) |  | 
| `void` | OnStartClient(`INetworkConnection` conn) |  | 
| `void` | OnStartHost() |  | 
| `void` | OnStartServer() |  | 
| `void` | OnStopHost() |  | 
| `void` | OnStopServer() |  | 
| `IEnumerator` | ServerList() |  | 
| `IEnumerator` | StartSteamLobby() |  | 
| `IEnumerator` | StartSteamServer() |  | 
| `void` | SteamServerConnect() |  | 
| `void` | SteamServerDisconnected(`Result` result) |  | 
| `void` | SteamServerFail(`Result` result, `Boolean` stillTrying) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | customMapJson |  | 
| `Boolean` | isDedicated |  | 
| `Lobby` | lobby |  | 
| `CustomNetworkManager` | manager |  | 
| `String` | mapName |  | 
| `Int32` | NetworkObjectCount |  | 
| `Boolean` | publicServer |  | 


