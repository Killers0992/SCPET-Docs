## `GenMapButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapEditor_20.GenMapButton
    : IMapEditorObject, IMapObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GenMapSeed` | seedstuff |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | gameObject |  | 
| `String` | ObjectId |  | 
| `String` | ObjectName |  | 
| `Transform` | transform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Deselected() |  | 
| `void` | JsonToObject(`JToken` json) |  | 
| `Object` | ObjectToJson() |  | 


## `IMapEditorObject`

```csharp
public interface VirtualBrightPlayz.SCP_ET.MapEditor_20.IMapEditorObject
    : IMapObject

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Deselected() |  | 


## `MapEditor2`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapEditor_20.MapEditor2
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<MapEdit>` | actions |  | 
| `Camera` | cam |  | 
| `Single` | camSpeed |  | 
| `GameObject` | DS_contentObj |  | 
| `GameObject` | DS_defButton |  | 
| `GenMapButton` | genMapButtonObj |  | 
| `TransformGizmo` | gizmo |  | 
| `Boolean` | isViewing |  | 
| `List<GameObject>` | mapObjects |  | 
| `GameObject` | OS_contentObj |  | 
| `GameObject` | OS_defButton |  | 
| `GameObject` | OS_scrollBox |  | 
| `GameObject` | PD_content |  | 
| `GameObject` | PD_floatField |  | 
| `GameObject` | PD_intField |  | 
| `GameObject` | PD_stringField |  | 
| `GameObject` | PD_templates |  | 
| `TMP_Dropdown` | PD_type |  | 
| `GameObject` | PD_vector3Field |  | 
| `IMapEditorObject` | prevEditorObject |  | 
| `RotateTool` | rotateTool |  | 
| `GameObject` | RS_contentObj |  | 
| `GameObject` | RS_defButton |  | 
| `GameObject` | RS_scrollBox |  | 
| `ScaleTool` | scaleTool |  | 
| `List<GameObject>` | selected |  | 
| `LayerMask` | selectMask |  | 
| `TranslateTool` | translateTool |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckInput() |  | 
| `void` | ClearMap() |  | 
| `void` | DeleteRoom(`GameObject` go) |  | 
| `void` | DisableGUI() |  | 
| `void` | DoorGUI() |  | 
| `void` | ExitEditor() |  | 
| `void` | Load(`String` path, `Boolean` relative) |  | 
| `void` | LoadUI() |  | 
| `void` | MapSeedGUI() |  | 
| `void` | ObjectGUI() |  | 
| `void` | PropertyGUI(`IMapObject` mapObject) |  | 
| `void` | RoomGUI() |  | 
| `void` | RotateRoom(`GameObject` go) |  | 
| `void` | RotateTool() |  | 
| `void` | Save(`String` path, `Boolean` relative) |  | 
| `void` | SaveUI() |  | 
| `void` | ScaleTool() |  | 
| `GameObject` | SpawnObject(`String` guid) |  | 
| `GameObject` | SpawnRoom(`String` guid) |  | 
| `void` | Start() |  | 
| `void` | TransformGUI(`GameObject` obj) |  | 
| `void` | TranslateTool() |  | 
| `void` | Undo() |  | 
| `void` | Update() |  | 
| `void` | Viewing() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MapEditor2` | editor |  | 


## `MapEditor2Field`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapEditor_20.MapEditor2Field
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `TMP_InputField[]` | fields |  | 
| `TextMeshProUGUI` | label |  | 
| `UnityEvent` | onEdited |  | 
| `MapFieldType` | type |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | Read() |  | 
| `void` | Write(`Object` obj) |  | 


## `RotateTool`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapEditor_20.RotateTool
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MapEditor2` | editor |  | 
| `GameObject` | tempGameObject |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | GetAxis(`Vector3` obj, `Vector3` point) |  | 
| `void` | Update() |  | 


## `ScaleTool`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapEditor_20.ScaleTool
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MapEditor2` | editor |  | 
| `GameObject` | tempGameObject |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | GetAxis(`Vector3` obj, `Vector3` point) |  | 
| `void` | Update() |  | 


## `TranslateTool`

```csharp
public class VirtualBrightPlayz.SCP_ET.MapEditor_20.TranslateTool
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MapEditor2` | editor |  | 
| `GameObject` | tempGameObject |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | GetAxis(`Vector3` obj, `Vector3` point) |  | 
| `void` | Update() |  | 


