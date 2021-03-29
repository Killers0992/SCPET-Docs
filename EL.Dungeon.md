## `DungeonData`

```csharp
public class EL.Dungeon.DungeonData
    : ScriptableObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<DungeonSet>` | sets |  | 


## `DungeonSet`

```csharp
public class EL.Dungeon.DungeonSet
    : ScriptableObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Room>` | bosses |  | 
| `List<Door>` | doors |  | 
| `List<Room>` | roomTemplates |  | 
| `List<Room>` | spawns |  | 


## `GeneratorDoor`

```csharp
public class EL.Dungeon.GeneratorDoor
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Door` | door |  | 
| `Boolean` | open |  | 
| `GeneratorDoor` | sharedDoor |  | 
| `GameObject` | voxelOwner |  | 


## `Room`

```csharp
public class EL.Dungeon.Room
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<GeneratorDoor>` | doors |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `GeneratorDoor` | GetFirstOpenDoor() |  | 
| `GeneratorDoor` | GetRandomDoor(`DRandom` random) |  | 
| `Boolean` | hasOpenDoors() |  | 


## `Volume`

```csharp
public class EL.Dungeon.Volume
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Bounds` | bounds |  | 
| `GameObject` | gameObjectContainer |  | 
| `Vector3` | generatorSize |  | 
| `List<GameObject>` | voxels |  | 
| `Single` | voxelScale |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AssignVoxelsToList() |  | 
| `void` | GenerateVoxelGrid() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | RecalculateBounds() |  | 
| `void` | ToggleGizmoToDraw() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | drawVolume |  | 


