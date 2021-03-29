## `FSMAI`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMAI
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `FSMGraph` | cloneGraph |  | 
| `FSMNode` | current |  | 
| `FSMGraph` | Graph |  | 
| `MonoBehaviour` | script |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | LoadState(`String` to) |  | 
| `void` | SetState(`FSMNode` to) |  | 


## `FSMCheck`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMCheck
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean[]` | Conditions |  | 
| `FSMNode` | enter |  | 
| `FSMNode` | exit |  | 
| `Boolean` | ExitIf |  | 
| `Boolean` | requireAll |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetValue(`NodePort` port) |  | 
| `void` | OnFixedUpdate(`FSMAI` ai) |  | 


## `FSMCheckPhysicsIHuman`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMCheckPhysicsIHuman
    : FSMCheck

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | mask |  | 
| `Single` | radius |  | 
| `Transform` | xform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMAI` ai) |  | 


## `FSMFloatOperator`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMFloatOperator
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | check |  | 
| `Single` | input |  | 
| `CompareMethod` | method |  | 
| `Boolean` | passedCheck |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetValue(`NodePort` port) |  | 


## `FSMGetBoolValue`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGetBoolValue
    : FSMGetValue

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetValue(`NodePort` port) |  | 
| `void` | OnFixedUpdate() |  | 


## `FSMGetComponentValue`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGetComponentValue
    : FSMGetOtherValue

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Component` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Component` | GetInterface(`Component[]` arr, `Type` t) |  | 
| `Object` | GetValue(`NodePort` port) |  | 
| `void` | OnFixedUpdate() |  | 


## `FSMGetFloatValue`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGetFloatValue
    : FSMGetValue

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetValue(`NodePort` port) |  | 
| `void` | OnFixedUpdate() |  | 


## `FSMGetNullValue`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGetNullValue
    : FSMGetValue

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetValue(`NodePort` port) |  | 
| `void` | OnFixedUpdate() |  | 


## `FSMGetObjectValue`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGetObjectValue
    : FSMGetValue

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetValue(`NodePort` port) |  | 
| `void` | OnFixedUpdate() |  | 


## `FSMGetOtherNullValue`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGetOtherNullValue
    : FSMGetOtherValue

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | value |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetValue(`NodePort` port) |  | 
| `void` | OnFixedUpdate() |  | 


## `FSMGetOtherValue`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGetOtherValue
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | behaviour |  | 
| `String` | field |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate() |  | 


## `FSMGetThisValue`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGetThisValue
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MonoBehaviour` | behaviour |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetValue(`NodePort` port) |  | 


## `FSMGetValue`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGetValue
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MonoBehaviour` | behaviour |  | 
| `String` | field |  | 
| `FieldInfo` | info |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate() |  | 


## `FSMGraph`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMGraph
    : NodeGraph

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MonoBehaviour` | behaviour |  | 
| `FSMNode` | entry |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ExitTo(`String` to) |  | 
| `void` | OnFixedUpdate() |  | 
| `void` | OnStart() |  | 


## `FSMManager`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `FSMState` | _current |  | 
| `IEntity` | attachedEntity |  | 
| `String` | FSMStartName |  | 
| `Object` | stateData |  | 
| `FSMState[]` | states |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | LoadState(`String` statename) |  | 
| `void` | SetState(`FSMState` state) |  | 
| `void` | SetState(`String` statename) |  | 


## `FSMNode`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMNode
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `FSMAI` | AI |  | 
| `FSMNode[]` | inputs |  | 
| `FSMNode` | node |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `FSMGraph` | FSM |  | 
| `GameObject` | gameObject |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Enter() |  | 
| `Object` | GetValue(`NodePort` port) |  | 
| `void` | OnEnterState() |  | 
| `void` | OnExitState() |  | 
| `void` | OnFixedUpdate() |  | 
| `void` | SetAsEntry() |  | 


## `FSMNotOperator`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMNotOperator
    : Node

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | input |  | 
| `Boolean` | output |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Object` | GetValue(`NodePort` port) |  | 


## `FSMState`

```csharp
public class VirtualBrightPlayz.SCP_ET.AI_FSM.FSMState
    : ScriptableObject

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | FSMName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateDisable(`FSMManager` manager, `FSMState` newstate) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


