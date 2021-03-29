## `SCP008`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP008
    : FSMMovementNPCBase, IElevatorTeleport, ISavable, IEntity, ICanTakeDamage, ICanTriggerTesla, ISCP

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Animator` | anim |  | 
| `BoxCollider` | attackBox |  | 
| `Boolean` | attacking |  | 
| `List<AudioClip>` | attackSounds |  | 
| `Boolean` | found |  | 
| `AudioClip` | idleSound |  | 
| `Single` | lerpSpeed |  | 
| `Single` | movement |  | 
| `Int32` | navpointLayers |  | 
| `GameObject` | zombieEntity |  | 
| `Single` | zombieHealth |  | 
| `AudioSource` | zombieNoises |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | godMode |  | 
| `Boolean` | isValidTarget |  | 
| `Int32` | maxDamage |  | 
| `Int32` | minDamage |  | 
| `Single` | Networkmovement |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Attack() |  | 
| `void` | CheckForNav() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Kill(`DeathTypes` type, `GameObject` go) |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | RpcPlayAttackAnim() |  | 
| `void` | RpcPlayAttackSound(`Int32` id) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | TakeDamage(`Single` amnt, `GameObject` go, `DeathTypes` type) |  | 
| `void` | UserCode_RpcPlayAttackAnim() |  | 
| `void` | UserCode_RpcPlayAttackSound(`Int32` id) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPlayAttackAnim(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayAttackSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP008Attack`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP008Attack
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | timeToFollow |  | 
| `Single` | timeToHit |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP008AttackBox`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP008AttackBox
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | boxcollider |  | 
| `SCP008` | scp |  | 


## `SCP008Follow`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP008Follow
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | maxFollowDistance |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP008Idle`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP008Idle
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


## `SCP008NavPoint`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP008NavPoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | layer |  | 


## `SCP008Wander`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP008Wander
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


## `SCP049`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP049
    : FSMMovementNPCBase, IElevatorTeleport, ISavable, IEntity, ISCP

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip` | alertSound |  | 
| `Animator` | anim |  | 
| `AudioClip[]` | attackSounds |  | 
| `AudioSource` | audioSrcAlert |  | 
| `AudioSource` | audioSrcDialogue |  | 
| `List<AudioClip>` | dialogueSounds |  | 
| `Single` | footstepTimer |  | 
| `Boolean` | isOutsideMoving |  | 
| `Boolean` | isShocked |  | 
| `Single` | maxFootstepTimer |  | 
| `Single` | maxMoveTimer |  | 
| `Single` | maxRepathTimer |  | 
| `Single` | minMoveDist |  | 
| `List<AudioClip>` | moveSounds |  | 
| `Single` | moveTimer |  | 
| `Int32` | navpointLayers |  | 
| `NetworkIdentitySyncvar` | PlayerTarget |  | 
| `Single` | plrCheckTimer |  | 
| `Single` | repathTimer |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `NetworkIdentity` | NetworkPlayerTarget |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Alert(`IHuman` controller) |  | 
| `void` | CheckForNav() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | RpcPlayDialogue(`Int32` id) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | Shock(`Single` time) |  | 
| `void` | TargetPlayAlert(`INetworkConnection` conn) |  | 
| `void` | UserCode_RpcPlayDialogue(`Int32` id) |  | 
| `void` | UserCode_TargetPlayAlert(`INetworkConnection` conn) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPlayDialogue(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetPlayAlert(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP049Attack`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP049Attack
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | attackTimer |  | 
| `BoxCollider` | boxcollider |  | 
| `Single` | maxAttackTimer |  | 
| `SCP049` | scp |  | 


## `SCP049Follow`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP049Follow
    : FSMState

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateDisable(`FSMManager` manager, `FSMState` newstate) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP049Idle`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP049Idle
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


## `SCP049NavPoint`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP049NavPoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | layer |  | 


## `SCP049Trigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP049Trigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | mask |  | 
| `Single` | maxTimer |  | 
| `SCP049` | scp |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CalcScpLook(`GameObject` ply) |  | 


## `SCP049Wander`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP049Wander
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


