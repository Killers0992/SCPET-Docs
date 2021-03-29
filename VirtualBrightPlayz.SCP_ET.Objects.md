## `ClassDSpawnObject`

```csharp
public class VirtualBrightPlayz.SCP_ET.Objects.ClassDSpawnObject
    : MapObject, IMapObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | classid |  | 
| `String` | objName |  | 
| `TextMeshPro` | text |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ObjectId |  | 
| `String` | ObjectName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetData() |  | 
| `void` | JsonToObject(`JToken` json) |  | 
| `Object` | ObjectToJson() |  | 
| `void` | SetData(`JToken` token) |  | 
| `void` | Start() |  | 


## `CustomObject`

```csharp
public class VirtualBrightPlayz.SCP_ET.Objects.CustomObject
    : MapObject, IMapObject

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ObjectId |  | 
| `String` | ObjectName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetData() |  | 
| `void` | JsonToObject(`JToken` json) |  | 
| `Object` | ObjectToJson() |  | 
| `void` | SetData(`JToken` token) |  | 
| `void` | Start() |  | 


## `EscapeAreaObject`

```csharp
public class VirtualBrightPlayz.SCP_ET.Objects.EscapeAreaObject
    : MapObject

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnTriggerEnter(`Collider` collision) |  | 


## `ItemSpawn`

```csharp
public class VirtualBrightPlayz.SCP_ET.Objects.ItemSpawn
    : MapObject, IMapObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | itemid |  | 
| `TextMeshPro` | text |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ObjectId |  | 
| `String` | ObjectName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetData() |  | 
| `void` | JsonToObject(`JToken` json) |  | 
| `Object` | ObjectToJson() |  | 
| `void` | SetData(`JToken` token) |  | 
| `void` | Start() |  | 


## `LightObject`

```csharp
public class VirtualBrightPlayz.SCP_ET.Objects.LightObject
    : MapObject, IMapObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | intensity |  | 
| `String` | LightColor |  | 
| `Single` | range |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | Networkintensity |  | 
| `String` | NetworkLightColor |  | 
| `Single` | Networkrange |  | 
| `String` | ObjectId |  | 
| `String` | ObjectName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `Object` | GetData() |  | 
| `void` | JsonToObject(`JToken` json) |  | 
| `Object` | ObjectToJson() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | SetData(`JToken` token) |  | 
| `void` | Start() |  | 


## `MapPoint`

```csharp
public class VirtualBrightPlayz.SCP_ET.Objects.MapPoint
    : NetworkBehaviour, IMapObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | objName |  | 
| `TextMeshPro` | text |  | 
| `String` | triggerName |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ObjectId |  | 
| `String` | ObjectName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetData() |  | 
| `void` | JsonToObject(`JToken` json) |  | 
| `Object` | ObjectToJson() |  | 
| `void` | SetData(`JToken` token) |  | 
| `void` | Start() |  | 


## `MapTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.Objects.MapTrigger
    : NetworkBehaviour, IMapObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | eventName |  | 
| `String` | objName |  | 
| `TextMeshPro` | text |  | 
| `String` | triggerName |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ObjectId |  | 
| `String` | ObjectName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetData() |  | 
| `void` | JsonToObject(`JToken` json) |  | 
| `Object` | ObjectToJson() |  | 
| `void` | OnTriggerEnter(`Collider` other) |  | 
| `void` | SetData(`JToken` token) |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


## `SkyboxArea`

```csharp
public class VirtualBrightPlayz.SCP_ET.Objects.SkyboxArea
    : MapObject, IMapObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | box |  | 
| `GameObject` | text |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ObjectId |  | 
| `String` | ObjectName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | JsonToObject(`JToken` json) |  | 
| `Object` | ObjectToJson() |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


## `TextureObject`

```csharp
public class VirtualBrightPlayz.SCP_ET.Objects.TextureObject
    : MapObject, IMapObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | HTMLColor |  | 
| `Vector2` | offset |  | 
| `MeshRenderer` | renderer |  | 
| `Vector2` | tiling |  | 
| `String` | weburl |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | NetworkHTMLColor |  | 
| `Vector2` | Networkoffset |  | 
| `Vector2` | Networktiling |  | 
| `String` | Networkweburl |  | 
| `String` | ObjectId |  | 
| `String` | ObjectName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `Object` | GetData() |  | 
| `void` | JsonToObject(`JToken` json) |  | 
| `Object` | ObjectToJson() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | SetData(`JToken` token) |  | 
| `void` | Start() |  | 
| `void` | UpdateMaterial() |  | 


