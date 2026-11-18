# operit.ui.common.markdown

> 函数 228 · 类型 48 · 顶层常量 50 · 共 326 条
> 每日定时任务自动生成。

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `BareUrl` | `BareUrl` | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | class BareUrl(val start: Int, val end: Int, val url: String) | A bare `http://` or `https://` URL found in plain inline text. [start] and [end] delimit … | 11 |
| `BareUrlLinkifierTest` | `BareUrlLinkifierTest` | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` | class BareUrlLinkifierTest |  | 7 |
| `BatchNodeUpdater` | `BatchNodeUpdater` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | class BatchNodeUpdater(private val nodes: SnapshotStateList<MarkdownNod…, private val renderNodes: SnapshotStateList<MarkdownNod…, private val nodeAnimationStates: MutableMap<String… | 批量节点更新器 - 负责将原始节点列表的更新批量应用到渲染节点列表 | 1131 |
| `CodeBlockColorRange` | `CodeBlockColorRange` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | class CodeBlockColorRange(val start: Int, val end: Int, val colorArgb: Int) |  | 62 |
| `CodeBlockLineRenderData` | `CodeBlockLineRenderData` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | class CodeBlockLineRenderData(val text: String, val colorRanges: List<CodeBlockColorRange>, val rows: List<CodeBlockWrappedRow>, val maxCells: Int) |  | 74 |
| `CodeBlockMetrics` | `CodeBlockMetrics` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | class CodeBlockMetrics(val charWidth: Float, val lineHeight: Float, val baseline: Float) |  | 56 |
| `CodeBlockPreviewType` | `CodeBlockPreviewType` | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | class CodeBlockPreviewType |  | 41 |
| `CodeBlockWrappedRow` | `CodeBlockWrappedRow` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | class CodeBlockWrappedRow(val start: Int, val end: Int, val cells: Int) |  | 68 |
| `DefaultXmlRenderer` | `DefaultXmlRenderer` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | class DefaultXmlRenderer : XmlContentRenderer | 默认XML渲染器 | 264 |
| `DrawInstruction` | `DrawInstruction` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | class DrawInstruction | 绘制指令 - 用于描述如何在 Canvas 上绘制内容 | 342 |
| `DrawInstruction.LayoutResult` | `DrawInstruction` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | class LayoutResult(val height: Float, val actualWidth: Float, val instructions: List<DrawInstruction>) | 布局计算结果 - 包含高度、实际使用的宽度和绘制指令 | 369 |
| `DrawInstruction.Line` | `DrawInstruction` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | class Line(val startX: Float, val startY: Float, val endX: Float, val endY: Float, val paint: android.graphics.Paint) : DrawInstruction |  | 350 |
| `DrawInstruction.Text` | `DrawInstruction` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | class Text(val text: String, val x: Float, val y: Float, val paint: android.graphics.Paint) : DrawInstruction |  | 343 |
| `DrawInstruction.TextLayout` | `DrawInstruction` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | class TextLayout(val layout: StaticLayout, val x: Float, val y: Float, val text: CharSequence?) : DrawInstruction |  | 358 |
| `EnhancedTableBlockAndroidTest` | `EnhancedTableBlockAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlockAndroidTest.kt` | class EnhancedTableBlockAndroidTest |  | 31 |
| `FontSizes` | `FontSizes` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | class FontSizes(val bodyMedium: TextUnit, val headlineLarge: TextUnit, val headlineMedium: TextUnit, val headlineSmall: TextUnit, val titleLarge: TextUnit, val titleMedium: T… | 字体大小数据类 | 494 |
| `InlineCodeMarkerSpan` | `InlineCodeMarkerSpan` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | class InlineCodeMarkerSpan(val backgroundColor: Int, val textScale: Float, val horizontalPaddingPx: Float, val verticalInsetPx: Float, val cornerRadiusPx: Float) |  | 138 |
| `InlineCodeStyleSpan` | `InlineCodeStyleSpan` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | class InlineCodeStyleSpan(private val textScale: Float) : MetricAffectingSpan |  | 120 |
| `InlineCodeTextRange` | `InlineCodeTextRange` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | class InlineCodeTextRange(val start: Int, val end: Int) |  | 146 |
| `LatexDrawableSpan` | `LatexDrawableSpan` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | class LatexDrawableSpan(private val drawable: Drawable) : ReplacementSpan | Places a formula around the surrounding text's visual center instead of aligning the draw… | 44 |
| `LayoutCache` | `LayoutCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | object LayoutCache |  | 270 |
| `LayoutCache.LayoutKey` | `LayoutCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | class LayoutKey(val text: String, val colorArgb: Int, val textSize: Float, val width: Int, val typeface: Typeface, val letterSpacing: Float, val lineSpacingMultiplier: Float) |  | 271 |
| `MarkdownCodeTypefaceCache` | `MarkdownCodeTypefaceCache` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownCodeTypeface.kt` | object MarkdownCodeTypefaceCache |  | 7 |
| `MarkdownGroupedItem` | `MarkdownGroupedItem` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownNodeGrouper.kt` | class MarkdownGroupedItem |  | 10 |
| `MarkdownGroupedItem.MarkdownNodeGrouper` | `MarkdownGroupedItem` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownNodeGrouper.kt` | interface MarkdownNodeGrouper |  | 20 |
| `MarkdownGroupedItem.Single` | `MarkdownGroupedItem` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownNodeGrouper.kt` | class Single(val index: Int) : MarkdownGroupedItem |  | 11 |
| `MarkdownNodeCache` | `MarkdownNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | object MarkdownNodeCache | A cache for parsed markdown nodes to improve performance. | 689 |
| `MarkdownPlainTextRendererAndroidTest` | `MarkdownPlainTextRendererAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRendererAndroidTest.kt` | class MarkdownPlainTextRendererAndroidTest |  | 12 |
| `MarkdownRenderMode` | `MarkdownRenderMode` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | class MarkdownRenderMode |  | 84 |
| `NestedInlineNodeCache` | `NestedInlineNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | object NestedInlineNodeCache |  | 95 |
| `NoopMarkdownNodeGrouper` | `NoopMarkdownNodeGrouper` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownNodeGrouper.kt` | object NoopMarkdownNodeGrouper : MarkdownNodeGrouper |  | 40 |
| `PaintCache` | `PaintCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | object PaintCache | Paint 对象池 - 避免重复创建相同样式的 Paint | 178 |
| `PaintCache.PaintKey` | `PaintCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | class PaintKey(val colorArgb: Int, val textSize: Float, val typeface: Typeface, val letterSpacingEm: Float) |  | 179 |
| `PendingLineBreakState` | `PendingLineBreakState` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | class PendingLineBreakState(val count: Int, val lastWasCarriageReturn: Boolean) |  | 91 |
| `RenderBatchCoordinator` | `RenderBatchCoordinator` | `com.ai.assistance.operit.ui.common.markdown` | `RenderBatchCoordinator.kt` | class RenderBatchCoordinator(private val scope: CoroutineScope, private val intervalMs: Long, private val onFlush: () -> Unit) | Coalesces render updates without losing the last mutation. Requests must be made after re… | 14 |
| `RenderBatchCoordinatorTest` | `RenderBatchCoordinatorTest` | `com.ai.assistance.operit.ui.common.markdown` | `RenderBatchCoordinatorTest.kt` | class RenderBatchCoordinatorTest |  | 17 |
| `StreamMarkdownRendererState` | `StreamMarkdownRendererState` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | class StreamMarkdownRendererState | StreamMarkdownRenderer的状态类 用于在流式渲染和静态渲染之间共享状态，避免切换时重新计算 | 328 |
| `TableCellRenderData` | `TableCellRenderData` | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | class TableCellRenderData(val layout: StaticLayout, val isHeader: Boolean) |  | 77 |
| `TableData` | `TableData` | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | class TableData(val rows: List<List<String>>, val hasHeader: Boolean) | 供表格渲染和复制为纯文本共用的表格解析结果。 | 72 |
| `TableRenderLayout` | `TableRenderLayout` | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | class TableRenderLayout(val columnWidthsPx: List<Int>, val rowHeightsPx: List<Int>, val cells: List<List<TableCellRenderData…, val totalWidthPx: Int, val totalHeightPx: Int, val rowC… |  | 82 |
| `XmlContentRenderer` | `XmlContentRenderer` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | interface XmlContentRenderer | XML内容渲染器接口，用于自定义XML渲染 | 242 |
| `XmlRenderPluginRegistry` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | object XmlRenderPluginRegistry |  | 91 |
| `XmlRenderPluginRegistryTest` | `XmlRenderPluginRegistryTest` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistryTest.kt` | class XmlRenderPluginRegistryTest |  | 10 |
| `XmlRenderPluginRegistryTest.FixedTagPlugin` | `XmlRenderPluginRegistryTest` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistryTest.kt` | class FixedTagPlugin(override val id: String, private val tags: Set<String>) : XmlRenderPlugin |  | 11 |
| `XmlRenderResult` | `XmlRenderResult` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | class XmlRenderResult |  | 45 |
| `XmlRenderResult.ComposableRender` | `XmlRenderResult` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | class ComposableRender(val render: (Modifier, Color, Stream<Stri…) : XmlRenderResult |  | 46 |
| `XmlRenderResult.Text` | `XmlRenderResult` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | class Text(val text: String) : XmlRenderResult |  | 50 |
| `XmlRenderResult.XmlRenderPlugin` | `XmlRenderResult` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | interface XmlRenderPlugin |  | 61 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `EnhancedTableBlockAndroidTest.streamingContentUpdate_keepsHorizontalScrollInteractive` | `EnhancedTableBlockAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlockAndroidTest.kt` |  | Unit |  | 37 ⚑ |
| `MarkdownPlainTextRendererAndroidTest.render` | `MarkdownPlainTextRendererAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRendererAndroidTest.kt` | markdown: String<br>latexToPlainText: (List<String>) -> List<String>? | String |  | 14 ⚑ |
| `MarkdownPlainTextRendererAndroidTest.markdownToPlainTextForCopy_preservesSingleLineUserText` | `MarkdownPlainTextRendererAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRendererAndroidTest.kt` |  | Unit |  | 19 ⚑ |
| `MarkdownPlainTextRendererAndroidTest.markdownToPlainTextForCopy_removesFormattingMarkers` | `MarkdownPlainTextRendererAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRendererAndroidTest.kt` |  | Unit |  | 24 ⚑ |
| `MarkdownPlainTextRendererAndroidTest.markdownToPlainTextForCopy_preservesCodeBlockContent` | `MarkdownPlainTextRendererAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRendererAndroidTest.kt` |  | Unit |  | 48 ⚑ |
| `MarkdownPlainTextRendererAndroidTest.markdownToPlainTextForCopy_convertsTableToTabbedText` | `MarkdownPlainTextRendererAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRendererAndroidTest.kt` |  | Unit |  | 67 ⚑ |
| `MarkdownPlainTextRendererAndroidTest.markdownToPlainTextForCopy_preservesLatexContent` | `MarkdownPlainTextRendererAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRendererAndroidTest.kt` |  | Unit |  | 78 ⚑ |
| `MarkdownPlainTextRendererAndroidTest.markdownToPlainTextForCopy_doesNotConvertLatexInsideCode` | `MarkdownPlainTextRendererAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRendererAndroidTest.kt` |  | Unit |  | 106 ⚑ |
| `MarkdownPlainTextRendererAndroidTest.markdownToPlainTextForCopy_batchesAllLatexFromClassicFormulaSample` | `MarkdownPlainTextRendererAndroidTest` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRendererAndroidTest.kt` |  | Unit |  | 123 ⚑ |
| `findBareUrls` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | text: CharSequence | List<BareUrl> | Returns every bare `http`/`https` URL in [text], in source order. The scan is local to on… | 32 |
| `schemeLengthAt` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | text: CharSequence<br>index: Int | Int |  | 79 |
| `matchesPrefixAt` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | index: Int<br>prefix: String | Boolean |  | 90 |
| `trimUrlTail` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | text: CharSequence<br>bodyStart: Int<br>bodyEnd: Int | Int | Trims what the surrounding prose contributed rather than what the writer put into the URL… | 101 |
| `isUrlBodyCodePoint` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | codePoint: Int | Boolean | URL text includes Unicode letters, numbers and combining marks as well as URI punctuation… | 143 |
| `isUrlHostStart` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | text: CharSequence<br>index: Int | Boolean |  | 153 |
| `isAsciiLetterOrDigit` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | char: Char | Boolean |  | 157 |
| `drawOnlyWhenVisible` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` |  | Modifier | 通用性能优化 Modifier：仅在组件进入屏幕可见区域时才进行绘制。 实现原理： 1. 使用 `onGloballyPositioned` 监听组件的布局位置和大小。 2. 获… | 92 |
| `trimAll` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` |  | String | 扩展函数：去除字符串首尾的所有空白字符 | 122 |
| `trimAllPreservingSpans` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` |  | CharSequence |  | 126 |
| `splitPlainTextParagraphs` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | content: CharSequence | List<CharSequence> |  | 141 |
| `PaintCache.getPaint` | `PaintCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | color: Color<br>textSize: Float<br>typeface: Typeface | android.graphics.Paint |  | 189 |
| `PaintCache.getTextPaint` | `PaintCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | color: Color<br>textSize: Float<br>typeface: Typeface<br>letterSpacingEm: Float | TextPaint |  | 201 |
| `PaintCache.clear` | `PaintCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` |  | Unit |  | 219 |
| `safeLayoutWidth` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | width: Int | Int | StaticLayout 缓存 - 避免重复创建相同的 StaticLayout 使用 LRU 策略，最多缓存 100 个 | 229 |
| `calculateCanvasLetterSpacingEm` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | fontSize: TextUnit<br>letterSpacingSp: Float | Float |  | 231 |
| `calculateCanvasLineSpacingMultiplier` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | lineHeightMultiplier: Float | Float |  | 239 |
| `createSafeInlineStaticLayout` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | children: List<MarkdownNodeStable><br>fallbackText: CharSequence<br>textColor: Color<br>primaryColor: Color<br>density: Density?<br>fontSize: TextUnit?<br>textPaint: TextPaint<br>width: Int<br>lineSpacingMultiplier: Float<br>contextLabel: … | StaticLayout |  | 243 |
| `LayoutCache.getLayout` | `LayoutCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | text: String<br>paint: TextPaint<br>width: Int<br>color: Color<br>typeface: Typeface<br>lineSpacingMultiplier: Float | StaticLayout |  | 283 |
| `LayoutCache.clear` | `LayoutCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` |  | Unit |  | 307 |
| `LayoutCache.createStaticLayout` | `LayoutCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | text: String<br>paint: TextPaint<br>width: Int<br>lineSpacingMultiplier: Float | StaticLayout |  | 311 |
| `DrawInstruction.extractAccessibleText` | `DrawInstruction` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | instructions: List<DrawInstruction> | String | 从绘制指令中提取文本内容用于无障碍朗读 | 378 |
| `CanvasMarkdownNodeRenderer` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | nodeKey: String<br>node: MarkdownNodeStable<br>textColor: Color<br>fontSize: TextUnit?<br>modifier: Modifier?<br>onLinkClick: ((String) -> Unit)??<br>index: Int<br>xmlRenderer: XmlContentRenderer<br>xmlStream: Stream<String>??<br>enableDia… | Unit | Canvas 版本的 Markdown 节点渲染器 优化策略： - 使用单个大 Canvas 绘制所有简单文本（标题、段落、列表项） - 复杂组件（代码块、表格、LaTeX）保留… | 416 |
| `scaleMarkdownTextUnit` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | base: TextUnit<br>scale: Float | TextUnit |  | 504 |
| `renderNodeContent` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | nodeKey: String<br>node: MarkdownNodeStable<br>content: String<br>textColor: Color<br>fontSizes: FontSizes<br>density: Density<br>modifier: Modifier<br>onLinkClick: ((String) -> Unit)?<br>xmlRenderer: XmlContentRenderer<br>xmlStream: Strea… | Unit |  | 515 |
| `UnifiedCanvasRenderer` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | nodeKey: String<br>node: MarkdownNodeStable<br>textColor: Color<br>bodyMediumSize: TextUnit<br>headlineLargeSize: TextUnit<br>headlineMediumSize: TextUnit<br>headlineSmallSize: TextUnit<br>titleLargeSize: TextUnit<br>titleMediumSize: TextU… | Unit | 统一的 Canvas 渲染器 在一个大 Canvas 中绘制标题、段落、列表等简单文本 | 797 |
| `calculateActualWidth` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | layout: StaticLayout<br>offsetX: Float?<br>availableWidthPx: Int | Float | 计算 StaticLayout 的实际使用宽度（取所有行的最大宽度） | 1195 |
| `calculateLayout` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | node: MarkdownNodeStable<br>textColor: Color<br>primaryColor: Color<br>bodyMediumSize: TextUnit<br>headlineLargeSize: TextUnit<br>headlineMediumSize: TextUnit<br>headlineSmallSize: TextUnit<br>titleLargeSize: TextUnit<br>titleMediumSize: T… | LayoutResult | 计算布局和生成绘制指令 | 1213 |
| `buildSpannableFromChildren` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | children: List<MarkdownNodeStable><br>textColor: Color<br>primaryColor: Color<br>density: Density??<br>fontSize: TextUnit?? | SpannableStringBuilder |  | 1594 |
| `SingleTextCanvas` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | text: String<br>textColor: Color<br>fontSize: TextUnit<br>fontWeight: FontWeight<br>density: Density<br>modifier: Modifier? | Unit | 单个文本的 Canvas 渲染器（用于引用块等简单场景） | 1614 |
| `SafeMeasureOrFallback` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | fallback: () -> Unit<br>content: () -> Unit | Unit |  | 1706 |
| `determineHeaderLevel` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | content: String | Int | 判断标题级别 | 1736 |
| `extractLatexContent` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | content: String | String | 提取LaTeX内容，移除各种分隔符 | 1745 |
| `createStaticLayout` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | text: CharSequence<br>paint: TextPaint<br>width: Int<br>lineSpacingMultiplier: Float | StaticLayout |  | 1755 |
| `CanvasMonospaceCodeBlockBody` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | code: String<br>codeLines: List<String><br>highlightedLines: List<AnnotatedString>?<br>autoWrapEnabled: Boolean<br>maxScrollableHeight: Dp<br>modifier: Modifier? | Unit |  | 85 |
| `flingOffset` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | animatable: Animatable<Float, AnimationVector1D><br>startValue: Float<br>initialVelocity: Float<br>maxOffset: Float<br>onUpdate: (Float) -> Unit | Unit |  | 337 |
| `canConsumeVerticalDrag` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | deltaY: Float | Boolean |  | 358 |
| `canConsumeHorizontalDrag` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | deltaX: Float | Boolean |  | 366 |
| `isVerticalDominantGesture` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | delta: Offset | Boolean |  | 374 |
| `shouldClaimDrag` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | totalDelta: Offset | Boolean |  | 378 |
| `shouldYieldDragToParent` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | delta: Offset | Boolean |  | 391 |
| `updateOffsets` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | deltaX: Float<br>deltaY: Float | Boolean |  | 402 |
| `requestPointerFocus` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` |  | Unit |  | 415 |
| `startGestureCapture` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` |  | Unit |  | 424 |
| `stopGestureCapture` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` |  | Unit |  | 433 |
| `buildCodeBlockLineRenderData` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | line: AnnotatedString<br>autoWrapEnabled: Boolean<br>maxColumns: Int<br>defaultTextColorArgb: Int | CodeBlockLineRenderData |  | 644 |
| `buildCodeBlockColorRanges` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | line: AnnotatedString<br>defaultTextColorArgb: Int | List<CodeBlockColorRange> |  | 660 |
| `wrapCodeBlockRows` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | text: String<br>autoWrapEnabled: Boolean<br>maxColumns: Int | List<CodeBlockWrappedRow> |  | 703 |
| `measureCodeBlockCells` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | text: String | Int |  | 743 |
| `findFirstVisibleCodeLine` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | lineTopsPx: FloatArray<br>lineHeightsPx: FloatArray<br>targetTopPx: Float | Int |  | 757 |
| `findLastVisibleCodeLine` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | lineTopsPx: FloatArray<br>targetBottomPx: Float | Int |  | 778 |
| `drawCodeBlockRow` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | canvas: AndroidCanvas<br>text: String<br>row: CodeBlockWrappedRow<br>colorRanges: List<CodeBlockColorRange><br>defaultColorArgb: Int<br>textPaint: Paint<br>systemGlyphPaint: Paint<br>charWidthPx: Float<br>startX: Float<br>baseline: Float | Unit |  | 797 |
| `colorForOffset` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | targetOffset: Int | Int |  | 821 |
| `flushRun` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` |  | Unit |  | 833 |
| `shouldRenderWithSystemGlyphs` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | codePoint: Int | Boolean |  | 888 |
| `shouldRenderWithSystemGlyphs` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | text: CharSequence<br>start: Int<br>end: Int | Boolean |  | 898 |
| `EnhancedCodeBlock` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | code: String<br>language: String?<br>modifier: Modifier? | Unit | 增强型代码块组件 具有以下功能： 1. 代码语法高亮 2. 复制按钮 3. 行号显示 4. 夜间模式风格 5. 行渲染保护（使用key机制避免重复渲染） 6. 记忆优化（减少不必… | 60 |
| `MermaidRenderer` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | code: String<br>modifier: Modifier? | Unit | Mermaid图表渲染组件 | 342 |
| `shouldOverrideUrlLoading` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | view: android.webkit.WebView<br>url: String | Boolean |  | 612 |
| `onPageFinished` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | view: android.webkit.WebView<br>url: String | Unit |  | 620 |
| `HtmlPreviewRenderer` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | code: String<br>modifier: Modifier? | Unit |  | 681 |
| `shouldOverrideUrlLoading` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | view: android.webkit.WebView<br>url: String | Boolean |  | 697 |
| `highlightSyntaxLine` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | line: String<br>language: String | AnnotatedString | 处理单行代码的语法高亮 | 748 |
| `appendWord` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` |  | Unit |  | 976 |
| `EnhancedTableBlock` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | tableContent: String<br>modifier: Modifier?<br>textColor: Color?<br>onLinkClick: ((String) -> Unit)?? | Unit |  | 96 |
| `cancelFling` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` |  | Unit |  | 178 |
| `startFling` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | initialVelocityPxPerSec: Float | Unit |  | 183 |
| `measureTableLayout` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | tableData: TableData<br>textColor: Color<br>density: androidx.compose.ui.unit.Density<br>bodyTextStyle: androidx.compose.ui.text.TextStyle<br>normalTypeface: Typeface<br>boldTypeface: Typeface<br>primaryColor: Color<br>globalLineHeightMult… | TableRenderLayout |  | 420 |
| `createCellStaticLayout` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | text: CharSequence<br>paint: TextPaint<br>widthPx: Int<br>lineSpacingMultiplier: Float | StaticLayout |  | 561 |
| `measureCellDesiredWidth` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | text: CharSequence<br>paint: TextPaint<br>widthPx: Int<br>lineSpacingMultiplier: Float | Float |  | 588 |
| `lineCountHint` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` |  | Int |  | 607 |
| `layoutLineHeightFallback` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | paint: TextPaint | Int |  | 612 |
| `calculateLetterSpacingEm` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | fontSizeSp: Float<br>letterSpacingSp: Float | Float |  | 617 |
| `parseTable` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | content: String | TableData | 将原始 Markdown 表格文本解析成行列结构，供渲染和复制为纯文本共用。 | 623 |
| `isHeaderSeparatorLine` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | line: String | Boolean |  | 624 |
| `parseCells` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | line: String | MutableList<String> |  | 630 |
| `normalizeMarkdownMediaUrl` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownAudioRenderer.kt` | url: String | String |  | 33 |
| `isLikelyAudioUrl` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownAudioRenderer.kt` | url: String | Boolean |  | 41 |
| `MarkdownAudioRenderer` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownAudioRenderer.kt` | audioMarkdown: String<br>modifier: Modifier? | Unit |  | 47 |
| `MarkdownCodeTypefaceCache.get` | `MarkdownCodeTypefaceCache` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownCodeTypeface.kt` | context: Context | Typeface |  | 11 |
| `getMarkdownCodeTypeface` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownCodeTypeface.kt` | context: Context | Typeface |  | 25 |
| `getMarkdownCodeTypeface` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownCodeTypeface.kt` |  | Typeface |  | 29 |
| `isCompleteImageMarkdown` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownImageRenderer.kt` | content: String | Boolean | 判断Markdown图片语法是否完整 检查是否有完整的 ![alt](url) 语法 | 72 |
| `extractMarkdownImageAlt` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownImageRenderer.kt` | imageContent: String | String | 从Markdown图片语法中提取Alt文本 | 80 |
| `extractMarkdownImageUrl` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownImageRenderer.kt` | imageContent: String | String | 从Markdown图片语法中提取URL | 92 |
| `isLargeImage` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownImageRenderer.kt` | url: String | Boolean | 判断是否为大图片 简单根据图片URL后缀来判断 | 103 |
| `MarkdownImageRenderer` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownImageRenderer.kt` | imageMarkdown: String<br>modifier: Modifier?<br>maxImageHeight: Int?<br>enableDialogs: Boolean? | Unit | Markdown图片渲染器组件 支持流式渲染和图片预览功能 | 111 |
| `FullScreenImageDialog` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownImageRenderer.kt` | imageUrl: String<br>imageAlt: String<br>onDismiss: () -> Unit | Unit | 全屏图片预览对话框 | 240 |
| `saveImageFromUrl` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownImageRenderer.kt` | context: Context<br>imageUrl: String | Boolean | 从URL保存图片到设备相册 | 434 |
| `LatexDrawableSpan.getSize` | `LatexDrawableSpan` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | paint: Paint<br>text: CharSequence<br>start: Int<br>end: Int<br>fontMetrics: Paint.FontMetricsInt? | Int |  | 54 |
| `LatexDrawableSpan.draw` | `LatexDrawableSpan` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | canvas: Canvas<br>text: CharSequence<br>start: Int<br>end: Int<br>x: Float<br>top: Int<br>baseline: Int<br>bottom: Int<br>paint: Paint | Unit |  | 75 |
| `NestedInlineNodeCache.getOrParse` | `NestedInlineNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | content: String | List<MarkdownNodeStable> |  | 100 |
| `inlineCodeBackgroundColor` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | textColor: Color | Int |  | 115 |
| `InlineCodeStyleSpan.updateDrawState` | `InlineCodeStyleSpan` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | textPaint: android.text.TextPaint | Unit |  | 123 |
| `InlineCodeStyleSpan.updateMeasureState` | `InlineCodeStyleSpan` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | textPaint: android.text.TextPaint | Unit |  | 127 |
| `InlineCodeStyleSpan.applyStyle` | `InlineCodeStyleSpan` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | textPaint: android.text.TextPaint | Unit |  | 131 |
| `createInlineCodeStyleSpan` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` |  | InlineCodeStyleSpan |  | 151 |
| `createInlineCodeMarkerSpan` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | textColor: Color<br>density: Density? | InlineCodeMarkerSpan |  | 155 |
| `createInlineCodePaint` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | basePaint: Paint<br>marker: InlineCodeMarkerSpan | Paint |  | 169 |
| `inlineCodeRangeAt` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | text: CharSequence<br>offset: Int | InlineCodeTextRange? |  | 177 |
| `selectedTextWithInlineCodeMarkers` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | text: CharSequence<br>start: Int<br>end: Int | CharSequence |  | 198 |
| `drawInlineCodeBackgrounds` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | layout: StaticLayout<br>canvas: Canvas | Unit |  | 245 |
| `stripUnderlineDelimiters` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | content: String | String |  | 299 |
| `extractInlineLatexContent` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | content: String | String |  | 307 |
| `appendInlineLatexFallback` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | builder: SpannableStringBuilder<br>rawContent: String | Unit |  | 317 |
| `resolveNestedInlineText` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | node: MarkdownNodeStable | String |  | 324 |
| `resolveNestedInlineChildren` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | node: MarkdownNodeStable | List<MarkdownNodeStable> |  | 333 |
| `appendInlineNode` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | builder: SpannableStringBuilder<br>child: MarkdownNodeStable<br>textColor: Color<br>primaryColor: Color<br>density: Density??<br>fontSize: TextUnit??<br>visitedNodes: Set<MarkdownNodeStable>?<br>depth: Int?<br>linkifyBareText: Boolean? | Unit |  | 357 |
| `appendLinkifiedText` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | builder: SpannableStringBuilder<br>text: String<br>primaryColor: Color | Unit | Appends [text] and gives every bare http/https URL in it the same [URLSpan] the explicit … | 566 |
| `buildMarkdownInlineSpannableFromChildren` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | children: List<MarkdownNodeStable><br>textColor: Color<br>primaryColor: Color<br>density: Density??<br>fontSize: TextUnit?? | SpannableStringBuilder |  | 598 |
| `buildMarkdownInlineSpannableFromText` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | text: String<br>textColor: Color<br>primaryColor: Color<br>density: Density??<br>fontSize: TextUnit?? | SpannableStringBuilder |  | 612 |
| `MarkdownGroupedItem.MarkdownNodeGrouper.group` | `MarkdownNodeGrouper` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownNodeGrouper.kt` | nodes: List<MarkdownNodeStable><br>rendererId: String | List<MarkdownGroupedItem> |  | 21 |
| `MarkdownGroupedItem.MarkdownNodeGrouper.RenderGroup` | `MarkdownNodeGrouper` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownNodeGrouper.kt` | group: MarkdownGroupedItem.Group<br>nodes: List<MarkdownNodeStable><br>rendererId: String<br>isVisible: Boolean<br>isLastNode: Boolean<br>modifier: Modifier<br>textColor: Color<br>onLinkClick: ((String) -> Unit)?<br>xmlRenderer: XmlContent… | Unit |  | 24 |
| `NoopMarkdownNodeGrouper.group` | `NoopMarkdownNodeGrouper` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownNodeGrouper.kt` | nodes: List<MarkdownNodeStable><br>rendererId: String | List<MarkdownGroupedItem> |  | 41 |
| `NoopMarkdownNodeGrouper.RenderGroup` | `NoopMarkdownNodeGrouper` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownNodeGrouper.kt` | group: MarkdownGroupedItem.Group<br>nodes: List<MarkdownNodeStable><br>rendererId: String<br>isVisible: Boolean<br>isLastNode: Boolean<br>modifier: Modifier<br>textColor: Color<br>onLinkClick: ((String) -> Unit)?<br>xmlRenderer: XmlContent… | Unit |  | 46 |
| `markdownToPlainTextForCopy` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | markdown: String<br>latexToPlainText: (List<String>) -> List<String>? | String | 把消息内容解析为适合直接粘贴的纯文本，复用 [parseMarkdownToNodes] 产出的同一份 AST， 保证"复制出来的内容"和屏幕上渲染的内容共享同一套边界判断（代码… | 11 |
| `joinBlocks` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | nodes: List<MarkdownNodeStable><br>latexSegments: MutableList<String> | String | 逐个拼接顶层节点：相邻的列表项（有序/无序混排也算）之间只用单个换行， 其余相邻块之间空一行；HTML_BREAK 节点本身不参与渲染，只是原始 Markdown 里空行数量的标… | 41 |
| `isListItem` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` |  | Boolean |  | 55 |
| `renderBlockNode` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | node: MarkdownNodeStable<br>latexSegments: MutableList<String> | String |  | 58 |
| `renderInlineBlock` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | node: MarkdownNodeStable<br>latexSegments: MutableList<String> | String |  | 74 |
| `plainInlineText` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | latexSegments: MutableList<String> | String |  | 79 |
| `resolvedChildrenText` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | node: MarkdownNodeStable<br>latexSegments: MutableList<String> | String |  | 92 |
| `renderCodeBlock` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | content: String | String |  | 98 |
| `renderTable` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | content: String<br>latexSegments: MutableList<String> | String |  | 109 |
| `renderRawInlineText` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | raw: String<br>latexSegments: MutableList<String> | String |  | 115 |
| `registerLatex` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | formula: String<br>latexSegments: MutableList<String> | String |  | 121 |
| `latexPlaceholder` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownPlainTextRenderer.kt` | index: Int | String |  | 127 |
| `isLikelyVideoUrl` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownVideoRenderer.kt` | url: String | Boolean |  | 37 |
| `MarkdownVideoRenderer` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownVideoRenderer.kt` | videoMarkdown: String<br>modifier: Modifier?<br>maxVideoHeight: Int? | Unit |  | 43 |
| `RenderBatchCoordinator.requestUpdate` | `RenderBatchCoordinator` | `com.ai.assistance.operit.ui.common.markdown` | `RenderBatchCoordinator.kt` |  | Unit |  | 23 |
| `appendPendingLineBreaks` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | parentNode: MarkdownNode<br>childNode: MarkdownNode<br>count: Int | Unit |  | 96 |
| `accumulatePendingLineBreak` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | state: PendingLineBreakState<br>char: Char | PendingLineBreakState |  | 111 |
| `appendInlineChunk` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | parentNode: MarkdownNode<br>getOrCreateChildNode: () -> MarkdownNode<br>chunk: String<br>pendingLineBreakState: PendingLineBreakState | PendingLineBreakState |  | 129 |
| `canMergeWithHtmlBreak` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | node: MarkdownNode? | Boolean |  | 166 |
| `replaceRollbackTail` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | nodes: SnapshotStateList<MarkdownNode><br>rollbackNodes: List<MarkdownNode><br>xmlNodeStreams: MutableMap<Int, Stream<String>> | Unit |  | 170 |
| `appendHtmlBreakNode` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | nodes: SnapshotStateList<MarkdownNode><br>count: Int? | Unit |  | 193 |
| `appendHtmlBreakNode` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | nodes: MutableList<MarkdownNode><br>count: Int? | Unit |  | 202 |
| `toStableNode` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` |  | MarkdownNodeStable | Converts a mutable [MarkdownNode] to an immutable, stable [MarkdownNodeStable]. This func… | 215 |
| `areRenderNodesSynchronized` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | nodes: SnapshotStateList<MarkdownNode><br>renderNodes: SnapshotStateList<MarkdownNodeStabl… | Boolean |  | 223 |
| `XmlContentRenderer.RenderXmlContent` | `XmlContentRenderer` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | xmlContent: String<br>modifier: Modifier<br>textColor: Color<br>xmlStream: Stream<String>?<br>renderInstanceKey: Any? | Unit |  | 244 |
| `RenderXmlContent` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | xmlContent: String<br>modifier: Modifier<br>textColor: Color<br>renderInstanceKey: Any?? | Unit |  | 254 |
| `DefaultXmlRenderer.RenderXmlContent` | `DefaultXmlRenderer` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | xmlContent: String<br>modifier: Modifier<br>textColor: Color<br>xmlStream: Stream<String>?<br>renderInstanceKey: Any? | Unit |  | 266 |
| `trimAll` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` |  | String | 扩展函数：去除字符串首尾的所有空白字符（包括空格、制表符、换行符等） 与标准trim()相比，这个函数更明确地处理所有类型的空白字符 | 319 |
| `StreamMarkdownRendererState.updateRendererId` | `StreamMarkdownRendererState` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | id: String | Unit | 更新渲染器ID | 348 |
| `StreamMarkdownRendererState.reset` | `StreamMarkdownRendererState` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` |  | Unit | 重置所有状态（用于切换内容源时） | 355 |
| `replaceStaticNodes` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | rendererId: String<br>parsedNodes: List<MarkdownNode> | Unit |  | 365 |
| `StreamMarkdownRenderer` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | markdownStream: Stream<Char><br>modifier: Modifier?<br>textColor: Color?<br>fontSize: TextUnit?<br>backgroundColor: Color?<br>onLinkClick: ((String) -> Unit)??<br>xmlRenderer: XmlContentRenderer?<br>nodeGrouper: MarkdownNodeGrouper?<br>sta… | Unit | 高性能流式Markdown渲染组件 通过Jetpack Compose实现，支持流式渲染Markdown内容 使用Stream处理系统，实现高效的异步处理 | 381 |
| `MarkdownNodeCache.sizeOf` | `MarkdownNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | key: String<br>value: List<MarkdownNode> | Int |  | 699 |
| `MarkdownNodeCache.get` | `MarkdownNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | key: String | List<MarkdownNode>? |  | 706 |
| `MarkdownNodeCache.put` | `MarkdownNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | key: String<br>value: List<MarkdownNode> | Unit |  | 710 |
| `MarkdownNodeCache.estimateNodeListBytes` | `MarkdownNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | nodes: List<MarkdownNode> | Long |  | 714 |
| `MarkdownNodeCache.estimateNodeBytes` | `MarkdownNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | node: MarkdownNode | Long |  | 722 |
| `MarkdownNodeCache.estimateStringBytes` | `MarkdownNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | text: String | Long |  | 732 |
| `parseMarkdownToNodes` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | content: String | List<MarkdownNode> | 将完整的 Markdown 字符串解析为 [MarkdownNode] 树，不依赖 Compose 状态。 静态渲染入口与其他需要完整 AST 的场景（如复制为纯文本）复用同一套… | 741 |
| `StreamMarkdownRenderer` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | content: String<br>modifier: Modifier?<br>textColor: Color?<br>fontSize: TextUnit?<br>backgroundColor: Color?<br>onLinkClick: ((String) -> Unit)??<br>xmlRenderer: XmlContentRenderer?<br>nodeGrouper: MarkdownNodeGrouper?<br>state: StreamMar… | Unit | 高性能静态Markdown渲染组件 接受一个完整的字符串，一次性解析和渲染，适用于静态内容显示。 | 875 |
| `AnimatedNode` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | nodeKey: String<br>node: MarkdownNodeStable<br>index: Int<br>isVisible: Boolean<br>textColor: Color<br>fontSize: TextUnit<br>onLinkClick: ((String) -> Unit)?<br>xmlRenderer: XmlContentRenderer<br>xmlStream: Stream<String>?<br>enableDialogs… | Unit | 独立的动画节点组件 - 隔离 alpha 动画状态，避免触发父组件重组 关键优化： - alpha 动画状态被隔离在这个组件内部 - 动画状态变化不会触发外部 Column 重组… | 1000 |
| `UnifiedMarkdownCanvas` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | nodes: List<MarkdownNodeStable><br>rendererId: String<br>nodeAnimationStates: Map<String, Boolean><br>textColor: Color<br>fontSize: TextUnit<br>onLinkClick: ((String) -> Unit)?<br>xmlRenderer: XmlContentRenderer<br>xmlStreamsByIndex: Map<I… | Unit |  | 1044 |
| `nodeKeyForIndex` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | index: Int | String |  | 1063 |
| `BatchNodeUpdater.requestUpdate` | `BatchNodeUpdater` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` |  | Unit |  | 1146 |
| `BatchNodeUpdater.requestStructuralUpdate` | `BatchNodeUpdater` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` |  | Unit |  | 1148 |
| `BatchNodeUpdater.appendBlockChunk` | `BatchNodeUpdater` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | node: MarkdownNode<br>contentChunk: String | Unit |  | 1153 |
| `BatchNodeUpdater.performBatchUpdate` | `BatchNodeUpdater` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` |  | Unit |  | 1158 |
| `synchronizeRenderNodes` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | nodes: SnapshotStateList<MarkdownNode><br>renderNodes: SnapshotStateList<MarkdownNodeStabl…<br>nodeAnimationStates: MutableMap<String, Boolean><br>xmlNodeStreams: MutableMap<Int, Stream<String>><br>rendererId: String<br>scope: CoroutineSco… | Unit | 同步渲染节点 - 确保所有节点都被渲染 在流处理完成或出现异常时调用，确保最终状态一致 | 1171 |
| `extractLinkText` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | linkContent: String | String | 从链接Markdown中提取链接文本 例如：从 [链接文本](https://example.com) 中提取 "链接文本" | 1225 |
| `extractLinkUrl` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | linkContent: String | String | 从链接Markdown中提取链接URL 例如：从 [链接文本](https://example.com) 中提取 "https://example.com" | 1238 |
| `XmlRenderResult.XmlRenderPlugin.supports` | `XmlRenderPlugin` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | tagName: String | Boolean |  | 64 |
| `XmlRenderResult.XmlRenderPlugin.resolve` | `XmlRenderPlugin` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | context: Context<br>xmlContent: String<br>tagName: String<br>textColor: Color<br>xmlStream: Stream<String>? | XmlRenderResult? |  | 66 |
| `buildXmlRenderComposeDslExecutionContextKey` | — | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | containerPackageName: String<br>screenPath: String<br>renderInstanceKey: Any? | String |  | 75 |
| `XmlRenderPluginRegistry.register` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | plugin: XmlRenderPlugin | Unit |  | 98 |
| `XmlRenderPluginRegistry.unregister` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | pluginId: String | Unit |  | 105 |
| `XmlRenderPluginRegistry.supportsTag` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | tagName: String | Boolean | 非 Compose 环境的渲染器查询。 消息处理链路（例如 Waifu 分句、XML 过滤）需要知道某个标签是否由插件渲染器接管， 才能只保留合法渲染标签（如 voice）而丢弃… | 119 |
| `XmlRenderPluginRegistry.notifyChanged` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` |  | Unit |  | 126 |
| `XmlRenderPluginRegistry.RenderIfMatched` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | xmlContent: String<br>tagName: String<br>modifier: Modifier<br>textColor: Color<br>xmlStream: Stream<String>?<br>renderInstanceKey: Any?? | Boolean |  | 131 |
| `XmlRenderPluginRegistry.RenderComposeDslScreen` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | result: XmlRenderResult.ComposeDslScreen<br>modifier: Modifier<br>xmlStream: Stream<String>?<br>renderInstanceKey: Any? | Unit |  | 231 |
| `XmlRenderPluginRegistry.buildModuleSpec` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | screenPath: String | Map<String, Any?> |  | 316 |
| `XmlRenderPluginRegistry.buildActionRuntimeOptions` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | screenPath: String | Map<String, Any?> |  | 330 |
| `XmlRenderPluginRegistry.hasPendingTextInputSyncs` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` |  | Boolean |  | 347 |
| `XmlRenderPluginRegistry.awaitPendingTextInputSyncs` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` |  | Unit |  | 349 |
| `XmlRenderPluginRegistry.requestComposeDslTreeRerender` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | source: String | Unit |  | 362 |
| `XmlRenderPluginRegistry.flushTextInputSyncsAndRerender` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` |  | Unit |  | 392 |
| `XmlRenderPluginRegistry.dispatchAction` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | actionId: String<br>payload: Any? | Unit |  | 399 |
| `XmlRenderPluginRegistry.dispatchTextInputAction` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | actionId: String<br>text: String | Unit |  | 431 |
| `BareUrlLinkifierTest.findsHttpsUrlInBodyText` | `BareUrlLinkifierTest` | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 9 ⚑ |
| `BareUrlLinkifierTest.findsHttpUrlAsWell` | `BareUrlLinkifierTest` | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 19 ⚑ |
| `BareUrlLinkifierTest.findsEveryUrlInOneRunInSourceOrder` | `BareUrlLinkifierTest` | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 30 ⚑ |
| `BareUrlLinkifierTest.dropsSentencePeriodAfterUrl` | `BareUrlLinkifierTest` | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 43 ⚑ |
| `BareUrlLinkifierTest.dropsSentencePunctuationAfterUrl` | `BareUrlLinkifierTest` | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 52 ⚑ |
| `keepsQueryAndFragmentBecauseTheyBelongToTheUrl` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 63 ⚑ |
| `dropsClosingParenthesisThatBelongsToTheSentence` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 73 ⚑ |
| `keepsClosingParenthesisThatTheUrlOpened` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 83 ⚑ |
| `dropsOnlyTheUnmatchedClosingParentheses` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 93 ⚑ |
| `stopsBeforeEmphasisMarker` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 104 ⚑ |
| `stopsBeforeFullWidthPunctuation` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 114 ⚑ |
| `findsUrlDirectlyAfterChineseText` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 124 ⚑ |
| `keepsChinesePathQueryAndFragment` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 134 ⚑ |
| `keepsInternationalizedHost` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 144 ⚑ |
| `keepsSupplementaryLettersAndCombiningMarks` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 154 ⚑ |
| `stopsBeforeFullWidthPunctuationAfterChinesePath` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 164 ⚑ |
| `keepsIpv6HostAndPort` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 175 ⚑ |
| `trimsProseBracketsWithoutTrimmingIpv6Host` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 185 ⚑ |
| `normalizesUppercaseSchemeForTheClickHandler` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 196 ⚑ |
| `ignoresSchemeThatIsNotFollowedByAHost` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 207 ⚑ |
| `ignoresSchemeGluedToTheEndOfAWord` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 213 ⚑ |
| `ignoresOtherSchemes` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 218 ⚑ |
| `leavesPlainTextWithoutUrlsUntouched` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 224 ⚑ |
| `reportedRangesSliceTheUrlOutOfTheSourceText` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 230 ⚑ |
| `rangesCoverTheUrlInsideMarkdownLinkSyntax` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 243 ⚑ |
| `rangesContainOnlyUrlCharacters` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` |  | Unit |  | 253 ⚑ |
| `assertUrlAndRange` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` | text: String<br>expectedUrl: String<br>expectedEnd: Int | Unit |  | 262 ⚑ |
| `assertCoversSourceText` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifierTest.kt` | text: String<br>urls: List<BareUrl> | Unit |  | 270 ⚑ |
| `RenderBatchCoordinatorTest.requestWhileBatchIsPending_isIncludedWithoutAnotherInput` | `RenderBatchCoordinatorTest` | `com.ai.assistance.operit.ui.common.markdown` | `RenderBatchCoordinatorTest.kt` |  | Unit |  | 19 ⚑ |
| `RenderBatchCoordinatorTest.requestDuringFlush_isDrainedBeforeCoordinatorBecomesIdle` | `RenderBatchCoordinatorTest` | `com.ai.assistance.operit.ui.common.markdown` | `RenderBatchCoordinatorTest.kt` |  | Unit |  | 37 ⚑ |
| `RenderBatchCoordinatorTest.toolXmlTailMutation_isRenderedWithoutAnotherInput` | `RenderBatchCoordinatorTest` | `com.ai.assistance.operit.ui.common.markdown` | `RenderBatchCoordinatorTest.kt` |  | Unit |  | 59 ⚑ |
| `RenderBatchCoordinatorTest.equalLengthBlockNodeReplacement_isRendered` | `RenderBatchCoordinatorTest` | `com.ai.assistance.operit.ui.common.markdown` | `RenderBatchCoordinatorTest.kt` |  | Unit |  | 88 ⚑ |
| `RenderBatchCoordinatorTest.equalLengthChildNodeReplacement_isRendered` | `RenderBatchCoordinatorTest` | `com.ai.assistance.operit.ui.common.markdown` | `RenderBatchCoordinatorTest.kt` |  | Unit |  | 112 ⚑ |
| `XmlRenderPluginRegistryTest.FixedTagPlugin.supports` | `FixedTagPlugin` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistryTest.kt` | tagName: String | Boolean |  | 15 ⚑ |
| `XmlRenderPluginRegistryTest.FixedTagPlugin.resolve` | `FixedTagPlugin` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistryTest.kt` | context: Context<br>xmlContent: String<br>tagName: String<br>textColor: Color<br>xmlStream: Stream<String>? | XmlRenderResult |  | 17 ⚑ |
| `XmlRenderPluginRegistryTest.supportsTag_tracksRegistrationLifecycle` | `XmlRenderPluginRegistryTest` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistryTest.kt` |  | Unit |  | 27 ⚑ |
| `XmlRenderPluginRegistryTest.supportsTag_multiplePluginsDoNotShadowEachOther` | `XmlRenderPluginRegistryTest` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistryTest.kt` |  | Unit |  | 43 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `CodeDefaultTextColor` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | inferred |  | 81 |
| `CodeLineNumberColor` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMonospaceCodeBlockBody.kt` | inferred |  | 82 |
| `DEFAULT_CANVAS_LINE_SPACING_MULTIPLIER` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 74 |
| `DEFAULT_PARAGRAPH_BREAK_DP` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 75 |
| `FADE_IN_DURATION_MS` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | inferred |  | 81 |
| `FALLBACK_MAX_TEXT_CHARS` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 77 |
| `HTTP_PREFIX` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | inferred |  | 17 |
| `HTTPS_PREFIX` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | inferred |  | 18 |
| `INLINE_LATEX_PLACEHOLDER` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | inferred |  | 33 |
| `LayoutCache.cache` | `LayoutCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 281 |
| `LocalMarkdownRenderMode` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | inferred |  | 89 |
| `MARKDOWN_AUDIO_EXTENSIONS` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownAudioRenderer.kt` | inferred |  | 30 |
| `MARKDOWN_VIDEO_EXTENSIONS` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownVideoRenderer.kt` | inferred |  | 34 |
| `MarkdownCodeTypefaceCache.cachedTypeface` | `MarkdownCodeTypefaceCache` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownCodeTypeface.kt` | Typeface? |  | 9 |
| `MarkdownNodeCache.cache` | `MarkdownNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | inferred |  | 697 |
| `MarkdownNodeCache.maxCacheBytes` | `MarkdownNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | inferred | Limit static markdown cache by estimated bytes instead of entry count, so incre… | 692 |
| `MAX_CANVAS_HEIGHT_PX` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 71 |
| `MAX_COMPOSE_CONSTRAINT_HEIGHT_PX` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 72 |
| `MAX_CONSECUTIVE_RENDERED_NEWLINES` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | inferred |  | 82 |
| `MAX_INLINE_RENDER_DEPTH` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | inferred |  | 34 |
| `NestedInlineNodeCache.cache` | `NestedInlineNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | inferred |  | 98 |
| `NestedInlineNodeCache.MAX_ENTRIES` | `NestedInlineNodeCache` | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | inferred |  | 96 |
| `nestedScrollInterop` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | inferred | 渲染WebView | 673 |
| `PaintCache.paintCache` | `PaintCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 186 |
| `PaintCache.textPaintCache` | `PaintCache` | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 187 |
| `RENDER_INTERVAL_MS` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | inferred |  | 80 |
| `TABLE_BORDER_WIDTH` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 63 |
| `TABLE_CELL_HORIZONTAL_PADDING` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 59 |
| `TABLE_CELL_VERTICAL_PADDING` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 60 |
| `TABLE_CORNER_RADIUS` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 62 |
| `TABLE_FLING_DECAY_RATE` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 67 |
| `TABLE_GRID_WIDTH` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 64 |
| `TABLE_LINE_SPACING_MULTIPLIER` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 66 |
| `TABLE_MAX_COLUMN_WIDTH` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 58 |
| `TABLE_MAX_FLING_VELOCITY` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 69 |
| `TABLE_MAX_MEASURE_LINE_CHARS` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 65 |
| `TABLE_MIN_COLUMN_WIDTH` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 57 |
| `TABLE_MIN_FLING_VELOCITY` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 68 |
| `TABLE_OUTER_VERTICAL_PADDING` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedTableBlock.kt` | inferred |  | 61 |
| `TAG` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 70 |
| `TAG` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownImageRenderer.kt` | inferred |  | 69 |
| `TAG` | — | `com.ai.assistance.operit.ui.common.markdown` | `MarkdownInlineSpannable.kt` | inferred |  | 32 |
| `TAG` | — | `com.ai.assistance.operit.ui.common.markdown` | `StreamMarkdownRenderer.kt` | inferred |  | 79 |
| `TRAILING_SENTENCE_PUNCTUATION` | — | `com.ai.assistance.operit.ui.common.markdown` | `BareUrlLinkifier.kt` | inferred | Characters that may follow a URL in prose without belonging to it. A `.` is by … | 24 |
| `TYPEWRITER_WINDOW_MS` | — | `com.ai.assistance.operit.ui.common.markdown` | `CanvasMarkdownNodeRenderer.kt` | inferred |  | 73 |
| `webView` | — | `com.ai.assistance.operit.ui.common.markdown` | `EnhancedCodeBlock.kt` | inferred | 记住WebView实例以便重用 | 593 |
| `XmlRenderPluginRegistry.changeVersion` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | StateFlow<Int> |  | 95 |
| `XmlRenderPluginRegistry.changeVersionMutable` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | inferred |  | 94 |
| `XmlRenderPluginRegistry.plugins` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | inferred |  | 93 |
| `XmlRenderPluginRegistry.TAG` | `XmlRenderPluginRegistry` | `com.ai.assistance.operit.ui.common.markdown` | `XmlRenderPluginRegistry.kt` | inferred |  | 92 |
