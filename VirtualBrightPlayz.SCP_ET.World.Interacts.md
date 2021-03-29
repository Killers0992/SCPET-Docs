## `ButtonSpawn`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.ButtonSpawn
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Access |  | 
| `Boolean` | applyScale |  | 
| `Boolean` | autoSpawn |  | 
| `Int32` | level |  | 
| `NetworkIdentity` | parent |  | 
| `GameObject` | prefab |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Spawn() |  | 


## `ButtonText`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.ButtonText
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Door[]` | doors |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | open |  | 
| `Outline` | outline |  | 
| `TMP_Text` | text |  | 


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
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `DoorButton2`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.DoorButton2
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Door[]` | doors |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | open |  | 
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
| `void` | StartUse(`PlayerController` user, `Boolean` isLocal) |  | 
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `void` | StopUse(`String&` status, `ButtonErrorType&` errorType) |  | 


## `IInteractable`

```csharp
public interface VirtualBrightPlayz.SCP_ET.World.Interacts.IInteractable

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `GameObject` | gameObject |  | 
| `InteractType` | IType |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Highlighted() |  | 
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `ILever`

```csharp
public interface VirtualBrightPlayz.SCP_ET.World.Interacts.ILever
    : IInteractable

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | UpdateLook(`PlayerController` user, `Vector2` look) |  | 


## `Interact`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.Interact
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Door[]` | doors |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | open |  | 
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
| `void` | StartUse(`PlayerController` user, `Boolean` isLocal) |  | 
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `void` | StopUse(`String&` status, `ButtonErrorType&` errorType) |  | 


## `InteractList`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.InteractList
    : NetworkBehaviour

```

## `InteractListChild`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.InteractListChild
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `NetworkIdentity` | parent |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | id |  | 


## `InteractParentSync`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.InteractParentSync
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `NetworkIdentitySyncvar` | parentObject |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `NetworkIdentity` | NetworkparentObject |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 


## `InteractType`

```csharp
public enum VirtualBrightPlayz.SCP_ET.World.Interacts.InteractType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Button |  | 
| `1` | Lever |  | 
| `2` | Hold |  | 


## `KeycardButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.KeycardButton
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Door[]` | doors |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | open |  | 
| `Outline` | outline |  | 
| `Int32` | ReqLevel |  | 


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
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `KeycardButtonText`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.KeycardButtonText
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Access |  | 
| `Collider` | basecollider |  | 
| `Door[]` | doors |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | open |  | 
| `Outline` | outline |  | 
| `Int32` | ReqLevel |  | 
| `TMP_Text` | text |  | 


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
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `KeycardIDButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.KeycardIDButton
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Access |  | 
| `Collider` | basecollider |  | 
| `Door[]` | doors |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | open |  | 
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
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `KeycardIDLvlButton`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.KeycardIDLvlButton
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Access |  | 
| `Collider` | basecollider |  | 
| `Door[]` | doors |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | open |  | 
| `Outline` | outline |  | 
| `Int32` | ReqLevel |  | 


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
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `LightSwitch`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.LightSwitch
    : NetworkBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | isOn |  | 
| `Light[]` | lights |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `InteractType` | IType |  | 
| `Boolean` | NetworkisOn |  | 
| `Boolean` | NoCooldown |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Highlighted() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | StartUseOnce(`PlayerController` plr, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 


## `PizzaSlice`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Interacts.PizzaSlice
    : MonoBehaviour, IInteractable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | box |  | 
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


