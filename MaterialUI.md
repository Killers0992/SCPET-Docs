## `Anim`

```csharp
public class MaterialUI.Anim
    : MonoBehaviour

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | Bounce(`Single` startValue, `Single` endValue, `Single` time, `Single` duration) |  | 
| `Vector2` | Bounce(`Vector2` startValue, `Vector2` endValue, `Single` time, `Single` duration) |  | 
| `Vector3` | Bounce(`Vector3` startValue, `Vector3` endValue, `Single` time, `Single` duration) |  | 
| `Color` | Bounce(`Color` startValue, `Color` endValue, `Single` time, `Single` duration) |  | 
| `Single` | Linear(`Single` startValue, `Single` endValue, `Single` time, `Single` duration) |  | 
| `Vector2` | Linear(`Vector2` startValue, `Vector2` endValue, `Single` time, `Single` duration) |  | 
| `Vector3` | Linear(`Vector3` startValue, `Vector3` endValue, `Single` time, `Single` duration) |  | 
| `Color` | Linear(`Color` startValue, `Color` endValue, `Single` time, `Single` duration) |  | 
| `Single` | Overshoot(`Single` startValue, `Single` endValue, `Single` time, `Single` duration) |  | 
| `Vector2` | Overshoot(`Vector2` startValue, `Vector2` endValue, `Single` time, `Single` duration) |  | 
| `Vector3` | Overshoot(`Vector3` startValue, `Vector3` endValue, `Single` time, `Single` duration) |  | 
| `Color` | Overshoot(`Color` startValue, `Color` endValue, `Single` time, `Single` duration) |  | 
| `Single` | Sin(`Single` startValue, `Single` amplitude, `Single` time, `Single` duration) |  | 
| `Vector2` | Sin(`Vector2` startValue, `Vector2` endValue, `Single` time, `Single` duration) |  | 
| `Vector3` | Sin(`Vector3` startValue, `Vector3` amplitude, `Single` time, `Single` duration) |  | 
| `Color` | Sin(`Color` startValue, `Color` amplitude, `Single` time, `Single` duration) |  | 


## `AnimType`

```csharp
public enum MaterialUI.AnimType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Linear |  | 
| `1` | Overshoot |  | 
| `2` | Bounce |  | 
| `3` | EaseOutCubed |  | 
| `4` | EaseOutQuint |  | 
| `5` | EaseOutSept |  | 
| `6` | EaseInCubed |  | 
| `7` | EaseInQuint |  | 
| `8` | EaseInSept |  | 
| `9` | EaseInOutCubed |  | 
| `10` | EaseInOutQuint |  | 
| `11` | EaseInOutSept |  | 
| `12` | SoftEaseOutCubed |  | 
| `13` | SoftEaseOutQuint |  | 
| `14` | SoftEaseOutSept |  | 


## `ButtonInteractableControl`

```csharp
public class MaterialUI.ButtonInteractableControl
    : MonoBehaviour

```

## `CheckboxConfig`

```csharp
public class MaterialUI.CheckboxConfig
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationDuration |  | 
| `Boolean` | changeRippleColor |  | 
| `Boolean` | changeTextColor |  | 
| `Color` | disabledColor |  | 
| `Color` | offColor |  | 
| `Color` | onColor |  | 
| `Color` | textDisabledColor |  | 
| `Color` | textNormalColor |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ToggleCheckbox() |  | 
| `void` | TurnOff() |  | 
| `void` | TurnOn() |  | 


## `CheckBoxToggler`

```csharp
public class MaterialUI.CheckBoxToggler
    : MonoBehaviour, IPointerClickHandler, IEventSystemHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Toggle` | theToggle |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnPointerClick(`PointerEventData` data) |  | 


## `ColorCopier`

```csharp
public class MaterialUI.ColorCopier
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Image` | sourceImage |  | 
| `Text` | sourceText |  | 


## `DialogBoxConfig`

```csharp
public class MaterialUI.DialogBoxConfig
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RectTransform` | backgroundTransform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | BackgroundClick() |  | 
| `void` | Close() |  | 
| `void` | Open() |  | 


## `EZAnim`

```csharp
public class MaterialUI.EZAnim
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `List<EZStruct>` | theStructs |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Animate() |  | 
| `void` | AnimateAll() |  | 
| `void` | AnimateByIndex(`Int32` index) |  | 
| `void` | AnimateByName(`String` name) |  | 
| `void` | AnimateByTag(`String` tag) |  | 


