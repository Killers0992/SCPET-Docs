## `AirlockController`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Airlock.AirlockController
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | alarm |  | 
| `GameObject` | ambient |  | 
| `GameObject` | buttonPrefab |  | 
| `List<GameObject>` | buttons |  | 
| `GameObject[]` | buttonSpawns |  | 
| `Door` | door1 |  | 
| `GameObject` | door1Spawn |  | 
| `Door` | door2 |  | 
| `GameObject` | door2Spawn |  | 
| `GameObject` | doorPrefab |  | 
| `Boolean` | isAlarm |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | NetworkisAlarm |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Door1Toggle() |  | 
| `void` | Door2Toggle() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


## `AirlockTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Airlock.AirlockTrigger
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | chance |  | 
| `AirlockController` | parent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnTriggerEnter(`Collider` other) |  | 


