## `Heap<T>`

```csharp
public class Assets.Heap<T>

```

Fields

| Type | Name | Summary | 
| --- | --- | --- | 
| `T[]` | items |  | 


Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | Count |  | 
| `Int32` | Max |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Add(`T` item) |  | 
| `Boolean` | Contains(`T` item) |  | 
| `T` | RemoveFirst() |  | 
| `void` | UpdateItem(`T` item) |  | 


## `IHeapItem<T>`

```csharp
public interface Assets.IHeapItem<T>
    : IComparable<T>

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | HeapIndex |  | 


