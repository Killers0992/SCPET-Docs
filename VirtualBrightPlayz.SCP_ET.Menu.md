## `SettingsPanelGen`

```csharp
public class VirtualBrightPlayz.SCP_ET.Menu.SettingsPanelGen
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | content |  | 
| `GameObject` | genericButton |  | 
| `GameObject` | genericCheckbox |  | 
| `GameObject` | genericDropdown |  | 
| `GameObject` | genericHeader |  | 
| `GameObject` | genericSlider |  | 
| `GameObject` | genericTextField |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | AddButton(`String` text, `String` btntext, `Action` callback) |  | 
| `GameObject` | AddCheckbox(`String` text, `String` setting) |  | 
| `GameObject` | AddHeader(`String` text) |  | 
| `GameObject` | AddSlider(`String` text, `String` setting, `Single` min = 0, `Single` max = 1, `Boolean` whole = False) |  | 
| `GameObject` | AddTextField(`String` text, `String` setting) |  | 
| `void` | ClearPage() |  | 
| `void` | GenPage() |  | 
| `T` | GetSettings(`String` setting) |  | 
| `void` | Save() |  | 
| `void` | Start() |  | 
| `void` | UpdateSettings(`String` setting, `Object` data) |  | 


