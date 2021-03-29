## `Class`

```csharp
public interface VirtualBrightPlayz.SCP_ET.Player.Classes.Class

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | classColor |  | 
| `Int32` | classId |  | 
| `String` | className |  | 
| `Single` | crouchSpeed |  | 
| `ItemBase[]` | defaultItems |  | 
| `GameObject` | DefaultModelPrefab |  | 
| `Single` | hp |  | 
| `Single` | maxHp |  | 
| `Single` | sprintSpeed |  | 
| `Single` | walkSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Shoot(`PlayerController` ctrl) |  | 


## `ClassD`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Classes.ClassD
    : Class

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | classColor |  | 
| `Int32` | classId |  | 
| `String` | className |  | 
| `Single` | crouchSpeed |  | 
| `ItemBase[]` | defaultItems |  | 
| `GameObject` | DefaultModelPrefab |  | 
| `Single` | hp |  | 
| `Single` | maxHp |  | 
| `Single` | sprintSpeed |  | 
| `Single` | walkSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Shoot(`PlayerController` ctrl) |  | 


## `ClassDPrefab`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Classes.ClassDPrefab
    : MonoBehaviour, ClassPrefab

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | _face |  | 
| `GameObject` | _hand |  | 
| `GameObject` | _head |  | 
| `Renderer` | _render |  | 
| `AnimationClip` | cIdle |  | 
| `AnimationClip` | cWalk |  | 
| `AnimationMixerPlayable` | duckIdleMixer |  | 
| `AnimationMixerPlayable` | duckMoveMixer |  | 
| `PlayableGraph` | graph |  | 
| `AnimationClip` | idle |  | 
| `AnimationMixerPlayable` | idleMixer |  | 
| `AnimationClip` | itemHold |  | 
| `AnimationMixerPlayable` | moveMixer |  | 
| `AnimationMixerPlayable` | rootMixer |  | 
| `AnimationClip` | sprint |  | 
| `AnimationClip` | walk |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Animator` | Animation |  | 
| `AnimationControl` | Control |  | 
| `GameObject` | Face |  | 
| `GameObject` | Hand |  | 
| `GameObject` | Head |  | 
| `Renderer` | Renderer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnDestroy() |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


## `ClassPrefab`

```csharp
public interface VirtualBrightPlayz.SCP_ET.Player.Classes.ClassPrefab

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Animator` | Animation |  | 
| `AnimationControl` | Control |  | 
| `GameObject` | Face |  | 
| `GameObject` | Hand |  | 
| `GameObject` | Head |  | 
| `Renderer` | Renderer |  | 


## `GenericPrefab`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Classes.GenericPrefab
    : MonoBehaviour, ClassPrefab

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | _face |  | 
| `GameObject` | _hand |  | 
| `GameObject` | _head |  | 
| `Renderer` | _render |  | 
| `AnimationClip` | cIdle |  | 
| `AnimationClip` | cWalk |  | 
| `AnimationMixerPlayable` | duckIdleMixer |  | 
| `AnimationMixerPlayable` | duckMoveMixer |  | 
| `PlayableGraph` | graph |  | 
| `AnimationClip` | idle |  | 
| `AnimationMixerPlayable` | idleMixer |  | 
| `AnimationMixerPlayable` | moveMixer |  | 
| `AnimationMixerPlayable` | rootMixer |  | 
| `AnimationClip` | sprint |  | 
| `AnimationClip` | walk |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Animator` | Animation |  | 
| `AnimationControl` | Control |  | 
| `GameObject` | Face |  | 
| `GameObject` | Hand |  | 
| `GameObject` | Head |  | 
| `Renderer` | Renderer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Awake() |  | 
| `void` | OnDestroy() |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


## `Guard`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Classes.Guard
    : Class

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | classColor |  | 
| `Int32` | classId |  | 
| `String` | className |  | 
| `Single` | crouchSpeed |  | 
| `ItemBase[]` | defaultItems |  | 
| `GameObject` | DefaultModelPrefab |  | 
| `Single` | hp |  | 
| `Single` | maxHp |  | 
| `Single` | sprintSpeed |  | 
| `Single` | walkSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Shoot(`PlayerController` ctrl) |  | 


## `Spectator`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Classes.Spectator
    : Class

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | classColor |  | 
| `Int32` | classId |  | 
| `String` | className |  | 
| `Single` | crouchSpeed |  | 
| `ItemBase[]` | defaultItems |  | 
| `GameObject` | DefaultModelPrefab |  | 
| `Single` | hp |  | 
| `Single` | maxHp |  | 
| `Single` | sprintSpeed |  | 
| `Single` | walkSpeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Shoot(`PlayerController` ctrl) |  | 