## `SCP096`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP096
    : FSMMovementNPCBase, IElevatorTeleport, ISavable, IEntity, ISCP

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ai2Setting |  | 
| `AudioClip` | ambient |  | 
| `AudioSource` | ambientSrc |  | 
| `Animator` | anim |  | 
| `Int32` | animState |  | 
| `AudioClip` | enrage |  | 
| `AudioSource` | enragesrc |  | 
| `AudioSource` | handsrc |  | 
| `Boolean` | hasTarget |  | 
| `AudioSource` | headsrc |  | 
| `AudioClip` | idle |  | 
| `AudioClip` | killSound |  | 
| `Single` | lerpSpeed |  | 
| `Single` | movement |  | 
| `Int32` | navpointLayers |  | 
| `NetworkIdentitySyncvar` | PlayerTarget |  | 
| `AudioClip` | scream |  | 
| `Int32` | soundMode |  | 
| `AudioClip` | trigger |  | 
| `AudioSource` | triggersrc |  | 
| `Single` | walkspeed |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | NetworkanimState |  | 
| `Boolean` | NetworkhasTarget |  | 
| `Single` | Networkmovement |  | 
| `NetworkIdentity` | NetworkPlayerTarget |  | 
| `Int32` | NetworksoundMode |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckForNav() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `GameObject` | GetRandomNavPoint() |  | 
| `void` | KillSound() |  | 
| `void` | LoadComplete() |  | 
| `IEnumerator` | LoadLate() |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `FSMNode&` animator) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | Start() |  | 
| `void` | SyncAnim(`Int32` old, `Int32` newint) |  | 
| `void` | TargetPlayerBecameTarget(`INetworkConnection` conn) |  | 
| `void` | UserCode_TargetPlayerBecameTarget(`INetworkConnection` conn) |  | 
| `void` | Walk(`FSMNode` animator, `Single` f) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcKillSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetPlayerBecameTarget(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP096Aggro`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP096Aggro
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | timeToAggro |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateDisable(`FSMManager` manager, `FSMState` newstate) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP096Face`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP096Face
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `LayerMask` | mask |  | 
| `SCP096` | scp |  | 
| `Single` | seeDist |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CalcPlyLook(`IHuman` ply) |  | 


## `SCP096Follow`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP096Follow
    : FSMState

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateDisable(`FSMManager` manager, `FSMState` newstate) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP096Hands`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP096Hands
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | boxcollider |  | 
| `SCP096` | scp |  | 
| `GameObject` | scpgo |  | 


## `SCP096Idle`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP096Idle
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


## `SCP096NavPoint`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP096NavPoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | layer |  | 


## `SCP096Wander`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP096Wander
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


## `SCP106`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP106
    : FSMMovementNPCBase, IElevatorTeleport, ISavable, IEntity, ICanTriggerTesla, ICanTakeDamage, ISCP

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ai2Setting |  | 
| `AudioClip` | ambient |  | 
| `AudioSource` | ambientSrc |  | 
| `Animator` | anim |  | 
| `Int32` | animState |  | 
| `AudioClip[]` | attackSounds |  | 
| `AudioSource` | audioSrc |  | 
| `GameObject` | coom |  | 
| `AudioClip[]` | corrodeSounds |  | 
| `Single` | followTimer |  | 
| `Single` | footstepTimer |  | 
| `SCP106Hands` | hand |  | 
| `AudioSource` | handsrc |  | 
| `Boolean` | isOutsideMoving |  | 
| `Boolean` | isShocked |  | 
| `AudioClip[]` | killSounds |  | 
| `Single` | lerpSpeed |  | 
| `LayerMask` | mask |  | 
| `Single` | maxFootstepTimer |  | 
| `Single` | maxMoveTimer |  | 
| `Single` | minMoveDist |  | 
| `Single` | minTeleportDist |  | 
| `Single` | movement |  | 
| `List<AudioClip>` | moveSounds |  | 
| `Single` | moveTimer |  | 
| `Int32` | navpointLayers |  | 
| `Boolean` | PlayerTarget |  | 
| `Single` | plrCheckTimer |  | 
| `Single` | repathTimer |  | 
| `LayerMask` | teleportMask |  | 
| `AudioClip[]` | teleportSounds |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | godMode |  | 
| `Boolean` | isValidTarget |  | 
| `Int32` | NetworkanimState |  | 
| `Single` | Networkmovement |  | 
| `Boolean` | NetworkPlayerTarget |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckForNav() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | FollowNearestPlayer() |  | 
| `IHuman` | GetRandomIHuman() |  | 
| `GameObject` | GetRandTarget() |  | 
| `IHuman[]` | getTogetherPlayers(`IHuman` player) |  | 
| `void` | Kill(`DeathTypes` type, `GameObject` go) |  | 
| `void` | KillSound() |  | 
| `void` | LoadComplete() |  | 
| `IEnumerator` | LoadLate() |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MoveNoCollide() |  | 
| `void` | PlayCorrodeSound() |  | 
| `void` | PlayFootStep(`Int32` id) |  | 
| `void` | RpcPlayCorrodeSound() |  | 
| `void` | RpcPlayTeleportSound(`Vector3` position) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | Shock(`Single` time) |  | 
| `void` | Start() |  | 
| `void` | SyncAnim(`Int32` old, `Int32` newint) |  | 
| `void` | TakeDamage(`Single` amnt, `GameObject` go, `DeathTypes` type) |  | 
| `void` | Teleport() |  | 
| `void` | Update() |  | 
| `void` | UserCode_RpcPlayCorrodeSound() |  | 
| `void` | UserCode_RpcPlayTeleportSound(`Vector3` position) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcKillSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayCorrodeSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayTeleportSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP106Follow`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP106Follow
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | maxDistanceBeforeTeleport |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP106Hands`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP106Hands
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | boxcollider |  | 
| `Int32` | grabDamage |  | 
| `SCP106` | scp |  | 
| `GameObject` | scpgo |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CheckKill(`Boolean` kill = False) |  | 


## `SCP106Idle`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP106Idle
    : FSMState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | maxRepathTimer |  | 
| `Int32` | minRepathTimer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP106NavPoint`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP106NavPoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | layer |  | 


## `SCP106NoCollide`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP106NoCollide
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider[]` | cols |  | 


## `SCP106PDFollow`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP106PDFollow
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | maxDistanceBeforeTeleport |  | 
| `Single` | timeToFollow |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateDisable(`FSMManager` manager, `FSMState` newstate) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP106RiseUp`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP106RiseUp
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | timeToRise |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateDisable(`FSMManager` manager, `FSMState` newstate) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP106Spawn`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP106Spawn
    : MonoBehaviour

```

## `SCP1499`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP1499
    : FSMMovementNPCBase, IElevatorTeleport, ISavable, IEntity, ISCP, ICanTakeDamage

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ai2Setting |  | 
| `Animator` | anim |  | 
| `Int32` | animState |  | 
| `Single` | lerpSpeed |  | 
| `Single` | movement |  | 
| `AudioClip[]` | praySound |  | 
| `AudioSource` | source |  | 
| `AudioClip` | triggeredSound |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | godMode |  | 
| `Boolean` | isValidTarget |  | 
| `Int32` | NetworkanimState |  | 
| `Single` | Networkmovement |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Kill(`DeathTypes` type, `GameObject` go) |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | RpcPraySound() |  | 
| `void` | RpcTriggeredSound() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | SyncAnim(`Int32` old, `Int32` cur) |  | 
| `void` | TakeDamage(`Single` amnt, `GameObject` go, `DeathTypes` type) |  | 
| `void` | UserCode_RpcPraySound() |  | 
| `void` | UserCode_RpcTriggeredSound() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPraySound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcTriggeredSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP1499Idle`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP1499Idle
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | idleTime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP1499Pray`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP1499Pray
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | idleTime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP1499Triggered`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP1499Triggered
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | idleTime |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP1499TriggerZone`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP1499TriggerZone
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `SCP1499` | scp |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnTriggerEnter(`Collider` other) |  | 


## `SCP1499Wander`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP1499Wander
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


## `SCP173`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP173
    : NetworkBehaviour, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | accel |  | 
| `NavMeshAgent` | agent |  | 
| `Camera` | cam |  | 
| `Boolean` | canMove |  | 
| `Boolean` | canMoveDirect |  | 
| `GameObject` | center |  | 
| `CharacterController` | ctrl |  | 
| `LayerMask` | doorCheckMask |  | 
| `Int32` | filter |  | 
| `Single` | gravity |  | 
| `Single` | gravMulti |  | 
| `SCP173Hands` | hands |  | 
| `AudioClip[]` | HorrorSounds |  | 
| `Boolean` | isGrounded |  | 
| `Boolean` | isHiding |  | 
| `Boolean` | isOutsideMoving |  | 
| `SCP173LookPoint[]` | lookPositions |  | 
| `LayerMask` | mask |  | 
| `Single` | maxTeleportTimer |  | 
| `Single` | maxTrackingDist |  | 
| `Single` | minMoveDist |  | 
| `List<AudioClip>` | moveSounds |  | 
| `NavMeshPath` | path |  | 
| `GameObject` | plr |  | 
| `String` | savePlrGuid |  | 
| `Single` | seeDist |  | 
| `GameObject` | shitPrefab |  | 
| `Single` | speed |  | 
| `Single` | timeFromSeen |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Guid |  | 
| `Boolean` | NetworkisHiding |  | 
| `String` | PrefabGuid |  | 
| `JSONVector` | savePos |  | 
| `JSONVector` | saveRot |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CalcPlyLook(`IHuman` ply) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | KillSound() |  | 
| `void` | LoadComplete() |  | 
| `void` | RpcMoveSound() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | TeleportToDoor() |  | 
| `void` | UserCode_RpcMoveSound() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanSeePoint(`IHuman` ply, `Vector3` point, `LayerMask` mask, `Single` dot = 0,65) |  | 
| `void` | Skeleton_RpcKillSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcMoveSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcTakeAShit(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP173Hands`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP173Hands
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | boxcollider |  | 
| `Boolean` | canOpenDoors |  | 
| `Single` | doorOpenTimer |  | 
| `AudioClip[]` | killSounds |  | 
| `Single` | maxDoorTimer |  | 
| `Single` | minDoorTimer |  | 
| `SCP173` | scp |  | 
| `GameObject` | scpgo |  | 


## `SCP173LookPoint`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP173LookPoint
    : MonoBehaviour

```

## `SCP939`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP939
    : FSMMovementNPCBase, IElevatorTeleport, ISavable, IEntity, ICanTriggerTesla, ICanTakeDamage, ISCP

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ai2Setting |  | 
| `AudioClip` | alertSound |  | 
| `Animator` | anim |  | 
| `AudioClip[]` | attackSounds |  | 
| `AudioSource` | audioSrc |  | 
| `AudioSource` | audioSrcAlert |  | 
| `AudioSource` | audioSrcScream |  | 
| `Single` | footstepTimer |  | 
| `List<AudioClip>` | idleSounds |  | 
| `Single` | idleSoundTimer |  | 
| `Boolean` | isOutsideMoving |  | 
| `Boolean` | isShocked |  | 
| `Single` | lerpSpeed |  | 
| `Single` | maxFootstepTimer |  | 
| `Single` | maxMoveTimer |  | 
| `Single` | maxRepathTimer |  | 
| `Single` | minMoveDist |  | 
| `Single` | movement |  | 
| `List<AudioClip>` | moveSounds |  | 
| `Single` | moveTimer |  | 
| `Int32` | navpointLayers |  | 
| `Single` | plrCheckTimer |  | 
| `Single` | repathTimer |  | 
| `List<AudioClip>` | screamSounds |  | 
| `TTSSimple` | tts |  | 
| `String[]` | ttsArray |  | 
| `Single` | walkAnimSpeed |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | godMode |  | 
| `Boolean` | isValidTarget |  | 
| `Single` | Networkmovement |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Alert(`IHuman` controller) |  | 
| `void` | CheckForNav() |  | 
| `void` | DamageSound() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `String` | GetDialog(`AudioClip` clip) |  | 
| `void` | Kill(`DeathTypes` type, `GameObject` go) |  | 
| `void` | LoadComplete() |  | 
| `IEnumerator` | LoadLate() |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | PlayFootStep(`Int32` id) |  | 
| `void` | RpcPlayIdleSound(`Int32` id) |  | 
| `void` | RpcPlayScream(`Int32` id) |  | 
| `void` | RpcPlayTTS(`String` tts) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | Shock(`Single` time) |  | 
| `void` | TakeDamage(`Single` amnt, `GameObject` go, `DeathTypes` type) |  | 
| `void` | TargetPlayAlert(`INetworkConnection` conn) |  | 
| `void` | Update() |  | 
| `void` | UserCode_RpcPlayIdleSound(`Int32` id) |  | 
| `void` | UserCode_RpcPlayScream(`Int32` id) |  | 
| `void` | UserCode_RpcPlayTTS(`String` tts) |  | 
| `void` | UserCode_TargetPlayAlert(`INetworkConnection` conn) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcDamage(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayIdleSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayScream(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayTTS(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetPlayAlert(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP939Attack`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP939Attack
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | attackTimer |  | 
| `BoxCollider` | boxcollider |  | 
| `Single` | doorTimer |  | 
| `LayerMask` | mask |  | 
| `Single` | maxAttackTimer |  | 
| `SCP939` | scp |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | damage |  | 
| `Single` | randDamage |  | 


## `SCP939Follow`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP939Follow
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | maxFollowDistance |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP939Idle`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP939Idle
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


## `SCP939NavPoint`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP939NavPoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | layer |  | 


## `SCP939Trigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP939Trigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | distance |  | 
| `Single` | maxTimer |  | 
| `SCP939` | scp |  | 


## `SCP939Wander`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP939Wander
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
| `void` | OnStateDisable(`FSMManager` manager, `FSMState` newstate) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP966`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP966
    : FSMMovementNPCBase, IElevatorTeleport, ISavable, IEntity, ICanTakeDamage, ISCP

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ai2Setting |  | 
| `Animator` | anim |  | 
| `Int32` | animState |  | 
| `BoxCollider` | attackBox |  | 
| `Boolean` | attacking |  | 
| `AudioClip` | attackSound |  | 
| `AudioSource` | attackSource |  | 
| `List<AudioClip>` | idleSounds |  | 
| `Single` | idleSoundTimer |  | 
| `AudioSource` | idleSource |  | 
| `Single` | lerpSpeed |  | 
| `Single` | movement |  | 
| `Int32` | navpointLayers |  | 
| `Renderer` | SCP966Mesh |  | 
| `Single` | scpHealth |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | godMode |  | 
| `Boolean` | isValidTarget |  | 
| `Int32` | NetworkanimState |  | 
| `Single` | Networkmovement |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Attack() |  | 
| `void` | CheckForNav() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | Kill(`DeathTypes` type, `GameObject` go) |  | 
| `void` | LoadComplete() |  | 
| `IEnumerator` | LoadLate() |  | 
| `void` | MiscFollowPlayer(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | MiscIdleMove(`Vector3&` move, `FSMNode&` animator) |  | 
| `void` | RpcPlayAttackSound() |  | 
| `void` | RpcPlayIdleSound(`Int32` id) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | SyncAnim(`Int32` old, `Int32` cur) |  | 
| `void` | TakeDamage(`Single` amnt, `GameObject` go, `DeathTypes` type) |  | 
| `void` | UserCode_RpcPlayAttackSound() |  | 
| `void` | UserCode_RpcPlayIdleSound(`Int32` id) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPlayAttackSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcPlayIdleSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP966Attack`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP966Attack
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | timeToFollow |  | 
| `Single` | timeToHit |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateDisable(`FSMManager` manager, `FSMState` newstate) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP966AttackBox`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP966AttackBox
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | boxcollider |  | 
| `SCP966` | scp |  | 


## `SCP966Follow`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP966Follow
    : FSMState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | maxFollowDistance |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnFixedUpdate(`FSMManager` manager) |  | 
| `void` | OnStateEnable(`FSMManager` manager, `FSMState` oldstate) |  | 
| `void` | OnUpdate(`FSMManager` manager) |  | 


## `SCP966Idle`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP966Idle
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


## `SCP966NavPoint`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP966NavPoint
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | layer |  | 


## `SCP966Wander`

```csharp
public class VirtualBrightPlayz.SCP_ET.NPCs.SCP.SCP966Wander
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


