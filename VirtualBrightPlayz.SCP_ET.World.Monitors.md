## `CheckpointLockDownMonitor`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Monitors.CheckpointLockDownMonitor
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioSource` | source |  | 
| `TMP_Text` | text |  | 


## `CheckpointLockDownMonitorEvent`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Monitors.CheckpointLockDownMonitorEvent
    : NetworkBehaviour

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnTriggerEnter(`Collider` other) |  | 


## `Monitor`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Monitors.Monitor
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MonitorCamera` | camCache |  | 
| `Boolean` | disable |  | 
| `String` | id |  | 
| `MeshRenderer` | render |  | 
| `Single` | timeBetweenSwitch |  | 
| `Single` | timer |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `MonitorCamera` | GetCamera() |  | 
| `MonitorCamera[]` | GetCameras() |  | 
| `void` | SwitchCamera() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<Monitor>` | cams |  | 


## `MonitorCamera`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Monitors.MonitorCamera
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Camera` | cam |  | 
| `List<Collider>` | collidedObjects |  | 
| `Int32` | fps |  | 
| `String` | id |  | 
| `Monitor` | monitor |  | 
| `List<RoomLightController>` | roomLightController |  | 
| `Boolean` | spawnSpectate |  | 
| `SpectateCam` | spectate |  | 
| `RenderTexture` | tex |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<MonitorCamera>` | cams |  | 


## `MonitorFpsRegulator`

```csharp
public class VirtualBrightPlayz.SCP_ET.World.Monitors.MonitorFpsRegulator
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `MonitorCamera` | cam |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnTriggerEnter(`Collider` other) |  | 
| `void` | OnTriggerExit(`Collider` other) |  | 


