## `AutoDestroy`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.AutoDestroy
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | timer |  | 
| `Single` | timeToLive |  | 


## `ClosetEvent`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.ClosetEvent
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | ambient |  | 
| `Door` | closetDoor |  | 
| `GameObject` | doorPrefab |  | 
| `GameObject` | doorSpawn |  | 
| `Boolean` | hasRun |  | 
| `List<IHuman>` | humans |  | 
| `Boolean` | isRunning |  | 
| `GameObject` | janitor |  | 
| `AudioClip` | janitorClip |  | 
| `GameObject` | janitorKeycard |  | 
| `AudioClip[]` | killSounds |  | 
| `Light[]` | lights |  | 
| `GameObject` | scientist |  | 
| `AudioClip` | scientistClip |  | 
| `SCP173` | scp |  | 
| `GameObject` | vent |  | 
| `AudioClip` | ventClip |  | 
| `GameObject` | ventPre |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CaptionInRange(`String` message, `Color` color, `GameObject` obj, `Single` range) |  | 
| `IEnumerator` | Event(`SCP173` scp) |  | 
| `void` | RpcRun() |  | 
| `void` | Start() |  | 
| `void` | Trigger(`SCP173` scp, `IHuman` human) |  | 
| `void` | Update() |  | 
| `void` | UserCode_RpcRun() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcRun(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `ClosetTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.ClosetTrigger
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ClosetEvent` | parent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnTriggerEnter(`Collider` other) |  | 


## `EndingTriggerEvent`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.EndingTriggerEvent
    : NetworkBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnTriggerEnter(`Collider` other) |  | 


## `EventTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.EventTrigger
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `UnityEvent` | onTriggered |  | 
| `UnityEvent<PlayerController>` | onTriggeredObject |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnTriggerEnter(`Collider` other) |  | 


## `IntroCutscene`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.IntroCutscene
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | blastDoorPrefab |  | 
| `Transform` | breachExplosion |  | 
| `AudioClip` | breachStartSiren |  | 
| `Door` | chamberDoor |  | 
| `GameObject` | chamberDoorSpawn |  | 
| `Door` | chamberLightDoor |  | 
| `GameObject` | chamberLightDoorSpawn |  | 
| `GameObject` | doorPrefab |  | 
| `Rigidbody[]` | enableOnBreach |  | 
| `GameObject` | fake173 |  | 
| `AudioClip` | firingClip |  | 
| `AudioSource` | guard |  | 
| `GameObject` | guardAnim |  | 
| `GameObject` | gunLight |  | 
| `GameObject` | invisibleWall |  | 
| `MonitorController` | monitorController |  | 
| `GameObject` | monitorPrefab |  | 
| `Scp173ContainmentMonitor[]` | monitors |  | 
| `GameObject` | monitorSpawn |  | 
| `String` | monitorText |  | 
| `AudioClip` | ohShitClip |  | 
| `AudioSource` | PAVoiceSrc |  | 
| `GameObject` | redLights |  | 
| `Single` | shotCount |  | 
| `GameObject[]` | sinkingObjects |  | 
| `AudioClip` | snap |  | 
| `AudioSource` | vent |  | 
| `AudioClip` | ventClip |  | 
| `AudioClip` | verbalWarning |  | 
| `GameObject` | whiteLights |  | 
| `AudioClip` | WtfIsHappening |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `IEnumerator` | Intro() |  | 
| `void` | RpcPlayIntro(`Single` shots) |  | 
| `IEnumerator` | SetupIntro() |  | 
| `void` | UserCode_RpcPlayIntro(`Single` shots) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPlayIntro(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `IntroEvent`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.IntroEvent
    : WorldEvent

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip` | audioClip |  | 
| `Int32` | gamemode |  | 
| `AudioSource[]` | source |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | TriggerEvent(`PlayerController` player) |  | 


## `MissionEvent`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.MissionEvent
    : WorldEvent

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | complete |  | 
| `MissionInfo` | mission |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | TriggerEvent(`PlayerController` player) |  | 


## `NetworkWorldAudio`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.NetworkWorldAudio
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip[]` | clips |  | 
| `AudioSource` | source |  | 
| `AudioSource` | source3d |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | RpcPlayAudio(`Int32` id, `Boolean` three) |  | 
| `void` | TargetPlayAudio(`INetworkConnection` conn, `Int32` id, `Boolean` three) |  | 
| `void` | UserCode_RpcPlayAudio(`Int32` id, `Boolean` three) |  | 
| `void` | UserCode_TargetPlayAudio(`INetworkConnection` conn, `Int32` id, `Boolean` three) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcPlayAudio(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetPlayAudio(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `NetworkWorldEvent`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.NetworkWorldEvent
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `WorldEvent` | ev |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | RpcCallEvent() |  | 
| `void` | UserCode_RpcCallEvent() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_RpcCallEvent(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `SCP173Event`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.SCP173Event
    : WorldEvent

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | distanceFrom173 |  | 
| `Single` | intensity |  | 
| `Light[]` | lights |  | 
| `Boolean` | lightsOut |  | 
| `NetworkRoomLight` | nrl |  | 
| `NetworkWorldAudio` | nwa |  | 
| `Boolean` | scareSound |  | 
| `GameObject[]` | spawn |  | 
| `Boolean` | spawnSound |  | 
| `Boolean` | willHide |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | TriggerEvent(`PlayerController` player) |  | 
| `void` | TriggerEventIHuman(`IHuman` player) |  | 


## `SCP173Glass`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.SCP173Glass
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | broken |  | 
| `GameObject` | glass |  | 
| `Int32` | stage |  | 
| `Transform[]` | teleportPoints |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | BreakGlass(`SCP173` scp) |  | 
| `void` | OnTriggerEnter(`Collider` other) |  | 


## `SinkingObject`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.SinkingObject
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | speed |  | 
| `Single` | target |  | 


## `WorldEvent`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Events.WorldEvent
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | chance |  | 
| `Boolean` | hasBeenTriggered |  | 
| `Boolean` | manualTrigger |  | 
| `NetworkWorldEvent` | net |  | 
| `Boolean` | triggerOnlyOnce |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | GetIsClient() |  | 
| `void` | TriggerEvent(`PlayerController` player) |  | 
| `void` | TriggerEventIHuman(`IHuman` player) |  | 
| `void` | Update() |  | 


