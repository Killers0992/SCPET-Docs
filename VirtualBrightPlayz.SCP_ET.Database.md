## `DatabaseManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.Database.DatabaseManager

```

Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<IObjectDatabase>` | databases |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | GetId(`Object` obj) |  | 
| `Object` | GetObject(`String` id) |  | 
| `void` | RegisterNetwork() |  | 
| `void` | Spawn(`GameObject` obj) |  | 


## `IObjectDatabase`

```csharp
public interface VirtualBrightPlayz.SCP_ET.Database.IObjectDatabase

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IDictionary<String, Object>` | Database |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | GetId(`Object` obj) |  | 
| `void` | RegisterNetwork() |  | 


