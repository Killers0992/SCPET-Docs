## `PlayerInputControls`

```csharp
public class InputActions.PlayerInputControls
    : IInputActionCollection, IEnumerable<InputAction>, IEnumerable, IDisposable

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `InputActionAsset` | asset |  | 
| `Nullable<InputBinding>` | bindingMask |  | 
| `ReadOnlyArray<InputControlScheme>` | controlSchemes |  | 
| `Nullable<ReadOnlyArray<InputDevice>>` | devices |  | 
| `EditorActions` | Editor |  | 
| `InputControlScheme` | GamepadScheme |  | 
| `GUIActions` | GUI |  | 
| `InputControlScheme` | PCScheme |  | 
| `InputControlScheme` | VRScheme |  | 
| `WorldActions` | World |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Contains(`InputAction` action) |  | 
| `void` | Disable() |  | 
| `void` | Dispose() |  | 
| `void` | Enable() |  | 
| `IEnumerator<InputAction>` | GetEnumerator() |  | 


