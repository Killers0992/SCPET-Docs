## `ButtonWallAdjuster`

```csharp
public class Assets.Scripts.ButtonWallAdjuster
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | found |  | 
| `LayerMask` | layerMask |  | 
| `Single` | offset |  | 


## `CanvasController`

```csharp
public class Assets.Scripts.CanvasController
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | inventory |  | 
| `PlayerController` | localplayerController |  | 
| `GameObject` | playerlist |  | 
| `GameObject` | textchat |  | 


## `NetworkVideoPlayer`

```csharp
public class Assets.Scripts.NetworkVideoPlayer
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isPlaying |  | 
| `GameObject` | screen |  | 
| `Double` | time |  | 
| `String` | url |  | 
| `VideoPlayer` | vplayer |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | NetworkisPlaying |  | 
| `Double` | Networktime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ApplyScreenParams(`Vector3` pos, `Vector3` rot, `Vector3` scale) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | RpcPlay() |  | 
| `void` | RpcStop() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | UserCode_RpcPlay() |  | 
| `void` | UserCode_RpcStop() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPlay(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcStop(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `PlayerListElement`

```csharp
public class Assets.Scripts.PlayerListElement
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Text` | groupnames |  | 
| `Button` | muteButton |  | 
| `Texture2D` | mutedIcon |  | 
| `Text` | nickname |  | 
| `PlayerController` | player |  | 
| `Button` | profileButton |  | 
| `Texture2D` | unmutedIcon |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Change() |  | 
| `void` | Click() |  | 
| `void` | ClickProfile() |  | 
| `void` | ClickReport() |  | 
| `void` | OnEnable() |  | 


