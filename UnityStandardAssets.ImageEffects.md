## `PostEffectsBase`

```csharp
public class UnityStandardAssets.ImageEffects.PostEffectsBase
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isSupported |  | 
| `Boolean` | supportDX11 |  | 
| `Boolean` | supportHDRTextures |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CheckResources() |  | 
| `Material` | CheckShaderAndCreateMaterial(`Shader` s, `Material` m2Create) |  | 
| `Boolean` | CheckSupport() |  | 
| `Boolean` | CheckSupport(`Boolean` needDepth) |  | 
| `Boolean` | CheckSupport(`Boolean` needDepth, `Boolean` needHdr) |  | 
| `Material` | CreateMaterial(`Shader` s, `Material` m2Create) |  | 
| `void` | DrawBorder(`RenderTexture` dest, `Material` material) |  | 
| `Boolean` | Dx11Support() |  | 
| `void` | NotSupported() |  | 
| `void` | ReportAutoDisable() |  | 
| `void` | Start() |  | 


## `Tonemapping`

```csharp
public class UnityStandardAssets.ImageEffects.Tonemapping
    : PostEffectsBase

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | adaptionSpeed |  | 
| `AdaptiveTexSize` | adaptiveTextureSize |  | 
| `Single` | exposureAdjustment |  | 
| `Single` | middleGrey |  | 
| `AnimationCurve` | remapCurve |  | 
| `Shader` | tonemapper |  | 
| `TonemapperType` | type |  | 
| `Boolean` | validRenderTextureFormat |  | 
| `Single` | white |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CheckResources() |  | 
| `Single` | UpdateCurve() |  | 


