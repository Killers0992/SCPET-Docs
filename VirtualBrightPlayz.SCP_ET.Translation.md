## `TextType`

```csharp
public enum VirtualBrightPlayz.SCP_ET.Translation.TextType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Common |  | 
| `1` | Menu |  | 
| `2` | Item |  | 
| `3` | NPC |  | 
| `4` | Effects |  | 
| `5` | Commands |  | 
| `6` | Hints |  | 
| `7` | Misc |  | 
| `8` | Mod |  | 


## `TranslationKeySet`

```csharp
public struct VirtualBrightPlayz.SCP_ET.Translation.TranslationKeySet

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | key |  | 
| `TextType` | section |  | 


## `TranslationManager`

```csharp
public static class VirtualBrightPlayz.SCP_ET.Translation.TranslationManager

```

Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isDownloading |  | 
| `UInt64` | version |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddModString(`String` name, `String` text) |  | 
| `void` | AddModStringSet(`Dictionary<String, String>` modStrings) |  | 
| `void` | CreateTestLang() |  | 
| `UniTask` | DownloadLangFile(`String` path, `String` lang) |  | 
| `String` | GetString(`TextType` TextType, `String` name) |  | 
| `void` | LoadLanguage(`String` lang) |  | 
| `UniTask` | LoadLanguageAsync(`String` lang) |  | 
| `void` | UpdateOrCreateEnglish() |  | 


## `TranslationText`

```csharp
public class VirtualBrightPlayz.SCP_ET.Translation.TranslationText

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Dictionary<String, String>` | Commands |  | 
| `Dictionary<String, String>` | Common |  | 
| `Dictionary<String, String>` | Effects |  | 
| `Dictionary<String, String>` | Hints |  | 
| `Dictionary<String, String>` | Item |  | 
| `String` | LangCode |  | 
| `Dictionary<String, String>` | Menu |  | 
| `Dictionary<String, String>` | Misc |  | 
| `Dictionary<String, String>` | Mod |  | 
| `Dictionary<String, String>` | NPC |  | 
| `UInt64` | version |  | 


## `TranslationTextMesh`

```csharp
public class VirtualBrightPlayz.SCP_ET.Translation.TranslationTextMesh
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Key |  | 
| `TMP_Text` | TextField |  | 
| `TextType` | ttype |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | RefreshText() |  | 
| `Boolean` | UpdateText(`TextType` tt, `String` k) |  | 


## `TranslationUTEXT`

```csharp
public class VirtualBrightPlayz.SCP_ET.Translation.TranslationUTEXT
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Key |  | 
| `Text` | TextField |  | 
| `TextType` | ttype |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | RefreshText() |  | 
| `Boolean` | UpdateText(`TextType` tt, `String` k) |  | 


