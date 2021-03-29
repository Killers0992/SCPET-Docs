## `BadEndingA1P`

```csharp
public class VirtualBrightPlayz.SCP_ET.Endings.BadEndingA1P
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<PlayerController, Boolean>` | scp106Contained |  | 
| `Dictionary<PlayerController, Int32>` | scp500Times |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Add500(`PlayerController` ctrl) |  | 
| `Boolean` | CheckEnding(`PlayerController` ctrl) |  | 
| `void` | Contain106(`PlayerController` ctrl) |  | 
| `void` | Start() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BadEndingA1P` | end |  | 


## `EndTrigger`

```csharp
public class VirtualBrightPlayz.SCP_ET.Endings.EndTrigger
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | AllowEndings |  | 
| `AudioSource` | endSounds |  | 
| `GameObject` | mtfUnit |  | 
| `AudioClip` | offer |  | 
| `AudioClip[]` | stop |  | 
| `AudioClip[]` | thereHeIs |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | NetworkAllowEndings |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | OnTriggerEnter(`Collider` other) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | Start() |  | 
| `void` | TargetPlayOfferSound(`INetworkConnection` connection) |  | 
| `void` | TargetPlayStopSound(`INetworkConnection` connection) |  | 
| `void` | TargetPlayThereHeIsSound(`INetworkConnection` connection) |  | 
| `void` | UserCode_TargetPlayOfferSound(`INetworkConnection` connection) |  | 
| `void` | UserCode_TargetPlayStopSound(`INetworkConnection` connection) |  | 
| `void` | UserCode_TargetPlayThereHeIsSound(`INetworkConnection` connection) |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_TargetPlayOfferSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetPlayStopSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_TargetPlayThereHeIsSound(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


