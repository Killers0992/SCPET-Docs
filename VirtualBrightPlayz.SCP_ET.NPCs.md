## `ClassDBackAway`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.ClassDBackAway
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | maxDistance |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `ClassDFollow`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.ClassDFollow
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | maxDistance |  | 
| `Single` | minDistance |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `ClassDIdle`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.ClassDIdle
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | timeToIdle |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `ClassDWander`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.ClassDWander
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | maxWanderDistance |  | 
| `Single` | timeToWander |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `FSMMovementNPCBase`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.FSMMovementNPCBase
    : NetworkBehaviour, IElevatorTeleport, ISavable, IEntity

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `NavMeshAgent` | agent |  | 
| `FSMManager` | ai2 |  | 
| `Boolean` | autoNullDimensionChange |  | 
| `Boolean` | autoNullPlr |  | 
| `Boolean` | bigPath |  | 
| `Single` | boxsize |  | 
| `CharacterController` | ctrl |  | 
| `Single` | distFromGrid |  | 
| `Single` | gravity |  | 
| `Single` | gravMulti |  | 
| `Single` | gridSize |  | 
| `Boolean` | hasPath |  | 
| `Boolean` | isteleport |  | 
| `Single` | maxTrackingDist |  | 
| `Single` | minDist |  | 
| `NPCData` | npcData |  | 
| `NavMeshPath` | path |  | 
| `Vector3[]` | path2 |  | 
| `Single` | path2Timer |  | 
| `Single` | pathCount |  | 
| `GameObject` | plr |  | 
| `Vector3` | prevRoom |  | 
| `Single` | rotateSpeed |  | 
| `String` | savePlrGuid |  | 
| `String[]` | saveTargets |  | 
| `Single` | speed |  | 
| `List<GameObject>` | targets |  | 
| `Vector3` | wanderPos |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | activeTarget |  | 
| `DimensionType` | CurrentDimension |  | 
| `IReadOnlyList<GameObject>` | currentTargets |  | 
| `String` | Guid |  | 
| `Boolean` | isTeleporting |  | 
| `Vector3` | newPosition |  | 
| `String` | PrefabGuid |  | 
| `JSONVector` | savePos |  | 
| `JSONVector` | saveRot |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddTarget(`GameObject` target) |  | 
| `void` | CheckForNav() |  | 
| `void` | ClearTargets() |  | 
| `void` | FollowPlayer(`FSMNode` animator) |  | 
| `void` | GetPath() |  | 
| `void` | IdleMove(`FSMNode` animator) |  | 
| `void` | LoadComplete() |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | RemoveTarget(`GameObject` target) |  | 
| `void` | Start() |  | 
| `void` | Update() |  | 


## `FSMMovementNPCBaseTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.FSMMovementNPCBaseTrigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `FSMMovementNPCBase` | scp |  | 


## `MovementNPCBase`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.MovementNPCBase
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CharacterController` | ctrl |  | 
| `Single` | gravity |  | 
| `Single` | gravMulti |  | 
| `Boolean` | isteleport |  | 
| `Single` | maxTrackingDist |  | 
| `NavMeshPath` | path |  | 
| `Vector3[]` | path2 |  | 
| `GameObject` | plr |  | 
| `Single` | speed |  | 
| `Animator` | state |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckForNav() |  | 
| `void` | FollowPlayer(`Animator` animator) |  | 
| `void` | GetPath() |  | 
| `void` | IdleMove(`Animator` animator) |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `Animator&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `Animator&` animator) |  | 
| `void` | Update() |  | 


## `MovementNPCBaseTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.MovementNPCBaseTrigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MovementNPCBase` | scp |  | 


## `NPCClassD`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.NPCClassD
    : FSMMovementNPCBase, IElevatorTeleport, ISavable, IEntity, IHuman, ICanTakeDamage, ICanTriggerTesla

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | _audible |  | 
| `Boolean` | _blinking |  | 
| `Boolean` | _has714 |  | 
| `Animator` | anim |  | 
| `GameObject` | enemyObj |  | 
| `GameObject` | face |  | 
| `AudioClip` | foundClip |  | 
| `Inventory` | inv |  | 
| `Boolean` | IsDead |  | 
| `Boolean` | isPlayer |  | 
| `Single` | npcHealth |  | 
| `IHuman` | player |  | 
| `Single` | repathTimer |  | 
| `FSMMovementNPCBase` | scp |  | 
| `SCPSkills` | skills |  | 
| `AudioSource` | voice |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | godMode |  | 
| `Boolean` | HasRing |  | 
| `Boolean` | IsBlinking |  | 
| `Single` | IsMakingSound |  | 
| `Boolean` | isValidTarget |  | 
| `GameObject` | rot |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | BackAway(`FSMNode` animator) |  | 
| `void` | FoundEnemy() |  | 
| `void` | FoundHuman() |  | 
| `void` | GetPathBackAway() |  | 
| `void` | Kill(`DeathTypes` type, `GameObject` go) |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | RpcFound() |  | 
| `void` | TakeDamage(`Single` amnt, `GameObject` go, `DeathTypes` type) |  | 
| `void` | UserCode_RpcFound() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcFound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `NPCClassDDetection`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.NPCClassDDetection
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | mask |  | 
| `NPCClassD` | scp |  | 
| `Single` | seeDist |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CalcPlyLook(`IHuman` ply) |  | 
| `Boolean` | CalcScpLook(`GameObject` ply) |  | 


## `NPCData`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.NPCData
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | NpcId |  | 
| `String` | NPCName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 


## `NPCDataBase`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.NPCDataBase
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<NPCData>` | NPCs |  | 
| `Dictionary<String, GameObject>` | PrefabDB |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | LoadNPCs() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `NPCDataBase` | db |  | 
| `Dictionary<String, String>` | NPCTEMPDB |  | 


## `NPCWaypoint`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.NPCWaypoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | NPCIds |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `NPCWaypoint` | GetWaypoint(`String` id) |  | 


