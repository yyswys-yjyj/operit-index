# operit.ui.features.chat.webview.workspace.editor

> 函数 212 · 类型 14 · 顶层常量 22 · 共 248 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `CanvasCodeEditorView` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | class CanvasCodeEditorView(context: Context, attrs: AttributeSet?, defStyleAttr: Int) : SurfaceView |  | 55 |
| `CanvasCodeEditorView.DragHandle` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | class DragHandle |  | 72 |
| `CanvasCodeEditorView.HandleCenters` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | class HandleCenters(val start: PointF, val end: PointF) |  | 78 |
| `CodeFormatter` | `CodeFormatter` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | object CodeFormatter | 代码格式化工具，支持 JavaScript、CSS、HTML 的基本格式化 | 8 |
| `EditorCompletionCallback` | `EditorCompletionCallback` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | interface EditorCompletionCallback |  | 49 |
| `EditorDocument` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | class EditorDocument(initialText: String) |  | 266 |
| `EditorEditCommand` | `EditorEditCommand` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | class EditorEditCommand(val start: Int, val beforeText: String, val afterText: String, val beforeSelectionStart: Int, val beforeSelectionEnd: Int, val afterSelectionStart: Int, val a… |  | 256 |
| `EditorInputConnection` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | class EditorInputConnection(this: , true: ) : BaseInputConnection |  | 1760 |
| `EditorMetrics` | `EditorMetrics` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorMetrics.kt` | class EditorMetrics(private val paint: Paint, textSizePx: Float) |  | 7 |
| `EditorSyntaxHighlighter` | `EditorSyntaxHighlighter` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | class EditorSyntaxHighlighter(initialLanguage: String, private val onResult: (HighlightSnapshot) -> Unit) |  | 18 |
| `HighlightSnapshot` | `HighlightSnapshot` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | class HighlightSnapshot(val version: Int, val colors: IntArray) |  | 13 |
| `LanguageDetector` | `LanguageDetector` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `LanguageDetector.kt` | object LanguageDetector | 根据文件名检测编程语言 | 6 |
| `NativeCodeEditor` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | class NativeCodeEditor(context: Context, attrs: AttributeSet?) : ViewGroup |  | 233 |
| `RenderThread` | `RenderThread` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | class RenderThread("CanvasCodeEditorRenderer": ) : Thread |  | 1892 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `EditorCompletionCallback.showCompletions` | `EditorCompletionCallback` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | items: List<CompletionItem><br>prefix: String | Unit |  | 50 |
| `EditorCompletionCallback.hideCompletions` | `EditorCompletionCallback` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 51 |
| `EditorCompletionCallback.isCompletionVisible` | `EditorCompletionCallback` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Boolean |  | 52 |
| `CanvasCodeEditorView.onScaleBegin` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | detector: ScaleGestureDetector | Boolean |  | 200 |
| `CanvasCodeEditorView.onScale` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | detector: ScaleGestureDetector | Boolean |  | 208 |
| `CanvasCodeEditorView.onScaleEnd` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | detector: ScaleGestureDetector | Unit |  | 213 |
| `CanvasCodeEditorView.onDown` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | e: MotionEvent | Boolean |  | 223 |
| `CanvasCodeEditorView.onScroll` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | e1: MotionEvent?<br>e2: MotionEvent<br>distanceX: Float<br>distanceY: Float | Boolean |  | 225 |
| `CanvasCodeEditorView.onFling` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | e1: MotionEvent?<br>e2: MotionEvent<br>velocityX: Float<br>velocityY: Float | Boolean |  | 238 |
| `CanvasCodeEditorView.onLongPress` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | e: MotionEvent | Unit |  | 251 |
| `CanvasCodeEditorView.onDoubleTap` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | e: MotionEvent | Boolean |  | 264 |
| `CanvasCodeEditorView.run` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 285 |
| `CanvasCodeEditorView.release` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 308 |
| `CanvasCodeEditorView.setEditorTheme` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | theme: EditorTheme | Unit |  | 322 |
| `CanvasCodeEditorView.setLanguage` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | language: String | Unit |  | 328 |
| `CanvasCodeEditorView.setReadOnly` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | readOnly: Boolean | Unit |  | 340 |
| `CanvasCodeEditorView.setShowLineNumbers` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | showLineNumbers: Boolean | Unit |  | 350 |
| `CanvasCodeEditorView.setCompletionEnabled` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | enabled: Boolean | Unit |  | 355 |
| `CanvasCodeEditorView.setViewportBottomPadding` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | bottomPaddingPx: Int | Unit |  | 364 |
| `CanvasCodeEditorView.setOnTextChangedListener` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | listener: (String) -> Unit | Unit |  | 374 |
| `CanvasCodeEditorView.setCompletionCallback` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | callback: EditorCompletionCallback? | Unit |  | 378 |
| `CanvasCodeEditorView.setTextContent` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | text: String | Unit |  | 387 |
| `CanvasCodeEditorView.getTextContent` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | String |  | 402 |
| `CanvasCodeEditorView.undo` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 404 |
| `CanvasCodeEditorView.redo` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 410 |
| `CanvasCodeEditorView.replaceAllText` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | newText: String | Unit |  | 416 |
| `CanvasCodeEditorView.insertSymbol` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | symbol: String | Unit |  | 424 |
| `CanvasCodeEditorView.applyCompletion` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | item: CompletionItem | Unit |  | 432 |
| `CanvasCodeEditorView.getCursorScreenPosition` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Point |  | 442 |
| `CanvasCodeEditorView.surfaceCreated` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | holder: SurfaceHolder | Unit |  | 444 |
| `CanvasCodeEditorView.surfaceChanged` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | holder: SurfaceHolder<br>format: Int<br>width: Int<br>height: Int | Unit |  | 448 |
| `CanvasCodeEditorView.surfaceDestroyed` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | holder: SurfaceHolder | Unit |  | 453 |
| `CanvasCodeEditorView.onAttachedToWindow` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 457 |
| `CanvasCodeEditorView.onDetachedFromWindow` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 464 |
| `CanvasCodeEditorView.onSizeChanged` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | w: Int<br>h: Int<br>oldw: Int<br>oldh: Int | Unit |  | 472 |
| `CanvasCodeEditorView.onCheckIsTextEditor` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Boolean |  | 479 |
| `CanvasCodeEditorView.onCreateInputConnection` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | outAttrs: EditorInfo? | InputConnection |  | 481 |
| `CanvasCodeEditorView.onTouchEvent` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | event: MotionEvent | Boolean |  | 491 |
| `CanvasCodeEditorView.performClick` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Boolean |  | 587 |
| `CanvasCodeEditorView.handleKeyEvent` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | event: KeyEvent | Boolean |  | 591 |
| `CanvasCodeEditorView.moveCursorHorizontal` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | delta: Int<br>extendSelection: Boolean | Unit |  | 733 |
| `CanvasCodeEditorView.moveCursorVertical` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | deltaLines: Int<br>extendSelection: Boolean | Unit |  | 765 |
| `CanvasCodeEditorView.applyScale` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | scaleFactor: Float<br>focusX: Float<br>focusY: Float | Unit |  | 783 |
| `CanvasCodeEditorView.applyScroll` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | distanceX: Float<br>distanceY: Float | Unit |  | 814 |
| `CanvasCodeEditorView.startFling` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | velocityX: Float<br>velocityY: Float | Unit |  | 821 |
| `CanvasCodeEditorView.setScrollOffsets` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | x: Float<br>y: Float<br>request: Boolean? | Unit |  | 841 |
| `CanvasCodeEditorView.clampScrollOffsets` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 857 |
| `CanvasCodeEditorView.requestRender` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 861 |
| `CanvasCodeEditorView.startRenderThread` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 868 |
| `CanvasCodeEditorView.stopRenderThread` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 879 |
| `CanvasCodeEditorView.onDocumentMutated` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 891 |
| `CanvasCodeEditorView.requestHighlight` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 904 |
| `CanvasCodeEditorView.notifySelectionChanged` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 911 |
| `CanvasCodeEditorView.updateCompletion` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 921 |
| `CanvasCodeEditorView.hideCompletions` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 944 |
| `CanvasCodeEditorView.refreshPaints` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 949 |
| `CanvasCodeEditorView.blendColors` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | baseColor: Int<br>overlayColor: Int<br>overlayRatio: Float | Int |  | 1022 |
| `CanvasCodeEditorView.drawEditor` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | canvas: Canvas | Unit |  | 1039 |
| `CanvasCodeEditorView.drawLineNumber` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | canvas: Canvas<br>line: Int<br>lineTop: Float<br>currentLine: Int<br>gutterWidth: Float | Unit |  | 1112 |
| `CanvasCodeEditorView.drawIndentGuides` | `CanvasCodeEditorView` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | canvas: Canvas<br>line: Int<br>lineTop: Float<br>textRegionLeft: Float | Unit |  | 1132 |
| `drawSelectionForLine` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | canvas: Canvas<br>line: Int<br>lineTop: Float<br>textRegionLeft: Float | Unit |  | 1172 |
| `drawTextForLine` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | canvas: Canvas<br>line: Int<br>lineTop: Float<br>textRegionLeft: Float | Unit |  | 1223 |
| `flushRun` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1243 |
| `drawComposingUnderline` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | canvas: Canvas<br>line: Int<br>lineTop: Float<br>textRegionLeft: Float | Unit |  | 1305 |
| `drawCursorForLine` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | canvas: Canvas<br>line: Int<br>lineTop: Float<br>cursorLine: Int<br>textRegionLeft: Float | Unit |  | 1329 |
| `drawSelectionHandles` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | canvas: Canvas | Unit |  | 1349 |
| `drawHandle` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | canvas: Canvas<br>center: PointF | Unit |  | 1355 |
| `colorForOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | offset: Int | Int |  | 1367 |
| `contentHeightPx` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Float |  | 1389 |
| `contentWidthPx` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Float |  | 1393 |
| `gutterWidth` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Float |  | 1397 |
| `textRegionLeft` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Float |  | 1414 |
| `gutterLeadingPaddingPx` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Float |  | 1418 |
| `gutterTrailingPaddingPx` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Float |  | 1427 |
| `textViewportWidth` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Float |  | 1436 |
| `maxScrollX` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Float |  | 1440 |
| `maxScrollY` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Float |  | 1444 |
| `xForOffsetInLine` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | offset: Int | Float |  | 1448 |
| `screenToOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | x: Float<br>y: Float | Int |  | 1452 |
| `offsetToPoint` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | offset: Int | Point |  | 1479 |
| `ensureCursorVisible` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1487 |
| `detectHandleHit` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | x: Float<br>y: Float | DragHandle |  | 1519 |
| `updateSelectionFromHandle` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | handle: DragHandle<br>x: Float<br>y: Float | Unit |  | 1534 |
| `selectionHandleCenters` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | HandleCenters? |  | 1549 |
| `showSelectionMenu` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1563 |
| `onCreateActionMode` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | mode: ActionMode<br>menu: Menu | Boolean |  | 1575 |
| `onPrepareActionMode` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | mode: ActionMode<br>menu: Menu | Boolean |  | 1585 |
| `onActionItemClicked` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | mode: ActionMode<br>item: MenuItem | Boolean |  | 1587 |
| `onDestroyActionMode` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | mode: ActionMode | Unit |  | 1618 |
| `onGetContentRect` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | mode: ActionMode<br>view: View<br>outRect: Rect | Unit |  | 1627 |
| `copySelectionToClipboard` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1665 |
| `cutSelectionToClipboard` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1675 |
| `pasteFromClipboard` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1684 |
| `showSoftKeyboard` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1702 |
| `hideSoftKeyboard` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1713 |
| `spToPx` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | valueSp: Float | Float |  | 1717 |
| `loadEditorTypeface` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Typeface |  | 1725 |
| `shouldRenderWithSystemGlyphs` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | codePoint: Int | Boolean |  | 1733 |
| `shouldRenderWithSystemGlyphs` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | text: CharSequence<br>start: Int<br>end: Int | Boolean |  | 1743 |
| `EditorInputConnection.commitText` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | text: CharSequence?<br>newCursorPosition: Int | Boolean |  | 1761 |
| `EditorInputConnection.setComposingText` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | text: CharSequence?<br>newCursorPosition: Int | Boolean |  | 1772 |
| `EditorInputConnection.finishComposingText` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Boolean |  | 1786 |
| `EditorInputConnection.deleteSurroundingText` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | beforeLength: Int<br>afterLength: Int | Boolean |  | 1793 |
| `EditorInputConnection.deleteSurroundingTextInCodePoints` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | beforeLength: Int<br>afterLength: Int | Boolean |  | 1802 |
| `EditorInputConnection.sendKeyEvent` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | event: KeyEvent? | Boolean |  | 1811 |
| `EditorInputConnection.setSelection` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | start: Int<br>end: Int | Boolean |  | 1821 |
| `EditorInputConnection.getTextBeforeCursor` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | n: Int<br>flags: Int | CharSequence |  | 1831 |
| `EditorInputConnection.getTextAfterCursor` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | n: Int<br>flags: Int | CharSequence |  | 1837 |
| `EditorInputConnection.getSelectedText` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | flags: Int | CharSequence? |  | 1843 |
| `EditorInputConnection.getExtractedText` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | request: ExtractedTextRequest?<br>flags: Int | ExtractedText |  | 1852 |
| `EditorInputConnection.performContextMenuAction` | `EditorInputConnection` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` | id: Int | Boolean |  | 1863 |
| `RenderThread.finish` | `RenderThread` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1896 |
| `RenderThread.run` | `RenderThread` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CanvasCodeEditorView.kt` |  | Unit |  | 1901 |
| `CodeEditor` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | code: String<br>language: String<br>onCodeChange: (String) -> Unit<br>modifier: Modifier?<br>readOnly: Boolean?<br>showLineNumbers: Boolean?<br>enableCompletion: Boolean?<br>editorRef: ((NativeCodeEditor?) -> Unit)?? | Unit |  | 51 |
| `updatePopupAnchor` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | editor: NativeCodeEditor? | Unit |  | 78 |
| `showCompletions` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | items: List<CompletionItem><br>prefix: String | Unit |  | 133 |
| `hideCompletions` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` |  | Unit |  | 142 |
| `isCompletionVisible` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` |  | Boolean |  | 147 |
| `SymbolButton` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | symbol: String<br>theme: EditorTheme<br>onClick: () -> Unit | Unit |  | 214 |
| `NativeCodeEditor.setOnTextChangedListener` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | listener: (String) -> Unit | Unit |  | 245 |
| `NativeCodeEditor.setEditorTheme` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | theme: EditorTheme | Unit |  | 252 |
| `NativeCodeEditor.setLanguage` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | language: String | Unit |  | 259 |
| `NativeCodeEditor.setReadOnly` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | readOnly: Boolean | Unit |  | 266 |
| `NativeCodeEditor.setShowLineNumbers` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | showLineNumbers: Boolean | Unit |  | 274 |
| `NativeCodeEditor.setCompletionEnabled` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | enableCompletion: Boolean | Unit |  | 281 |
| `NativeCodeEditor.setViewportBottomPadding` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | bottomPaddingPx: Int | Unit |  | 288 |
| `NativeCodeEditor.setText` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | text: String<br>fromUpdate: Boolean? | Unit |  | 295 |
| `NativeCodeEditor.getText` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` |  | String |  | 304 |
| `NativeCodeEditor.setCompletionCallback` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | callback: EditorCompletionCallback? | Unit |  | 306 |
| `NativeCodeEditor.applyCompletion` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | item: CompletionItem | Unit |  | 313 |
| `NativeCodeEditor.undo` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` |  | Unit |  | 320 |
| `NativeCodeEditor.redo` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` |  | Unit |  | 327 |
| `NativeCodeEditor.insertSymbol` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | symbol: String | Unit |  | 334 |
| `NativeCodeEditor.replaceAllText` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | newText: String | Unit |  | 341 |
| `NativeCodeEditor.getCursorScreenPosition` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` |  | Point |  | 348 |
| `NativeCodeEditor.release` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` |  | Unit |  | 351 |
| `NativeCodeEditor.onMeasure` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | widthMeasureSpec: Int<br>heightMeasureSpec: Int | Unit |  | 360 |
| `NativeCodeEditor.onLayout` | `NativeCodeEditor` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeEditor.kt` | changed: Boolean<br>l: Int<br>t: Int<br>r: Int<br>b: Int | Unit |  | 370 |
| `CodeFormatter.format` | `CodeFormatter` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | code: String<br>language: String | String | 根据语言类型格式化代码 | 17 |
| `CodeFormatter.formatJavaScript` | `CodeFormatter` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | code: String | String | 格式化 JavaScript 代码 | 37 |
| `formatCSS` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | code: String | String | 格式化 CSS 代码 | 197 |
| `formatHTML` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | code: String | String | 格式化 HTML 代码 | 279 |
| `editorCellWidth` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | char: Char | Int |  | 12 |
| `editorCellWidth` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | codePoint: Int | Int |  | 19 |
| `editorCodeUnitLength` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: CharSequence<br>offset: Int<br>limit: Int? | Int |  | 26 |
| `editorNextCharacterOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: CharSequence<br>offset: Int<br>limit: Int? | Int |  | 48 |
| `editorPreviousCharacterOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: CharSequence<br>offset: Int | Int |  | 58 |
| `editorNextSymbolOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: CharSequence<br>offset: Int<br>limit: Int? | Int |  | 75 |
| `editorPreviousSymbolOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: CharSequence<br>offset: Int | Int |  | 125 |
| `editorCellWidth` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: CharSequence<br>offset: Int<br>limit: Int? | Int |  | 145 |
| `editorSnapOffsetToCharacterBoundary` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: CharSequence<br>offset: Int | Int |  | 184 |
| `editorExpandOffsetToCharacterEnd` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: CharSequence<br>offset: Int | Int |  | 197 |
| `isWideEditorCodePoint` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | codePoint: Int | Boolean |  | 210 |
| `isEmojiLikeCodePoint` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | codePoint: Int | Boolean |  | 227 |
| `isEmojiModifier` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | codePoint: Int | Boolean |  | 235 |
| `isRegionalIndicator` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | codePoint: Int | Boolean |  | 239 |
| `isVariationSelector` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | codePoint: Int | Boolean |  | 243 |
| `isCombiningMark` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | codePoint: Int | Boolean |  | 247 |
| `EditorDocument.text` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | CharSequence |  | 290 |
| `EditorDocument.textString` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | String |  | 292 |
| `EditorDocument.length` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Int |  | 294 |
| `EditorDocument.lineCount` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Int |  | 296 |
| `EditorDocument.hasSelection` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Boolean |  | 298 |
| `EditorDocument.hasComposingRegion` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Boolean |  | 300 |
| `EditorDocument.clearHistory` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Unit |  | 302 |
| `EditorDocument.canUndo` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Boolean |  | 307 |
| `EditorDocument.canRedo` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Boolean |  | 309 |
| `EditorDocument.setText` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | newText: String<br>clearHistory: Boolean? | Unit |  | 311 |
| `EditorDocument.replaceAllText` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | newText: String | Unit |  | 333 |
| `EditorDocument.insertTextAtCursor` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: String | Unit |  | 344 |
| `EditorDocument.insertTextProgrammatically` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | start: Int<br>text: String | Unit |  | 357 |
| `EditorDocument.applyCompletion` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | prefixLength: Int<br>replacement: String | Unit |  | 370 |
| `EditorDocument.replaceSelection` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: String<br>recordHistory: Boolean? | Unit |  | 383 |
| `EditorDocument.setComposingText` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | text: String | Unit |  | 396 |
| `EditorDocument.finishComposingText` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Unit |  | 411 |
| `EditorDocument.deleteSurroundingText` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | beforeLength: Int<br>afterLength: Int | Unit |  | 415 |
| `EditorDocument.deleteBackward` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Unit |  | 442 |
| `EditorDocument.deleteForward` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Unit |  | 459 |
| `EditorDocument.deleteSurroundingCodePoints` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | beforeLength: Int<br>afterLength: Int | Unit |  | 476 |
| `EditorDocument.insertNewlineWithIndent` | `EditorDocument` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Unit |  | 504 |
| `setSelection` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | start: Int<br>end: Int | Unit |  | 545 |
| `collapseSelection` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | offset: Int | Unit |  | 551 |
| `selectWordAt` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | offset: Int | Unit |  | 555 |
| `selectAll` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Unit |  | 584 |
| `undo` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Boolean |  | 588 |
| `redo` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Boolean |  | 594 |
| `getLineForOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | offset: Int | Int |  | 600 |
| `getLineStart` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | line: Int | Int |  | 618 |
| `getLineEnd` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | line: Int | Int |  | 623 |
| `getLineText` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | line: Int | CharSequence |  | 631 |
| `getCellColumnForOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | offset: Int | Int |  | 637 |
| `getOffsetForLineAndCellColumn` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | line: Int<br>targetCells: Int | Int |  | 655 |
| `previousCursorOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | offset: Int | Int |  | 676 |
| `nextCursorOffset` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | offset: Int | Int |  | 680 |
| `lineDigits` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Int |  | 685 |
| `activeReplaceRange` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | IntRange |  | 687 |
| `normalizedSelection` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | IntRange |  | 695 |
| `replaceRangeInternal` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | start: Int<br>end: Int<br>replacement: String<br>afterSelectionStart: Int<br>afterSelectionEnd: Int<br>recordHistory: Boolean | Unit |  | 701 |
| `applyCommand` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | command: EditorEditCommand<br>reverse: Boolean<br>targetStack: ArrayDeque<EditorEditCommand> | Unit |  | 747 |
| `clearComposingRegion` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Unit |  | 776 |
| `rebuildMetadata` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` |  | Unit |  | 781 |
| `isWordChar` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | char: Char | Boolean |  | 809 |
| `EditorMetrics.update` | `EditorMetrics` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorMetrics.kt` | textSizePx: Float | Unit |  | 25 |
| `EditorMetrics.getCellWidth` | `EditorMetrics` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorMetrics.kt` | char: Char | Int |  | 34 |
| `EditorSyntaxHighlighter.setLanguage` | `EditorSyntaxHighlighter` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | language: String | Unit |  | 37 |
| `EditorSyntaxHighlighter.requestHighlight` | `EditorSyntaxHighlighter` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | text: String<br>version: Int | Unit |  | 43 |
| `EditorSyntaxHighlighter.release` | `EditorSyntaxHighlighter` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` |  | Unit |  | 74 |
| `EditorSyntaxHighlighter.parseFullText` | `EditorSyntaxHighlighter` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | text: String<br>colors: IntArray<br>support: LanguageSupport? | Unit |  | 83 |
| `simpleHighlight` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | text: String<br>colors: IntArray | Unit |  | 209 |
| `consumeNumber` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | text: String<br>startIndex: Int | Int |  | 254 |
| `fill` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | colors: IntArray<br>start: Int<br>end: Int<br>color: Int | Unit |  | 265 |
| `LanguageDetector.detectLanguage` | `LanguageDetector` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `LanguageDetector.kt` | fileName: String | String | 根据文件名获取编程语言 | 12 |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `CodeFormatter.TAG` | `CodeFormatter` | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred |  | 9 |
| `color` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | inferred |  | 179 |
| `COMBINING_KEYCAP` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | inferred |  | 9 |
| `EDITOR_TAB_SPACES` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | inferred |  | 7 |
| `end` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | inferred |  | 92 |
| `end` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | inferred |  | 164 |
| `endPos` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred | 找到DOCTYPE结束位置 | 362 |
| `firstCodePoint` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | inferred |  | 91 |
| `firstCodePoint` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | inferred |  | 159 |
| `index` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | inferred |  | 165 |
| `isCapitalized` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | inferred |  | 178 |
| `isClosingTag` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred |  | 374 |
| `isEmptyBracket` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred |  | 116 |
| `isEmptyBracket` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred |  | 135 |
| `lastNonWhitespace` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred | 检查是否是空的 {} 或 []（向前查找对应的开括号） | 130 |
| `MAX_SYMBOL_BACKTRACK_CODE_POINTS` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | inferred |  | 10 |
| `nextChar` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorSyntaxHighlighter.kt` | inferred |  | 177 |
| `tagEnd` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred | 获取标签名 | 377 |
| `tagName` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred |  | 382 |
| `tagName` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred |  | 422 |
| `tagStart` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `CodeFormatter.kt` | inferred | 获取刚刚闭合的标签名 | 408 |
| `ZERO_WIDTH_JOINER` | — | `com.ai.assistance.operit.ui.features.chat.webview.workspace.editor` | `EditorDocument.kt` | inferred |  | 8 |
