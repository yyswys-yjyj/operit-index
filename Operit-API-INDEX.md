# Operit 源码 API 索引

扫描 `../Operit` 下全部 Kotlin 源码，抽取每一个可调用单元。

| 指标 | 数值 |
| --- | --- |
| 源文件 | 1476 |
| 代码行 | 500,753 |
| 包 | 264 |
| 函数 | 14,543 |
| 类型（class/object/interface/enum） | 3,042 |
| 顶层常量 / object 属性 | 1,640 |
| 合计声明 | 19,225 |
| 其中测试代码 | 1,577（表格里标 ⚑） |

生成时间：2026-11-14T08:30:20.203Z

---

## 怎么用这张表

| 你想要 | 打开 |
| --- | --- |
| 查某个函数在哪、怎么调 | 本文件「核心 API 速查」，或 `Operit-API-INDEX/*.md` 里搜函数名 |
| 插件能调什么 JS API | [`Operit-API-INDEX/js-runtime.md`](Operit-API-INDEX/js-runtime.md)（`Tools.*` / `ToolPkg.*` 共 179+17 个） |
| 机器读 / 写代码生成 | `Operit-API-INDEX.json`（18.6 MB，含参数类型、默认值、可见性、注解、关键词） |
| grep / 导入 Excel | `Operit-API-INDEX/functions.tsv`（制表符分隔，一行一条） |
| 按关键词找入口 | 本文件「关键词倒排」 |

**列含义**

每条声明都带三个定位字段，JSON 里是 `package` / `className` / `fileName`，表格里是「包名 / 类名 / 文件名」三列：

- **包名**：`package` 声明的完整包名，如 `com.ai.assistance.operit.api.chat`；文件没写 package 则为空（表格显示 —）。
- **类名**：该声明所属的类/对象名。类型声明自身就是自己的名字；顶层函数与顶层属性没有类，显示 —。**嵌套类只给最近一层**（`Outer.Inner` → `Inner`），完整嵌套链看 `container` / `qualified`。
- **文件名**：纯文件名（含 `.kt`），不带目录，如 `JsEngine.kt`。完整相对路径看 `file`，行号看 `line`。

其余：

- **参数**：`名字: 类型`，结尾 `?` 表示该参数有默认值（调用时可省略）。
- **返回**：Kotlin 返回类型；`Unit` 表示无返回值。集合类型即导出结构。
- **签名 / 字段**：`data class` 的括号里是构造参数，也就是它序列化后的字段。
- **说明**：取自 KDoc 首段；空表示源码本身没写注释（不是我漏抓）。
- **行**：声明在文件里的行号，和「文件名」拼起来就是完整位置。

---

## 核心 API 速查

按插件开发 / 运行时调试最常打交道的区域挑出来，完整清单见分册。

### ToolPkg 装载 / 注册 / 生命周期

`com.ai.assistance.operit.core.tools.packTool…` · 370 个函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `PackageDebugRefreshReceiver.onReceive` | `PackageDebugRefreshReceiver` | `com.ai.assistance.operit.core.tools.packTool` | `PackageDebugRefreshReceiver.kt` | context: Context, intent: Intent | Unit | 21 |
| `PackageDebugRefreshReceiver.refreshPackages` | `PackageDebugRefreshReceiver` | `com.ai.assistance.operit.core.tools.packTool` | `PackageDebugRefreshReceiver.kt` | context: Context, reactivateActivePackages: Boolean | Unit | 37 |
| `PackageManager.getInstance` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | context: Context, aiToolHandler: AIToolHandler | PackageManager | 89 |
| `PackageManager.peekInstance` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` |  | PackageManager? | 100 |
| `PackageManager.onToolPkgRuntimeChanged` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit | 302 |
| `PackageManager.logToolPkgInfo` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | message: String | Unit | 339 |
| `PackageManager.logToolPkgError` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | message: String, tr: Throwable?? | Unit | 343 |
| `PackageManager.persistEnabledPackageNamesToPrefs` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | enabledPackageNames: List<String> | Unit | 351 |
| `PackageManager.persistToolPkgSubpackageStatesToPrefs` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | states: Map<String, Boolean> | Unit | 357 |
| `PackageManager.decodeEnabledPackageNamesFromPrefs` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` |  | List<String> | 363 |
| `PackageManager.migrateRenamedPackagePreferencesIfNeeded` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` |  | Unit | 376 |
| `PackageManager.migrate` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | packageNames: List<String> | List<String> | 381 |
| `PackageManager.decodeToolPkgSubpackageStatesFromPrefs` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` |  | Map<String, Boolean> | 410 |
| `PackageManager.buildEnabledToolPkgContainerRuntimes` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | enabledPackageNames: List<String> | List<ToolPkgContainerRuntime> | 422 |
| `PackageManager.updateToolPkgPluginOrder` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | order: List<String> | Unit | 432 |
| `PackageManager.notifyToolPkgRuntimeChangeListeners` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` |  | Unit | 442 |
| `PackageManager.refreshToolPkgRuntimeState` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | persistIfChanged: Boolean, enabledPackageNamesOverride: List<String>??, subpackageStatesOverride: Map<String, Boolean>?? | Unit | 454 |
| `PackageManager.getToolPkgExecutionEngine` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | contextKey: String, containerPackageName: String | JsEngine | 489 |
| `PackageManager.acquireToolPkgExecutionEngine` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | contextKey: String, containerPackageName: String | JsEngine | 496 |
| `PackageManager.findToolPkgExecutionEngine` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | contextKey: String | JsEngine? | 503 |
| `PackageManager.releaseToolPkgExecutionEngine` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | contextKey: String, executionEngine: JsEngine | Unit | 507 |
| `PackageManager.releaseToolPkgExecutionEngine` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | contextKey: String | Unit | 514 |
| `PackageManager.destroyToolPkgExecutionEngines` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | packageName: String | Unit | 519 |
| `PackageManager.resolveToolPkgSubpackageRuntimeInternal` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | nameOrId: String | ToolPkgSubpackageRuntime? | 531 |
| `PackageManager.getToolPkgMainScriptInternal` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | containerPackageName: String | String? | 535 |
| `PackageManager.addToolPkgRuntimeChangeListener` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | listener: ToolPkgRuntimeChangeListener | Unit | 539 |
| `PackageManager.removeToolPkgRuntimeChangeListener` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | listener: ToolPkgRuntimeChangeListener | Unit | 553 |
| `PackageManager.getEnabledPackageNameSetInternal` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` |  | Set<String> | 557 |
| `PackageManager.getEnabledToolPkgContainerRuntimes` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` |  | List<ToolPkgContainerRuntime> | 565 |
| `PackageManager.cancelToolPkgExecutionsForChat` | `PackageManager` | `com.ai.assistance.operit.core.tools.packTool` | `PackageManager.kt` | chatId: String, reason: String? | Boolean | 573 |
| … | | | | 还有 340 个，见分册 | | |

### QuickJS 引擎与 JS 桥接

`com.ai.assistance.operit.core.tools.javascript…` · 467 个函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `readJavaScriptAsset` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsAssetLoader.kt` | context: Context, assetPath: String, label: String | String | 8 |
| `loadUINodeJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsAssetLoader.kt` | context: Context | String | 21 |
| `loadAndroidUtilsJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsAssetLoader.kt` | context: Context | String | 24 |
| `loadOkHttp3Js` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsAssetLoader.kt` | context: Context | String | 27 |
| `buildComposeDslContextBridgeDefinition` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` |  | String | 3 |
| `buildComposeDslRuntimeWrappedScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | script: String | String | 3 |
| `loadPakoJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEmbeddedLibraryLoader.kt` | context: Context | String | 5 |
| `loadCryptoJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEmbeddedLibraryLoader.kt` | context: Context | String | 7 |
| `loadJimpJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEmbeddedLibraryLoader.kt` | context: Context | String | 9 |
| `loadEmbeddedLibrary` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEmbeddedLibraryLoader.kt` | context: Context, assetPath: String | String | 11 |
| `JsEngine.canScheduleQuickJsWork` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Boolean | 130 |
| `JsEngine.withTemporaryToolPkgTextResourceResolver` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | resolver: (String, String) -> String?, block: () -> T | T | 134 |
| `JsEngine.resolveTemporaryToolPkgTextResource` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageNameOrSubpackageId: String, resourcePath: String | String? | 141 |
| `JsEngine.hasTemporaryToolPkgTextResourceResolver` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Boolean | 158 |
| `JsEngine.getJavaBridgeBaseClassLoader` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | ClassLoader | 162 |
| `JsEngine.getJavaBridgeClassLoader` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | ClassLoader | 168 |
| `JsEngine.runOnQuickJsThreadBlocking` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | allowWhenDestroyed: Boolean?, block: () -> T | T | 172 |
| `JsEngine.ensureQuickJs` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Unit | 186 |
| `JsEngine.quickJsMemorySample` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | resetPeak: Boolean | ToolPkgRuntimeMonitor.MemorySample? | 210 |
| `JsEngine.getQuickJsMemoryUsage` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | QuickJsMemoryUsage? | 224 |
| `JsEngine.getQuickJsRuntimeTid` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Long? | 229 |
| `JsEngine.interruptQuickJs` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | reason: String | Unit | 234 |
| `JsEngine.disposeQuickJsForReinit` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | reason: String | Unit | 243 |
| `JsEngine.evaluateQuickJsBlocking` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | script: String, fileName: String? | T? | 266 |
| `JsEngine.launchQuickJsEvaluation` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | script: String, fileName: String?, onError: ((Exception) -> Unit)?? | Unit | 280 |
| `JsEngine.launchQuickJsFunctionCall` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | functionName: String, argsJson: String, callSite: String?, onError: ((Exception) -> Unit)?? | Unit | 308 |
| `JsEngine.nextExecutionCallId` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String | 338 |
| `JsEngine.createExecutionSession` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, script: String, functionName: String, params: Map<String, Any?>, envOverrides: Map<String, String>, onIntermediateResult: ((Any?) -> Unit)?, di… | ExecutionSession | 342 |
| `JsEngine.resolveToolPkgApiVersionForExecution` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | params: Map<String, Any?>, explicitApiVersion: String? | ToolPkgApiVersion? | 374 |
| `JsEngine.buildToolPkgApiContextJson` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | apiVersion: ToolPkgApiVersion? | Any | 396 |
| … | | | | 还有 437 个，见分册 | | |

