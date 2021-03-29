## `CommandGroup`

```csharp
public class CommandUndoRedo.CommandGroup
    : ICommand

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Add(`ICommand` command) |  | 
| `void` | Clear() |  | 
| `void` | Execute() |  | 
| `void` | Remove(`ICommand` command) |  | 
| `void` | Set(`List<ICommand>` commands) |  | 
| `void` | UnExecute() |  | 


## `DropoutStack<T>`

```csharp
public class CommandUndoRedo.DropoutStack<T>
    : LinkedList<T>, ICollection<T>, IEnumerable<T>, IEnumerable, ICollection, IReadOnlyCollection<T>, ISerializable, IDeserializationCallback

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | maxLength |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `T` | Pop() |  | 
| `void` | Push(`T` item) |  | 


## `ICommand`

```csharp
public interface CommandUndoRedo.ICommand

```

Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Execute() |  | 
| `void` | UnExecute() |  | 


## `UndoRedo`

```csharp
public class CommandUndoRedo.UndoRedo

```

Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | maxUndoStored |  | 


Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clear() |  | 
| `void` | Execute(`ICommand` command) |  | 
| `void` | Insert(`ICommand` command) |  | 
| `void` | Redo() |  | 
| `void` | Undo() |  | 


## `UndoRedoManager`

```csharp
public static class CommandUndoRedo.UndoRedoManager

```

Static Properties

| Type | Name | Summary | 
| --- | --- | --- | 
| `Int32` | maxUndoStored |  | 


Static Methods

| Type | Name | Summary | 
| --- | --- | --- | 
| `void` | Clear() |  | 
| `void` | Execute(`ICommand` command) |  | 
| `void` | Insert(`ICommand` command) |  | 
| `void` | Redo() |  | 
| `void` | Undo() |  | 


