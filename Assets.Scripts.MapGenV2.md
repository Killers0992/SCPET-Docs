## `LukeMapGen`

```csharp
public class Assets.Scripts.MapGenV2.LukeMapGen
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | corner |  | 
| `List<Cube>` | CubeList |  | 
| `Cube[,]` | CubePos |  | 
| `GameObject` | endroom |  | 
| `List<Cube[,][]>` | filterList |  | 
| `GameObject` | hall |  | 
| `List<Cube>` | largestCubePatch |  | 
| `Int32` | MaxHeight |  | 
| `Int32` | MaxWidth |  | 
| `List<Cube>` | ramCubePatch |  | 
| `GameObject` | RemovedRoom |  | 
| `Random` | rng |  | 
| `Int32` | Seed |  | 
| `GameObject` | troom |  | 
| `GameObject` | xroom |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddAllFilters() |  | 
| `void` | AddFilter(`Cube[,]` from, `Cube[,]` to) |  | 
| `Cube` | CreateCube(`Int32` x, `Int32` y, `RoomDir` rot = none, `RoomType` type = none) |  | 
| `Cube[]` | CreateRandLine(`Int32` MinSize, `Int32` MaxSize) |  | 
| `Boolean` | CubeIsConnected(`Cube` fro, `Cube` to) |  | 
| `Vector2` | DirToDirection(`RoomDir` dir) |  | 
| `void` | FilterThrough() |  | 
| `void` | GenMap(`Int32` Seed) |  | 
| `IEnumerator` | GenMapInterval(`Int32` Seed = 0) |  | 
| `Cube[]` | GetConnectedCubes(`Cube` inpCube) |  | 
| `Cube` | GetCube(`Int32` x, `Int32` y) |  | 
| `GameObject` | GetPrefab(`RoomType` typ) |  | 
| `void` | mapGenThread() |  | 
| `List<Cube>` | RemoveUselessCubes(`List<Cube>` cubes) |  | 
| `void` | TransformCubes() |  | 
| `Quaternion` | TranslateAng(`RoomAng` ang) |  | 


## `MapGenTree`

```csharp
public class Assets.Scripts.MapGenV2.MapGenTree
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | endingRoom |  | 
| `String` | startingRoom |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GenerateMap() |  | 


## `MapGenV4Room`

```csharp
public class Assets.Scripts.MapGenV2.MapGenV4Room
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsSpecialRoom |  | 
| `BoxCollider` | LightBorder |  | 
| `Boolean` | MaxSpawns |  | 
| `BoxCollider[]` | RoomBorders |  | 
| `Int32` | RoomId |  | 
| `RoomType` | RoomType |  | 
| `RoomZone` | RoomZone |  | 