### 聊天 Hook 注册表（19 类事件）

`com.ai.assistance.operit.core.chat.hooks…` · 70 个函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `buildActivePromptHookMetadata` | — | `com.ai.assistance.operit.core.chat.hooks` | `ActivePromptHookMetadata.kt` | context: Context, chatId: String??, roleCardId: String?? | Map<String, Any?> | 14 |
| `resolveHookActivePrompt` | — | `com.ai.assistance.operit.core.chat.hooks` | `ActivePromptHookMetadata.kt` | context: Context, chatId: String?, roleCardId: String? | ActivePrompt | 24 |
| `resolveBoundChatForHookMetadata` | — | `com.ai.assistance.operit.core.chat.hooks` | `ActivePromptHookMetadata.kt` | context: Context, chatId: String? | ChatHistory? | 56 |
| `activePromptToMetadata` | — | `com.ai.assistance.operit.core.chat.hooks` | `ActivePromptHookMetadata.kt` | context: Context, activePrompt: ActivePrompt | Map<String, Any?> | 67 |
| `ChatRuntimeHook.onEvent` | `ChatRuntimeHook` | `com.ai.assistance.operit.core.chat.hooks` | `ChatRuntimeHookRegistry.kt` | event: ChatRuntimeHookEvent, context: ChatRuntimeHookContext | Unit | 34 |
| `ChatRuntimeHookRegistry.registerHook` | `ChatRuntimeHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `ChatRuntimeHookRegistry.kt` | hook: ChatRuntimeHook | Unit | 45 |
| `ChatRuntimeHookRegistry.unregisterHook` | `ChatRuntimeHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `ChatRuntimeHookRegistry.kt` | hookId: String | Unit | 51 |
| `ChatRuntimeHookRegistry.dispatch` | `ChatRuntimeHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `ChatRuntimeHookRegistry.kt` | event: ChatRuntimeHookEvent, context: ChatRuntimeHookContext | Unit | 55 |
| `ChatRuntimeHookRegistry.dispatchAsync` | `ChatRuntimeHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `ChatRuntimeHookRegistry.kt` | event: ChatRuntimeHookEvent, context: ChatRuntimeHookContext | Unit | 72 |
| `PromptInputHook.onEvent` | `PromptInputHook` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | context: PromptHookContext | PromptHookMutation? | 41 |
| `PromptHistoryHook.onEvent` | `PromptHistoryHook` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | context: PromptHookContext | PromptHookMutation? | 47 |
| `PromptEstimateHistoryHook.onEvent` | `PromptEstimateHistoryHook` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | context: PromptHookContext | PromptHookMutation? | 53 |
| `SystemPromptComposeHook.onEvent` | `SystemPromptComposeHook` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | context: PromptHookContext | PromptHookMutation? | 59 |
| `ToolPromptComposeHook.onEvent` | `ToolPromptComposeHook` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | context: PromptHookContext | PromptHookMutation? | 65 |
| `PromptFinalizeHook.onEvent` | `PromptFinalizeHook` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | context: PromptHookContext | PromptHookMutation? | 71 |
| `PromptEstimateFinalizeHook.onEvent` | `PromptEstimateFinalizeHook` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | context: PromptHookContext | PromptHookMutation? | 77 |
| `PromptHookRegistry.registerPromptInputHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hook: PromptInputHook | Unit | 90 |
| `PromptHookRegistry.unregisterPromptInputHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hookId: String | Unit | 96 |
| `PromptHookRegistry.registerPromptHistoryHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hook: PromptHistoryHook | Unit | 101 |
| `PromptHookRegistry.unregisterPromptHistoryHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hookId: String | Unit | 107 |
| `PromptHookRegistry.registerPromptEstimateHistoryHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hook: PromptEstimateHistoryHook | Unit | 112 |
| `PromptHookRegistry.unregisterPromptEstimateHistoryHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hookId: String | Unit | 118 |
| `PromptHookRegistry.registerSystemPromptComposeHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hook: SystemPromptComposeHook | Unit | 123 |
| `PromptHookRegistry.unregisterSystemPromptComposeHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hookId: String | Unit | 129 |
| `PromptHookRegistry.registerToolPromptComposeHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hook: ToolPromptComposeHook | Unit | 134 |
| `PromptHookRegistry.unregisterToolPromptComposeHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hookId: String | Unit | 140 |
| `PromptHookRegistry.registerPromptFinalizeHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hook: PromptFinalizeHook | Unit | 145 |
| `PromptHookRegistry.unregisterPromptFinalizeHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hookId: String | Unit | 151 |
| `PromptHookRegistry.registerPromptEstimateFinalizeHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hook: PromptEstimateFinalizeHook | Unit | 156 |
| `PromptHookRegistry.unregisterPromptEstimateFinalizeHook` | `PromptHookRegistry` | `com.ai.assistance.operit.core.chat.hooks` | `PromptHookRegistry.kt` | hookId: String | Unit | 162 |
| … | | | | 还有 40 个，见分册 | | |

### 聊天服务与 LLM Provider

`com.ai.assistance.operit.api.chat…` · 1312 个函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `FileBindingServiceTest.setUp` | `FileBindingServiceTest` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 20 |
| `FileBindingServiceTest.invokeApplyLineBasedPatch` | `FileBindingServiceTest` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` | originalContent: String, patch: String | Pair<Boolean, String> | 34 |
| `FileBindingServiceTest.testComplexMixedOperations_ShouldApplyCorrectly` | `FileBindingServiceTest` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 40 |
| `FileBindingServiceTest.main` | `FileBindingServiceTest` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 42 |
| `FileBindingServiceTest.main` | `FileBindingServiceTest` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 75 |
| `testBoundaryOperations_AtStartAndEndOfFile` | — | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 96 |
| `testInsertOnlyOperations_InMiddleOfFile` | — | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 138 |
| `testFuzzyReplace_ShouldNotEarlyStopOnWrongWindowSize` | — | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 168 |
| `testHighComplexityMixedOperations_ShouldSucceed` | — | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 221 |
| `main` | — | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 223 |
| `main` | — | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 271 |
| `testExtremeComplexity_TortureTest` | — | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Unit | 301 |
| `Calculator.add` | `Calculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` | a: Int, b: Int | Int | 313 |
| `Calculator.subtract` | `Calculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` | a: Int, b: Int | Int | 323 |
| `Calculator.multiply` | `Calculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` | a: Int, b: Int | Int | 330 |
| `Calculator.getLastResult` | `Calculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Double | 334 |
| `AdvancedCalculator.subtract` | `AdvancedCalculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` | a: Int, b: Int | Int | 353 |
| `AdvancedCalculator.power` | `AdvancedCalculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` | base: Double, exp: Double | Double | 363 |
| `AdvancedCalculator.AdvancedCalculator.add` | `AdvancedCalculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` | a: Int, b: Int | Int | 381 |
| `AdvancedCalculator.AdvancedCalculator.subtract` | `AdvancedCalculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` | a: Int, b: Int | Int | 392 |
| `AdvancedCalculator.AdvancedCalculator.getLastResult` | `AdvancedCalculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` |  | Double | 399 |
| `AdvancedCalculator.AdvancedCalculator.power` | `AdvancedCalculator` | `com.ai.assistance.operit.api.chat.enhance` | `FileBindingServiceTest.kt` | base: Double, exp: Double | Double | 402 |
| `ToolExecutionManagerTest.extractToolInvocations_shouldKeepAllToolBlocksInSameChunk` | `ToolExecutionManagerTest` | `com.ai.assistance.operit.api.chat.enhance` | `ToolExecutionManagerTest.kt` |  | Unit | 13 |
| `MediaLinkBuilderAndroidTest.imageLink_usesImageTypeMarkup` | `MediaLinkBuilderAndroidTest` | `com.ai.assistance.operit.api.chat.llmprovider` | `MediaLinkBuilderAndroidTest.kt` |  | Unit | 15 |
| `MediaLinkBuilderAndroidTest.audioLink_usesAudioTypeMarkup` | `MediaLinkBuilderAndroidTest` | `com.ai.assistance.operit.api.chat.llmprovider` | `MediaLinkBuilderAndroidTest.kt` |  | Unit | 19 |
| `MediaLinkBuilderAndroidTest.videoLink_usesVideoTypeMarkup` | `MediaLinkBuilderAndroidTest` | `com.ai.assistance.operit.api.chat.llmprovider` | `MediaLinkBuilderAndroidTest.kt` |  | Unit | 23 |
| `MediaLinkBuilderAndroidTest.imageLink_embedsRequestedId` | `MediaLinkBuilderAndroidTest` | `com.ai.assistance.operit.api.chat.llmprovider` | `MediaLinkBuilderAndroidTest.kt` |  | Unit | 27 |
| `MediaLinkBuilderAndroidTest.audioLink_embedsRequestedId` | `MediaLinkBuilderAndroidTest` | `com.ai.assistance.operit.api.chat.llmprovider` | `MediaLinkBuilderAndroidTest.kt` |  | Unit | 31 |
| `MediaLinkBuilderAndroidTest.videoLink_embedsRequestedId` | `MediaLinkBuilderAndroidTest` | `com.ai.assistance.operit.api.chat.llmprovider` | `MediaLinkBuilderAndroidTest.kt` |  | Unit | 35 |
| `MediaLinkBuilderAndroidTest.imageLink_supportsNumericId` | `MediaLinkBuilderAndroidTest` | `com.ai.assistance.operit.api.chat.llmprovider` | `MediaLinkBuilderAndroidTest.kt` |  | Unit | 39 |
| … | | | | 还有 1282 个，见分册 | | |

### App 内插件（菜单项 / 聊天视图 Hook）

`com.ai.assistance.operit.plugins…` · 157 个函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `OperitPlugin.register` | `OperitPlugin` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` |  | Unit | 12 |
| `PluginRegistry.register` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` | plugin: OperitPlugin | Unit | 23 |
| `PluginRegistry.initializeBuiltins` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` |  | Unit | 29 |
| `PluginRegistry.installAll` | `PluginRegistry` | `com.ai.assistance.operit.plugins` | `PluginRegistry.kt` |  | Unit | 40 |
| `ChatMessageMenuItemPlugin.createMenuItems` | `ChatMessageMenuItemPlugin` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | params: ChatMessageMenuItemParams | List<ChatMessageMenuItemDefinition> | 41 |
| `ChatMessageMenuItemRegistry.register` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | plugin: ChatMessageMenuItemPlugin | Unit | 50 |
| `ChatMessageMenuItemRegistry.unregister` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | pluginId: String | Unit | 57 |
| `ChatMessageMenuItemRegistry.notifyChanged` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` |  | Unit | 64 |
| `ChatMessageMenuItemRegistry.createMenuItems` | `ChatMessageMenuItemRegistry` | `com.ai.assistance.operit.plugins.chatmessage` | `ChatMessageMenuItemRegistry.kt` | params: ChatMessageMenuItemParams | List<ChatMessageMenuItemDefinition> | 68 |
| `ChatViewHookPlugin.onEvent` | `ChatViewHookPlugin` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | event: ChatViewEvent, params: ChatViewHookParams | Unit | 30 |
| `ChatViewHookPluginRegistry.register` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | plugin: ChatViewHookPlugin | Unit | 44 |
| `ChatViewHookPluginRegistry.unregister` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | pluginId: String | Unit | 50 |
| `ChatViewHookPluginRegistry.dispatch` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | event: ChatViewEvent, params: ChatViewHookParams | Unit | 54 |
| `ChatViewHookPluginRegistry.dispatchAsync` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | event: ChatViewEvent, params: ChatViewHookParams | Unit | 72 |
| `ChatViewHookPluginRegistry.getReplayableOpenViewParams` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` |  | List<ChatViewHookParams> | 81 |
| `ChatViewHookPluginRegistry.recordReplayableState` | `ChatViewHookPluginRegistry` | `com.ai.assistance.operit.plugins.chatview` | `ChatViewHookPluginRegistry.kt` | event: ChatViewEvent, params: ChatViewHookParams | Unit | 87 |
| `AppLifecycleHookPlugin.onEvent` | `AppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | event: AppLifecycleEvent, params: AppLifecycleHookParams | Unit | 51 |
| `AppLifecycleHookPluginRegistry.register` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | plugin: AppLifecycleHookPlugin | Unit | 66 |
| `AppLifecycleHookPluginRegistry.unregister` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | pluginId: String | Unit | 72 |
| `AppLifecycleHookPluginRegistry.dispatch` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | event: AppLifecycleEvent, params: AppLifecycleHookParams | Unit | 76 |
| `AppLifecycleHookPluginRegistry.dispatchAsync` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | event: AppLifecycleEvent, params: AppLifecycleHookParams | Unit | 90 |
| `AppLifecycleHookPluginRegistry.getReplayableApplicationEvents` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` |  | List<AppLifecycleReplayEvent> | 99 |
| `AppLifecycleHookPluginRegistry.recordReplayableState` | `AppLifecycleHookPluginRegistry` | `com.ai.assistance.operit.plugins.lifecycle` | `AppLifecycleHookPluginRegistry.kt` | event: AppLifecycleEvent, params: AppLifecycleHookParams | Unit | 122 |
| `ToolPkgAppLifecycleHookPlugin.onEvent` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | event: AppLifecycleEvent, params: AppLifecycleHookParams | Unit | 30 |
| `ToolPkgAppLifecycleHookPlugin.syncToolPkgRegistrations` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | activeContainers: List<ToolPkgContainerRuntime> | Map<String, List<ToolPkgAppLifecycleHookRegistrat… | 41 |
| `ToolPkgAppLifecycleHookPlugin.replayHooks` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | replayEvents: List<AppLifecycleReplayEvent>, hooksToReplayByEvent: Map<String, List<ToolPkgAppLi… | Unit | 78 |
| `ToolPkgAppLifecycleHookPlugin.dispatchHooks` | `ToolPkgAppLifecycleHookPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | hooks: List<ToolPkgAppLifecycleHookR…, params: AppLifecycleHookParams | Unit | 99 |
| `ToolboxPlugin.register` | `ToolboxPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` |  | Unit | 145 |
| `ToolboxPlugin.syncAndReplayToolPkgLifecycleHooks` | `ToolboxPlugin` | `com.ai.assistance.operit.plugins.toolbox` | `ToolboxPlugin.kt` | activeContainers: List<ToolPkgContainerRuntime> | Unit | 156 |
| `ToolPkgAiProviderRegistry.register` | `ToolPkgAiProviderRegistry` | `com.ai.assistance.operit.plugins.toolpkg` | `ToolPkgAiProviderRegistry.kt` |  | Unit | 18 |
| … | | | | 还有 127 个，见分册 | | |

### 内建工具实现

`com.ai.assistance.operit.core.tools.defaultTool…` · 1281 个函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `PathValidator.validateAndroidPath` | `PathValidator` | `com.ai.assistance.operit.core.tools.defaultTool` | `PathValidator.kt` | path: String, toolName: String, paramName: String? | ToolResult? | 8 |
| `PathValidator.validateLinuxPath` | `PathValidator` | `com.ai.assistance.operit.core.tools.defaultTool` | `PathValidator.kt` | path: String, toolName: String, paramName: String? | ToolResult? | 33 |
| `ToolGetter.getFileSystemTools` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardFileSystemTools | 20 |
| `ToolGetter.getShellToolExecutor` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardShellToolExecutor | 36 |
| `ToolGetter.getUITools` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardUITools | 45 |
| `ToolGetter.getSystemOperationTools` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardSystemOperationTools | 61 |
| `ToolGetter.getDeviceInfoToolExecutor` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardDeviceInfoToolExecutor | 77 |
| `ToolGetter.getHttpTools` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardHttpTools | 93 |
| `ToolGetter.getWebVisitTool` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardWebVisitTool | 102 |
| `ToolGetter.getBrowserSessionTools` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardBrowserSessionTools | 111 |
| `ToolGetter.getIntentToolExecutor` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardIntentToolExecutor | 120 |
| `ToolGetter.getSendBroadcastToolExecutor` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardSendBroadcastToolExecutor | 129 |
| `ToolGetter.getTerminalCommandExecutor` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardTerminalCommandExecutor | 138 |
| `ToolGetter.getMusicPlaybackTools` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardMusicPlaybackTools | 147 |
| `ToolGetter.getMemoryQueryToolExecutor` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | MemoryQueryToolExecutor | 156 |
| `ToolGetter.getFFmpegToolExecutor` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardFFmpegToolExecutor | 165 |
| `ToolGetter.getFFmpegInfoToolExecutor` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` |  | StandardFFmpegInfoToolExecutor | 174 |
| `ToolGetter.getFFmpegConvertToolExecutor` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardFFmpegConvertToolExecutor | 183 |
| `ToolGetter.getCalculator` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` |  | Unit | 191 |
| `ToolGetter.getWorkflowTools` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardWorkflowTools | 198 |
| `ToolGetter.getChatManagerTool` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardChatManagerTool | 207 |
| `ToolGetter.getSoftwareSettingsModifyTools` | `ToolGetter` | `com.ai.assistance.operit.core.tools.defaultTool` | `ToolGetter.kt` | context: Context | StandardSoftwareSettingsModifyTools | 216 |
| `AccessibilityUITools.isAccessibilityServiceEnabled` | `AccessibilityUITools` | `com.ai.assistance.operit.core.tools.defaultTool.accessbility` | `AccessibilityUITools.kt` |  | Boolean | 38 |
| `AccessibilityUITools.withAccessibilityCheck` | `AccessibilityUITools` | `com.ai.assistance.operit.core.tools.defaultTool.accessbility` | `AccessibilityUITools.kt` | tool: AITool, block: suspend () -> T | T | 45 |
| `AccessibilityUITools.getUIHierarchyWithRetry` | `AccessibilityUITools` | `com.ai.assistance.operit.core.tools.defaultTool.accessbility` | `AccessibilityUITools.kt` |  | String | 56 |
| `AccessibilityUITools.getPageInfo` | `AccessibilityUITools` | `com.ai.assistance.operit.core.tools.defaultTool.accessbility` | `AccessibilityUITools.kt` | tool: AITool | ToolResult | 78 |
| `AccessibilityUITools.extractFocusInfoFromAccessibility` | `AccessibilityUITools` | `com.ai.assistance.operit.core.tools.defaultTool.accessbility` | `AccessibilityUITools.kt` |  | FocusInfo | 132 |
| `AccessibilityUITools.simplifyLayout` | `AccessibilityUITools` | `com.ai.assistance.operit.core.tools.defaultTool.accessbility` | `AccessibilityUITools.kt` | xml: String | SimplifiedUINode | 166 |
| `AccessibilityUITools.createNode` | `AccessibilityUITools` | `com.ai.assistance.operit.core.tools.defaultTool.accessbility` | `AccessibilityUITools.kt` | parser: XmlPullParser | UINode | 208 |
| `AccessibilityUITools.clickElement` | `AccessibilityUITools` | `com.ai.assistance.operit.core.tools.defaultTool.accessbility` | `AccessibilityUITools.kt` | tool: AITool | ToolResult | 228 |
| … | | | | 还有 1251 个，见分册 | | |

### 数据模型

`com.ai.assistance.operit.data.model…` · 63 个函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ApiKeyFormatValidator.normalize` | `ApiKeyFormatValidator` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidator.kt` | value: String | String | 4 |
| `ApiKeyFormatValidator.isValid` | `ApiKeyFormatValidator` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidator.kt` | value: String | Boolean | 6 |
| `ApiKeyFormatValidator.hasUsableKey` | `ApiKeyFormatValidator` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidator.kt` | config: ModelConfigData | Boolean | 13 |
| `BillingMode.fromString` | `BillingMode` | `com.ai.assistance.operit.data.model` | `BillingMode.kt` | value: String? | BillingMode | 26 |
| `CharacterCardToolAccessConfig.normalized` | `CharacterCardToolAccessConfig` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` |  | CharacterCardToolAccessConfig | 15 |
| `CharacterCardToolAccessConfig.hasExternalSelections` | `CharacterCardToolAccessConfig` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` |  | Boolean | 24 |
| `CharacterCardToolAccessConfig.normalizeEntries` | `CharacterCardToolAccessConfig` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | values: List<String> | List<String> | 30 |
| `CharacterCardChatModelBindingMode.normalize` | `CharacterCardChatModelBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | mode: String? | String | 69 |
| `CharacterCardMemoryProfileBindingMode.normalize` | `CharacterCardMemoryProfileBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | mode: String? | String | 78 |
| `ChatEntity.toChatHistory` | `ChatEntity` | `com.ai.assistance.operit.data.model` | `ChatEntity.kt` | messages: List<ChatMessage> | ChatHistory | 30 |
| `ChatEntity.fromChatHistory` | `ChatEntity` | `com.ai.assistance.operit.data.model` | `ChatEntity.kt` | chatHistory: ChatHistory | ChatEntity | 62 |
| `ChatMessage.writeToParcel` | `ChatMessage` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | parcel: Parcel, flags: Int | Unit | 60 |
| `ChatMessage.describeContents` | `ChatMessage` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` |  | Int | 81 |
| `ChatMessage.CREATOR.readDisplayModeFromParcel` | `CREATOR` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | parcel: Parcel | ChatMessageDisplayMode | 86 |
| `ChatMessage.CREATOR.readBooleanFromParcel` | `CREATOR` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | parcel: Parcel | Boolean | 97 |
| `ChatMessage.CREATOR.createFromParcel` | `CREATOR` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | parcel: Parcel | ChatMessage | 101 |
| `ChatMessage.CREATOR.newArray` | `CREATOR` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | size: Int | Array<ChatMessage?> | 105 |
| `ChatMessageTimestampAllocator.next` | `ChatMessageTimestampAllocator` | `com.ai.assistance.operit.data.model` | `ChatMessageTimestampAllocator.kt` | baseTimestamp: Long? | Long | 14 |
| `ChatMessageTimestampAllocator.observe` | `ChatMessageTimestampAllocator` | `com.ai.assistance.operit.data.model` | `ChatMessageTimestampAllocator.kt` | timestamp: Long | Unit | 24 |
| `CloudEmbeddingConfig.normalized` | `CloudEmbeddingConfig` | `com.ai.assistance.operit.data.model` | `CloudEmbeddingConfig.kt` |  | CloudEmbeddingConfig | 9 |
| `CloudEmbeddingConfig.isReady` | `CloudEmbeddingConfig` | `com.ai.assistance.operit.data.model` | `CloudEmbeddingConfig.kt` |  | Boolean | 17 |
| `Embedding.equals` | `Embedding` | `com.ai.assistance.operit.data.model` | `Embedding.kt` | other: Any? | Boolean | 11 |
| `Embedding.hashCode` | `Embedding` | `com.ai.assistance.operit.data.model` | `Embedding.kt` |  | Int | 18 |
| `EmbeddingConverter.convertToEntityProperty` | `EmbeddingConverter` | `com.ai.assistance.operit.data.model` | `EmbeddingConverter.kt` | databaseValue: ByteArray? | Embedding? | 10 |
| `EmbeddingConverter.convertToDatabaseValue` | `EmbeddingConverter` | `com.ai.assistance.operit.data.model` | `EmbeddingConverter.kt` | entityProperty: Embedding? | ByteArray? | 21 |
| `MemoryAutoSaveCandidate.isSelectedUserMessageSource` | `MemoryAutoSaveCandidate` | `com.ai.assistance.operit.data.model` | `MemoryAutoSaveCandidate.kt` | sourceType: String | Boolean | 28 |
| `DateSerializer.serialize` | `DateSerializer` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | encoder: Encoder, value: Date | Unit | 20 |
| `DateSerializer.deserialize` | `DateSerializer` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | decoder: Decoder | Date | 24 |
| `MemorySearchConfig.normalized` | `MemorySearchConfig` | `com.ai.assistance.operit.data.model` | `MemorySearchConfig.kt` |  | MemorySearchConfig | 16 |
| `MessageEntity.toChatMessage` | `MessageEntity` | `com.ai.assistance.operit.data.model` | `MessageEntity.kt` |  | ChatMessage | 43 |
| … | | | | 还有 33 个，见分册 | | |

