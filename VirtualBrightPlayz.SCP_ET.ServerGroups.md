## `AdminCommand`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.AdminCommand
    : Attribute, _Attribute

```

## `AdminMenu`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.AdminMenu
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | ListIsOpen |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdAdminCommand(`String` arguments) |  | 
| `void` | CmdUpdatePlayerIndex(`NetworkIdentity` idx) |  | 
| `void` | doorBtnPress(`String` door, `Int32` curdoorcount) |  | 
| `void` | doorLockBtnPress(`String` door, `Int32` curdoorcount) |  | 
| `void` | Start() |  | 
| `void` | TargetRefreshDoorMenu(`INetworkConnection` conn) |  | 
| `void` | UpdateCurrPlayerIndex(`Int32` currentIndex) |  | 
| `void` | UserCode_CmdAdminCommand(`String` arguments) |  | 
| `void` | UserCode_CmdUpdatePlayerIndex(`NetworkIdentity` idx) |  | 
| `void` | UserCode_doorBtnPress(`String` door, `Int32` curdoorcount) |  | 
| `void` | UserCode_doorLockBtnPress(`String` door, `Int32` curdoorcount) |  | 
| `void` | UserCode_TargetRefreshDoorMenu(`INetworkConnection` conn) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, IAdminCommand>` | commands |  | 
| `AdminMenu` | MenuOfAdmin |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdAdminCommand(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdUpdatePlayerIndex(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_doorBtnPress(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_doorLockBtnPress(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetRefreshDoorMenu(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `AdminMenuUI`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.AdminMenuUI
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | AdminSettings |  | 
| `TMP_InputField` | commandInput |  | 
| `GameObject` | defaultDoorBtn |  | 
| `Dictionary<String, Door>` | doors |  | 
| `GameObject` | doorsTabContent |  | 
| `TMP_Dropdown` | PlayerDropdown |  | 
| `TMP_Dropdown` | TabDropdown |  | 
| `List<GameObject>` | tabs |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | registerDoors() |  | 
| `void` | SendCommand(`String` cmd) |  | 
| `void` | SendCommand() |  | 
| `void` | Start() |  | 
| `void` | UpdateCurrPlayerIndex(`Int32` currentIndex) |  | 
| `void` | UpdateTab() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AdminMenuUI` | MenuOfAdmin |  | 


## `BanHandler`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.BanHandler
    : NetworkBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Addban(`INetworkConnection` conn, `String` reason, `TimeSpan` duration) |  | 
| `BanInfo` | GetBan(`INetworkConnection` conn) |  | 
| `void` | Removeban(`String` steamid, `String` ip) |  | 
| `void` | Start() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BanHandler` | singleton |  | 


## `BanInfo`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.BanInfo

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `DateTime` | BannedOn |  | 
| `TimeSpan` | Duration |  | 
| `String` | Ip |  | 
| `String` | Nickname |  | 
| `String` | Reason |  | 
| `String` | Steamid |  | 


## `IngameReport`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.IngameReport
    : NetworkBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdReportToGlobalModeration(`Int32` reporterId, `Int32` reportedId, `String` reason) |  | 
| `void` | CmdReportToStaff(`Int32` reporterId, `Int32` reportedId, `String` reason) |  | 
| `UniTask` | Sendwebhook(`Webhook` webhook, `List<Embed>` embeds, `Boolean` docallback) |  | 
| `void` | Start() |  | 
| `void` | TargetReportCallback(`INetworkConnection` conn, `Boolean` reportsuccess, `String` reason, `Boolean` translated) |  | 
| `void` | UserCode_CmdReportToGlobalModeration(`Int32` reporterId, `Int32` reportedId, `String` reason) |  | 
| `void` | UserCode_CmdReportToStaff(`Int32` reporterId, `Int32` reportedId, `String` reason) |  | 
| `void` | UserCode_TargetReportCallback(`INetworkConnection` conn, `Boolean` reportsuccess, `String` reason, `Boolean` translated) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `IngameReport` | singleton |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdReportToGlobalModeration(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdReportToStaff(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetReportCallback(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `IngameReportUI`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.IngameReportUI
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | animatedImage |  | 
| `Button` | cancelButton |  | 
| `GameObject` | innerImage |  | 
| `Boolean` | isSending |  | 
| `GameObject` | outerImage |  | 
| `GameObject` | overlay |  | 
| `TMP_InputField` | ReasonInput |  | 
| `PlayerController` | reported |  | 
| `TMP_Text` | reportedNameText |  | 
| `Button` | sendToGlobalModerationButton |  | 
| `Button` | sendToStaffButton |  | 
| `GameObject` | Window |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | closeBox() |  | 
| `void` | FixedUpdate() |  | 
| `void` | OpenBox(`PlayerController` reportedplayer) |  | 
| `void` | Report(`Boolean` isCheat) |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `IngameReportUI` | singleton |  | 


## `MuteHandler`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.MuteHandler
    : NetworkBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddMute(`INetworkConnection` conn, `String` reason, `TimeSpan` duration) |  | 
| `MuteInfo` | GetMute(`INetworkConnection` conn) |  | 
| `void` | RemoveMute(`String` steamid, `String` ip) |  | 
| `void` | Start() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MuteHandler` | singleton |  | 


## `MuteInfo`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.MuteInfo

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `TimeSpan` | Duration |  | 
| `String` | Ip |  | 
| `DateTime` | MutedOn |  | 
| `String` | Nickname |  | 
| `String` | Reason |  | 
| `String` | Steamid |  | 


## `ReportingModel`

```csharp
public struct VirtualBrightPlayz.SCP_ET.ServerGroups.ReportingModel

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ReportedAuth |  | 
| `Int32` | ReportedPlayerId |  | 
| `String` | ReporterAuth |  | 
| `String` | ReportReason |  | 
| `String` | Server |  | 


## `ServerGroups`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerGroups.ServerGroups
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `HolidayUpdate` | holidayUpdate |  | 
| `Int32` | lastPlayerId |  | 
| `Int32` | maxPlayers |  | 
| `ServerGroup` | serverGroup |  | 
| `String` | serverUri |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `HolidayUpdate` | NetworkholidayUpdate |  | 
| `Int32` | NetworkmaxPlayers |  | 
| `String` | NetworkserverUri |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `GroupData` | ApplyGroup(`INetworkConnection` connection) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | GenerateGroupsConfig(`String` path) |  | 
| `void` | Reload() |  | 
| `IEnumerator` | RequestTag(`String` sid, `String` token, `Boolean` hidetag) |  | 
| `void` | RpcValidateGlobalBadge(`NetworkIdentity` player, `String` groups, `String` steamid) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | UserCode_RpcValidateGlobalBadge(`NetworkIdentity` player, `String` groups, `String` steamid) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ServerGroups` | singleton |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CheckPermission(`INetworkConnection` connection, `String` permission) |  | 
| `Boolean` | CheckPermission(`PlayerController` ctrl, `String` permission, `Boolean` outputNoPermission = False, `String` noPermissionMessage = No permission. ( required permission: %permission% )) |  | 
| `void` | Skeleton_RpcValidateGlobalBadge(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


