## `MapObject`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGen.MapObject
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ObjectCategory |  | 
| `String` | ObjectName |  | 
| `String` | ObjectParams |  | 
| `MapObjectType` | ObjectType |  | 
| `Object` | tempData |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | NetworkObjectParams |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `Object` | GetData() |  | 
| `Object` | GetObjectSettings() |  | 
| `void` | LoadObjectWithParameters(`String` oldVal, `String` str) |  | 
| `void` | LoadSettings(`Object` settings) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | SetData(`JToken` token) |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


## `PMapCluster`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGen.PMapCluster
    : MonoBehaviour, IMapCluster

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | _boundingBox |  | 
| `String` | clusterId |  | 
| `List<GameObject>` | doors |  | 
| `Int32` | maxSpawned |  | 
| `Boolean` | require |  | 
| `String` | zone |  | 


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


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GenGUID() |  | 
| `void` | OnDrawGizmos() |  | 
| `void` | Update() |  | 


## `PMapDoor`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGen.PMapDoor
    : MonoBehaviour, IMapDoor

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | _prefab |  | 
| `String` | zone |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsNotSpawned |  | 
| `GameObject` | Prefab |  | 
| `String` | Zone |  | 


## `PMapFeature`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGen.PMapFeature
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | featurePrefab |  | 
| `Int32` | maxAmount |  | 


## `PMapGen`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGen.PMapGen
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | allowCustom |  | 
| `Boolean` | autoGenOnStart |  | 
| `Boolean` | bakeNavMesh |  | 
| `Texture2D[]` | layouts |  | 
| `MapData` | map |  | 
| `MapGenType` | mapGenType |  | 
| `Int32` | MapSeed |  | 
| `NavMeshDataInstance` | navMeshInstance |  | 
| `Random` | rng |  | 
| `Boolean` | useNetworkManager |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GenMap(`Int32` seed) |  | 
| `void` | GenMapCustom() |  | 
| `GameObject` | GetObjectByID(`String` obj) |  | 
| `GameObject` | GetRoomById(`String` roomname) |  | 
| `void` | OnDisable() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SpawnDoors() |  | 
| `void` | SpawnFeatures() |  | 


## `PMapRandomizer`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGen.PMapRandomizer
    : MonoBehaviour, IRoomRandomizer

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RoomType` | _roomType |  | 
| `String` | _roomZone |  | 
| `Single` | debugScale |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `RoomType` | RoomType |  | 
| `String` | RoomZone |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDrawGizmos() |  | 


## `PMapRoom`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGen.PMapRoom
    : MonoBehaviour, IRoom

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | _boundingBox |  | 
| `String` | _roomName |  | 
| `RoomType` | _roomType |  | 
| `String` | _roomZone |  | 
| `Int32` | maxSpawned |  | 
| `Boolean` | require |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Bounds` | Bounds |  | 
| `Boolean` | IsInEditMode |  | 
| `IMapDoor[]` | MapDoors |  | 
| `Int32` | MaxTimesToSpawn |  | 
| `Boolean` | Required |  | 
| `String` | RoomId |  | 
| `String` | RoomName |  | 
| `RoomType` | RoomType |  | 
| `String` | RoomZone |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDrawGizmos() |  | 


## `PMapSwitcher`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapGen.PMapSwitcher
    : MonoBehaviour, IRoomSwitcher

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | _room |  | 
| `GameObject[]` | _roomsFail |  | 
| `String` | guid |  | 
| `Int32` | max |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IRoom[]` | FailureRooms |  | 
| `Int32` | MaxRooms |  | 
| `IRoom` | Room |  | 
| `String` | SwitcherId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | GenGUID() |  | 