### 系统提示词与工具目录

`com.ai.assistance.operit.core.config…` · 72 个函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `FunctionalPrompts.summaryPrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | String | 114 |
| `FunctionalPrompts.summarySectionTitles` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | List<String> | 120 |
| `FunctionalPrompts.summaryPromptTemplate` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | SummaryPromptTemplate | 133 |
| `FunctionalPrompts.legacyPromptSections` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | List<SummarySectionConfig> | 162 |
| `FunctionalPrompts.resolveSummarySections` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | overrides: List<SummarySectionOverride>, useEnglish: Boolean | List<SummarySectionConfig> | 166 |
| `FunctionalPrompts.buildSummarySectionOverrides` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | sections: List<SummarySectionConfig>, useEnglish: Boolean | List<SummarySectionOverride> | 183 |
| `FunctionalPrompts.buildSummarySystemPrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | previousSummary: String?, useEnglish: Boolean, summaryConfig: ConversationSummaryConfig? | String | 209 |
| `FunctionalPrompts.applySummarySectionOverrides` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | overrides: List<SummarySectionOverride>, useEnglish: Boolean | String | 224 |
| `FunctionalPrompts.summarySectionHeader` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | title: String, useEnglish: Boolean | String | 262 |
| `FunctionalPrompts.appendPreviousSummary` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | prompt: String, previousSummary: String?, useEnglish: Boolean | String | 266 |
| `FunctionalPrompts.fileBindingMergePrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | String | 323 |
| `FunctionalPrompts.memoryAutoCategorizeUserMessage` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | String | 327 |
| `FunctionalPrompts.knowledgeGraphExistingMemoriesPrefix` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | String | 331 |
| `FunctionalPrompts.knowledgeGraphNoExistingMemoriesMessage` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | String | 339 |
| `FunctionalPrompts.knowledgeGraphExistingFoldersPrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | existingFolders: List<String>, useEnglish: Boolean | String | 347 |
| `FunctionalPrompts.knowledgeGraphDuplicateTitleInstruction` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | title: String, count: Int, useEnglish: Boolean | String | 364 |
| `FunctionalPrompts.knowledgeGraphSimilarTitleInstruction` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | titles: List<String>, useEnglish: Boolean | String | 372 |
| `FunctionalPrompts.knowledgeGraphDuplicateHeader` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | String | 381 |
| `FunctionalPrompts.summaryUserMessage` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | String | 396 |
| `FunctionalPrompts.conversationTitleSystemPrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | String | 401 |
| `FunctionalPrompts.conversationTitleUserPrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | userText: String, attachmentFileNames: List<String>, useEnglish: Boolean | String | 423 |
| `FunctionalPrompts.waifuEmotionRule` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | emotionListText: String | String | 462 |
| `FunctionalPrompts.waifuNoCustomEmojiRule` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` |  | String | 466 |
| `FunctionalPrompts.waifuCustomPromptRule` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | customPrompt: String | String | 470 |
| `FunctionalPrompts.waifuSelfieRule` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | waifuSelfiePrompt: String | String | 474 |
| `FunctionalPrompts.avatarMoodRulesText` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | customMoodDefinitions: List<AvatarCustomMoodDefiniti…?, useEnglish: Boolean? | String | 483 |
| `FunctionalPrompts.translationSystemPrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` |  | String | 563 |
| `FunctionalPrompts.translationUserPrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | targetLanguage: String, text: String | String | 567 |
| `FunctionalPrompts.packageDescriptionSystemPrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | useEnglish: Boolean | String | 577 |
| `FunctionalPrompts.packageDescriptionUserPrompt` | `FunctionalPrompts` | `com.ai.assistance.operit.core.config` | `FunctionalPrompts.kt` | pluginName: String, toolList: String, useEnglish: Boolean | String | 585 |
| … | | | | 还有 42 个，见分册 | | |

### 暴露给 JS 的宿主方法（`@JavascriptInterface`）

共 106 个。这些是插件在 QuickJS 里能直接碰到的原生边界。

| 方法 | 类名 | 包名 | 文件名 | 参数 | 返回 |
| --- | --- | --- | --- | --- | --- |
| `__javaReleaseInstanceInternal` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String | String |
| `callTool` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | toolType: String, toolName: String, paramsJson: String | String |
| `callToolAsync` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String, toolType: String, toolName: String, paramsJson: String | Unit |
| `callToolAsyncStreaming` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String, intermediateCallbackId: String, toolType: String, toolName: String, paramsJson: String | Unit |
| `crypto` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | algorithm: String, operation: String, argsJson: String | String |
| `image_processing` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String, operation: String, argsJson: String | Unit |
| `javaCallInstance` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String, methodName: String, argsJson: String | String |
| `javaCallInstanceSuspend` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String, methodName: String, argsJson: String, callbackId: String | Unit |
| `javaCallInstanceSuspendForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, instanceHandle: String, methodName: String, argsJson: String, callbackId: String | Unit |
| `javaCallStatic` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String, methodName: String, argsJson: String | String |
| `javaCallStaticSuspend` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String, methodName: String, argsJson: String, callbackId: String | Unit |
| `javaCallStaticSuspendForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, className: String, methodName: String, argsJson: String, callbackId: String | Unit |
| `javaClassExists` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String | Boolean |
| `javaGetApplicationContext` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |
| `javaGetCurrentActivity` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |
| `javaGetInstanceField` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String, fieldName: String | String |
| `javaGetStaticField` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String, fieldName: String | String |
| `javaHasInstanceMethod` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String, methodName: String | String |
| `javaListLoadedCodePaths` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |
| `javaLoadDex` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | path: String, optionsJson: String | String |
| `javaLoadJar` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | path: String, optionsJson: String | String |
| `javaNewInstance` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String, argsJson: String | String |
| `javaPollPendingJsCallback` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |
| `javaResolvePendingJsCallback` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | requestId: String, responseJson: String | Unit |
| `javaSetInstanceField` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String, fieldName: String, valueJson: String | String |
| `javaSetStaticField` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String, fieldName: String, valueJson: String | String |
| `javaSleepMillis` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | durationText: String? | Unit |
| `logDebug` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | message: String, data: String | Unit |
| `logError` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | message: String | Unit |
| `logErrorForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, message: String | Unit |
| `logInfo` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | message: String | Unit |
| `logInfoForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, message: String | Unit |
| `logWarnForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, message: String | Unit |
| `registerImageFromBase64` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | base64: String, mimeType: String | String |
| `registerImageFromPath` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | path: String | String |
| `reportError` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | errorType: String, errorMessage: String, errorLine: Int, errorStack: String | Unit |
| `reportErrorForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, errorType: String, errorMessage: String, errorLine: Int, errorStack: String | Unit |
| `sendCallIntermediateResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, result: String | Unit |
| `setCallError` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, error: String | Unit |
| `setCallResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, result: String | Unit |
| `capturePoster` | `AnnualReportBridge` | `com.ai.assistance.operit.ui.features.annualreport` | `AnnualReportWebSupport.kt` | action: String, left: Double, top: Double, width: Double, height: Double, ratio: Double | Unit |
| `close` | `AnnualReportBridge` | `com.ai.assistance.operit.ui.features.annualreport` | `AnnualReportWebSupport.kt` |  | Unit |
| `haptic` | `AnnualReportBridge` | `com.ai.assistance.operit.ui.features.annualreport` | `AnnualReportWebSupport.kt` | kind: String | Unit |
| `recordClick` | `BrowserAsyncBridge` | `com.ai.assistance.operit.core.tools.defaultTool.websession.browser` | `BrowserPageExecutionSupport.kt` | payload: String? | Unit |
| `reject` | `BrowserAsyncBridge` | `com.ai.assistance.operit.core.tools.defaultTool.websession.browser` | `BrowserPageExecutionSupport.kt` | callId: String?, error: String? | Unit |
| `resolve` | `BrowserAsyncBridge` | `com.ai.assistance.operit.core.tools.defaultTool.websession.browser` | `BrowserPageExecutionSupport.kt` | callId: String?, payload: String? | Unit |
| `hideActions` | `BrowserTextSelectionBridge` | `com.ai.assistance.operit.core.tools.defaultTool.websession.browser` | `BrowserPageExecutionSupport.kt` |  | Unit |
| `performHapticFeedback` | `BrowserTextSelectionBridge` | `com.ai.assistance.operit.core.tools.defaultTool.websession.browser` | `BrowserPageExecutionSupport.kt` |  | Unit |
| `showActions` | `BrowserTextSelectionBridge` | `com.ai.assistance.operit.core.tools.defaultTool.websession.browser` | `BrowserPageExecutionSupport.kt` | anchorX: Double, anchorY: Double | Unit |
| `downloadBase64` | `BrowserWebDownloadBridge` | `com.ai.assistance.operit.core.tools.defaultTool.websession.browser` | `BrowserPageExecutionSupport.kt` | base64Data: String?, fileName: String?, mimeType: String? | Unit |
| `log` | `BrowserWebDownloadBridge` | `com.ai.assistance.operit.core.tools.defaultTool.websession.browser` | `BrowserPageExecutionSupport.kt` | message: String? | Unit |
| `invoke` | `ComposeDslWebViewPageBridge` | `com.ai.assistance.operit.ui.common.composedsl` | `ToolPkgComposeDslWebView.kt` | interfaceName: String, methodName: String, argsJson: String | String |
| `listInterfaces` | `ComposeDslWebViewPageBridge` | `com.ai.assistance.operit.ui.common.composedsl` | `ToolPkgComposeDslWebView.kt` |  | String |
| `onError` | `DeepseekJsInterface` | `com.ai.assistance.operit.ui.features.token.webview` | `DeepseekJsInterface.kt` | error: String | Unit |
| `onKeyCreated` | `DeepseekJsInterface` | `com.ai.assistance.operit.ui.features.token.webview` | `DeepseekJsInterface.kt` | key: String | Unit |
| `onKeyDeleted` | `DeepseekJsInterface` | `com.ai.assistance.operit.ui.features.token.webview` | `DeepseekJsInterface.kt` | success: Boolean | Unit |
| `onKeysReceived` | `DeepseekJsInterface` | `com.ai.assistance.operit.ui.features.token.webview` | `DeepseekJsInterface.kt` | json: String | Unit |
| `callToolPkgWasm` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageNameOrSubpackageId: String, moduleId: String, exportName: String, argsJson: String | String |
| `captureToolPkgMarketOrigin` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `composeOpenFilePickerSuspend` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | payloadJson: String, callbackId: String | Unit |
| `composeWebViewControllerCommand` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | payloadJson: String | String |
| `composeWebViewControllerCommandSuspend` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | payloadJson: String, callbackId: String | Unit |
| `decompress` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | data: String, algorithm: String | String |
| `getEnvForCall` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String, key: String | String? |
| `getPluginConfigDir` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | pluginId: String | String |
| `importPackage` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String | String |
| `invokeToolPkgFloatingWindowCommand` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String, owner: String, operation: String, argsJson: String | Unit |
| `invokeToolPkgIpcAsync` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String, packageTarget: String, callerContextKey: String, targetContextKey: String, targetRuntime: String, channel: String, payl… | Unit |
| `isPackageImported` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String | Boolean |
| `listHostRoutes` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |
| `listImportedPackagesJson` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |
| `listRoutes` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |
| `measureComposeText` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | payloadJson: String | String |
| `navigateToRoute` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | routeId: String, argsJson: String | Unit |
| `readToolPkgResource` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageNameOrSubpackageId: String, resourceKey: String, outputFileName: String, internal: String | String |
| `readToolPkgTextResource` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageNameOrSubpackageId: String, resourcePath: String | String |
| `registerToolPkgAiProvider` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgAppLifecycleHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgChatInputHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgChatMessageHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgChatMessageMenuItem` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgChatRuntimeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgChatViewHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgDesktopWidget` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgInputMenuTogglePlugin` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgMessageProcessingPlugin` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgNavigationEntry` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgPromptEstimateFinalizeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgPromptEstimateHistoryHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgPromptFinalizeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgPromptHistoryHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgPromptInputHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgSummaryGenerateHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgSystemPromptComposeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgToolboxUiModule` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgToolLifecycleHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgToolPromptComposeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgUiRoute` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `registerToolPkgXmlRenderPlugin` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |
| `removePackage` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String | String |
| `resolveToolName` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String, subpackageId: String, toolName: String, preferImported: String | String |
| `setEnv` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | key: String, value: String? | Unit |
| `setEnvs` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | valuesJson: String | Unit |
| `usePackage` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String | String |
| `downloadBlob` | `BlobDownloadInterface` | `com.ai.assistance.operit.ui.features.chat.webview` | `WebViewHandler.kt` | base64Data: String, fileName: String, mimeType: String | Unit |
| `log` | `BlobDownloadInterface` | `com.ai.assistance.operit.ui.features.chat.webview` | `WebViewHandler.kt` | message: String | Unit |

