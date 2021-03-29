## `ColorHex`

```csharp
public struct Sabresaurus.SabreCSG.ColorHex

```

## `CSGModelRuntime`

```csharp
public class Sabresaurus.SabreCSG.CSGModelRuntime
    : MonoBehaviour

```

## `EnumHelper`

```csharp
public static class Sabresaurus.SabreCSG.EnumHelper

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsFlagSet(`Enum` candidate, `Enum` test) |  | 


## `ExpandPropertiesAttribute`

```csharp
public class Sabresaurus.SabreCSG.ExpandPropertiesAttribute
    : PropertyAttribute, _Attribute

```

## `Extensions`

```csharp
public static class Sabresaurus.SabreCSG.Extensions

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | Abs(this `Vector3` a) |  | 
| `Transform` | AddChild(this `Transform` parentTransform, `String` name) |  | 
| `T` | AddOrGetComponent(this `MonoBehaviour` behaviour) |  | 
| `T` | AddOrGetComponent(this `GameObject` gameObject) |  | 
| `Boolean` | Contains(this `Bounds` bounds1, `Bounds` bounds2) |  | 
| `Boolean` | Contains(this `LayerMask` layerMask, `Int32` layer) |  | 
| `Boolean` | ContainsApproximate(this `Bounds` bounds1, `Vector3` point) |  | 
| `Boolean` | ContainsWithin(this `Bounds` bounds1, `Bounds` bounds2) |  | 
| `Boolean` | ContentsEquals(this `T[]` array1, `T[]` array2) |  | 
| `Boolean` | ContentsEquals(this `List<T>` list1, `List<T>` list2) |  | 
| `void` | DestroyChildrenImmediate(this `Transform` parentTransform) |  | 
| `Vector3` | Divide(this `Vector3` a, `Vector3` b) |  | 
| `Vector2` | Divide(this `Vector2` a, `Vector2` b) |  | 
| `Boolean` | Equals(this `Color32` color, `Color32` other) |  | 
| `Boolean` | EqualsWithEpsilon(this `Single` a, `Single` b) |  | 
| `Boolean` | EqualsWithEpsilon(this `Vector3` a, `Vector3` b) |  | 
| `Boolean` | EqualsWithEpsilonLower(this `Vector3` a, `Vector3` b) |  | 
| `Boolean` | EqualsWithEpsilonLower3(this `Vector3` a, `Vector3` b) |  | 
| `Rect` | ExpandFromCenter(this `Rect` rect, `Vector2` expansion) |  | 
| `void` | ForceRefreshSharedMesh(this `MeshCollider` meshCollider) |  | 
| `void` | ForceRefreshSharedMesh(this `MeshFilter` meshFilter) |  | 
| `Single` | GetLargestExtent(this `Bounds` bounds) |  | 
| `Int32` | GetSetAxisCount(this `Vector3` vector) |  | 
| `Single` | GetSmallestExtent(this `Bounds` bounds) |  | 
| `Int32[]` | GetTrianglesSafe(this `Mesh` mesh) |  | 
| `Boolean` | HasComponent(this `MonoBehaviour` behaviour) |  | 
| `Boolean` | HasComponent(this `GameObject` gameObject) |  | 
| `Boolean` | IntersectsApproximate(this `Bounds` bounds1, `Bounds` bounds2) |  | 
| `Boolean` | IsParentOf(this `Transform` thisTransform, `Transform` otherTransform) |  | 
| `Vector3` | Multiply(this `Vector3` a, `Vector3` b) |  | 
| `Vector2` | Multiply(this `Vector2` a, `Vector2` b) |  | 
| `Boolean` | NotEquals(this `Color32` color, `Color32` other) |  | 
| `Vector2` | Rotate(this `Vector2` vector, `Single` angle) |  | 
| `Vector3` | SetAxis(this `Vector3` vector, `Int32` axis, `Single` newValue) |  | 
| `String` | ToGeneratedHierarchyString(this `Bounds` bounds) |  | 
| `String` | ToStringLong(this `Vector3` source) |  | 
| `String` | ToStringLong(this `Plane` source) |  | 
| `String` | ToStringWithSuffix(this `Int32` number, `String` suffixSingular, `String` suffixPlural) |  | 


