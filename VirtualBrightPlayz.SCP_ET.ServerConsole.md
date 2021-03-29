## `ConsoleCommandHandler`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerConsole.ConsoleCommandHandler
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | FixedUpdate() |  | 
| `void` | Start() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, IConsoleCommand>` | commands |  | 


## `TcpConsole`

```csharp
public class VirtualBrightPlayz.SCP_ET.ServerConsole.TcpConsole
    : MonoBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Start() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ConcurrentQueue<String>` | chatqueue |  | 
| `ConcurrentQueue<String>` | consolecommandqueue |  | 
| `ConcurrentQueue<String>` | messagequeue |  | 
| `TcpConsole` | singleton |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Addlog(`String` message, `Color32` color) |  | 


