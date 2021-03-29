## `CompCache`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.Interfaces.CompCache
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | attackMask |  | 
| `List<IHuman>` | human |  | 
| `Boolean` | isRunning |  | 
| `Single` | maxRefreshTimer |  | 
| `Single` | refreshTimer |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CompCache` | cache |  | 


## `DimensionType`

```csharp
public enum VirtualBrightPlayz.SCP_ET.NPCs.Interfaces.DimensionType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | World |  | 
| `1` | Scp1499 |  | 
| `2` | Pocket |  | 
| `3` | Scp1123 |  | 
| `4` | Scp860 |  | 


## `ICanTakeDamage`

```csharp
public interface VirtualBrightPlayz.SCP_ET.NPCs.Interfaces.ICanTakeDamage
    : IEntity

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | godMode |  | 
| `Boolean` | isValidTarget |  | 
| `Transform` | transform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Kill(`DeathTypes` type, `GameObject` go) |  | 
| `void` | TakeDamage(`Single` amnt, `GameObject` go, `DeathTypes` type) |  | 


## `ICanTakeDamageNoStats`

```csharp
public interface VirtualBrightPlayz.SCP_ET.NPCs.Interfaces.ICanTakeDamageNoStats
    : IEntity

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Kill(`DeathTypes` type, `GameObject` go) |  | 
| `void` | TakeDamage(`Single` amnt, `GameObject` go, `DeathTypes` type) |  | 


## `ICanTriggerTesla`

```csharp
public interface VirtualBrightPlayz.SCP_ET.NPCs.Interfaces.ICanTriggerTesla
    : ICanTakeDamage, IEntity

```

## `IElevatorTeleport`

```csharp
public interface VirtualBrightPlayz.SCP_ET.NPCs.Interfaces.IElevatorTeleport

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | gameObject |  | 
| `Boolean` | isTeleporting |  | 
| `Vector3` | newPosition |  | 


## `IEntity`

```csharp
public interface VirtualBrightPlayz.SCP_ET.NPCs.Interfaces.IEntity

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `DimensionType` | CurrentDimension |  | 
| `GameObject` | gameObject |  | 


## `IHuman`

```csharp
public interface VirtualBrightPlayz.SCP_ET.NPCs.Interfaces.IHuman
    : ICanTakeDamage, IEntity

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | HasRing |  | 
| `Boolean` | IsBlinking |  | 
| `Single` | IsMakingSound |  | 
| `GameObject` | rot |  | 


## `ISCP`

```csharp
public interface VirtualBrightPlayz.SCP_ET.NPCs.Interfaces.ISCP
    : IEntity

```

