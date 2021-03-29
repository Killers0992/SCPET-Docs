## `Inventory`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.Inventory
    : NetworkBehaviour, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | CurItem |  | 
| `Int32` | CurWornItem |  | 
| `Boolean` | disablePickUpClientSound |  | 
| `SyncList<ItemBase>` | Items |  | 
| `String` | page |  | 
| `PlayerController` | plrCtrl |  | 
| `List<SaveItem>` | saveItems |  | 
| `AudioClip` | shoot1 |  | 
| `AudioSource` | src |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | current |  | 
| `ItemBase` | currentWorn |  | 
| `String` | Guid |  | 
| `Int32` | NetworkCurItem |  | 
| `Int32` | NetworkCurWornItem |  | 
| `String` | Networkpage |  | 
| `String` | PrefabGuid |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | ChangeCurItem(`Int32` old, `Int32` cur) |  | 
| `void` | ClearDropInv() |  | 
| `void` | ClearInv() |  | 
| `void` | ClientCraftItem(`Int32` item1, `Int32` item2) |  | 
| `void` | ClientDropItemIndex(`Int32` index) |  | 
| `void` | ClientEquipItem(`Int32` index) |  | 
| `void` | ClientUnEquipItem(`Int32` index) |  | 
| `void` | CmdCraftItems(`Int32` index1, `Int32` index2) |  | 
| `void` | CmdDropItemIndex(`Int32` index) |  | 
| `void` | CmdEquipItem(`Int32` index) |  | 
| `void` | CmdUnEquipItem(`Int32` index) |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | DestroyItem(`Int32` index) |  | 
| `Boolean` | Interact(`GameObject` other) |  | 
| `void` | LoadComplete() |  | 
| `IEnumerator` | LoadLate() |  | 
| `void` | OnDestroy() |  | 
| `Boolean` | PickupItem(`ItemBase` item, `GameObject` itemObject) |  | 
| `void` | RemoveItem(`Int32` index) |  | 
| `void` | RpcSetInventory(`Int32` item, `Int32` wornItem) |  | 
| `void` | RpcShootSound1() |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 
| `void` | UserCode_CmdCraftItems(`Int32` index1, `Int32` index2) |  | 
| `void` | UserCode_CmdDropItemIndex(`Int32` index) |  | 
| `void` | UserCode_CmdEquipItem(`Int32` index) |  | 
| `void` | UserCode_CmdUnEquipItem(`Int32` index) |  | 
| `void` | UserCode_RpcSetInventory(`Int32` item, `Int32` wornItem) |  | 
| `void` | UserCode_RpcShootSound1() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Skeleton_CmdCraftItems(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdDropItemIndex(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdEquipItem(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_CmdUnEquipItem(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcSetInventory(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 
| `void` | Skeleton_RpcShootSound1(`NetworkBehaviour` obj, `NetworkReader` reader, `INetworkConnection` senderConnection, `Int32` replyId) |  | 


## `Item1499Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.Item1499Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemAmmo`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemAmmo
    : ItemBase, SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | ammo |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetAmmo() |  | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | SetAmmo(`Int32` ammo) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


## `ItemAmmoSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemAmmoSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemAnomGasmask`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemAnomGasmask
    : ItemBase, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsWornItem |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 


## `ItemAnomGasmaskSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemAnomGasmaskSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemBadge`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBadge
    : ItemBase, SaveState, ItemKeycardID

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | name |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Access |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 


## `ItemBadgeSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBadgeSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemBase`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBase
    : SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Inventory` | inv |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `GameObject` | gameObject |  | 
| `Boolean` | IsWornItem |  | 
| `String` | ItemId |  | 
| `String` | TypeName |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 
| `Boolean` | OnInteract(`GameObject` other) |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnUnEquip() |  | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


## `ItemBaseReadWrite`

```csharp
public static class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBaseReadWrite

```

Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | ReadBase(this `NetworkReader` reader) |  | 
| `void` | WriteBase(this `NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemBaseSerializer`

```csharp
public abstract class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemBaseUI`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBaseUI
    : MonoBehaviour, IPointerClickHandler, IEventSystemHandler, IPointerEnterHandler, IPointerExitHandler, IBeginDragHandler, IEndDragHandler, IDragHandler

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | index |  | 
| `ItemBase` | item |  | 


## `ItemBattery`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBattery
    : ItemBase, SaveState, ItemCraftable

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Craft(`ItemCraftable` other, `ItemBase&` final) |  | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 


## `ItemBatterySerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBatterySerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemBVGoggles`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBVGoggles
    : ItemBase, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsWornItem |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnUnEquip() |  | 


## `ItemBVGogglesSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemBVGogglesSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemCraftable`

```csharp
public interface VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemCraftable

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Craft(`ItemCraftable` other, `ItemBase&` final) |  | 


## `ItemCup`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemCup
    : ItemBase, SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | DrinkId |  | 
| `Boolean` | IsEmpty |  | 
| `String` | Name |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Apply294Effect(`PlayerController` plr, `String[]` args) |  | 


## `ItemCupSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemCupSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemDocument`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemDocument
    : ItemBase, SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | Document |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 


## `ItemDocumentSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemDocumentSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemEyedrops`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemEyedrops
    : ItemBase, SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Double` | strength |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 


## `ItemEyedropsSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemEyedropsSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemFlashlight`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemFlashlight
    : ItemBase, SaveState, ItemMelee

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | battery |  | 
| `Boolean` | IsDirty |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | FireRate |  | 
| `String` | ItemId |  | 
| `Single` | Range |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 
| `Boolean` | OnUnEquip() |  | 
| `void` | Swing(`Inventory` ctrl) |  | 


## `ItemFlashlightSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemFlashlightSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemGasmask`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemGasmask
    : ItemBase, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsWornItem |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 


## `ItemGasmaskSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemGasmaskSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemIVGoggles`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemIVGoggles
    : ItemBase, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsWornItem |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnUnEquip() |  | 


## `ItemIVGogglesSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemIVGogglesSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemJanitor1`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemJanitor1
    : ItemBase, SaveState, ItemKeycardID

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | name |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Access |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 


## `ItemJanitor1Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemJanitor1Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemKeycard`

```csharp
public interface VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | Level |  | 


## `ItemKeycard0`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard0
    : ItemBase, SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | material |  | 
| `Texture` | texture |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnInteract(`GameObject` other) |  | 


## `ItemKeycard0Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard0Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemKeycard1`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard1
    : ItemBase, SaveState, ItemKeycard

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | material |  | 
| `Texture` | texture |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 
| `Int32` | Level |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 


## `ItemKeycard1Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard1Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemKeycard2`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard2
    : ItemBase, SaveState, ItemKeycard

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | material |  | 
| `Texture` | texture |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 
| `Int32` | Level |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 


## `ItemKeycard2Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard2Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemKeycard3`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard3
    : ItemBase, SaveState, ItemKeycard

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | material |  | 
| `Texture` | texture |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 
| `Int32` | Level |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 


## `ItemKeycard3Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard3Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemKeycard4`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard4
    : ItemBase, SaveState, ItemKeycard

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | material |  | 
| `Texture` | texture |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 
| `Int32` | Level |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 


## `ItemKeycard4Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard4Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemKeycard5`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard5
    : ItemBase, SaveState, ItemKeycard

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | material |  | 
| `Texture` | texture |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 
| `Int32` | Level |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 


## `ItemKeycard5Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycard5Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemKeycardID`

```csharp
public interface VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemKeycardID

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Access |  | 


## `ItemMedkit`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemMedkit
    : ItemBase, SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Double` | healing |  | 
| `Single` | severityReduction |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 


## `ItemMedkitSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemMedkitSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemMedkitSmall`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemMedkitSmall
    : ItemBase, SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Double` | healing |  | 
| `Single` | severityReduction |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 


## `ItemMedkitSmallSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemMedkitSmallSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemMelee`

```csharp
public interface VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemMelee

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | FireRate |  | 
| `Single` | Range |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Swing(`Inventory` ctrl) |  | 


## `ItemNVGoggles`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemNVGoggles
    : ItemBase, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsWornItem |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnUnEquip() |  | 


## `ItemNVGogglesSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemNVGogglesSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemP90`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemP90
    : ItemBase, SaveState, ItemWeapon, IEquatable<ItemBase>

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | ammo |  | 
| `Boolean` | IsDirty |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | FireRate |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Equals(`Object` obj) |  | 
| `Boolean` | Equals(`ItemBase` other) |  | 
| `Int32` | GetAmmo() |  | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 
| `Boolean` | OnUnEquip() |  | 
| `void` | SetAmmo(`Int32` ammo) |  | 
| `void` | Shoot(`Inventory` ctrl) |  | 


## `ItemP90Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemP90Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemPowered`

```csharp
public interface VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemPowered

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | CurrentPower |  | 
| `Single` | DrainRate |  | 
| `Single` | MaxPower |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Drain() |  | 
| `void` | OnDead() |  | 
| `void` | WhenPoweredOn() |  | 


## `ItemRadio`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemRadio
    : ItemBase, SaveState, ItemPowered, ItemCraftable

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | CurrentPower |  | 
| `Single` | DrainRate |  | 
| `String` | ItemId |  | 
| `Single` | MaxPower |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Craft(`ItemCraftable` other, `ItemBase&` final) |  | 
| `void` | Drain() |  | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `void` | OnDead() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 
| `void` | WhenPoweredOn() |  | 


## `ItemRadioSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemRadioSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemRing`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemRing
    : ItemBase, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsWornItem |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 


## `ItemRingSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemRingSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemSCP035`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSCP035
    : ItemBase, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnPickup(`GameObject` plr, `GameObject` item) |  | 


## `ItemSCP035Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSCP035Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemSCP1025`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSCP1025
    : ItemBase, SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | currentPage |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 


## `ItemSCP1025Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSCP1025Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemSCP1499`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSCP1499
    : ItemBase, SaveState

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | isIn |  | 
| `JSONVector` | position |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | IsWornItem |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 
| `Boolean` | OnEquip() |  | 
| `Boolean` | OnUnEquip() |  | 


## `ItemSCP500`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSCP500
    : ItemBase, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnEquip() |  | 


## `ItemSCP500Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSCP500Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemSCP860`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSCP860
    : ItemBase, SaveState

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 


## `ItemSCP860Serializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSCP860Serializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemSNav`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSNav
    : ItemBase, SaveState, ItemCraftable

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | CurrentPower |  | 
| `Single` | DrainRate |  | 
| `String` | ItemId |  | 
| `Single` | MaxPower |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | Craft(`ItemCraftable` other, `ItemBase&` final) |  | 
| `Texture` | GetItemIcon() |  | 
| `String` | GetItemName() |  | 
| `Boolean` | OnDrop(`GameObject` plr, `GameObject` item) |  | 


## `ItemSNavSerializer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemSNavSerializer
    : ItemBaseSerializer

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `ItemBase` | Read(`NetworkReader` reader, `String` id) |  | 
| `void` | Write(`NetworkWriter` writer, `ItemBase` item) |  | 


## `ItemWeapon`

```csharp
public interface VirtualBrightPlayz.SCP_ET.Items.ItemSystem.ItemWeapon

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Single` | FireRate |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | GetAmmo() |  | 
| `void` | SetAmmo(`Int32` ammo) |  | 
| `void` | Shoot(`Inventory` ctrl) |  | 


## `SNavUI`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.SNavUI
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RawImage` | bg |  | 
| `Boolean` | equipped |  | 
| `GameObject` | playerBox |  | 
| `GameObject` | roomBox |  | 
| `List<IRoom>` | rooms |  | 
| `Single` | scale |  | 
| `GameObject` | snavMask |  | 
| `List<SNavUIRoom>` | spawnedMap |  | 
| `List<SNavUIPlayer>` | spawnedPlayers |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Update() |  | 
| `void` | UpdateRoomCache() |  | 


## `SNavUIPlayer`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.SNavUIPlayer
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RawImage` | image |  | 
| `PlayerController` | player |  | 


## `SNavUIRoom`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.SNavUIRoom
    : MonoBehaviour

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `RawImage` | image |  | 
| `IRoom` | room |  | 


## `WorldItem1025`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItem1025
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 
| `void` | LoadFromItem(`ItemBase` item) |  | 


## `WorldItem1499`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItem1499
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemAmmo`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemAmmo
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | ammo |  | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemAnomGasmask`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemAnomGasmask
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemBadge`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemBadge
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Access |  | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `String` | itemName |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 
| `void` | LoadFromItem(`ItemBase` item) |  | 


## `WorldItemBase`

```csharp
public abstract class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemBase
    : NetworkBehaviour, IInteractable, ISavable

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Boolean` | CanUse |  | 
| `String` | Guid |  | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 
| `InteractType` | IType |  | 
| `String` | PrefabGuid |  | 
| `JSONVector` | savePos |  | 
| `JSONVector` | saveRot |  | 
| `JSONVector` | saveScl |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 
| `void` | Highlighted() |  | 
| `void` | LoadComplete() |  | 
| `void` | LoadFromItem(`ItemBase` item) |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | StartUseOnce(`PlayerController` user, `Boolean` isLocal, `String&` status, `ButtonErrorType&` errorType) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


## `WorldItemBattery`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemBattery
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemBVGoggles`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemBVGoggles
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemCup`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemCup
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `String` | DrinkId |  | 
| `Boolean` | gizmo |  | 
| `Boolean` | IsEmpty |  | 
| `String` | Name |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


## `WorldItemDocument`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemDocument
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `String` | Document |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 
| `void` | Read(`BinaryReader` reader) |  | 
| `void` | Write(`BinaryWriter` writer) |  | 


## `WorldItemEyedrops`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemEyedrops
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 
| `Double` | strength |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemFlashlight`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemFlashlight
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Int32` | battery |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemGasmask`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemGasmask
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemIVGoggles`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemIVGoggles
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemJanitor1`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemJanitor1
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `String[]` | Access |  | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `String` | itemName |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 
| `void` | LoadFromItem(`ItemBase` item) |  | 


## `WorldItemKeycard0`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemKeycard0
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Texture` | icon |  | 
| `Int32` | level |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 
| `Int32` | Networklevel |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 


## `WorldItemKeycard1`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemKeycard1
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Texture` | icon |  | 
| `Int32` | level |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 
| `Int32` | Networklevel |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DeserializeSyncVars(`NetworkReader` reader, `Boolean` initialState) |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 
| `Boolean` | SerializeSyncVars(`NetworkWriter` writer, `Boolean` initialize) |  | 


## `WorldItemKeycard2`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemKeycard2
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Texture` | icon |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemKeycard3`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemKeycard3
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Texture` | icon |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemKeycard4`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemKeycard4
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Texture` | icon |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemKeycard5`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemKeycard5
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Texture` | icon |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemMedkit`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemMedkit
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Double` | healing |  | 
| `Outline` | outline |  | 
| `Single` | severityReduction |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemMedkitSmall`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemMedkitSmall
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Double` | healing |  | 
| `Outline` | outline |  | 
| `Single` | severityReduction |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemNVGoggles`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemNVGoggles
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemP90`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemP90
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | ammo |  | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemRadio`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemRadio
    : WorldItemBase, IInteractable, ISavable, IWorldRadio

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 
| `Single` | power |  | 
| `AudioSource` | source |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 
| `void` | OnDisable() |  | 
| `void` | OnEnable() |  | 
| `void` | PlayData(`Single[]` data, `Int32` pos) |  | 
| `void` | Stop() |  | 


## `WorldItemRing`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemRing
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemSCP035`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemSCP035
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Texture` | icon |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemSCP500`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemSCP500
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemSCP860`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemSCP860
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `Collider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


## `WorldItemSNav`

```csharp
public class VirtualBrightPlayz.SCP_ET.Items.ItemSystem.WorldItemSNav
    : WorldItemBase, IInteractable, ISavable

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `BoxCollider` | basecollider |  | 
| `Boolean` | gizmo |  | 
| `Outline` | outline |  | 
| `Single` | power |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Type` | ItemBase |  | 
| `String` | ItemId |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | AddItemRW() |  | 
| `void` | DrawGizmo() |  | 
| `ItemBase` | GetAsItemBase(`Inventory` plr) |  | 


