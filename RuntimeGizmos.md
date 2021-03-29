## `AddTargetCommand`

```csharp
public class RuntimeGizmos.AddTargetCommand
    : SelectCommand, ICommand

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Execute() |  | 
| `void` | UnExecute() |  | 


## `Axis`

```csharp
public enum RuntimeGizmos.Axis
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | None |  | 
| `1` | X |  | 
| `2` | Y |  | 
| `3` | Z |  | 
| `4` | Any |  | 


## `AxisInfo`

```csharp
public struct RuntimeGizmos.AxisInfo

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | pivot |  | 
| `Vector3` | xDirection |  | 
| `Vector3` | yDirection |  | 
| `Vector3` | zDirection |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | GetAxisEnd(`Vector3` direction, `Single` size) |  | 
| `Vector3` | GetXAxisEnd(`Single` size) |  | 
| `Vector3` | GetYAxisEnd(`Single` size) |  | 
| `Vector3` | GetZAxisEnd(`Single` size) |  | 
| `void` | Set(`Transform` target, `Vector3` pivot, `TransformSpace` space) |  | 


## `AxisVectors`

```csharp
public class RuntimeGizmos.AxisVectors

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Vector3>` | all |  | 
| `List<Vector3>` | x |  | 
| `List<Vector3>` | y |  | 
| `List<Vector3>` | z |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Add(`AxisVectors` axisVectors) |  | 
| `void` | Clear() |  | 


## `CenterType`

```csharp
public enum RuntimeGizmos.CenterType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | All |  | 
| `1` | Solo |  | 


## `ClearAndAddTargetCommand`

```csharp
public class RuntimeGizmos.ClearAndAddTargetCommand
    : SelectCommand, ICommand

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Execute() |  | 
| `void` | UnExecute() |  | 


## `ClearTargetsCommand`

```csharp
public class RuntimeGizmos.ClearTargetsCommand
    : SelectCommand, ICommand

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Execute() |  | 
| `void` | UnExecute() |  | 


## `CustomTransformGizmos`

```csharp
public class RuntimeGizmos.CustomTransformGizmos

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | anyAxisGizmo |  | 
| `Transform` | xAxisGizmo |  | 
| `Transform` | yAxisGizmo |  | 
| `Transform` | zAxisGizmo |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Axis` | GetSelectedAxis(`Collider` selectedCollider) |  | 
| `void` | Init(`Int32` layer) |  | 
| `void` | ScaleMultiply(`Vector4` scaleMultiplier) |  | 
| `void` | SetAxis(`AxisInfo` axisInfo) |  | 
| `void` | SetEnable(`Boolean` enable) |  | 
| `void` | SetPosition(`Vector3` position) |  | 


## `ExtMathf`

```csharp
public static class RuntimeGizmos.ExtMathf

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | SafeDivide(`Single` value, `Single` divider) |  | 
| `Single` | Squared(this `Single` value) |  | 


## `ExtTransform`

```csharp
public static class RuntimeGizmos.ExtTransform

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | GetCenter(this `Transform` transform, `CenterType` centerType) |  | 
| `void` | SetScaleFrom(this `Transform` target, `Vector3` worldPivot, `Vector3` newScale) |  | 
| `void` | SetScaleFromOffset(this `Transform` target, `Vector3` worldPivot, `Vector3` newScale) |  | 


## `ExtTransformType`

```csharp
public static class RuntimeGizmos.ExtTransformType

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | TransformTypeContains(this `TransformType` mainType, `TransformType` type, `TransformSpace` space) |  | 


## `ExtVector3`

```csharp
public static class RuntimeGizmos.ExtVector3

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | Abs(this `Vector3` vector) |  | 
| `Boolean` | IsInDirection(`Vector3` direction, `Vector3` otherDirection) |  | 
| `Boolean` | IsParallel(`Vector3` direction, `Vector3` otherDirection, `Single` precision = 0,0001) |  | 
| `Single` | MagnitudeInDirection(`Vector3` vector, `Vector3` direction, `Boolean` normalizeParameters = True) |  | 


## `Geometry`

```csharp
public static class RuntimeGizmos.Geometry

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | ClampToSegment(`Vector3` point, `Vector3` linePoint1, `Vector3` linePoint2) |  | 
| `IntersectPoints` | ClosestPointsOnSegmentToLine(`Vector3` segment0, `Vector3` segment1, `Vector3` linePoint, `Vector3` lineDirection) |  | 
| `IntersectPoints` | ClosestPointsOnTwoLines(`Vector3` point1, `Vector3` point1Direction, `Vector3` point2, `Vector3` point2Direction) |  | 
| `Single` | LinePlaneDistance(`Vector3` linePoint, `Vector3` lineVec, `Vector3` planePoint, `Vector3` planeNormal) |  | 
| `Vector3` | LinePlaneIntersect(`Vector3` linePoint, `Vector3` lineVec, `Vector3` planePoint, `Vector3` planeNormal) |  | 


## `IntersectPoints`

```csharp
public struct RuntimeGizmos.IntersectPoints

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | first |  | 
| `Vector3` | second |  | 


## `RemoveTargetCommand`

```csharp
public class RuntimeGizmos.RemoveTargetCommand
    : SelectCommand, ICommand

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Execute() |  | 
| `void` | UnExecute() |  | 


## `ScaleType`

```csharp
public enum RuntimeGizmos.ScaleType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | FromPoint |  | 
| `1` | FromPointOffset |  | 


## `SelectCommand`

```csharp
public abstract class RuntimeGizmos.SelectCommand
    : ICommand

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Transform` | target |  | 
| `TransformGizmo` | transformGizmo |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Execute() |  | 
| `void` | UnExecute() |  | 


## `Square`

