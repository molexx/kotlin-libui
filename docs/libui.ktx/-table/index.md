[libui.ktx](../index.md) / [Table](./index.md)

# Table

`class Table<T> : `[`Disposable`](../-disposable/index.md)`<`[`uiTableModel`](../../libui/ui-table-model.md)`>`

Wrapper class for [uiTableModel](../../libui/ui-table-model.md)

### Types

| Name | Summary |
|---|---|
| [TableColumn](-table-column/index.md) | `inner class TableColumn<T>` |

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `Table(data: List<`[`T`](-table-column/index.md#T)`>, handler: CPointer<`[`ktTableHandler`](../../libui/kt-table-handler/index.md)`> = nativeHeap.alloc<ktTableHandler>().ptr)`<br>Wrapper class for [uiTableModel](../../libui/ui-table-model.md) |

### Properties

| Name | Summary |
|---|---|
| [data](data.md) | `val data: List<`[`T`](-table-column/index.md#T)`>` |

### Inherited Properties

| Name | Summary |
|---|---|
| [disposed](../-disposable/disposed.md) | `val disposed: Boolean`<br>Returns `true` if object was disposed - in this case [dispose](../-disposable/dispose.md) will do nothing, all other operations are invalid and will `throw Error("Resource is disposed")`. |

### Functions

| Name | Summary |
|---|---|
| [background](background.md) | `fun background(get: (row: Int) -> `[`Color`](../../libui.ktx.draw/-color/index.md)`?): Unit` |
| [column](column.md) | `fun column(name: String, init: `[`TableColumn`](-table-column/index.md)`<`[`T`](-table-column/index.md#T)`>.() -> Unit): Unit` |
| [rowChanged](row-changed.md) | `fun rowChanged(index: Int): Unit` |
| [rowDeleted](row-deleted.md) | `fun rowDeleted(oldIndex: Int): Unit` |
| [rowInserted](row-inserted.md) | `fun rowInserted(newIndex: Int): Unit` |

### Inherited Functions

| Name | Summary |
|---|---|
| [dispose](../-disposable/dispose.md) | `open fun dispose(): Unit`<br>Dispose and free all allocated native resources. |

### Extension Functions

| Name | Summary |
|---|---|
| [image](../../libui.ktx.draw/image.md) | `fun `[`Table`](./index.md)`<*>.image(width: Int, height: Int, block: `[`Image`](../../libui.ktx.draw/-image/index.md)`.() -> Unit = {}): `[`Image`](../../libui.ktx.draw/-image/index.md) |