## `EZStruct`

```csharp
public struct MaterialUI.EZStruct

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationDuration |  | 
| `AnimType` | animationType |  | 
| `Single` | animDeltaTime |  | 
| `String` | animName |  | 
| `Single` | animStartTime |  | 
| `String` | animTag |  | 
| `Boolean` | called |  | 
| `Single` | delay |  | 
| `Single` | delayValue |  | 
| `Single` | duration |  | 
| `Color` | initialColor |  | 
| `Single` | initialFloat |  | 
| `Int32` | initialInt |  | 
| `Material` | initialMaterial |  | 
| `Rect` | initialRect |  | 
| `Vector2` | initialVector2 |  | 
| `Vector3` | initialVector3 |  | 
| `Vector4` | initialVector4 |  | 
| `Boolean` | isField |  | 
| `Boolean` | methodOnEnd |  | 
| `String` | methodParam |  | 
| `Component` | methodRealComponent |  | 
| `MethodInfo` | methodRealMethod |  | 
| `String` | methodTargetComponent |  | 
| `GameObject` | methodTargetGameObject |  | 
| `String` | methodTargetMethod |  | 
| `Boolean` | modifyParameter1 |  | 
| `Boolean` | modifyParameter2 |  | 
| `Boolean` | modifyParameter3 |  | 
| `Boolean` | modifyParameter4 |  | 
| `Component` | RealComponent |  | 
| `FieldInfo` | realField |  | 
| `PropertyInfo` | realProperty |  | 
| `Color` | targetColor |  | 
| `String` | targetComponent |  | 
| `Single` | targetFloat |  | 
| `GameObject` | targetGameObject |  | 
| `Int32` | targetInt |  | 
| `Material` | targetMaterial |  | 
| `Rect` | targetRect |  | 
| `String` | targetVariable |  | 
| `Vector2` | targetVector2 |  | 
| `Vector3` | targetVector3 |  | 
| `Vector4` | targetVector4 |  | 
| `ValType` | valueType |  | 
| `String` | variableType |  | 


## `FPSCounter`

```csharp
public class MaterialUI.FPSCounter
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Text` | theText |  | 
| `Single` | updateInterval |  | 


## `HSBColor`

```csharp
public struct MaterialUI.HSBColor

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | a |  | 
| `Single` | b |  | 
| `Single` | h |  | 
| `Single` | s |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | ToColor() |  | 
| `String` | ToString() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `HSBColor` | FromColor(`Color` color) |  | 
| `HSBColor` | Lerp(`HSBColor` a, `HSBColor` b, `Single` t) |  | 
| `void` | Test() |  | 
| `Color` | ToColor(`HSBColor` hsbColor) |  | 


## `InputFieldConfig`

```csharp
public class MaterialUI.InputFieldConfig
    : MonoBehaviour, ISelectHandler, IEventSystemHandler, IDeselectHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | activeColor |  | 
| `Single` | animationDuration |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | CalculateHeight() |  | 
| `void` | OnDeselect(`BaseEventData` data) |  | 
| `void` | OnSelect(`BaseEventData` data) |  | 


## `MaterialGlobals`

```csharp
public class MaterialUI.MaterialGlobals
    : MonoBehaviour

```

Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Vector4` | shadowSpriteBorder |  | 
| `Single` | uiScale |  | 


## `MaterialUIScaler`

```csharp
public class MaterialUI.MaterialUIScaler
    : MonoBehaviour

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | scaleFactor |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Update() |  | 


## `MenuArrowAnim`

```csharp
public class MaterialUI.MenuArrowAnim
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationDuration |  | 
| `RectTransform` | bottomTransform |  | 
| `Boolean` | isArrow |  | 
| `RectTransform` | middleTransform |  | 
| `RectTransform` | topTransform |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Arrow() |  | 
| `void` | Menu() |  | 
| `void` | Toggle() |  | 


