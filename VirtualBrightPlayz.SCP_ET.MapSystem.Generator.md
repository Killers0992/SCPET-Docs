## `ClusterGenerator`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapSystem.Generator.ClusterGenerator
    : MonoBehaviour, IMapGenerator

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | boundsPadding |  | 
| `GameObject[]` | clusterObjects |  | 
| `Single` | distanceToStop |  | 
| `Int32` | maxClusterRemove |  | 
| `Int32` | maxHallLength |  | 
| `Int32` | maxHalls |  | 
| `Int32` | maxIterations |  | 
| `Int32` | minHalls |  | 
| `Boolean` | requireAllRequiredClusters |  | 
| `GameObject[]` | roomObjects |  | 
| `Boolean` | showFailedClusters |  | 
| `String` | startingZone |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IMapCluster[]` | clusters |  | 
| `Int32` | MaxIterations |  | 
| `IMapCluster[]` | requiredClusters |  | 
| `IRoom[]` | requiredRooms |  | 
| `IRoom[]` | rooms |  | 
| `List<IRoom>` | SpawnedRooms |  | 
| `IMapDoor` | StartDoor |  | 
| `Dictionary<String, Int32>` | UsedClusters |  | 
| `Dictionary<String, Int32>` | UsedSwitchers |  | 
| `IMapCluster[]` | validClusters |  | 
| `Dictionary<String, Int32>` | ZoneIterations |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IRoom[]` | GenerateMap(`Int32` seed, `Boolean` root) |  | 
| `void` | Start() |  | 


## `GridGenerator`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapSystem.Generator.GridGenerator
    : MonoBehaviour, IMapGenerator

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Cell>` | cells |  | 
| `List<Vector2Int>` | gennedCells |  | 
| `Int32` | maxIterations |  | 
| `Int32` | minIterationsToNewGen |  | 
| `Int32` | newGenChance |  | 
| `Component` | newGenComponent |  | 
| `GameObject[]` | rooms |  | 
| `Vector2Int` | size |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | MaxIterations |  | 
| `IMapGenerator` | newGen |  | 
| `List<IRoom>` | SpawnedRooms |  | 
| `IMapDoor` | StartDoor |  | 
| `Dictionary<String, Int32>` | UsedClusters |  | 
| `Dictionary<String, Int32>` | UsedSwitchers |  | 
| `Dictionary<String, Int32>` | ZoneIterations |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Cell[]` | CellsInDir(`WallType` dir, `Cell` cell, `Int32` amount) |  | 
| `IRoom[]` | GenerateMap(`Int32` seed, `Boolean` root) |  | 
| `IRoom[]` | GenerateSubMap(`Int32` seed, `IRoom` extend, `List<IRoom>` rooms, `List<IMapCluster>` clusters, `Dictionary<String, Int32>` usedClusters, `Dictionary<String, Int32>` usedSwitchers, `Dictionary<String, Int32>` zoneIterations) |  | 
| `Boolean` | GenRecur(`Random` rng, `Cell` startcell, `Int32` recur) |  | 
| `Cell` | GetCellAt(`Vector2Int` pos) |  | 
| `Cell[]` | GetCellsNear(`Cell` cell) |  | 
| `WallType` | GetCellWallType(`Cell` cell) |  | 
| `GameObject` | GetRoomFromType(`Random` rng, `RoomType` type, `Boolean` filter) |  | 
| `RoomType` | GetRoomTypeFromWallType(`WallType` wallType) |  | 
| `Single` | GetYEulerFromWallType(`WallType` wallType, `RoomType` roomType) |  | 
| `Boolean` | IsSameDir(`IMapDoor` door, `WallType` wallType) |  | 
| `IRoom[]` | RequiredRooms(`RoomType` type) |  | 
| `void` | RoomAdd(`IRoom` room) |  | 
| `Int32` | RoomUses(`IRoom` room) |  | 
| `void` | SetCellAt(`Vector2Int` pos, `Cell` cell) |  | 
| `void` | Start() |  | 
| `WallType` | WallTypeFromTwoCellsDiff(`Cell` cell1, `Cell` cell2) |  | 
| `WallType` | WallTypeFromTwoCellsDiff(`WallType` intype, `Cell` cell1, `Cell` cell2) |  | 


## `IMapGenerator`

```csharp
public interface VirtualBrightPlayz.SCP_ET.MapSystem.Generator.IMapGenerator

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | MaxIterations |  | 
| `List<IRoom>` | SpawnedRooms |  | 
| `IMapDoor` | StartDoor |  | 
| `Dictionary<String, Int32>` | UsedClusters |  | 
| `Dictionary<String, Int32>` | UsedSwitchers |  | 
| `Dictionary<String, Int32>` | ZoneIterations |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IRoom[]` | GenerateMap(`Int32` seed, `Boolean` root) |  | 


## `MapCluster`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapSystem.Generator.MapCluster
    : MonoBehaviour, IMapCluster

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | _boundingBox |  | 
| `GameObject[]` | doors |  | 
| `Int32` | maxSpawned |  | 
| `Boolean` | require |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Bounds` | Bounds |  | 
| `String` | ClusterId |  | 
| `IMapDoor[]` | Doors |  | 
| `Int32` | MaxTimesToSpawn |  | 
| `IRoomRandomizer[]` | Randomizers |  | 
| `Boolean` | Required |  | 
| `IRoom[]` | Rooms |  | 
| `IRoomSwitcher[]` | Switchers |  | 
| `String` | Zone |  | 


## `MapGenCaller`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapSystem.Generator.MapGenCaller
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | genOnStart |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GenRandomMap() |  | 
| `void` | Start() |  | 


