## `SCP012Control`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_012.SCP012Control
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | closePos |  | 
| `AnimationCurve` | curve |  | 
| `Boolean` | isPaperDown |  | 
| `GameObject` | killTrigger |  | 
| `GameObject` | modelPos |  | 
| `GameObject` | openPos |  | 
| `Single` | progress |  | 
| `Single` | speed |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | NetworkisPaperDown |  | 
| `Single` | Networkspeed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `IEnumerator` | ToggleLate(`Boolean` value) |  | 


## `SCP012HoistButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_012.SCP012HoistButton
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `SCP012Control` | control |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Highlighted() |  | 
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `SCP012Trigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.SCP_012.SCP012Trigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | center |  | 
| `SCP012Control` | control |  | 
| `Single` | lookSpeed |  | 
| `SCP012TriggerMode` | mode |  | 
| `Single` | moveoverrideLerp |  | 
| `Single` | speed |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Start() |  | 


