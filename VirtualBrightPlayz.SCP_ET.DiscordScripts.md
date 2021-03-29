## `StatusManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.DiscordScripts.StatusManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | cooldown |  | 
| `String` | currentRoom |  | 
| `Guid` | currParty |  | 
| `Discord` | discord |  | 
| `Dictionary<Int64, String>` | discordInvites |  | 
| `List<Int64>` | discordRelations |  | 
| `RelationshipManager` | relman |  | 
| `String` | serverProvider |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | FriendCheck(`Relationship&` relationship) |  | 
| `void` | InGame(`String` room) |  | 
| `void` | InRoom(`String` room, `Boolean` includePrefix = True) |  | 
| `void` | MainMenu() |  | 
| `void` | OnApplicationQuit() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int64` | DiscordAppId |  | 
| `StatusManager` | manager |  | 


## `StatusRoom`

```csharp
public class VirtualBrightPlayz.SCP_ET.DiscordScripts.StatusRoom
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `PMapRoom` | room |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | RoomName |  | 


## `StatusTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.DiscordScripts.StatusTrigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Text |  | 


