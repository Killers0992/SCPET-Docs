## `SCP1499Child`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_1499.SCP1499Child
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ParticleSystem` | effect |  | 
| `HeightmapMesh` | heightmap |  | 
| `Vector2Int` | offset |  | 
| `GameObject[]` | rngObjects |  | 
| `Transform[]` | rngSpawns |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | Setup() |  | 
| `void` | Start() |  | 


## `SCP1499World`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_1499.SCP1499World
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | amount |  | 
| `Bounds` | bounds |  | 
| `List<SCP1499Child>` | children |  | 
| `AudioClip` | clip |  | 
| `Color` | color |  | 
| `GameObject` | defaultInstance |  | 
| `Single` | distanceNpcSpawn |  | 
| `ParticleSystem` | effect |  | 
| `Single` | farClip |  | 
| `Boolean` | isExiting |  | 
| `FastNoiseLite` | noise |  | 
| `Int32` | npcSpawnAmount |  | 
| `List<GameObject>` | scpSpawns |  | 
| `Int32` | seed |  | 
| `Material` | sky |  | 
| `Vector3` | spawnpos |  | 
| `Transform` | sun |  | 
| `Color` | sunColor |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | Networkseed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | GenChunks(`Vector2Int` dims) |  | 
| `void` | OnDrawGizmos() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | ServerDeleteNpc() |  | 
| `void` | ServerSpawnNpc() |  | 
| `void` | SyncSeed(`Int32` old, `Int32` cur) |  | 
| `void` | Update() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SCP1499World` | instance |  | 


