## `BinaryExtend`

```csharp
public static class VirtualBrightPlayz.SCP_ET.SaveLoad.BinaryExtend

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `JSONVector` | ReadVector(this `BinaryReader` reader) |  | 
| `void` | WriteString(this `BinaryWriter` writer, `String` str) |  | 
| `void` | WriteVector(this `BinaryWriter` writer, `JSONVector` vector) |  | 


## `ISavable`

```csharp
public interface VirtualBrightPlayz.SCP_ET.SaveLoad.ISavable

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Guid |  | 
| `String` | PrefabGuid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | LoadComplete() |  | 


## `SaveContract<T>`

```csharp
public class VirtualBrightPlayz.SCP_ET.SaveLoad.SaveContract<T>
    : DefaultContractResolver, IContractResolver

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IList<JsonProperty>` | CreateProperties(`Type` type, `MemberSerialization` memberSerialization) |  | 


## `SavedData`

```csharp
public class VirtualBrightPlayz.SCP_ET.SaveLoad.SavedData
    : Attribute, _Attribute

```

## `SaveManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.SaveLoad.SaveManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<GameObject>` | saveGuidObjectPrefabs |  | 
| `Boolean` | useSaveLoad |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | GetGameObject(`String` guid) |  | 
| `GameObject` | GetGameObjectByGuid(`String` guid) |  | 
| `void` | Load(`String` savename = quicksave) |  | 
| `void` | Save(`String` savename = quicksave) |  | 
| `IEnumerator` | SpawnLate(`List<GameObject>` used) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SaveManager` | manager |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, Object>` | GetSaveObject(`Object` obj) |  | 


## `SaveObject`

```csharp
public class VirtualBrightPlayz.SCP_ET.SaveLoad.SaveObject
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | guid |  | 
| `String` | prefabGuid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | GenGUID() |  | 
| `void` | LoadFinished() |  | 


## `UnsavedData`

```csharp
public class VirtualBrightPlayz.SCP_ET.SaveLoad.UnsavedData
    : Attribute, _Attribute

```

