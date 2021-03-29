## `Door`

```csharp
public abstract class PluginFramework.Classes.Door

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | GameObject |  | 
| `Boolean` | IsOpen |  | 
| `Vector3` | Position |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Close() |  | 
| `void` | Open() |  | 


## `Effect`

```csharp
public abstract class PluginFramework.Classes.Effect

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | id |  | 
| `Single` | Intensity |  | 
| `Boolean` | Temporary |  | 
| `Single` | TimeLeft |  | 


## `IPlayer`

```csharp
public interface PluginFramework.Classes.IPlayer
    : IEntity

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `PlayerController` | PlayerController |  | 
| `String` | PlayerName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | KillPlayer() |  | 
| `void` | SendPlayerChatMessage(`String` message) |  | 


## `IScp`

```csharp
public interface PluginFramework.Classes.IScp
    : IEntity

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ScpName |  | 


## `IScript`

```csharp
public interface PluginFramework.Classes.IScript

```

