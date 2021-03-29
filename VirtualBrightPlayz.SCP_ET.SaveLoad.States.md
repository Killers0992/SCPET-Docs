## `BinaryItemExt`

```csharp
public static class VirtualBrightPlayz.SCP_ET.SaveLoad.States.BinaryItemExt

```

## `CanSaveState`

```csharp
public class VirtualBrightPlayz.SCP_ET.SaveLoad.States.CanSaveState
    : SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | gameObject |  | 
| `String` | TypeName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


## `ItemState`

```csharp
public class VirtualBrightPlayz.SCP_ET.SaveLoad.States.ItemState
    : CanSaveState, SaveState

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


## `NPCState`

```csharp
public class VirtualBrightPlayz.SCP_ET.SaveLoad.States.NPCState
    : CanSaveState, SaveState

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


## `PlayerState`

```csharp
public class VirtualBrightPlayz.SCP_ET.SaveLoad.States.PlayerState
    : CanSaveState, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | TypeName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


## `SaveState`

```csharp
public interface VirtualBrightPlayz.SCP_ET.SaveLoad.States.SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | gameObject |  | 
| `String` | TypeName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