```csharp
public struct RuntimeGizmos.Square

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | bottomLeft |  | 
| `Vector3` | bottomRight |  | 
| `Vector3` | topLeft |  | 
| `Vector3` | topRight |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | Item |  | 


## `TargetInfo`

```csharp
public class RuntimeGizmos.TargetInfo

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | centerPivotPoint |  | 
| `Vector3` | previousPosition |  | 


## `TransformCommand`

```csharp
public class RuntimeGizmos.TransformCommand
    : ICommand

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Execute() |  | 
| `void` | StoreNewTransformValues() |  | 
| `void` | UnExecute() |  | 


## `TransformGizmo`

```csharp
public class RuntimeGizmos.TransformGizmo
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `KeyCode` | ActionKey |  | 
| `KeyCode` | AddSelection |  | 
| `Color` | allColor |  | 
| `Single` | allMoveHandleLengthMultiplier |  | 
| `Single` | allRotateHandleLengthMultiplier |  | 
| `Single` | allRotateSpeedMultiplier |  | 
| `Single` | allScaleHandleLengthMultiplier |  | 
| `Single` | boxSize |  | 
| `CenterType` | centerType |  | 
| `Int32` | circleDetail |  | 
| `Boolean` | circularRotationMethod |  | 
| `Boolean` | forceUpdatePivotPointOnChange |  | 
| `Single` | handleLength |  | 
| `Single` | handleWidth |  | 
| `Color` | hoverColor |  | 
| `Boolean` | manuallyHandleGizmo |  | 
| `Int32` | maxUndoStored |  | 
| `Single` | minSelectedDistanceCheck |  | 
| `Single` | movementSnap |  | 
| `Single` | moveSpeedMultiplier |  | 
| `Axis` | nearAxis |  | 
| `Action` | onCheckForSelectedAxis |  | 
| `Action` | onDrawCustomGizmo |  | 
| `TransformPivot` | pivot |  | 
| `Single` | planeSize |  | 
| `Single` | planesOpacity |  | 
| `KeyCode` | RedoAction |  | 
| `KeyCode` | RemoveSelection |  | 
| `Single` | rotateSpeedMultiplier |  | 
| `Single` | rotationSnap |  | 
| `Single` | scaleSnap |  | 
| `Single` | scaleSpeedMultiplier |  | 
| `ScaleType` | scaleType |  | 
| `Color` | selectedColor |  | 
| `LayerMask` | selectionMask |  | 
| `KeyCode` | SetAllTransformType |  | 
| `KeyCode` | SetCenterTypeToggle |  | 
| `KeyCode` | SetMoveType |  | 
| `KeyCode` | SetPivotModeToggle |  | 
| `KeyCode` | SetRotateType |  | 
| `KeyCode` | SetScaleType |  | 
| `KeyCode` | SetScaleTypeToggle |  | 
| `KeyCode` | SetSpaceToggle |  | 
| `TransformSpace` | space |  | 
| `TransformType` | transformType |  | 
| `KeyCode` | translationSnapping |  | 
| `Single` | triangleSize |  | 
| `KeyCode` | UndoAction |  | 
| `Boolean` | useFirstSelectedAsMain |  | 
| `Color` | xColor |  | 
| `Color` | yColor |  | 
| `Color` | zColor |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | hasTranslatingAxisPlane |  | 
| `Boolean` | isTransforming |  | 
| `Transform` | mainTargetRoot |  | 
| `Camera` | myCamera |  | 
| `Vector3` | pivotPoint |  | 
| `Quaternion` | totalRotationAmount |  | 
| `Single` | totalScaleAmount |  | 
| `TransformType` | transformingType |  | 
| `Axis` | translatingAxis |  | 
| `Axis` | translatingAxisPlane |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddTarget(`Transform` target, `Boolean` addCommand = True) |  | 
| `void` | ClearTargets(`Boolean` addCommand = True) |  | 
| `AxisInfo` | GetAxisInfo() |  | 
| `Single` | GetDistanceMultiplier() |  | 
| `Single` | GetHandleLength(`TransformType` type, `Axis` axis = None, `Boolean` multiplyDistanceMultiplier = True) |  | 
| `TransformSpace` | GetProperTransformSpace() |  | 
| `void` | RemoveTarget(`Transform` target, `Boolean` addCommand = True) |  | 
| `void` | SetPivotPoint() |  | 
| `void` | SetTranslatingAxis(`TransformType` type, `Axis` axis, `Axis` planeAxis = None) |  | 
| `Boolean` | TransformTypeContains(`TransformType` type) |  | 
| `Boolean` | TransformTypeContains(`TransformType` mainType, `TransformType` type) |  | 
| `Boolean` | TranslatingTypeContains(`TransformType` type, `Boolean` checkIsTransforming = True) |  | 


## `TransformGizmoCustomGizmo`

```csharp
public class RuntimeGizmos.TransformGizmoCustomGizmo
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | autoFindTransformGizmo |  | 
| `CustomTransformGizmos` | customRotationGizmos |  | 
| `CustomTransformGizmos` | customScaleGizmos |  | 
| `CustomTransformGizmos` | customTranslationGizmos |  | 
| `Int32` | gizmoLayer |  | 
| `Boolean` | scaleBasedOnDistance |  | 
| `Single` | scaleMultiplier |  | 
| `TransformGizmo` | transformGizmo |  | 


## `TransformPivot`

```csharp
public enum RuntimeGizmos.TransformPivot
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Pivot |  | 
| `1` | Center |  | 


## `TransformSpace`

```csharp
public enum RuntimeGizmos.TransformSpace
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Global |  | 
| `1` | Local |  | 


## `TransformType`

```csharp
public enum RuntimeGizmos.TransformType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Move |  | 
| `1` | Rotate |  | 
| `2` | Scale |  | 
| `3` | All |  | 