---

## 分册（全量）

| 模块 | 声明数 | 文件 |
| --- | --- | --- |
| operit.ui.（其余零散） | 3490 | [operit.ui.__other.md](Operit-API-INDEX/operit.ui.__other.md) |
| operit.core.（其余零散） | 2001 | [operit.core.__other.md](Operit-API-INDEX/operit.core.__other.md) |
| operit.data.（其余零散） | 1307 | [operit.data.__other.md](Operit-API-INDEX/operit.data.__other.md) |
| operit.util.(root) | 1200 | [operit.util._root_.md](Operit-API-INDEX/operit.util._root_.md) |
| operit.api.chat.llmprovider | 1099 | [operit.api.chat.llmprovider.md](Operit-API-INDEX/operit.api.chat.llmprovider.md) |
| operit.core.tools.defaultTool.standard | 680 | [operit.core.tools.defaultTool.standard.md](Operit-API-INDEX/operit.core.tools.defaultTool.standard.md) |
| operit.data.preferences | 668 | [operit.data.preferences.md](Operit-API-INDEX/operit.data.preferences.md) |
| operit.core.tools.javascript | 617 | [operit.core.tools.javascript.md](Operit-API-INDEX/operit.core.tools.javascript.md) |
| operit.core.tools.packTool | 566 | [operit.core.tools.packTool.md](Operit-API-INDEX/operit.core.tools.packTool.md) |
| operit.services | 547 | [operit.services.md](Operit-API-INDEX/operit.services.md) |
| operit.ui.features.chat.components.lazy | 501 | [operit.ui.features.chat.components.lazy.md](Operit-API-INDEX/operit.ui.features.chat.components.lazy.md) |
| operit.core.tools.defaultTool.websession.browser | 446 | [operit.core.tools.defaultTool.websession.browser.md](Operit-API-INDEX/operit.core.tools.defaultTool.websession.browser.md) |
| operit.api.（其余零散） | 430 | [operit.api.__other.md](Operit-API-INDEX/operit.api.__other.md) |
| operit.core.tools | 421 | [operit.core.tools.md](Operit-API-INDEX/operit.core.tools.md) |
| com.ai.assistance | 418 | [com.ai.assistance.md](Operit-API-INDEX/com.ai.assistance.md) |
| operit.ui.common.composedsl | 417 | [operit.ui.common.composedsl.md](Operit-API-INDEX/operit.ui.common.composedsl.md) |
| operit.data.repository | 414 | [operit.data.repository.md](Operit-API-INDEX/operit.data.repository.md) |
| operit.integrations | 400 | [operit.integrations.md](Operit-API-INDEX/operit.integrations.md) |
| operit.util.stream | 369 | [operit.util.stream.md](Operit-API-INDEX/operit.util.stream.md) |
| operit.ui.common.markdown | 326 | [operit.ui.common.markdown.md](Operit-API-INDEX/operit.ui.common.markdown.md) |
| operit.plugins | 321 | [operit.plugins.md](Operit-API-INDEX/operit.plugins.md) |
| operit.data.model | 290 | [operit.data.model.md](Operit-API-INDEX/operit.data.model.md) |
| operit.api.voice | 277 | [operit.api.voice.md](Operit-API-INDEX/operit.api.voice.md) |
| operit.util.（其余零散） | 260 | [operit.util.__other.md](Operit-API-INDEX/operit.util.__other.md) |
| operit.data.stats | 248 | [operit.data.stats.md](Operit-API-INDEX/operit.data.stats.md) |
| operit.ui.features.chat.webview.workspace.editor | 248 | [operit.ui.features.chat.webview.workspace.editor.md](Operit-API-INDEX/operit.ui.features.chat.webview.workspace.editor.md) |
| operit.ui.features.packages.market | 244 | [operit.ui.features.packages.market.md](Operit-API-INDEX/operit.ui.features.packages.market.md) |
| operit.api.chat.enhance | 229 | [operit.api.chat.enhance.md](Operit-API-INDEX/operit.api.chat.enhance.md) |
| operit.ui.features.chat.viewmodel | 226 | [operit.ui.features.chat.viewmodel.md](Operit-API-INDEX/operit.ui.features.chat.viewmodel.md) |
| operit.ui.features.settings.screens | 221 | [operit.ui.features.settings.screens.md](Operit-API-INDEX/operit.ui.features.settings.screens.md) |
| com.k2fsa.sherpa | 94 | [com.k2fsa.sherpa.md](Operit-API-INDEX/com.k2fsa.sherpa.md) |
| operit.provider | 93 | [operit.provider.md](Operit-API-INDEX/operit.provider.md) |
| operit.widget | 64 | [operit.widget.md](Operit-API-INDEX/operit.widget.md) |
| com.dragonbones | 56 | [com.dragonbones.md](Operit-API-INDEX/com.dragonbones.md) |
| com.java.myapplication | 18 | [com.java.myapplication.md](Operit-API-INDEX/com.java.myapplication.md) |
| operit.terminal | 8 | [operit.terminal.md](Operit-API-INDEX/operit.terminal.md) |
| org.jetbrains.kotlinx | 5 | [org.jetbrains.kotlinx.md](Operit-API-INDEX/org.jetbrains.kotlinx.md) |
| androidx.compose.foundation | 4 | [androidx.compose.foundation.md](Operit-API-INDEX/androidx.compose.foundation.md) |
| (default) | 1 | [_default_.md](Operit-API-INDEX/_default_.md) |
| com.example.operit_flutter_project | 1 | [com.example.operit_flutter_project.md](Operit-API-INDEX/com.example.operit_flutter_project.md) |