## `NavDrawerConfig`

```csharp
public class MaterialUI.NavDrawerConfig
    : MonoBehaviour, IBeginDragHandler, IEventSystemHandler, IDragHandler, IEndDragHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationDuration |  | 
| `Image` | backgroundImage |  | 
| `Boolean` | darkenBackground |  | 
| `Image` | ShadowImage |  | 
| `Boolean` | tapBackgroundToClose |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | BackgroundTap() |  | 
| `void` | Close() |  | 
| `void` | OnBeginDrag(`PointerEventData` data) |  | 
| `void` | OnDrag(`PointerEventData` data) |  | 
| `void` | OnEndDrag(`PointerEventData` data) |  | 
| `void` | Open() |  | 


## `RadioConfig`

```csharp
public class MaterialUI.RadioConfig
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationDuration |  | 
| `Boolean` | changeRippleColor |  | 
| `Boolean` | changeTextColor |  | 
| `Color` | disabledColor |  | 
| `Color` | offColor |  | 
| `Color` | onColor |  | 
| `Color` | textDisabledColor |  | 
| `Color` | textNormalColor |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnEnable() |  | 
| `void` | ToggleCheckbox(`Boolean` state) |  | 


## `RectTransformSnap`

```csharp
public class MaterialUI.RectTransformSnap
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | percentage |  | 
| `Boolean` | sizeOnly |  | 
| `Boolean` | snapEveryFrame |  | 
| `RectTransform` | targetRect |  | 
| `Single` | xPadding |  | 
| `Single` | xPercent |  | 
| `Single` | yPadding |  | 
| `Single` | yPercent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Snap() |  | 


## `RippleAnim`

```csharp
public class MaterialUI.RippleAnim
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Sprite` | im1024px |  | 
| `Sprite` | im128px |  | 
| `Sprite` | im256px |  | 
| `Sprite` | im384px |  | 
| `Sprite` | im512px |  | 
| `Sprite` | im640px |  | 
| `Sprite` | im64px |  | 
| `Sprite` | im768px |  | 
| `Sprite` | im896px |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ClearRipple() |  | 
| `void` | MakeRipple(`Int32` size, `Single` animSpeed, `Single` startAlpha, `Single` endAlpha, `Color` color, `Vector3` endPosition) |  | 


## `RippleConfig`

```csharp
public class MaterialUI.RippleConfig
    : MonoBehaviour, IPointerEnterHandler, IEventSystemHandler, IPointerDownHandler, IPointerUpHandler, IPointerExitHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | autoSize |  | 
| `Boolean` | dontRippleOnScroll |  | 
| `HighlightActive` | highlightWhen |  | 
| `Boolean` | moveTowardCenter |  | 
| `Color` | rippleColor |  | 
| `Single` | rippleEndAlpha |  | 
| `Int32` | rippleSize |  | 
| `Single` | rippleSpeed |  | 
| `Single` | rippleStartAlpha |  | 
| `Single` | scrollDelayCheckTime |  | 
| `Single` | sizePercentage |  | 
| `Boolean` | toggleMask |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnPointerDown(`PointerEventData` data) |  | 
| `void` | OnPointerEnter(`PointerEventData` data) |  | 
| `void` | OnPointerExit(`PointerEventData` data) |  | 
| `void` | OnPointerUp(`PointerEventData` data) |  | 
| `void` | Refresh() |  | 
| `void` | Setup() |  | 


## `RippleControl`

