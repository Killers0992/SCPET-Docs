## `CleanRoomActivateEvent`

```csharp
public class PluginFramework.Events.EventsArgs.CleanRoomActivateEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `CleanRoomController` | Controller |  | 
| `IHuman` | Human |  | 
| `CleanRoomTrigger` | Trigger |  | 


## `DoorToggleEvent`

```csharp
public class PluginFramework.Events.EventsArgs.DoorToggleEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Door` | Door |  | 
| `IEntity` | Entity |  | 


## `ItemDropEvent`

```csharp
public class PluginFramework.Events.EventsArgs.ItemDropEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | item |  | 
| `IPlayer` | player |  | 


## `ItemPickupEvent`

```csharp
public class PluginFramework.Events.EventsArgs.ItemPickupEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | item |  | 
| `IPlayer` | player |  | 


## `PlayerAuthEvent`

```csharp
public class PluginFramework.Events.EventsArgs.PlayerAuthEvent
    : EventArgs

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AuthRequestMessage` | RequestMessage |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `INetworkConnection` | Connection |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Reject(`String` reason) |  | 


## `PlayerClassChangeEvent`

```csharp
public class PluginFramework.Events.EventsArgs.PlayerClassChangeEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | newClassId |  | 
| `IPlayer` | player |  | 
| `Int32` | prevClassId |  | 


## `PlayerDamageEvent`

```csharp
public class PluginFramework.Events.EventsArgs.PlayerDamageEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEntity` | damager |  | 
| `IEntity` | victim |  | 


## `PlayerDeathEvent`

```csharp
public class PluginFramework.Events.EventsArgs.PlayerDeathEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEntity` | killer |  | 
| `IEntity` | victim |  | 


## `PlayerEffectEvent`

```csharp
public class PluginFramework.Events.EventsArgs.PlayerEffectEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEffect` | effect |  | 
| `IPlayer` | player |  | 


## `PlayerJoinFinalEvent`

```csharp
public class PluginFramework.Events.EventsArgs.PlayerJoinFinalEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IPlayer` | player |  | 


## `PlayerLeaveEvent`

```csharp
public class PluginFramework.Events.EventsArgs.PlayerLeaveEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IPlayer` | player |  | 


## `PlayerPreJoinEvent`

```csharp
public class PluginFramework.Events.EventsArgs.PlayerPreJoinEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IPlayer` | player |  | 


## `RoundEndEvent`

```csharp
public class PluginFramework.Events.EventsArgs.RoundEndEvent
    : EventArgs

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | EscapedPlayers |  | 
| `Boolean` | ForceEnded |  | 