---

## 关键词倒排

按主题词定位入口。完整倒排（3000 词）在 JSON 的 `keywordIndex` 里。

- **toolpkg** (71) — `TOOLPKG_EXECUTION_ENTRY_FUNCTION` `PackageManager.loadAvailablePackages` `PackageManager.addPackageFileFromExternalStorage` `PackageManager.enablePackage` `PackageManager.disablePackage` `TOOLPKG_RUNTIME_COMPOSE_DSL` `TOOLPKG_EVENT_APPLICATION_ON_CREATE` `TOOLPKG_EVENT_APPLICATION_ON_FOREGROUND` `TOOLPKG_EVENT_APPLICATION_ON_BACKGROUND` `TOOLPKG_EVENT_APPLICATION_ON_LOW_MEMORY` `TOOLPKG_EVENT_APPLICATION_ON_TRIM_MEMORY` `TOOLPKG_EVENT_APPLICATION_ON_TERMINATE` …
- **plugin** (236) — `MessageProcessingPlugin` `MessageProcessingPluginRegistry` `PerformanceMonitorManager.KEY_PLUGIN_PREFIX` `McpRestartLogPluginResultItem` `withToolPkgPluginTag` `JsToolCallInterface.getPluginConfigDir` `JsToolCallInterface.registerToolPkgMessageProcessingPlugin` `JsToolCallInterface.registerToolPkgXmlRenderPlugin` `JsToolCallInterface.registerToolPkgInputMenuTogglePlugin` `JsNativeInterfaceDelegates.getPluginConfigDir` `JsToolPkgExecutionContext.hasActivePluginIdForLogs` `JsToolPkgExecutionContext.withPluginTag` …
- **hook** (232) — `ChatRuntimeHolder.RuntimeHookObservation` `EnhancedAIService.applyPromptFinalizeHooks` `EnhancedAIService.bypassPromptHooks` `EnhancedAIService.serializePromptHookModelParameters` `EnhancedAIService.serializePromptHookToolPrompts` `EnhancedAIService.deserializePromptHookToolPrompts` `EnhancedAIService.deserializePromptHookToolParameters` `ConversationService.serializeSummaryHookModelParameters` `ToolPkgJsAiProviderService.ProviderHookValue` `ToolPkgJsAiProviderService.ProviderHookValue.NullValue` `ToolPkgJsAiProviderService.ProviderHookValue.BooleanValue` `ToolPkgJsAiProviderService.ProviderHookValue.NumberValue` …
- **prompt** (345) — `EnhancedAIService.applyPromptFinalizeHooks` `EnhancedAIService.bypassPromptHooks` `EnhancedAIService.buildPromptFinalizeMetadata` `EnhancedAIService.applyFinalizedCurrentUserTurn` `EnhancedAIService.generateSummaryFromPromptTurns` `EnhancedAIService.prepareConversationHistory` `EnhancedAIService.serializePromptHookModelParameters` `EnhancedAIService.serializePromptHookToolPrompts` `EnhancedAIService.deserializePromptHookToolPrompts` `EnhancedAIService.deserializePromptHookToolParameters` `EnhancedAIService.applyToolPromptComposeHooksToAvailableTools` `EnhancedAIService.getAvailableToolsForFunction` …
- **compose** (216) — `EnhancedAIService.applyToolPromptComposeHooksToAvailableTools` `rememberWebPAvatarController` `SystemPromptComposeHook` `ToolPromptComposeHook` `PromptHookRegistry.systemPromptComposeHooks` `PromptHookRegistry.toolPromptComposeHooks` `PromptHookRegistry.registerSystemPromptComposeHook` `PromptHookRegistry.unregisterSystemPromptComposeHook` `PromptHookRegistry.registerToolPromptComposeHook` `PromptHookRegistry.unregisterToolPromptComposeHook` `PromptHookRegistry.dispatchSystemPromptComposeHooks` `PromptHookRegistry.dispatchToolPromptComposeHooks` …
- **javascript** (12) — `evaluateJavascriptAsync` `ComposeDslWebViewHostRegistry.javascriptInterfaceActionIds` `ComposeDslWebViewHostRegistry.findJavascriptInterfaceActionId` `ComposeDslWebViewHostRegistry.registerJavascriptInterface` `ComposeDslWebViewHostRegistry.unregisterJavascriptInterface` `ComposeDslWebViewHostRegistry.listJavascriptInterfaces` `evaluateJavascriptBlocking` `extractComposeDslJavascriptInterfaceMethods` `buildComposeDslWebViewJavascriptInterfaceRuntimeScript` `refreshComposeDslJavascriptInterfaces` `ComposeDslWebViewPageBridge.executeJavascriptInterfaceInvocation` `installJavascriptInterfacesIfPossible`
- **tool** (1480) — `EnhancedAIService` `EnhancedAIService.SendMessageCallbacks.onToolInvocation` `EnhancedAIService.SendMessageCallbacks.onSubtaskToolResult` `EnhancedAIService.enhanceToolDetection` `EnhancedAIService.normalizeToolXml` `EnhancedAIService.isToolXmlBlock` `EnhancedAIService.TruncatedToolRoundRecovery` `EnhancedAIService.detectAndRepairTruncatedToolRound` `EnhancedAIService.buildTruncatedToolRepairSuffix` `EnhancedAIService.handleToolInvocation` `EnhancedAIService.awaitToolJob` `EnhancedAIService.processToolResults` …
- **registration** (75) — `ActionHandler.buildScreenshotRegistrationOptions` `UserscriptWebRequestRegistration` `executeToolPkgMainRegistrationFunction` `JsToolCallInterface.requireToolPkgRegistrationOperationAllowed` `ToolPkgMainRegistrationCapture` `RegistrationBucket` `JsToolPkgRegistrationSession` `JsToolPkgRegistrationSession.finish` `JsToolPkgRegistrationSession.normalizeRegistrationSpec` `buildToolPkgRegistrationBridgeScript` `PackageManager` `PackageManager.withToolPkgRegistrationEngine` …
- **chat** (744) — `AIForegroundService.observeChatRuntimeStats` `ChatRuntimeHolder` `ChatRuntimeHolder.getCore` `ChatRuntimeHolder.syncMainChatSelectionToFloating` `ChatRuntimeHolder.registerChatSelectionSync` `ChatRuntimeHolder.syncChatSelection` `ChatRuntimeHolder.getInstance` `ChatRuntimeSlot` `EnhancedAIService.getChatInstance` `EnhancedAIService.releaseChatInstance` `ConversationService.processChatMessageWithTools` `MultiServiceManager.getDefaultService` …
- **message** (572) — `EnhancedAIService.SendMessageCallbacks` `EnhancedAIService.SendMessageOptions` `EnhancedAIService.MessageExecutionContext` `EnhancedAIService.sendMessage` `ConversationMarkupManager.formatToolResultForMessage` `ConversationMarkupManager.buildToolResultMessage` `ConversationMarkupManager.createMultipleToolsWarning` `ConversationMarkupManager.createToolNotAvailableError` `ConversationService.processChatMessageWithTools` `SubtaskExecutionState` `SubtaskExecutionState.stopMessage` `buildToolNotAvailableErrorMessage` …
- **stream** (250) — `asCharStream` `EnhancedAIService.sendMessage` `EnhancedAIService.processStreamCompletion` `ToolExecutionBatch` `SubtaskExecutionState.recordToolResult` `ToolExecutionManager.PackageContextInjection.ensureOwnLine` `AIService.sendMessage` `sendMessage` `DeepseekProvider.sendMessage` `KimiProvider.sendMessage` `LlamaProvider.sendMessage` `MNNProvider.sendMessage` …
- **provider** (280) — `AIForegroundService.ensureWakeSpeechProvider` `AIForegroundService.releaseWakeSpeechProvider` `EnhancedAIService.getProviderAndModelForFunction` `EnhancedAIService.getDisplayProviderAndModelForFunction` `ApiKeyProvider` `SingleApiKeyProvider` `MultiApiKeyProvider` `ClaudeProvider` `CodexAccessTokenProvider` `CodexProvider` `DeepseekProvider` `DeepseekResponsesProvider` …
- **model** (442) — `EnhancedAIService.getModelConfigForFunction` `EnhancedAIService.ModelExecutionSnapshot` `EnhancedAIService.getModelExecutionSnapshot` `EnhancedAIService.releaseModelExecutionSnapshot` `EnhancedAIService.getProviderAndModelForFunction` `EnhancedAIService.getDisplayProviderAndModelForFunction` `EnhancedAIService.getModelParametersForFunction` `EnhancedAIService.callFunctionModel` `EnhancedAIService.serializePromptHookModelParameters` `ConversationMarkupManager.splitImageLinksForModel` `ConversationService.serializeSummaryHookModelParameters` `ConversationService.normalizeConversationHistoryForModel` …
- **token** (334) — `EnhancedAIService.TurnTokenSnapshot` `EnhancedAIService.getCurrentInputTokenCountForFunction` `EnhancedAIService.getCurrentOutputTokenCountForFunction` `EnhancedAIService.resetTokenCountersForFunction` `EnhancedAIService.resetTokenCounters` `EnhancedAIService.SendMessageCallbacks.onTokenLimitExceeded` `EnhancedAIService.getCurrentInputTokenCount` `EnhancedAIService.getCurrentOutputTokenCount` `EnhancedAIService.getCurrentCachedInputTokenCount` `EnhancedAIService.captureCurrentTurnTokenSnapshot` `EnhancedAIService.setCurrentTurnTokenCounts` `MultiServiceManager.resetAllTokenCounters` …
- **file** (542) — `testBoundaryOperations_AtStartAndEndOfFile` `testInsertOnlyOperations_InMiddleOfFile` `EnhancedAIService.applyFileBinding` `EnhancedAIService.applyFileBindingOperations` `ConversationService.extractApplyFileRequestContent` `FileBindingService` `FileBindingService.processFileBinding` `FileBindingService.processFileBindingOperations` `getOutputImagesDir` `fileExtensionForImageMime` `LlamaProvider.getModelsDir` `LlamaProvider.getModelFile` …
- **zip** (47) — `VitsVoiceProvider.extractZipPackage` `copyZipEntry` `addWebContentToZip` `DebuggerFileSystemTools.zipFiles` `DebuggerFileSystemTools.unzipFiles` `StandardFileSystemTools.zipFiles` `StandardFileSystemTools.addDirectoryToZip` `StandardFileSystemTools.addDirectoryContentsToZip` `StandardFileSystemTools.unzipFiles` `PackageManager.zipToolPkgResourceDirectory` `ToolPkgArchiveParser.buildZipEntryIndex` `ToolPkgArchiveParser.normalizeZipEntryPath` …
- **permission** (167) — `AIForegroundService.hasRecordAudioPermission` `SubtaskExecutionState.tryStartTool` `checkToolPermission` `AIToolHandler.getToolPermissionSystem` `AIToolHandler.notifyToolPermissionChecked` `AIToolHandler.refreshPermissionState` `AIToolHookDecision.AIToolHook.onToolCallIntercept` `AIToolHookDecision.AIToolHook.onToolPermissionChecked` `executeProxyTargetWithPermissionCheck` `StandardSystemOperationTools.needsBluetoothConnectPermission` `StandardSystemOperationTools.hasBluetoothConnectPermission` `StandardSystemOperationTools.hasBluetoothScanPermission` …
- **sandbox** (14) — `SandboxScriptExecutionResultData` `SandboxPackageResultItem` `SandboxPackagesResultData` `SandboxPackageUpdateResultData` `StandardSoftwareSettingsModifyTools.listSandboxPackages` `StandardSoftwareSettingsModifyTools.setSandboxPackageEnabled` `StandardSoftwareSettingsModifyTools.executeSandboxScriptDirect` `StandardSoftwareSettingsModifyTools.executeSandboxScriptDirectResult` `StandardSoftwareSettingsModifyTools.buildFailure` `JsExecutionTraceRecorder.buildPayload` `JsExecutionTraceRecorder.buildResultData` `SANDBOX_PACKAGE_DEV_INSTALL_SCRIPT_URL` …
- **registry** (38) — `RateLimiterRegistry` `RequestConcurrencyRegistry` `ThinkingQualityMappingRegistry` `ChatRuntimeHookRegistry` `PromptHookRegistry` `SummaryHookRegistry` `MessageProcessingPluginRegistry` `PhoneAgentJobRegistry` `ShowerBinderRegistry` `ExtractedWebData.ServiceLifecycleOwner` `buildPageRegistry` `BrowserPageRegistry` …
- **manifest** (39) — `VitsVoiceProvider.manifestPath` `modifyManifestBytes` `PackageManager.getToolPkgApiVersion` `ToolPkgManifestRequirement` `ToolPkgManifest` `ToolPkgManifestSubpackage` `ToolPkgManifestResource` `ToolPkgManifestWasmModule` `ToolPkgManifestPreview` `ToolPkgArchiveParser.resolveManifestRelativeZipEntryPath` `ToolPkgArchiveParser.resolveManifestRelativeResourcePath` `ToolPkgArchiveParser.readToolPkgManifestPreview` …
- **package** (260) — `tryGetClientPackageName` `EnhancedAIService.generatePackageDescription` `generatePackageDescription` `ToolExecutionManager.PACKAGE_PROXY_TOOL_NAME` `ToolExecutionManager.PACKAGE_CALLER_NAME_PARAM` `ToolExecutionManager.PACKAGE_CHAT_ID_PARAM` `ToolExecutionManager.PACKAGE_CALLER_CARD_ID_PARAM` `ToolExecutionManager.PackageContextInjection` `ToolExecutionManager.PackageContextInjection.Ready` `ToolExecutionManager.isJsPackageTool` `ToolExecutionManager.addPackageContextParamIfMissing` `ToolExecutionManager.injectPackageCallContext` …
- **install** (88) — `DebuggerSystemOperationTools.installApp` `BluetoothSessionManager.BleReadCallback.install` `BluetoothSessionManager.BleWriteCallback.install` `StandardSystemOperationTools.stageApkForInstallIfNeeded` `StandardSystemOperationTools.installApp` `onInstallUserscriptFromUrl` `onConfirmUserscriptInstall` `onCancelUserscriptInstall` `isUserscriptInstallUri` `WebSessionBrowserHost.Callbacks.onInstallUserscriptFromUrl` `WebSessionBrowserHost.Callbacks.onConfirmUserscriptInstall` `WebSessionBrowserHost.Callbacks.onCancelUserscriptInstall` …
- **ui** (120) — `FunctionalPrompts.UI_CONTROLLER_PROMPT` `FunctionalPrompts.UI_CONTROLLER_PROMPT_CN` `FunctionalPrompts.uiControllerPrompt` `FunctionalPrompts.UI_AUTOMATION_AGENT_PROMPT` `FunctionalPrompts.UI_AUTOMATION_AGENT_PROMPT_EN` `FunctionalPrompts.uiAutomationAgentPrompt` `FunctionalPrompts.buildUiAutomationAgentPrompt` `executeUiToolWithVisibility` `uiTools` `SimplifiedUINode` `UIPageResultData` `UIActionResultData` …
- **screen** (241) — `distinctScreenTexts` `ActivityLifecycleManager.keepScreenOnPreferenceRequestCount` `ActivityLifecycleManager.keepScreenOnForcedRequestCount` `ActivityLifecycleManager.checkAndApplyKeepScreenOn` `ActivityLifecycleManager.forceKeepScreenOn` `ActivityLifecycleManager.applyKeepScreenOnRequest` `AvatarController.lookAt` `TerminalSessionScreenResultData` `PhoneAgent` `PhoneAgent.ensureRequiredVirtualScreenOrError` `PhoneAgent.prewarmMainScreenShowerIfPossible` `PhoneAgent.prewarmMainScreenLaunchIfNeeded` …
- **navigation** (65) — `traceBrowserNavigation` `updateNavigationState` `syncNavigationStateUi` `refreshNavigationStateFromWebView` `refreshNavigationStateAsync` `handleNavigationOverrideOnMain` `JsToolCallInterface.registerToolPkgNavigationEntry` `JsToolPkgRegistrationSession.appendNavigationEntry` `PackageManager.ToolPkgNavigationEntry` `PackageManager.ToolPkgNavigationActionHook` `PackageManager.getToolPkgNavigationEntries` `PackageManager.runToolPkgNavigationEntryAction` …
- **sidebar** (8) — `TOOLPKG_NAV_SURFACE_MAIN_SIDEBAR_PLUGINS` `SidebarPermissionStatus` `resolveSidebarPermissionStatus` `NewSidebarTopContent` `SidebarInfoCard` `SidebarQuickActionCard` `SidebarQuickActionBadge` `ScreenRouteRegistry.mainSidebarEntries`
- **widget** (35) — `JsToolCallInterface.registerToolPkgDesktopWidget` `JsToolPkgRegistrationSession.appendDesktopWidget` `PackageManager.ToolPkgDesktopWidget` `PackageManager.getToolPkgDesktopWidgets` `PackageManagerToolPkgFacade.buildToolPkgDesktopWidgets` `PackageManagerToolPkgFacade.getToolPkgDesktopWidgets` `TOOLPKG_REGISTRATION_DESKTOP_WIDGET` `ToolPkgMainRegistrationScriptParser.parseRegisteredDesktopWidgets` `ToolPkgDesktopWidgetRuntime` `ToolPkgRegisteredDesktopWidget` `launchFloatingWindowInMode` `ToolPkgDesktopGlanceWidget` …
- **overlay** (49) — `AIForegroundService.updateKeepAliveOverlayVisibility` `AIForegroundService.showKeepAliveOverlayIfPossible` `AIForegroundService.hideKeepAliveOverlay` `StandardWebVisitTool.syncWebOverlayToIndicator` `StandardWebVisitTool.updateOverlayWindowLayout` `ensureOverlayPermission` `ensureOverlayOnMain` `destroyOverlayOnMain` `WebSessionBrowserHost.showTextSelectionActionsOverlay` `WebSessionBrowserHost.hideTextSelectionActionsOverlay` `WebSessionBrowserHost.createOverlayLayoutParams` `WebSessionOverlayLifecycleOwner` …
- **floating** (74) — `AIForegroundService.setWakeListeningSuspendedForFloatingFullscreen` `AIForegroundService.updateWakeListeningSuspendedForFloatingFullscreen` `ChatRuntimeHolder.syncMainChatSelectionToFloating` `JsToolCallInterface.invokeToolPkgFloatingWindowCommand` `sendToolPkgFloatingWindowResult` `floatingWindowsApi` `ToolPkgFloatingWindowController` `ToolPkgFloatingWindowOptions` `ToolPkgFloatingWindowOptions.mergedOver` `ToolPkgFloatingWindowOptions.toJson` `ToolPkgFloatingWindowOptions.fromJson` `ToolPkgFloatingWindowSurface` …

---

## 边界说明

- 只索引 Kotlin。Compose UI 的 `@Composable` 函数也在内（它们在 `ui` 分册），但那是 App 自己的界面，插件改不到。
- 属性只收**文件顶层**与 `object` 直接成员；函数体内的局部 `val` 不是 API，已排除。
- 生成期之外没有被手改过任何一行源码。