```csharp
public static class MaterialUI.RippleControl

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Initialize() |  | 
| `GameObject` | MakeRipple(`Vector3` position, `Transform` parent, `Int32` size, `Color` color) |  | 
| `GameObject` | MakeRipple(`Vector3` position, `Transform` parent, `Int32` size, `Single` animSpeed, `Single` startAlpha, `Single` endAlpha, `Color` color) |  | 
| `GameObject` | MakeRipple(`Vector3` position, `Transform` parent, `Int32` size, `Single` animSpeed, `Single` startAlpha, `Single` endAlpha, `Color` color, `Vector3` endPosition) |  | 


## `ScreenConfig`

```csharp
public class MaterialUI.ScreenConfig
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationDuration |  | 
| `RectTransform` | currentRipple |  | 
| `Boolean` | fadeIn |  | 
| `Single` | fadeInStartValue |  | 
| `Boolean` | fadeOut |  | 
| `Single` | fadeOutEndValue |  | 
| `Boolean` | scaleIn |  | 
| `Single` | scaleInStartValue |  | 
| `Boolean` | scaleOut |  | 
| `Single` | scaleOutEndValue |  | 
| `String` | screenName |  | 
| `GameObject` | screenSpace |  | 
| `SlideDirection` | slideIn |  | 
| `Single` | slideInPercent |  | 
| `SlideDirection` | slideOut |  | 
| `Single` | slideOutPercent |  | 
| `TransitionType` | transitionInType |  | 
| `TransitionType` | transitionOutType |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Hide() |  | 
| `void` | HideWithoutTransition() |  | 
| `void` | Show(`ScreenConfig` screenToHide) |  | 
| `void` | Show() |  | 
| `void` | ShowWithoutTransition() |  | 


## `ScreenManager`

```csharp
public class MaterialUI.ScreenManager
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `ScreenConfig` | currentScreen |  | 
| `ScreenConfig` | lastScreen |  | 
| `ScreenConfig[]` | screens |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Back() |  | 
| `void` | Set(`Int32` index) |  | 
| `void` | Set(`String` name) |  | 


## `SelectionBoxConfig`

```csharp
public class MaterialUI.SelectionBoxConfig
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationDuration |  | 
| `Boolean` | autoMaxItemHeight |  | 
| `Image` | cancelLayer |  | 
| `Int32` | currentSelection |  | 
| `PopDirection` | expandDirection |  | 
| `Color` | expandedListColor |  | 
| `Int32` | expandedListShadowLevel |  | 
| `Boolean` | highlightLastSelected |  | 
| `HighlightActive` | highlightWhen |  | 
| `Image` | icon |  | 
| `PickItem` | ItemPicked |  | 
| `String[]` | listItems |  | 
| `GameObject` | listLayer |  | 
| `Int32` | manualMaxItemHeight |  | 
| `Boolean` | moveTowardCenter |  | 
| `Single` | percentageOfScreenHeight |  | 
| `Color` | rippleColor |  | 
| `Boolean` | rippleEnabled |  | 
| `Single` | rippleEndAlpha |  | 
| `Int32` | rippleSize |  | 
| `Single` | rippleSpeed |  | 
| `Single` | rippleStartAlpha |  | 
| `Image` | scrollbar |  | 
| `Text` | selectedText |  | 
| `Image` | textLine |  | 
| `Boolean` | toggleMask |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ContractList() |  | 
| `void` | ExpandList() |  | 
| `void` | Select(`Int32` selectionId) |  | 
| `void` | Setup() |  | 


## `SelectionBoxSubscriber`

```csharp
public class MaterialUI.SelectionBoxSubscriber
    : MonoBehaviour

```

## `SelectionListItemConfig`

```csharp
public class MaterialUI.SelectionListItemConfig
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | listId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SelectMe() |  | 
| `void` | Setup() |  | 


## `ShadowAnim`

```csharp
public class MaterialUI.ShadowAnim
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | anim |  | 
| `Boolean` | isOn |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | SetShadow(`Boolean` set) |  | 


## `ShadowConfig`

