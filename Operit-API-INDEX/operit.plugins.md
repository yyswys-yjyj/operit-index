# operit.plugins

> 函数 157 · 类型 63 · 顶层常量 101 · 共 321 条
> 每日定时任务自动生成。

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `AppLifecycleEvent` | `AppLifecycleEvent` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | class AppLifecycleEvent(val wireName: String) |  | 23 |
| `AppLifecycleHookParams` | `AppLifecycleHookParams` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | class AppLifecycleHookParams(val context: Context, val extras: Map<String, Any?>) |  | 38 |
| `AppLifecycleHookPlugin` | `AppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | interface AppLifecycleHookPlugin |  | 48 |
| `AppLifecycleHookPluginRegistry` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | object AppLifecycleHookPluginRegistry |  | 57 |
| `AppLifecycleReplayEvent` | `AppLifecycleReplayEvent` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | class AppLifecycleReplayEvent(val event: AppLifecycleEvent, val params: AppLifecycleHookParams) |  | 43 |
| `ChatMessageMenuDialogRequest` | `ChatMessageMenuDialogRequest` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | class ChatMessageMenuDialogRequest(val containerPackageName: String, val screenPath: String, val title: String, val state: Map<String, Any?>, val moduleSpec: Map<String, Any?>) |  | 18 |
| `ChatMessageMenuItemClickResult` | `ChatMessageMenuItemClickResult` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | class ChatMessageMenuItemClickResult(val dialog: ChatMessageMenuDialogRequest?) |  | 26 |
| `ChatMessageMenuItemDefinition` | `ChatMessageMenuItemDefinition` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | class ChatMessageMenuItemDefinition(val id: String, val title: String, val icon: String?, val order: Int, val onClick: suspend (ChatMessageMenuItemP…) : suspend |  | 30 |
| `ChatMessageMenuItemParams` | `ChatMessageMenuItemParams` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | class ChatMessageMenuItemParams(val context: Context, val chatId: String, val messageIndex: Int, val message: ChatMessage) |  | 11 |
| `ChatMessageMenuItemPlugin` | `ChatMessageMenuItemPlugin` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | interface ChatMessageMenuItemPlugin |  | 38 |
| `ChatMessageMenuItemRegistry` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | object ChatMessageMenuItemRegistry |  | 44 |
| `ChatViewEvent` | `ChatViewEvent` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | class ChatViewEvent(val wireName: String) |  | 11 |
| `ChatViewHookParams` | `ChatViewHookParams` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | class ChatViewHookParams(val context: Context, val viewId: String, val chatId: String?, val workspacePath: String?, val workspaceEnv: String?, val runtime: String, val title: String?) |  | 17 |
| `ChatViewHookPlugin` | `ChatViewHookPlugin` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | interface ChatViewHookPlugin |  | 27 |
| `ChatViewHookPluginRegistry` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | object ChatViewHookPluginRegistry |  | 36 |
| `OperitPlugin` | `OperitPlugin` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` | interface OperitPlugin |  | 9 |
| `ParsedMessageProcessingResult` | `ParsedMessageProcessingResult` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | class ParsedMessageProcessingResult(val matched: Boolean, val chunks: List<String>) |  | 356 |
| `PluginRegistry` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` | object PluginRegistry |  | 15 |
| `RegisteredMessageProcessingController` | `RegisteredMessageProcessingController` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | class RegisteredMessageProcessingController(private val executionId: String, private val hook: ToolPkgMessageProcessingHookR…) : MessageProcessingController |  | 440 |
| `ToolboxPlugin` | `ToolboxPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | object ToolboxPlugin : OperitPlugin |  | 136 |
| `ToolLifecycleDispatch` | `ToolLifecycleDispatch` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | class ToolLifecycleDispatch(val eventName: String, val eventPayload: Map<String, Any?>) |  | 26 |
| `ToolPkgAiProviderRegistration` | `ToolPkgAiProviderRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgAiProviderRegistration(val containerPackageName: String, val providerId: String, val displayName: String, val description: String, val listModelsFunctionName: String, val listModels… |  | 103 |
| `ToolPkgAiProviderRegistry` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` | object ToolPkgAiProviderRegistry |  | 7 |
| `ToolPkgAppLifecycleHookPlugin` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | object ToolPkgAppLifecycleHookPlugin : AppLifecycleHookPlugin |  | 23 |
| `ToolPkgAppLifecycleHookRegistration` | `ToolPkgAppLifecycleHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgAppLifecycleHookRegistration(val containerPackageName: String, val hookId: String, val event: String, val functionName: String, val functionSource: String?) |  | 14 |
| `ToolPkgChatInputHookBridge` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | object ToolPkgChatInputHookBridge |  | 21 |
| `ToolPkgChatInputHookBridge.Bridge` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | object Bridge : ChatInputHook |  | 30 |
| `ToolPkgChatInputHookRegistration` | `ToolPkgChatInputHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgChatInputHookRegistration(val containerPackageName: String, val hookId: String, val functionName: String, val functionSource: String?) |  | 44 |
| `ToolPkgChatMessageHookBridge` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | object ToolPkgChatMessageHookBridge |  | 17 |
| `ToolPkgChatMessageHookBridgeTest` | `ToolPkgChatMessageHookBridgeTest` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridgeTest.kt` | class ToolPkgChatMessageHookBridgeTest |  | 10 |
| `ToolPkgChatMessageHookRegistration` | `ToolPkgChatMessageHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgChatMessageHookRegistration(val containerPackageName: String, val hookId: String, val functionName: String, val functionSource: String?) |  | 58 |
| `ToolPkgChatMessageMenuDialogRegistration` | `ToolPkgChatMessageMenuDialogRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgChatMessageMenuDialogRegistration(val screenPath: String, val title: LocalizedText) |  | 65 |
| `ToolPkgChatMessageMenuItemBridge` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | object ToolPkgChatMessageMenuItemBridge : ChatMessageMenuItemPlugin |  | 24 |
| `ToolPkgChatMessageMenuItemRegistration` | `ToolPkgChatMessageMenuItemRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgChatMessageMenuItemRegistration(val containerPackageName: String, val itemId: String, val title: LocalizedText, val icon: String?, val order: Int, val senders: List<String>, val functionName… |  | 70 |
| `ToolPkgChatRuntimeHookBridge` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | object ToolPkgChatRuntimeHookBridge : ChatRuntimeHook |  | 18 |
| `ToolPkgChatRuntimeHookRegistration` | `ToolPkgChatRuntimeHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgChatRuntimeHookRegistration(val containerPackageName: String, val hookId: String, val functionName: String, val functionSource: String?) |  | 82 |
| `ToolPkgChatViewHookBridge` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | object ToolPkgChatViewHookBridge : ChatViewHookPlugin |  | 20 |
| `ToolPkgChatViewHookRegistration` | `ToolPkgChatViewHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgChatViewHookRegistration(val containerPackageName: String, val hookId: String, val functionName: String, val functionSource: String?) |  | 51 |
| `ToolPkgCommonBridgePlugin` | `ToolPkgCommonBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | object ToolPkgCommonBridgePlugin : OperitPlugin |  | 888 |
| `ToolPkgHookExecutionBudget` | `ToolPkgHookExecutionBudget` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookExecutionBudget.kt` | class ToolPkgHookExecutionBudget(private val startedAtNanos: Long, private val deadlineNanos: Long) | A shared deadline for one synchronous ToolPkg hook dispatch chain. A chain may invoke sev… | 16 |
| `ToolPkgInputMenuToggleBridgePlugin` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | object ToolPkgInputMenuToggleBridgePlugin : InputMenuTogglePlugin |  | 638 |
| `ToolPkgInputMenuToggleBridgePlugin.InputMenuSpec` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | class InputMenuSpec(val containerPackageName: String, val functionName: String, val pluginId: String, val functionSource: String?, val id: String, val title: String, val descript… |  | 834 |
| `ToolPkgInputMenuToggleHookRegistration` | `ToolPkgInputMenuToggleHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgInputMenuToggleHookRegistration(val containerPackageName: String, val pluginId: String, val functionName: String, val functionSource: String?) |  | 37 |
| `ToolPkgMessageProcessingBridgePlugin` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | object ToolPkgMessageProcessingBridgePlugin : MessageProcessingPlugin |  | 89 |
| `ToolPkgMessageProcessingCancellationRegistry` | `ToolPkgMessageProcessingCancellationRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgMessageProcessingCancellationRegistry.kt` | object ToolPkgMessageProcessingCancellationRegistry |  | 7 |
| `ToolPkgMessageProcessingHookRegistration` | `ToolPkgMessageProcessingHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgMessageProcessingHookRegistration(val containerPackageName: String, val pluginId: String, val functionName: String, val functionSource: String?) |  | 22 |
| `ToolPkgPromptHookBridge` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | object ToolPkgPromptHookBridge |  | 31 |
| `ToolPkgPromptHookBridge.PromptEstimateFinalizeBridge` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | object PromptEstimateFinalizeBridge : PromptEstimateFinalizeHook |  | 130 |
| `ToolPkgPromptHookBridge.PromptEstimateHistoryBridge` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | object PromptEstimateHistoryBridge : PromptEstimateHistoryHook |  | 78 |
| `ToolPkgPromptHookBridge.PromptFinalizeBridge` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | object PromptFinalizeBridge : PromptFinalizeHook |  | 117 |
| `ToolPkgPromptHookBridge.PromptHistoryBridge` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | object PromptHistoryBridge : PromptHistoryHook |  | 65 |
| `ToolPkgPromptHookBridge.PromptInputBridge` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | object PromptInputBridge : PromptInputHook |  | 52 |
| `ToolPkgPromptHookBridge.SystemPromptComposeBridge` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | object SystemPromptComposeBridge : SystemPromptComposeHook |  | 91 |
| `ToolPkgPromptHookBridge.ToolPromptComposeBridge` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | object ToolPromptComposeBridge : ToolPromptComposeHook |  | 104 |
| `ToolPkgPromptHookRegistration` | `ToolPkgPromptHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgPromptHookRegistration(val containerPackageName: String, val hookId: String, val functionName: String, val functionSource: String?) |  | 96 |
| `ToolPkgSummaryHookBridge` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | object ToolPkgSummaryHookBridge |  | 20 |
| `ToolPkgSummaryHookBridge.SummaryGenerateBridge` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | object SummaryGenerateBridge : SummaryGenerateHook |  | 29 |
| `ToolPkgToolLifecycleBridge` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | object ToolPkgToolLifecycleBridge : AIToolHook |  | 31 |
| `ToolPkgToolLifecycleHookRegistration` | `ToolPkgToolLifecycleHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgToolLifecycleHookRegistration(val containerPackageName: String, val hookId: String, val functionName: String, val functionSource: String?) |  | 89 |
| `ToolPkgXmlRenderBridgePlugin` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | object ToolPkgXmlRenderBridgePlugin : XmlRenderPlugin |  | 453 |
| `ToolPkgXmlRenderHookRegistration` | `ToolPkgXmlRenderHookRegistration` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | class ToolPkgXmlRenderHookRegistration(val containerPackageName: String, val pluginId: String, val tag: String, val functionName: String, val functionSource: String?) |  | 29 |
| `WorkflowAppLifecycleHookPlugin` | `WorkflowAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.workflow` | `WorkflowLifecyclePlugin.kt` | object WorkflowAppLifecycleHookPlugin : AppLifecycleHookPlugin |  | 11 |
| `WorkflowLifecyclePlugin` | `WorkflowLifecyclePlugin` | `com.ai.assistance.operit.plugins.workflow` | `WorkflowLifecyclePlugin.kt` | object WorkflowLifecyclePlugin : OperitPlugin |  | 50 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `ChatMessageMenuItemPlugin.createMenuItems` | `ChatMessageMenuItemPlugin` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | params: ChatMessageMenuItemParams | List<ChatMessageMenuItemDefinition> |  | 41 |
| `ChatMessageMenuItemRegistry.register` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | plugin: ChatMessageMenuItemPlugin | Unit |  | 50 |
| `ChatMessageMenuItemRegistry.unregister` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | pluginId: String | Unit |  | 57 |
| `ChatMessageMenuItemRegistry.notifyChanged` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` |  | Unit |  | 64 |
| `ChatMessageMenuItemRegistry.createMenuItems` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | params: ChatMessageMenuItemParams | List<ChatMessageMenuItemDefinition> |  | 68 |
| `ChatViewHookPlugin.onEvent` | `ChatViewHookPlugin` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | event: ChatViewEvent<br>params: ChatViewHookParams | Unit |  | 30 |
| `ChatViewHookPluginRegistry.register` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | plugin: ChatViewHookPlugin | Unit |  | 44 |
| `ChatViewHookPluginRegistry.unregister` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | pluginId: String | Unit |  | 50 |
| `ChatViewHookPluginRegistry.dispatch` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | event: ChatViewEvent<br>params: ChatViewHookParams | Unit |  | 54 |
| `ChatViewHookPluginRegistry.dispatchAsync` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | event: ChatViewEvent<br>params: ChatViewHookParams | Unit |  | 72 |
| `ChatViewHookPluginRegistry.getReplayableOpenViewParams` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` |  | List<ChatViewHookParams> |  | 81 |
| `ChatViewHookPluginRegistry.recordReplayableState` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | event: ChatViewEvent<br>params: ChatViewHookParams | Unit |  | 87 |
| `AppLifecycleHookPlugin.onEvent` | `AppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | event: AppLifecycleEvent<br>params: AppLifecycleHookParams | Unit |  | 51 |
| `AppLifecycleHookPluginRegistry.register` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | plugin: AppLifecycleHookPlugin | Unit |  | 66 |
| `AppLifecycleHookPluginRegistry.unregister` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | pluginId: String | Unit |  | 72 |
| `AppLifecycleHookPluginRegistry.dispatch` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | event: AppLifecycleEvent<br>params: AppLifecycleHookParams | Unit |  | 76 |
| `AppLifecycleHookPluginRegistry.dispatchAsync` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | event: AppLifecycleEvent<br>params: AppLifecycleHookParams | Unit |  | 90 |
| `AppLifecycleHookPluginRegistry.getReplayableApplicationEvents` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` |  | List<AppLifecycleReplayEvent> |  | 99 |
| `AppLifecycleHookPluginRegistry.recordReplayableState` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | event: AppLifecycleEvent<br>params: AppLifecycleHookParams | Unit |  | 122 |
| `OperitPlugin.register` | `OperitPlugin` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` |  | Unit |  | 12 |
| `PluginRegistry.register` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` | plugin: OperitPlugin | Unit |  | 23 |
| `PluginRegistry.initializeBuiltins` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` |  | Unit |  | 29 |
| `PluginRegistry.installAll` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` |  | Unit |  | 40 |
| `ToolPkgAppLifecycleHookPlugin.onEvent` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | event: AppLifecycleEvent<br>params: AppLifecycleHookParams | Unit |  | 30 |
| `ToolPkgAppLifecycleHookPlugin.syncToolPkgRegistrations` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | activeContainers: List<ToolPkgContainerRuntime> | Map<String, List<ToolPkgAppLifecycleHookRegistration>> |  | 41 |
| `ToolPkgAppLifecycleHookPlugin.replayHooks` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | replayEvents: List<AppLifecycleReplayEvent><br>hooksToReplayByEvent: Map<String, List<ToolPkgAppLifecycl… | Unit |  | 78 |
| `ToolPkgAppLifecycleHookPlugin.dispatchHooks` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | hooks: List<ToolPkgAppLifecycleHookRegistr…<br>params: AppLifecycleHookParams | Unit |  | 99 |
| `ToolboxPlugin.register` | `ToolboxPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` |  | Unit |  | 145 |
| `ToolboxPlugin.syncAndReplayToolPkgLifecycleHooks` | `ToolboxPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 156 |
| `ToolPkgAiProviderRegistry.register` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` |  | Unit |  | 18 |
| `ToolPkgAiProviderRegistry.get` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` | providerId: String | ToolPkgAiProviderRegistration? |  | 26 |
| `ToolPkgAiProviderRegistry.list` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` |  | List<ToolPkgAiProviderRegistration> |  | 31 |
| `ToolPkgAiProviderRegistry.releasedTokenProviderAliases` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` |  | Map<String, String> |  | 36 |
| `ToolPkgAiProviderRegistry.syncToolPkgRegistrations` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 48 |
| `ToolPkgChatInputHookBridge.Bridge.onEvent` | `Bridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | context: ChatInputHookContext | ChatInputHookResult? |  | 33 |
| `ToolPkgChatInputHookBridge.register` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` |  | Unit |  | 38 |
| `ToolPkgChatInputHookBridge.dispatchChatInputHooks` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | context: ChatInputHookContext | ChatInputHookResult? |  | 49 |
| `ToolPkgChatInputHookBridge.syncToolPkgRegistrations` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 163 |
| `ToolPkgChatInputHookBridge.buildChatInputEventPayload` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | context: ChatInputHookContext | Map<String, Any?> |  | 181 |
| `ToolPkgChatInputHookBridge.parseChatInputHookResult` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | decoded: Any? | ChatInputHookResult? |  | 195 |
| `ToolPkgChatMessageHookBridge.register` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` |  | Unit |  | 27 |
| `ToolPkgChatMessageHookBridge.dispatchMessagePersisted` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | chatId: String<br>message: ChatMessage | Unit |  | 40 |
| `ToolPkgChatMessageHookBridge.syncToolPkgRegistrations` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 72 |
| `ToolPkgChatMessageHookBridge.buildChatMessageEventPayload` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | chatId: String<br>message: ChatMessage | Map<String, Any?> |  | 90 |
| `ToolPkgChatMessageMenuItemBridge.register` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` |  | Unit |  | 35 |
| `ToolPkgChatMessageMenuItemBridge.createMenuItems` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | params: ChatMessageMenuItemParams | List<ChatMessageMenuItemDefinition> |  | 46 |
| `ToolPkgChatMessageMenuItemBridge.syncToolPkgRegistrations` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 65 |
| `ToolPkgChatMessageMenuItemBridge.dispatchClick` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | item: ToolPkgChatMessageMenuItemRegistrat…<br>params: ChatMessageMenuItemParams | ChatMessageMenuItemClickResult? |  | 95 |
| `ToolPkgChatMessageMenuItemBridge.buildDialogRequest` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | context: Context<br>item: ToolPkgChatMessageMenuItemRegistrat…<br>eventPayload: Map<String, Any?><br>decoded: Any? | ChatMessageMenuDialogRequest? |  | 145 |
| `ToolPkgChatMessageMenuItemBridge.buildEventPayload` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | params: ChatMessageMenuItemParams<br>menuItemId: String | Map<String, Any?> |  | 185 |
| `ToolPkgChatMessageMenuItemBridge.buildMessagePayload` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | message: ChatMessage | Map<String, Any?> |  | 197 |
| `ToolPkgChatRuntimeHookBridge.register` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` |  | Unit |  | 29 |
| `ToolPkgChatRuntimeHookBridge.onEvent` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | event: ChatRuntimeHookEvent<br>context: ChatRuntimeHookContext | Unit |  | 40 |
| `ToolPkgChatRuntimeHookBridge.syncToolPkgRegistrations` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 74 |
| `ToolPkgChatRuntimeHookBridge.buildChatRuntimeEventPayload` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | context: ChatRuntimeHookContext | Map<String, Any?> |  | 92 |
| `ToolPkgChatRuntimeHookBridge.stateName` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | state: InputProcessingState | String |  | 108 |
| `ToolPkgChatRuntimeHookBridge.stateMessage` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | state: InputProcessingState | String? |  | 123 |
| `ToolPkgChatRuntimeHookBridge.stateToolName` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | state: InputProcessingState | String? |  | 135 |
| `ToolPkgChatRuntimeHookBridge.stateProgress` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | state: InputProcessingState | Float? |  | 143 |
| `ToolPkgChatRuntimeHookBridge.stateIsActive` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | state: InputProcessingState | Boolean |  | 149 |
| `ToolPkgChatViewHookBridge.register` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` |  | Unit |  | 32 |
| `ToolPkgChatViewHookBridge.onEvent` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | event: ChatViewEvent<br>params: ChatViewHookParams | Unit |  | 43 |
| `ToolPkgChatViewHookBridge.syncAndReplayToolPkgRegistrations` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 77 |
| `ToolPkgChatViewHookBridge.replayOpenViews` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | hooksToReplay: List<ToolPkgChatViewHookRegistratio…<br>replayParams: List<ChatViewHookParams> | Unit |  | 111 |
| `ToolPkgChatViewHookBridge.buildChatViewEventPayload` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | params: ChatViewHookParams | Map<String, Any?> |  | 146 |
| `packageManager` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | context: Context | PackageManager |  | 50 |
| `decodeHookResult` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | raw: Any? | Any? |  | 54 |
| `logPreview` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | text: String<br>maxLength: Int? | String |  | 74 |
| `summarizeHookValue` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | value: Any? | String |  | 82 |
| `ToolPkgMessageProcessingBridgePlugin.replaceHooks` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | updatedHooks: List<ToolPkgMessageProcessingHookRe… | Unit |  | 94 |
| `ToolPkgMessageProcessingBridgePlugin.createExecutionIfMatched` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | params: MessageProcessingHookParams | MessageProcessingExecution? |  | 98 |
| `ToolPkgMessageProcessingBridgePlugin.buildMessageEventPayload` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | params: MessageProcessingHookParams<br>probeOnly: Boolean | Map<String, Any?> |  | 188 |
| `ToolPkgMessageProcessingBridgePlugin.promptTurnToMap` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | turn: PromptTurn | Map<String, Any?> |  | 203 |
| `ToolPkgMessageProcessingBridgePlugin.runMessageProcessingHook` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | manager: PackageManager<br>hook: ToolPkgMessageProcessingHookRegistr…<br>eventPayload: Map<String, Any?><br>onIntermediateResult: ((Any?) -> Unit)?? | Any? |  | 212 |
| `ToolPkgMessageProcessingBridgePlugin.nextMessageProcessingExecutionId` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | hook: ToolPkgMessageProcessingHookRegistr… | String |  | 283 |
| `ToolPkgMessageProcessingBridgePlugin.createStreamingExecution` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | manager: PackageManager<br>hook: ToolPkgMessageProcessingHookRegistr…<br>eventPayload: Map<String, Any?><br>executionId: String | MessageProcessingExecution |  | 289 |
| `parseMessageProcessingResult` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | decoded: Any? | ParsedMessageProcessingResult? |  | 361 |
| `extractMessageChunks` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | decoded: Any? | List<String> |  | 396 |
| `RegisteredMessageProcessingController.cancel` | `RegisteredMessageProcessingController` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` |  | Unit |  | 444 |
| `ToolPkgXmlRenderBridgePlugin.replaceHooksByTag` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | updatedHooksByTag: Map<String, List<ToolPkgXmlRenderHo… | Unit |  | 458 |
| `ToolPkgXmlRenderBridgePlugin.supports` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | tagName: String | Boolean |  | 468 |
| `ToolPkgXmlRenderBridgePlugin.resolve` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | context: Context<br>xmlContent: String<br>tagName: String<br>textColor: Color<br>xmlStream: Stream<String>? | XmlRenderResult? |  | 476 |
| `ToolPkgXmlRenderBridgePlugin.parseXmlRenderHookObjectResult` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | decoded: Any? | ToolPkgXmlRenderHookObjectResult? |  | 548 |
| `ToolPkgXmlRenderBridgePlugin.parseComposeDslResult` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | raw: Any? | ToolPkgXmlRenderHookComposeDslResult? |  | 571 |
| `ToolPkgXmlRenderBridgePlugin.asMap` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | value: Any? | Map<String, Any?> |  | 596 |
| `ToolPkgXmlRenderBridgePlugin.asList` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | value: Any? | List<Any?> |  | 614 |
| `ToolPkgXmlRenderBridgePlugin.normalizeValue` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | value: Any? | Any? |  | 628 |
| `ToolPkgInputMenuToggleBridgePlugin.replaceHooks` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | updatedHooks: List<ToolPkgInputMenuToggleHookRegi… | Unit |  | 655 |
| `ToolPkgInputMenuToggleBridgePlugin.createToggles` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | params: InputMenuToggleHookParams | List<InputMenuToggleDefinition> |  | 667 |
| `ToolPkgInputMenuToggleBridgePlugin.buildCacheKey` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | params: InputMenuToggleHookParams | String |  | 691 |
| `ToolPkgInputMenuToggleBridgePlugin.buildToggleDefinitions` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | specs: List<InputMenuSpec><br>params: InputMenuToggleHookParams | List<InputMenuToggleDefinition> |  | 697 |
| `ToolPkgInputMenuToggleBridgePlugin.createLoadingToggle` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` |  | InputMenuToggleDefinition |  | 745 |
| `ToolPkgInputMenuToggleBridgePlugin.triggerRefresh` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | params: InputMenuToggleHookParams<br>registryVersion: Long<br>paramsCacheKey: String | Unit |  | 756 |
| `ToolPkgInputMenuToggleBridgePlugin.loadSpecs` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | params: InputMenuToggleHookParams | List<InputMenuSpec> |  | 783 |
| `ToolPkgInputMenuToggleBridgePlugin.parseInputMenuDefinitions` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | decoded: Any?<br>containerPackageName: String<br>functionName: String<br>pluginId: String<br>functionSource: String? | List<InputMenuSpec> |  | 847 |
| `ToolPkgCommonBridgePlugin.register` | `ToolPkgCommonBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` |  | Unit |  | 896 |
| `ToolPkgCommonBridgePlugin.syncToolPkgRegistrations` | `ToolPkgCommonBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 917 |
| `toolPkgPackageManager` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` |  | PackageManager |  | 133 |
| `decodeToolPkgHookResult` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | raw: Any? | Any? |  | 138 |
| `jsonObjectToMap` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | jsonObject: JSONObject | Map<String, Any?> |  | 158 |
| `jsonArrayToList` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | jsonArray: JSONArray | List<Any?> |  | 162 |
| `jsonValueToKotlin` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookBridgeSupport.kt` | value: Any? | Any? |  | 166 |
| `ToolPkgHookExecutionBudget.create` | `ToolPkgHookExecutionBudget` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookExecutionBudget.kt` |  | ToolPkgHookExecutionBudget |  | 21 |
| `ToolPkgHookExecutionBudget.remainingMillis` | `ToolPkgHookExecutionBudget` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookExecutionBudget.kt` |  | Long? |  | 33 |
| `ToolPkgHookExecutionBudget.elapsedMillis` | `ToolPkgHookExecutionBudget` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookExecutionBudget.kt` |  | Long |  | 41 |
| `ToolPkgHookExecutionBudget.logDeadlineReached` | `ToolPkgHookExecutionBudget` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookExecutionBudget.kt` | tag: String<br>stage: String<br>containerPackageName: String<br>hookId: String | Unit |  | 44 |
| `ToolPkgHookExecutionBudget.logTimeoutIfPresent` | `ToolPkgHookExecutionBudget` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgHookExecutionBudget.kt` | result: Result<Any?><br>tag: String<br>stage: String<br>containerPackageName: String<br>hookId: String | Boolean |  | 56 |
| `ToolPkgMessageProcessingCancellationRegistry.register` | `ToolPkgMessageProcessingCancellationRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgMessageProcessingCancellationRegistry.kt` | executionId: String<br>controller: MessageProcessingController | Boolean |  | 14 |
| `ToolPkgMessageProcessingCancellationRegistry.unregister` | `ToolPkgMessageProcessingCancellationRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgMessageProcessingCancellationRegistry.kt` | executionId: String | Boolean |  | 34 |
| `ToolPkgMessageProcessingCancellationRegistry.cancel` | `ToolPkgMessageProcessingCancellationRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgMessageProcessingCancellationRegistry.kt` | executionId: String | Boolean |  | 45 |
| `ToolPkgPromptHookBridge.PromptInputBridge.onEvent` | `PromptInputBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | context: PromptHookContext | PromptHookMutation? |  | 55 |
| `ToolPkgPromptHookBridge.PromptHistoryBridge.onEvent` | `PromptHistoryBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | context: PromptHookContext | PromptHookMutation? |  | 68 |
| `ToolPkgPromptHookBridge.PromptEstimateHistoryBridge.onEvent` | `PromptEstimateHistoryBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | context: PromptHookContext | PromptHookMutation? |  | 81 |
| `ToolPkgPromptHookBridge.SystemPromptComposeBridge.onEvent` | `SystemPromptComposeBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | context: PromptHookContext | PromptHookMutation? |  | 94 |
| `ToolPkgPromptHookBridge.ToolPromptComposeBridge.onEvent` | `ToolPromptComposeBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | context: PromptHookContext | PromptHookMutation? |  | 107 |
| `ToolPkgPromptHookBridge.PromptFinalizeBridge.onEvent` | `PromptFinalizeBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | context: PromptHookContext | PromptHookMutation? |  | 120 |
| `ToolPkgPromptHookBridge.PromptEstimateFinalizeBridge.onEvent` | `PromptEstimateFinalizeBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | context: PromptHookContext | PromptHookMutation? |  | 133 |
| `ToolPkgPromptHookBridge.register` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` |  | Unit |  | 143 |
| `ToolPkgPromptHookBridge.dispatchPromptHooks` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | hooks: List<ToolPkgPromptHookRegistration><br>familyEvent: String<br>context: PromptHookContext<br>parseMutation: (Any?, PromptHookContext) -> Prompt… | PromptHookMutation? |  | 159 |
| `ToolPkgPromptHookBridge.syncToolPkgRegistrations` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 246 |
| `ToolPkgPromptHookBridge.buildPromptEventPayload` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | context: PromptHookContext | Map<String, Any?> |  | 360 |
| `ToolPkgPromptHookBridge.promptTurnToMap` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | message: PromptTurn | Map<String, Any?> |  | 379 |
| `ToolPkgPromptHookBridge.applyMutation` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | context: PromptHookContext<br>mutation: PromptHookMutation | PromptHookContext |  | 388 |
| `ToolPkgPromptHookBridge.parsePromptInputMutation` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | decoded: Any?<br>context: PromptHookContext | PromptHookMutation? |  | 404 |
| `ToolPkgPromptHookBridge.parsePromptHistoryMutation` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | decoded: Any?<br>context: PromptHookContext | PromptHookMutation? |  | 416 |
| `ToolPkgPromptHookBridge.parseSystemPromptMutation` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | decoded: Any?<br>context: PromptHookContext | PromptHookMutation? |  | 435 |
| `ToolPkgPromptHookBridge.parseToolPromptMutation` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | decoded: Any?<br>context: PromptHookContext | PromptHookMutation? |  | 447 |
| `ToolPkgPromptHookBridge.parsePromptFinalizeMutation` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | decoded: Any?<br>context: PromptHookContext | PromptHookMutation? |  | 459 |
| `ToolPkgPromptHookBridge.parsePromptHookObject` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | jsonObject: JSONObject | PromptHookMutation |  | 475 |
| `ToolPkgPromptHookBridge.parsePromptToolItems` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | jsonArray: JSONArray? | List<Map<String, Any?>>? |  | 489 |
| `ToolPkgPromptHookBridge.parsePromptTurns` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | jsonArray: JSONArray? | List<PromptTurn>? |  | 501 |
| `ToolPkgSummaryHookBridge.SummaryGenerateBridge.onEvent` | `SummaryGenerateBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | context: SummaryHookContext | SummaryHookMutation? |  | 32 |
| `ToolPkgSummaryHookBridge.register` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` |  | Unit |  | 41 |
| `ToolPkgSummaryHookBridge.dispatchSummaryHooks` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | hooks: List<ToolPkgPromptHookRegistration><br>familyEvent: String<br>context: SummaryHookContext | SummaryHookMutation? |  | 51 |
| `ToolPkgSummaryHookBridge.syncToolPkgRegistrations` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 132 |
| `ToolPkgSummaryHookBridge.buildSummaryEventPayload` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | context: SummaryHookContext | Map<String, Any?> |  | 150 |
| `ToolPkgSummaryHookBridge.promptTurnToMap` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | message: PromptTurn | Map<String, Any?> |  | 166 |
| `ToolPkgSummaryHookBridge.applyMutation` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | context: SummaryHookContext<br>mutation: SummaryHookMutation | SummaryHookContext |  | 175 |
| `ToolPkgSummaryHookBridge.parseSummaryMutation` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | decoded: Any?<br>context: SummaryHookContext | SummaryHookMutation? |  | 189 |
| `ToolPkgSummaryHookBridge.parseSummaryHookObject` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | jsonObject: JSONObject | SummaryHookMutation |  | 206 |
| `ToolPkgSummaryHookBridge.parsePromptTurns` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | jsonArray: JSONArray? | List<PromptTurn>? |  | 218 |
| `ToolPkgToolLifecycleBridge.register` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` |  | Unit |  | 50 |
| `ToolPkgToolLifecycleBridge.onToolCallRequested` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | tool: AITool | Unit |  | 60 |
| `ToolPkgToolLifecycleBridge.onToolCallIntercept` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | tool: AITool | AIToolHookDecision |  | 67 |
| `ToolPkgToolLifecycleBridge.onToolPermissionChecked` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | tool: AITool<br>granted: Boolean<br>reason: String? | Unit |  | 110 |
| `ToolPkgToolLifecycleBridge.onToolExecutionStarted` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | tool: AITool | Unit |  | 120 |
| `ToolPkgToolLifecycleBridge.onToolExecutionResult` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | tool: AITool<br>result: ToolResult | Unit |  | 127 |
| `ToolPkgToolLifecycleBridge.onToolExecutionError` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | tool: AITool<br>throwable: Throwable | Unit |  | 139 |
| `ToolPkgToolLifecycleBridge.onToolExecutionFinished` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | tool: AITool | Unit |  | 149 |
| `ToolPkgToolLifecycleBridge.enqueue` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | eventName: String<br>eventPayload: Map<String, Any?> | Unit |  | 156 |
| `ToolPkgToolLifecycleBridge.deliver` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | dispatch: ToolLifecycleDispatch | Unit |  | 168 |
| `ToolPkgToolLifecycleBridge.parseToolCallInterceptDecision` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | decoded: Any? | AIToolHookDecision? |  | 191 |
| `ToolPkgToolLifecycleBridge.buildBasePayload` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | tool: AITool | Map<String, Any?> |  | 224 |
| `ToolPkgToolLifecycleBridge.parseToolResultJson` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | result: ToolResult | Any? |  | 232 |
| `ToolPkgToolLifecycleBridge.syncToolPkgRegistrations` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit |  | 245 |
| `WorkflowAppLifecycleHookPlugin.onEvent` | `WorkflowAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.workflow` | `WorkflowLifecyclePlugin.kt` | event: AppLifecycleEvent<br>params: AppLifecycleHookParams | Unit |  | 18 |
| `WorkflowLifecyclePlugin.register` | `WorkflowLifecyclePlugin` | `com.ai.assistance.operit.plugins.workflow` | `WorkflowLifecyclePlugin.kt` |  | Unit |  | 53 |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `AppLifecycleHookPluginRegistry.applicationCreateParams` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | AppLifecycleHookParams? |  | 62 |
| `AppLifecycleHookPluginRegistry.applicationForegroundParams` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | AppLifecycleHookParams? |  | 63 |
| `AppLifecycleHookPluginRegistry.dispatchScope` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | inferred |  | 60 |
| `AppLifecycleHookPluginRegistry.plugins` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | inferred |  | 59 |
| `AppLifecycleHookPluginRegistry.stateLock` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | inferred |  | 61 |
| `AppLifecycleHookPluginRegistry.TAG` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | inferred |  | 58 |
| `CHAT_MESSAGE_EVENT_MESSAGE_PERSISTED` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | inferred |  | 15 |
| `CHAT_MESSAGE_MENU_ITEM_CLICK` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | inferred |  | 22 |
| `ChatMessageMenuItemRegistry.changeVersion` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | StateFlow<Int> |  | 47 |
| `ChatMessageMenuItemRegistry.changeVersionMutable` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | inferred |  | 46 |
| `ChatMessageMenuItemRegistry.plugins` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | inferred |  | 45 |
| `ChatViewHookPluginRegistry.dispatchScope` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | inferred |  | 39 |
| `ChatViewHookPluginRegistry.openViewsById` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | inferred |  | 41 |
| `ChatViewHookPluginRegistry.plugins` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | inferred |  | 38 |
| `ChatViewHookPluginRegistry.stateLock` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | inferred |  | 40 |
| `ChatViewHookPluginRegistry.TAG` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | inferred |  | 37 |
| `PluginRegistry.builtinsInitialized` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` | inferred |  | 20 |
| `PluginRegistry.installedPluginIds` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` | inferred |  | 17 |
| `PluginRegistry.plugins` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` | inferred |  | 16 |
| `TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | inferred |  | 19 |
| `TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | inferred |  | 14 |
| `TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | inferred |  | 21 |
| `TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | inferred |  | 16 |
| `TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | inferred |  | 18 |
| `TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | inferred |  | 47 |
| `TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | inferred |  | 29 |
| `TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | inferred |  | 18 |
| `TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | inferred |  | 23 |
| `TOOL_LIFECYCLE_EVENT_TOOL_CALL_INTERCEPT` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | inferred |  | 24 |
| `ToolboxPlugin.id` | `ToolboxPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | String |  | 137 |
| `ToolboxPlugin.installed` | `ToolboxPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | inferred |  | 138 |
| `ToolboxPlugin.replayScope` | `ToolboxPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | inferred |  | 139 |
| `ToolboxPlugin.runtimeChangeListener` | `ToolboxPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | inferred |  | 140 |
| `TOOLPKG_LOG_TAG` | — | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | inferred |  | 48 |
| `ToolPkgAiProviderRegistry.installed` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` | inferred |  | 8 |
| `ToolPkgAiProviderRegistry.providersById` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` | Map<String, ToolPkgAiProviderRegistration> |  | 11 |
| `ToolPkgAiProviderRegistry.runtimeChangeListener` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` | inferred |  | 13 |
| `ToolPkgAppLifecycleHookPlugin.hooksByEvent` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | Map<String, List<ToolPkgAppLifecycleHookRegistration>> |  | 26 |
| `ToolPkgAppLifecycleHookPlugin.id` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | String |  | 28 |
| `ToolPkgAppLifecycleHookPlugin.TAG` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | inferred |  | 24 |
| `ToolPkgChatInputHookBridge.hooks` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | List<ToolPkgChatInputHookRegistration> |  | 24 |
| `ToolPkgChatInputHookBridge.installed` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | inferred |  | 22 |
| `ToolPkgChatInputHookBridge.runtimeChangeListener` | `ToolPkgChatInputHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatInputHookBridge.kt` | inferred |  | 25 |
| `ToolPkgChatMessageHookBridge.dispatchScope` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | inferred |  | 19 |
| `ToolPkgChatMessageHookBridge.hooks` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | List<ToolPkgChatMessageHookRegistration> |  | 21 |
| `ToolPkgChatMessageHookBridge.installed` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | inferred |  | 18 |
| `ToolPkgChatMessageHookBridge.onMessagePersistedDispatchedForTest` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | ((chatId: String, message: ChatMessage) -> Unit)? |  | 38 |
| `ToolPkgChatMessageHookBridge.runtimeChangeListener` | `ToolPkgChatMessageHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageHookBridge.kt` | inferred |  | 22 |
| `ToolPkgChatMessageMenuItemBridge.id` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | String |  | 33 |
| `ToolPkgChatMessageMenuItemBridge.installed` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | inferred |  | 25 |
| `ToolPkgChatMessageMenuItemBridge.menuItems` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | List<ToolPkgChatMessageMenuItemRegistration> |  | 27 |
| `ToolPkgChatMessageMenuItemBridge.runtimeChangeListener` | `ToolPkgChatMessageMenuItemBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatMessageMenuItemBridge.kt` | inferred |  | 28 |
| `ToolPkgChatRuntimeHookBridge.hooks` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | List<ToolPkgChatRuntimeHookRegistration> |  | 21 |
| `ToolPkgChatRuntimeHookBridge.id` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | String |  | 27 |
| `ToolPkgChatRuntimeHookBridge.installed` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | inferred |  | 19 |
| `ToolPkgChatRuntimeHookBridge.runtimeChangeListener` | `ToolPkgChatRuntimeHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatRuntimeHookBridge.kt` | inferred |  | 22 |
| `ToolPkgChatViewHookBridge.hooks` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | List<ToolPkgChatViewHookRegistration> |  | 24 |
| `ToolPkgChatViewHookBridge.id` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | String |  | 30 |
| `ToolPkgChatViewHookBridge.installed` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | inferred |  | 21 |
| `ToolPkgChatViewHookBridge.replayScope` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | inferred |  | 22 |
| `ToolPkgChatViewHookBridge.runtimeChangeListener` | `ToolPkgChatViewHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgChatViewHookBridge.kt` | inferred |  | 25 |
| `ToolPkgCommonBridgePlugin.id` | `ToolPkgCommonBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | String |  | 889 |
| `ToolPkgCommonBridgePlugin.installed` | `ToolPkgCommonBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | inferred |  | 890 |
| `ToolPkgCommonBridgePlugin.runtimeChangeListener` | `ToolPkgCommonBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | inferred |  | 891 |
| `ToolPkgInputMenuToggleBridgePlugin.hasLoadedOnce` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | inferred |  | 646 |
| `ToolPkgInputMenuToggleBridgePlugin.hookRegistryVersion` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | inferred |  | 648 |
| `ToolPkgInputMenuToggleBridgePlugin.hooks` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | List<ToolPkgInputMenuToggleHookRegistration> |  | 642 |
| `ToolPkgInputMenuToggleBridgePlugin.id` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | String |  | 639 |
| `ToolPkgInputMenuToggleBridgePlugin.lastHookRegistryVersion` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | inferred |  | 650 |
| `ToolPkgInputMenuToggleBridgePlugin.lastParamsCacheKey` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | String? |  | 652 |
| `ToolPkgInputMenuToggleBridgePlugin.refreshFlag` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | inferred |  | 653 |
| `ToolPkgInputMenuToggleBridgePlugin.scope` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | inferred |  | 640 |
| `ToolPkgInputMenuToggleBridgePlugin.specsCache` | `ToolPkgInputMenuToggleBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | List<InputMenuSpec> |  | 644 |
| `ToolPkgMessageProcessingBridgePlugin.hooks` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | List<ToolPkgMessageProcessingHookRegistration> |  | 92 |
| `ToolPkgMessageProcessingBridgePlugin.id` | `ToolPkgMessageProcessingBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | String |  | 90 |
| `ToolPkgMessageProcessingCancellationRegistry.controllers` | `ToolPkgMessageProcessingCancellationRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgMessageProcessingCancellationRegistry.kt` | inferred |  | 10 |
| `ToolPkgMessageProcessingCancellationRegistry.pendingCancels` | `ToolPkgMessageProcessingCancellationRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgMessageProcessingCancellationRegistry.kt` | inferred |  | 11 |
| `ToolPkgMessageProcessingCancellationRegistry.TAG` | `ToolPkgMessageProcessingCancellationRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgMessageProcessingCancellationRegistry.kt` | inferred |  | 8 |
| `ToolPkgPromptHookBridge.installed` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | inferred |  | 32 |
| `ToolPkgPromptHookBridge.promptEstimateFinalizeHooks` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | List<ToolPkgPromptHookRegistration> |  | 46 |
| `ToolPkgPromptHookBridge.promptEstimateHistoryHooks` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | List<ToolPkgPromptHookRegistration> |  | 38 |
| `ToolPkgPromptHookBridge.promptFinalizeHooks` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | List<ToolPkgPromptHookRegistration> |  | 44 |
| `ToolPkgPromptHookBridge.promptHistoryHooks` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | List<ToolPkgPromptHookRegistration> |  | 36 |
| `ToolPkgPromptHookBridge.promptInputHooks` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | List<ToolPkgPromptHookRegistration> |  | 34 |
| `ToolPkgPromptHookBridge.runtimeChangeListener` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | inferred |  | 47 |
| `ToolPkgPromptHookBridge.systemPromptComposeHooks` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | List<ToolPkgPromptHookRegistration> |  | 40 |
| `ToolPkgPromptHookBridge.toolPromptComposeHooks` | `ToolPkgPromptHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgPromptHookBridge.kt` | List<ToolPkgPromptHookRegistration> |  | 42 |
| `ToolPkgSummaryHookBridge.installed` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | inferred |  | 21 |
| `ToolPkgSummaryHookBridge.runtimeChangeListener` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | inferred |  | 24 |
| `ToolPkgSummaryHookBridge.summaryGenerateHooks` | `ToolPkgSummaryHookBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgSummaryHookBridge.kt` | List<ToolPkgPromptHookRegistration> |  | 23 |
| `ToolPkgToolLifecycleBridge.dispatchChannel` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | inferred |  | 34 |
| `ToolPkgToolLifecycleBridge.dispatchScope` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | inferred |  | 33 |
| `ToolPkgToolLifecycleBridge.hooks` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | List<ToolPkgToolLifecycleHookRegistration> |  | 36 |
| `ToolPkgToolLifecycleBridge.installed` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | inferred |  | 32 |
| `ToolPkgToolLifecycleBridge.runtimeChangeListener` | `ToolPkgToolLifecycleBridge` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgToolLifecycleBridge.kt` | inferred |  | 37 |
| `ToolPkgXmlRenderBridgePlugin.hooksByTag` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | Map<String, List<ToolPkgXmlRenderHookRegistration>> |  | 456 |
| `ToolPkgXmlRenderBridgePlugin.id` | `ToolPkgXmlRenderBridgePlugin` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgCommonBridgePlugin.kt` | String |  | 454 |
| `WorkflowAppLifecycleHookPlugin.firstActivityStartHandled` | `WorkflowAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.workflow` | `WorkflowLifecyclePlugin.kt` | inferred |  | 14 |
| `WorkflowAppLifecycleHookPlugin.id` | `WorkflowAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.workflow` | `WorkflowLifecyclePlugin.kt` | String |  | 16 |
| `WorkflowAppLifecycleHookPlugin.TAG` | `WorkflowAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.workflow` | `WorkflowLifecyclePlugin.kt` | inferred |  | 12 |
| `WorkflowLifecyclePlugin.id` | `WorkflowLifecyclePlugin` | `com.ai.assistance.operit.plugins.workflow` | `WorkflowLifecyclePlugin.kt` | String |  | 51 |
