## `PlayerEvents`

```csharp
public class PluginFramework.Events.PlayerEvents

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InvokeCleanRoomActivate(`IHuman` human, `CleanRoomController` controller, `CleanRoomTrigger` trigger) |  | 
| `void` | InvokeItemDrop(`IPlayer` player, `ItemBase` item) |  | 
| `void` | InvokeItemPickup(`IPlayer` player, `ItemBase` item) |  | 
| `void` | InvokePlayerAuth(`INetworkConnection` connection, `AuthRequestMessage` requestmessage) |  | 
| `void` | InvokePlayerClassChange(`IPlayer` player, `Int32` prevClassId, `Int32` newClassId) |  | 
| `void` | InvokePlayerDamage(`IEntity` victim, `IEntity` damager) |  | 
| `void` | InvokePlayerDeath(`IEntity` victim, `IEntity` killer) |  | 
| `void` | InvokePlayerEffect(`IPlayer` player, `IEffect` effect) |  | 
| `void` | InvokePlayerJoinFinal(`IPlayer` player) |  | 
| `void` | InvokePlayerLeave(`IPlayer` player) |  | 
| `void` | InvokePlayerPreJoin(`IPlayer` player) |  | 


## `WorldEvents`

```csharp
public class PluginFramework.Events.WorldEvents

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InvokeDoorOpen(`IEntity` ent, `Door` door) |  | 
| `void` | InvokeRoundEnd(`Int32` escapedplayers, `Boolean` forceended) |  | 
| `void` | InvokeRoundRestart() |  | 
| `void` | InvokeRoundStart() |  | 