```csharp
public class MaterialUI.ShadowConfig
    : MonoBehaviour, IPointerEnterHandler, IEventSystemHandler, IPointerDownHandler, IPointerUpHandler, IPointerExitHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isEnabled |  | 
| `Int32` | shadowActiveSize |  | 
| `Int32` | shadowNormalSize |  | 
| `ShadowAnim[]` | shadows |  | 
| `ShadowsActive` | shadowsActiveWhen |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnPointerDown(`PointerEventData` data) |  | 
| `void` | OnPointerEnter(`PointerEventData` data) |  | 
| `void` | OnPointerExit(`PointerEventData` data) |  | 
| `void` | OnPointerUp(`PointerEventData` data) |  | 
| `void` | SetShadows(`Int32` shadowOn) |  | 


## `ShadowSnap`

```csharp
public class MaterialUI.ShadowSnap
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | percentage |  | 
| `RectTransform` | targetRect |  | 
| `Single` | xPadding |  | 
| `Single` | xPercent |  | 
| `Single` | yPadding |  | 
| `Single` | yPercent |  | 


## `SliderConfig`

```csharp
public class MaterialUI.SliderConfig
    : MonoBehaviour, IPointerDownHandler, IEventSystemHandler, IPointerUpHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationDuration |  | 
| `RectTransform` | handle |  | 
| `Boolean` | hasPopup |  | 
| `RectTransform` | popup |  | 
| `Text` | popupText |  | 
| `Boolean` | textHasDecimal |  | 
| `Boolean` | textIsPercent |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnPointerDown(`PointerEventData` data) |  | 
| `void` | OnPointerUp(`PointerEventData` data) |  | 
| `void` | UpdateText() |  | 


## `SnapButtonToText`

```csharp
public class MaterialUI.SnapButtonToText
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | snapEveryFrame |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Snap() |  | 
| `void` | Update() |  | 


## `SpriteSwapper`

```csharp
public class MaterialUI.SpriteSwapper
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Sprite` | sprite1x |  | 
| `Sprite` | sprite2x |  | 
| `Sprite` | sprite4x |  | 


## `SwitchConfig`

```csharp
public class MaterialUI.SwitchConfig
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | animationDuration |  | 
| `Color` | backDisabledColor |  | 
| `Color` | backOffColor |  | 
| `Boolean` | changeRippleColor |  | 
| `Boolean` | changeTextColor |  | 
| `Color` | disabledColor |  | 
| `Color` | offColor |  | 
| `Color` | onColor |  | 
| `Color` | textDisabledColor |  | 
| `Color` | textNormalColor |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ToggleSwitch() |  | 
| `void` | TurnOff() |  | 
| `void` | TurnOn() |  | 


## `TextInputLine`

```csharp
public class MaterialUI.TextInputLine
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Color` | lineColor |  | 
| `Text` | placeholderText |  | 
| `RectTransform` | textInputRect |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Activate() |  | 
| `void` | Deactivate() |  | 


## `ToastAnim`

```csharp
public class MaterialUI.ToastAnim
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `CanvasGroup` | canvasGroup |  | 
| `Image` | panelImage |  | 
| `Image` | shadowImage |  | 
| `Text` | text |  | 
| `RectTransform` | thisRect |  | 


## `ToastControl`

```csharp
public static class MaterialUI.ToastControl

```

Static Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Canvas` | parentCanvas |  | 
| `Single` | toastDuration |  | 
| `Int32` | toastFontSize |  | 
| `Color` | toastPanelColor |  | 
| `String` | toastText |  | 
| `Color` | toastTextColor |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | InitToastSystem(`Canvas` theCanvas) |  | 
| `void` | MakeToast(`String` content, `Single` duration, `Color` panelColor, `Color` textColor, `Int32` fontSize) |  | 


## `Toaster`

```csharp
public class MaterialUI.Toaster
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | duration |  | 
| `Int32` | fontSize |  | 
| `Color` | panelColor |  | 
| `String` | text |  | 
| `Color` | textColor |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | PopupToast() |  | 


## `ToggleConfig`

```csharp
public class MaterialUI.ToggleConfig
    : MonoBehaviour, IPointerUpHandler, IEventSystemHandler

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | OnPointerUp(`PointerEventData` data) |  | 


## `ValType`

```csharp
public enum MaterialUI.ValType
    : Enum, IComparable, IFormattable, IConvertible

```

Enum

| Value | Name | Summary | 
| --- | --- | --- | 
| `0` | Field |  | 
| `1` | Property |  | 


