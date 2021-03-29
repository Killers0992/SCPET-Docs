## `ChangeLogItem`

```csharp
public class Assets.Scripts.Mainmenu.ChangeLogItem
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | defaultItem |  | 
| `Text` | text |  | 


## `ConnectPage`

```csharp
public class Assets.Scripts.Mainmenu.ConnectPage
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `InputField` | address |  | 
| `InputField` | password |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ConnectTo() |  | 


## `DisconnectBox`

```csharp
public class Assets.Scripts.Mainmenu.DisconnectBox
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | disconnectBox |  | 
| `TMP_Text` | headerText |  | 
| `GameObject` | imageGroup |  | 
| `GameObject` | innerImage |  | 
| `TMP_Text` | messageText |  | 
| `Button` | okBtn |  | 
| `GameObject` | OuterImage |  | 
| `GameObject` | overlay |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Close() |  | 
| `void` | displayBox(`String` message, `String` header, `Boolean` showokbutton = True, `Func<Int32, Boolean>` callback = null) |  | 
| `void` | OK() |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `DisconnectBox` | singleton |  | 


## `FriendData`

```csharp
public class Assets.Scripts.Mainmenu.FriendData
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Activity` | activity |  | 
| `Int64` | discordId |  | 
| `Boolean` | discordInvite |  | 
| `Boolean` | discordLobby |  | 
| `Lobby` | lobby |  | 
| `Int64` | lobbyId |  | 
| `GameObject` | objectRef |  | 
| `RawImage` | profileImage |  | 
| `TMP_Text` | username |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnClick() |  | 


## `FriendsListPage`

```csharp
public class Assets.Scripts.Mainmenu.FriendsListPage
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `FriendData` | defaultData |  | 
| `GameObject` | emptyFriendslistInfo |  | 
| `List<FriendData>` | friendData |  | 
| `Coroutine` | friendsHandler |  | 
| `Int32` | pCount |  | 
| `Transform` | rootObject |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture2D` | GetSteamImageAsTexture2D(`Nullable<Image>` iImage) |  | 
| `void` | LoadFriendsList() |  | 
| `IEnumerator` | LoadFriendslistAsync() |  | 
| `void` | Update() |  | 


## `HostPage`

```csharp
public class Assets.Scripts.Mainmenu.HostPage
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dropdown` | hosttype |  | 
| `Dropdown` | maps |  | 
| `InputField` | maxPlayers |  | 
| `InputField` | password |  | 
| `InputField` | serverName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Host() |  | 
| `void` | LoadPage() |  | 
| `void` | OnEnable() |  | 


## `ServerData`

```csharp
public class Assets.Scripts.Mainmenu.ServerData
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | dedicated |  | 
| `String` | ip |  | 
| `Lobby` | lobby |  | 
| `String` | map |  | 
| `Int32` | maxplayers |  | 
| `GameObject` | objectRef |  | 
| `Boolean` | official |  | 
| `Text` | OfficialText |  | 
| `String` | PastebinId |  | 
| `Int32` | players |  | 
| `Text` | playerstext |  | 
| `String` | port |  | 
| `String` | serverName |  | 
| `Text` | serverNametext |  | 
| `Boolean` | verified |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | GetPastebin() |  | 
| `void` | OnClick() |  | 
| `void` | Play() |  | 


## `ServerListPage`

```csharp
public class Assets.Scripts.Mainmenu.ServerListPage
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ServerData` | currData |  | 
| `ServerData` | defaultData |  | 
| `GameObject` | emptyServerlistInfo |  | 
| `GameObject` | InfoBox |  | 
| `TMP_Text` | InfoHeaderText |  | 
| `TMP_Text` | InfoText |  | 
| `Boolean` | isLoading |  | 
| `List<ServerData>` | serverData |  | 
| `Coroutine` | serversHandler |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | FindByName(`InputField` field) |  | 
| `void` | LoadServerList(`Boolean` first = False) |  | 
| `IEnumerator` | LoadServerlistAsync() |  | 
| `void` | OnClick() |  | 
| `void` | OnClickClose() |  | 
| `void` | Refresh() |  | 
| `void` | SortServerList() |  | 
| `void` | Start() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ServerListPage` | singleton |  | 


