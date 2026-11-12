# operit.widget

> 函数 42 · 类型 8 · 顶层常量 14 · 共 64 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ToolPkgDesktopGlanceWidget` | `ToolPkgDesktopGlanceWidget` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopGlanceWidget.kt` | class ToolPkgDesktopGlanceWidget : GlanceAppWidget |  | 32 |
| `ToolPkgDesktopWidgetConfigActivity` | `ToolPkgDesktopWidgetConfigActivity` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetConfigActivity.kt` | class ToolPkgDesktopWidgetConfigActivity : ComponentActivity |  | 45 |
| `ToolPkgDesktopWidgetHost` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | object ToolPkgDesktopWidgetHost |  | 12 |
| `ToolPkgDesktopWidgetHost.WidgetSelection` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | class WidgetSelection(val key: String, val widget: PackageManager.ToolPkgDesktop…) |  | 28 |
| `ToolPkgDesktopWidgetReceiver` | `ToolPkgDesktopWidgetReceiver` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetReceiver.kt` | class ToolPkgDesktopWidgetReceiver : GlanceAppWidgetReceiver |  | 8 |
| `ToolPkgDesktopWidgetRenderData` | `ToolPkgDesktopWidgetRenderData` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | class ToolPkgDesktopWidgetRenderData(val renderRouteId: String, val renderResult: ToolPkgComposeDslRenderResult?, val errorMessage: String?) |  | 36 |
| `VoiceAssistantGlanceWidget` | `VoiceAssistantGlanceWidget` | `com.ai.assistance.operit.widget` | `VoiceAssistantGlanceWidget.kt` | class VoiceAssistantGlanceWidget : GlanceAppWidget | Voice Assistant Widget using Glance (Jetpack Compose for Widgets) This widget provides a … | 44 |
| `VoiceAssistantWidgetReceiver` | `VoiceAssistantWidgetReceiver` | `com.ai.assistance.operit.widget` | `VoiceAssistantWidgetReceiver.kt` | class VoiceAssistantWidgetReceiver : GlanceAppWidgetReceiver | Widget Receiver for Voice Assistant Widget This receiver handles widget lifecycle events … | 11 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `ToolPkgDesktopGlanceWidget.provideGlance` | `ToolPkgDesktopGlanceWidget` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopGlanceWidget.kt` | context: Context<br>id: GlanceId | Unit |  | 33 |
| `ToolPkgDesktopWidgetContent` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopGlanceWidget.kt` | context: Context<br>appWidgetId: Int<br>selection: ToolPkgDesktopWidgetHost.WidgetSele…<br>renderData: ToolPkgDesktopWidgetRenderData? | Unit |  | 57 |
| `ToolPkgDesktopWidgetConfigActivity.onCreate` | `ToolPkgDesktopWidgetConfigActivity` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetConfigActivity.kt` | savedInstanceState: Bundle? | Unit |  | 49 |
| `ToolPkgDesktopWidgetConfigActivity.onStop` | `ToolPkgDesktopWidgetConfigActivity` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetConfigActivity.kt` |  | Unit |  | 93 |
| `ToolPkgDesktopWidgetConfigScreen` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetConfigActivity.kt` | appWidgetId: Int<br>onCancel: () -> Unit<br>onSelect: (PackageManager.ToolPkgDesktopWidge… | Unit |  | 110 |
| `loadToolPkgDesktopWidgetRenderData` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | context: Context<br>appWidgetId: Int<br>selection: ToolPkgDesktopWidgetHost.WidgetSele… | ToolPkgDesktopWidgetRenderData |  | 42 |
| `RenderToolPkgDesktopWidgetDsl` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | node: ToolPkgComposeDslNode<br>routeClickAction: Action | Unit |  | 149 |
| `renderToolPkgDesktopWidgetDslNode` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | node: ToolPkgComposeDslNode<br>routeClickAction: Action<br>defaultClickable: Boolean? | Unit |  | 161 |
| `renderToolPkgDesktopWidgetDslChildren` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | node: ToolPkgComposeDslNode<br>routeClickAction: Action | Unit |  | 270 |
| `collectWidgetChildren` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | node: ToolPkgComposeDslNode | List<ToolPkgComposeDslNode> |  | 282 |
| `extractNodeText` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | node: ToolPkgComposeDslNode | String |  | 291 |
| `widgetModifierFromNode` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | node: ToolPkgComposeDslNode<br>routeClickAction: Action<br>defaultClickable: Boolean?<br>clickable: Boolean? | GlanceModifier |  | 306 |
| `applyWidgetPadding` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | base: GlanceModifier<br>rawPadding: Any?<br>props: Map<String, Any?> | GlanceModifier |  | 344 |
| `hasClickableModifierOp` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | rawModifier: Any? | Boolean |  | 367 |
| `parseTextColor` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | value: Any? | ColorProvider |  | 376 |
| `parseColorProvider` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | value: Any? | ColorProvider? |  | 380 |
| `parseColorToken` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | token: String? | Color? |  | 391 |
| `parseColorString` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | raw: String | Color? |  | 405 |
| `parseFontWeight` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | raw: String? | FontWeight? |  | 418 |
| `ToolPkgDesktopWidgetHost.buildSelectionKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | containerPackageName: String<br>widgetId: String | String |  | 33 |
| `ToolPkgDesktopWidgetHost.listAvailableWidgets` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | context: Context | List<PackageManager.ToolPkgDesktopWidget> |  | 37 |
| `ToolPkgDesktopWidgetHost.resolveSelection` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | context: Context<br>appWidgetId: Int | WidgetSelection? |  | 42 |
| `ToolPkgDesktopWidgetHost.saveSelection` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | context: Context<br>appWidgetId: Int<br>widget: PackageManager.ToolPkgDesktopWidget | Boolean |  | 60 |
| `ToolPkgDesktopWidgetHost.clearSelection` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | context: Context<br>appWidgetId: Int | Unit |  | 82 |
| `ToolPkgDesktopWidgetHost.buildLaunchIntent` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | context: Context<br>routeId: String<br>routeArgsJson: String?? | Intent |  | 99 |
| `ToolPkgDesktopWidgetHost.buildConfigIntent` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | context: Context<br>appWidgetId: Int | Intent |  | 111 |
| `ToolPkgDesktopWidgetHost.refreshAll` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | context: Context | Unit |  | 118 |
| `ToolPkgDesktopWidgetHost.loadSelectionKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | context: Context<br>appWidgetId: Int | String? |  | 124 |
| `ToolPkgDesktopWidgetHost.loadPersistedSelection` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | context: Context<br>appWidgetId: Int | WidgetSelection? |  | 132 |
| `ToolPkgDesktopWidgetHost.selectionPrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 167 |
| `ToolPkgDesktopWidgetHost.routePrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 168 |
| `ToolPkgDesktopWidgetHost.renderRoutePrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 169 |
| `ToolPkgDesktopWidgetHost.containerPrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 170 |
| `ToolPkgDesktopWidgetHost.widgetIdPrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 171 |
| `ToolPkgDesktopWidgetHost.titlePrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 172 |
| `ToolPkgDesktopWidgetHost.subtitlePrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 173 |
| `ToolPkgDesktopWidgetHost.descriptionPrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 174 |
| `ToolPkgDesktopWidgetHost.iconPrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 175 |
| `ToolPkgDesktopWidgetHost.orderPrefKey` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | appWidgetId: Int | String |  | 176 |
| `ToolPkgDesktopWidgetReceiver.onDeleted` | `ToolPkgDesktopWidgetReceiver` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetReceiver.kt` | context: Context<br>appWidgetIds: IntArray | Unit |  | 12 |
| `VoiceAssistantGlanceWidget.provideGlance` | `VoiceAssistantGlanceWidget` | `com.ai.assistance.operit.widget` | `VoiceAssistantGlanceWidget.kt` | context: Context<br>id: GlanceId | Unit |  | 46 |
| `VoiceAssistantWidgetContent` | — | `com.ai.assistance.operit.widget` | `VoiceAssistantGlanceWidget.kt` | context: Context | Unit |  | 54 |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ToolPkgDesktopWidgetHost.EXTRA_OPEN_ROUTE_ARGS_JSON` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 14 |
| `ToolPkgDesktopWidgetHost.EXTRA_OPEN_ROUTE_ID` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 13 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_CONTAINER` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 20 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_DESCRIPTION` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 24 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_ICON` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 25 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_ORDER` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 26 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_RENDER_ROUTE` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 19 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_ROUTE` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 18 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_SELECTION` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 17 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_SUBTITLE` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 23 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_TITLE` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 22 |
| `ToolPkgDesktopWidgetHost.KEY_PREFIX_WIDGET_ID` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 21 |
| `ToolPkgDesktopWidgetHost.PREFS_NAME` | `ToolPkgDesktopWidgetHost` | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetHost.kt` | inferred |  | 16 |
| `WIDGET_DSL_TAG` | — | `com.ai.assistance.operit.widget` | `ToolPkgDesktopWidgetDslRenderer.kt` | inferred |  | 34 |
