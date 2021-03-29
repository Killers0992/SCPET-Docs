## `PhysicsVolumeComponent`

```csharp
public class Sabresaurus.SabreCSG.Volumes.PhysicsVolumeComponent
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | filterTag |  | 
| `Vector3` | force |  | 
| `PhysicsVolumeForceMode` | forceMode |  | 
| `PhysicsVolumeForceSpace` | forceSpace |  | 
| `PhysicsVolumeGravityMode` | gravity |  | 
| `LayerMask` | layer |  | 
| `Vector3` | relativeForce |  | 
| `PhysicsVolumeForceMode` | relativeForceMode |  | 
| `PhysicsVolumeForceSpace` | relativeForceSpace |  | 
| `Vector3` | relativeTorque |  | 
| `PhysicsVolumeForceMode` | relativeTorqueForceMode |  | 
| `PhysicsVolumeForceSpace` | relativeTorqueSpace |  | 
| `Vector3` | torque |  | 
| `PhysicsVolumeForceMode` | torqueForceMode |  | 
| `PhysicsVolumeForceSpace` | torqueSpace |  | 
| `Boolean` | useFilterTag |  | 


## `PhysicsVolumeForceMode`

```csharp
public enum Sabresaurus.SabreCSG.Volumes.PhysicsVolumeForceMode
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | None |  | 
| `1` | Force |  | 
| `2` | Impulse |  | 
| `3` | VelocityChange |  | 
| `4` | Acceleration |  | 


## `PhysicsVolumeForceSpace`

```csharp
public enum Sabresaurus.SabreCSG.Volumes.PhysicsVolumeForceSpace
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Relative |  | 
| `1` | World |  | 


## `PhysicsVolumeGravityMode`

```csharp
public enum Sabresaurus.SabreCSG.Volumes.PhysicsVolumeGravityMode
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | None |  | 
| `1` | Enable |  | 
| `2` | Disable |  | 
| `3` | ZeroGravity |  | 
| `4` | ZeroGravityRestore |  | 


## `TriggerVolumeComponent`

```csharp
public class Sabresaurus.SabreCSG.Volumes.TriggerVolumeComponent
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | filterTag |  | 
| `LayerMask` | layer |  | 
| `TriggerVolumeEvent` | onEnterEvent |  | 
| `TriggerVolumeEvent` | onExitEvent |  | 
| `TriggerVolumeEvent` | onStayEvent |  | 
| `Boolean` | triggerOnceOnly |  | 
| `TriggerVolumeTriggerType` | triggerType |  | 
| `Boolean` | useFilterTag |  | 


## `TriggerVolumeEvent`

```csharp
public class Sabresaurus.SabreCSG.Volumes.TriggerVolumeEvent
    : UnityEvent, ISerializationCallbackReceiver

```

## `TriggerVolumeTriggerType`

```csharp
public enum Sabresaurus.SabreCSG.Volumes.TriggerVolumeTriggerType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | UnityEvent |  | 


