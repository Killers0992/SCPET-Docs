## `ExtensionFilter`

```csharp
public struct SFB.ExtensionFilter

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Extensions |  | 
| `String` | Name |  | 


## `IStandaloneFileBrowser`

```csharp
public interface SFB.IStandaloneFileBrowser

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | OpenFilePanel(`String` title, `String` directory, `ExtensionFilter[]` extensions, `Boolean` multiselect) |  | 
| `void` | OpenFilePanelAsync(`String` title, `String` directory, `ExtensionFilter[]` extensions, `Boolean` multiselect, `Action<String[]>` cb) |  | 
| `String[]` | OpenFolderPanel(`String` title, `String` directory, `Boolean` multiselect) |  | 
| `void` | OpenFolderPanelAsync(`String` title, `String` directory, `Boolean` multiselect, `Action<String[]>` cb) |  | 
| `String` | SaveFilePanel(`String` title, `String` directory, `String` defaultName, `ExtensionFilter[]` extensions) |  | 
| `void` | SaveFilePanelAsync(`String` title, `String` directory, `String` defaultName, `ExtensionFilter[]` extensions, `Action<String>` cb) |  | 


## `StandaloneFileBrowser`

```csharp
public class SFB.StandaloneFileBrowser

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | OpenFilePanel(`String` title, `String` directory, `String` extension, `Boolean` multiselect) |  | 
| `String[]` | OpenFilePanel(`String` title, `String` directory, `ExtensionFilter[]` extensions, `Boolean` multiselect) |  | 
| `void` | OpenFilePanelAsync(`String` title, `String` directory, `String` extension, `Boolean` multiselect, `Action<String[]>` cb) |  | 
| `void` | OpenFilePanelAsync(`String` title, `String` directory, `ExtensionFilter[]` extensions, `Boolean` multiselect, `Action<String[]>` cb) |  | 
| `String[]` | OpenFolderPanel(`String` title, `String` directory, `Boolean` multiselect) |  | 
| `void` | OpenFolderPanelAsync(`String` title, `String` directory, `Boolean` multiselect, `Action<String[]>` cb) |  | 
| `String` | SaveFilePanel(`String` title, `String` directory, `String` defaultName, `String` extension) |  | 
| `String` | SaveFilePanel(`String` title, `String` directory, `String` defaultName, `ExtensionFilter[]` extensions) |  | 
| `void` | SaveFilePanelAsync(`String` title, `String` directory, `String` defaultName, `String` extension, `Action<String>` cb) |  | 
| `void` | SaveFilePanelAsync(`String` title, `String` directory, `String` defaultName, `ExtensionFilter[]` extensions, `Action<String>` cb) |  | 


## `StandaloneFileBrowserWindows`

```csharp
public class SFB.StandaloneFileBrowserWindows
    : IStandaloneFileBrowser

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | OpenFilePanel(`String` title, `String` directory, `ExtensionFilter[]` extensions, `Boolean` multiselect) |  | 
| `void` | OpenFilePanelAsync(`String` title, `String` directory, `ExtensionFilter[]` extensions, `Boolean` multiselect, `Action<String[]>` cb) |  | 
| `String[]` | OpenFolderPanel(`String` title, `String` directory, `Boolean` multiselect) |  | 
| `void` | OpenFolderPanelAsync(`String` title, `String` directory, `Boolean` multiselect, `Action<String[]>` cb) |  | 
| `String` | SaveFilePanel(`String` title, `String` directory, `String` defaultName, `ExtensionFilter[]` extensions) |  | 
| `void` | SaveFilePanelAsync(`String` title, `String` directory, `String` defaultName, `ExtensionFilter[]` extensions, `Action<String>` cb) |  | 


## `WindowWrapper`

```csharp
public class SFB.WindowWrapper
    : IWin32Window

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `IntPtr` | Handle |  | 