## `MathHelper`

```csharp
public static class Sabresaurus.SabreCSG.MathHelper

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | ClosestPointOnLine(`Ray` ray, `Vector3` lineStart, `Vector3` lineEnd) |  | 
| `Vector3` | ClosestPointOnPlane(`Vector3` point, `Plane` plane) |  | 
| `Boolean` | ClosestPointsOnTwoLines(`Vector3&` closestPointLine1, `Vector3&` closestPointLine2, `Vector3` linePoint1, `Vector3` lineVec1, `Vector3` linePoint2, `Vector3` lineVec2) |  | 
| `Single` | DistanceToRay(`Vector3` X0, `Ray` ray) |  | 
| `Int32` | GetSideThick(`Plane` plane, `Vector3` point) |  | 
| `Single` | InverseLerpNoClamp(`Single` from, `Single` to, `Single` value) |  | 
| `Boolean` | IsVectorInteger(`Vector3` vector) |  | 
| `Boolean` | IsVectorOnGrid(`Vector3` position, `Vector3` mask, `Single` gridScale) |  | 
| `Boolean` | PlaneEquals(`Plane` plane1, `Plane` plane2) |  | 
| `Boolean` | PlaneEqualsLooser(`Plane` plane1, `Plane` plane2) |  | 
| `Boolean` | PlaneEqualsLooserWithFlip(`Plane` plane1, `Plane` plane2) |  | 
| `Int32` | PointOnWhichSideOfLineSegment(`Vector3` linePoint1, `Vector3` linePoint2, `Vector3` point) |  | 
| `Vector3` | ProjectPointOnLine(`Vector3` linePoint, `Vector3` lineVec, `Vector3` point) |  | 
| `Vector3` | ProjectPointOnLineSegment(`Vector3` linePoint1, `Vector3` linePoint2, `Vector3` point) |  | 
| `Single` | RoundFloat(`Single` value, `Single` gridScale) |  | 
| `Vector2` | RoundVector2(`Vector3` vector) |  | 
| `Vector2` | RoundVector2(`Vector2` vector, `Single` gridScale) |  | 
| `Vector3` | RoundVector3(`Vector3` vector) |  | 
| `Vector3` | RoundVector3(`Vector3` vector, `Single` gridScale) |  | 
| `Vector2` | Vector2Cross(`Vector2` vector) |  | 
| `Vector3` | VectorAbs(`Vector3` vector) |  | 
| `Vector3` | VectorInDirection(`Vector3` sourceVector, `Vector3` direction) |  | 
| `Int32` | Wrap(`Int32` i, `Int32` range) |  | 
| `Single` | Wrap(`Single` i, `Single` range) |  | 
| `Single` | WrapAngle(`Single` angle) |  | 


## `SerializablePlane`

```csharp
public struct Sabresaurus.SabreCSG.SerializablePlane

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | Distance |  | 
| `Vector3` | Normal |  | 
| `Plane` | UnityPlane |  | 


## `StringHelper`

```csharp
public static class Sabresaurus.SabreCSG.StringHelper

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ParseDisplayString(`String` input) |  | 
| `Boolean` | TryParseScale(`String` inputString, `Vector3&` outputScale) |  | 
| `Boolean` | TryParseScale(`String` inputString, `Vector2&` outputScale) |  | 


## `TransformData`

```csharp
public class Sabresaurus.SabreCSG.TransformData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | LocalPosition |  | 
| `Quaternion` | LocalRotation |  | 
| `Vector3` | LocalScale |  | 
| `Transform` | Parent |  | 
| `Int32` | SiblingIndex |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | SetFromTransform(`Transform` sourceTransform, `Boolean` ignoreSiblingChange = False) |  | 


## `WorldTransformData`

```csharp
public class Sabresaurus.SabreCSG.WorldTransformData

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector3` | LossyScale |  | 
| `Transform` | Parent |  | 
| `Vector3` | Position |  | 
| `Quaternion` | Rotation |  | 
| `Int32` | SiblingIndex |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | SetFromTransform(`Transform` sourceTransform, `Boolean` ignoreSiblingChange = False) |  | 


