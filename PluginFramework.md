## `IGameGlobals`

```csharp
public interface PluginFramework.IGameGlobals

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SendAdminCommand(`String` command, `IPlayer` player) |  | 
| `void` | SendChatCommand(`String` command, `IPlayer` player) |  | 
| `void` | SendGlobalChatMessage(`String` message) |  | 
| `void` | SpawnNpc(`String` id, `Vector3` position) |  | 


## `Plugin`

```csharp
public abstract class PluginFramework.Plugin

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 


## `PluginSystem`

```csharp
public class PluginFramework.PluginSystem

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<String>` | loadedDependencies |  | 
| `Dictionary<String, Plugin>` | loadedPlugins |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IGameGlobals` | GameGlobals |  | 
| `Logger` | Logger |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ExecuteCleanRoomActivate(`CleanRoomActivateEvent` ev) |  | 
| `void` | ExecuteDoorOpen(`DoorToggleEvent` ev) |  | 
| `void` | ExecuteItemDrop(`ItemDropEvent` ev) |  | 
| `void` | ExecuteItemPickup(`ItemPickupEvent` ev) |  | 
| `void` | ExecutePlayerAuth(`PlayerAuthEvent` ev) |  | 
| `void` | ExecutePlayerClassChange(`PlayerClassChangeEvent` ev) |  | 
| `void` | ExecutePlayerDamage(`PlayerDamageEvent` ev) |  | 
| `void` | ExecutePlayerDeath(`PlayerDeathEvent` ev) |  | 
| `void` | ExecutePlayerEffect(`PlayerEffectEvent` ev) |  | 
| `void` | ExecutePlayerJoinFinal(`PlayerJoinFinalEvent` ev) |  | 
| `void` | ExecutePlayerLeave(`PlayerLeaveEvent` ev) |  | 
| `void` | ExecutePlayerPreJoin(`PlayerPreJoinEvent` ev) |  | 
| `void` | ExecuteRoundEnd(`RoundEndEvent` ev) |  | 
| `void` | ExecuteRoundRestart() |  | 
| `void` | ExecuteRoundStart() |  | 
| `void` | LoadDependency(`Int32` index, `Int32` count, `String` path) |  | 
| `void` | LoadPlugin(`Int32` index, `Int32` count, `String` path) |  | 
| `void` | LoadPlugins(`String` pluginsDirectory) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, List<MethodInfo>>` | plugins |  | 


Static Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `PluginSystem` | Manager |  | 


Static Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `CleanRoomActivate` | CleanRoomActivateEvent |  | 
| `ItemDrop` | ItemDropEvent |  | 
| `ItemPickup` | ItemPickupEvent |  | 
| `PlayerAuth` | PlayerAuthEvent |  | 
| `PlayerClassChange` | PlayerClassChangeEvent |  | 
| `PlayerDamage` | PlayerDamageEvent |  | 
| `PlayerDeath` | PlayerDeathEvent |  | 
| `PlayerEffect` | PlayerEffectEvent |  | 
| `PlayerJoinFinal` | PlayerJoinFinalEvent |  | 
| `PlayerLeave` | PlayerLeaveEvent |  | 
| `PlayerPreJoin` | PlayerPreJoinEvent |  | 
| `RoundEnd` | RoundEndEvent |  | 
| `RoundRestart` | RoundRestartEvent |  | 
| `RoundStart` | RoundStartEvent |  | 


