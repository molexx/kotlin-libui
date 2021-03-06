[libui.ktx](../index.md) / [Disposable](./index.md)

# Disposable

`abstract class Disposable<T : CPointed>`

Base class for all objects that have a holder reference to the native C resource(s).

* Allocates one resource during construction,
    and may allocate some additional resources during operation.
* Must free all its resource once [dispose](dispose.md) is invoked.
* [disposed](disposed.md) is a final state of the class, it is not supposed
    to be used after being disposed.

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `Disposable(alloc: CPointer<`[`T`](index.md#T)`>?)`<br>Base class for all objects that have a holder reference to the native C resource(s). |

### Properties

| Name | Summary |
|---|---|
| [disposed](disposed.md) | `val disposed: Boolean`<br>Returns `true` if object was disposed - in this case [dispose](dispose.md) will do nothing, all other operations are invalid and will `throw Error("Resource is disposed")`. |

### Functions

| Name | Summary |
|---|---|
| [dispose](dispose.md) | `open fun dispose(): Unit`<br>Dispose and free all allocated native resources. |

### Inheritors

| Name | Summary |
|---|---|
| [Attribute](../../libui.ktx.draw/-attribute/index.md) | `abstract class Attribute : `[`Disposable`](./index.md)`<`[`uiAttribute`](../../libui/ui-attribute.md)`>`<br>Stores information about an attribute in a [AttributedString](../../libui.ktx.draw/-attributed-string/index.md). |
| [AttributedString](../../libui.ktx.draw/-attributed-string/index.md) | `class AttributedString : `[`Disposable`](./index.md)`<`[`uiAttributedString`](../../libui/ui-attributed-string.md)`>`<br>Represents a string of UTF-8 text that can be embellished with formatting attributes. |
| [Brush](../../libui.ktx.draw/-brush/index.md) | `class Brush : `[`Disposable`](./index.md)`<`[`uiDrawBrush`](../../libui/ui-draw-brush/index.md)`>`<br>Defines the color(s) to draw a path with. |
| [Control](../-control/index.md) | `abstract class Control<T : CPointed> : `[`Disposable`](./index.md)`<`[`T`](../-control/index.md#T)`>`<br>Base class for all GUI controls (widgets). |
| [Font](../../libui.ktx.draw/-font/index.md) | `class Font : `[`Disposable`](./index.md)`<`[`uiFontDescriptor`](../../libui/ui-font-descriptor/index.md)`>`<br>Provides a complete description of a font where one is needed. |
| [Image](../../libui.ktx.draw/-image/index.md) | `class Image : `[`Disposable`](./index.md)`<`[`uiImage`](../../libui/ui-image.md)`>` |
| [Matrix](../../libui.ktx.draw/-matrix/index.md) | `class Matrix : `[`Disposable`](./index.md)`<`[`uiDrawMatrix`](../../libui/ui-draw-matrix/index.md)`>`<br>Defines a transformation (e.g. rotation, translation) |
| [OpenTypeFeatures](../../libui.ktx.draw/-open-type-features/index.md) | `class OpenTypeFeatures : `[`Disposable`](./index.md)`<`[`uiOpenTypeFeatures`](../../libui/ui-open-type-features.md)`>`<br>Represents a set of OpenType feature tag-value pairs, for applying OpenType features to text. |
| [Path](../../libui.ktx.draw/-path/index.md) | `class Path : `[`Disposable`](./index.md)`<`[`uiDrawPath`](../../libui/ui-draw-path.md)`>`<br>Represent a path that could be drawed on a [DrawContext](../-draw-context.md) |
| [Stroke](../../libui.ktx.draw/-stroke/index.md) | `class Stroke : `[`Disposable`](./index.md)`<`[`uiDrawStrokeParams`](../../libui/ui-draw-stroke-params/index.md)`>`<br>Describes the stroke to draw with. |
| [Table](../-table/index.md) | `class Table<T> : `[`Disposable`](./index.md)`<`[`uiTableModel`](../../libui/ui-table-model.md)`>`<br>Wrapper class for [uiTableModel](../../libui/ui-table-model.md) |
| [TextLayout](../../libui.ktx.draw/-text-layout/index.md) | `class TextLayout : `[`Disposable`](./index.md)`<`[`uiDrawTextLayout`](../../libui/ui-draw-text-layout.md)`>`<br>Representation of a [AttributedString](../../libui.ktx.draw/-attributed-string/index.md) that can be displayed in a [DrawContext](../-draw-context.md). |
