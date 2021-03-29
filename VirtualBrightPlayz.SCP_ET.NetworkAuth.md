## `AdminPasswordAuth`

```csharp
public class VirtualBrightPlayz.SCP_ET.NetworkAuth.AdminPasswordAuth
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | systemPassword |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdSendPassword(`Byte[]` encryptedPassword) |  | 
| `void` | SendPassword(`String` plaintext) |  | 
| `void` | Start() |  | 
| `void` | TargetSendPubkey(`INetworkConnection` connection, `String` xml) |  | 
| `void` | UserCode_CmdSendPassword(`Byte[]` encryptedPassword) |  | 
| `void` | UserCode_TargetSendPubkey(`INetworkConnection` connection, `String` xml) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Byte[]` | RSADecrypt(`Byte[]` data, `RSAParameters` keyinfo) |  | 
| `Byte[]` | RSAEncrypt(`Byte[]` data, `RSAParameters` keyinfo) |  | 
| `void` | Skeleton_CmdSendPassword(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetSendPubkey(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `AuthenticatedUser`

```csharp
public class VirtualBrightPlayz.SCP_ET.NetworkAuth.AuthenticatedUser

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | AuthToken |  | 
| `UInt64` | SteamId |  | 


## `SteamAuth2`

```csharp
public class VirtualBrightPlayz.SCP_ET.NetworkAuth.SteamAuth2
    : NetworkAuthenticator

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<INetworkConnection>` | pending |  | 
| `Dictionary<UInt64, NetworkConnection>` | requests |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | DelayedDisconnect(`INetworkConnection` conn, `Single` waitTime) |  | 
| `IEnumerator` | DelayedDisconnect2(`INetworkConnection` conn, `Single` waitTime) |  | 
| `IEnumerator` | GetAuthTicket(`INetworkConnection` conn, `AuthTicket` authres) |  | 
| `void` | GetModsHashes(`INetworkConnection` conn) |  | 
| `UniTask` | GetSteamAuthTicket(`INetworkConnection` conn) |  | 
| `void` | OnAuthRequestMessage(`INetworkConnection` connection, `AuthRequestMessage` message) |  | 
| `void` | OnAuthResponseMessage(`INetworkConnection` conn, `AuthResponseMessage` msg) |  | 
| `void` | OnClientAuthenticate(`INetworkConnection` conn) |  | 
| `void` | OnModResponseMessage(`INetworkConnection` conn, `ModResponseMessage` msg) |  | 
| `void` | OnModResponseMessageServer(`INetworkConnection` conn, `ModResponseMessage` msg) |  | 
| `void` | OnServerAuthenticate(`INetworkConnection` conn) |  | 
| `void` | OnStartClient() |  | 
| `void` | OnStartServer() |  | 
| `void` | Start() |  | 
| `IEnumerator` | StartAuthentication(`INetworkConnection` conn, `AuthRequestMessage` msg) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | currentOfflineMode |  | 
| `String` | currentPassword |  | 


