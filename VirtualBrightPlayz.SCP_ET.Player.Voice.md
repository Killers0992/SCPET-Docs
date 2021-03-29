## `RadioPlayback`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Voice.RadioPlayback
    : MonoBehaviour, IWorldRadio

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioSource` | source |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | PlayData(`Single[]` data, `Int32` pos) |  | 
| `void` | Start() |  | 
| `void` | Stop() |  | 


## `Recorder`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Voice.Recorder
    : NetworkBehaviour

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isRecording |  | 


Events

| Type | Name | Summary | 
| --- | --- | --- | 
| `Action<Single[]>` | OnAudioReady |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | GetRMS() |  | 
| `void` | StartRec() |  | 
| `void` | StopRec() |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | samplingFrequency |  | 


## `VoiceChatV2`

```csharp
public class VirtualBrightPlayz.SCP_ET.Player.Voice.VoiceChatV2
    : NetworkBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `AudioClip` | BackClip |  | 
| `BinaryReader` | breader |  | 
| `AudioClip` | clip |  | 
| `Single` | distanceNormal |  | 
| `Single` | distanceRadio |  | 
| `Single` | interval |  | 
| `Boolean` | isMuted |  | 
| `Boolean` | isRadio |  | 
| `Boolean` | isServerMuted |  | 
| `Boolean` | isSpeaking |  | 
| `Boolean` | profile |  | 
| `GameObject` | spkIcon |  | 
| `AudioSource` | src |  | 
| `Int32` | syncFrameSize |  | 
| `Boolean` | useDistance |  | 
| `Single` | volume |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | NetworkisServerMuted |  | 
| `Int32` | NetworksyncFrameSize |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CmdSetVoice2(`Byte[]` data, `Int32` offset, `Int32` frame_size, `Int32` ms, `Int32` len, `Double` time) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | RpcSetVoice2(`Byte[]` data, `Int32` offset, `Int32` frame_size, `Int32` ms, `Int32` enclen, `Double` time) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | UserCode_CmdSetVoice2(`Byte[]` data, `Int32` offset, `Int32` frame_size, `Int32` ms, `Int32` len, `Double` time) |  | 
| `void` | UserCode_RpcSetVoice2(`Byte[]` data, `Int32` offset, `Int32` frame_size, `Int32` ms, `Int32` enclen, `Double` time) |  | 


Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | clipLen |  | 
| `Int32` | frameSize |  | 
| `List<IWorldRadio>` | radios |  | 
| `SamplingFrequency` | samplingFrequency |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdSetVoice2(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSetVoice2(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


