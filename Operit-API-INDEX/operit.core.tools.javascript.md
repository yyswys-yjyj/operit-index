# operit.core.tools.javascript

> 函数 467 · 类型 47 · 顶层常量 103 · 共 617 条
> 每日定时任务自动生成。

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `JavaSuspendLifecycleProbe` | `JavaSuspendLifecycleProbe` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeSuspendLifecycleTest.kt` | class JavaSuspendLifecycleProbe |  | 18 |
| `JsBootstrapModule` | `JsBootstrapModule` | `com.ai.assistance.operit.core.tools.javascript` | `JsLibraries.kt` | class JsBootstrapModule(val fileName: String, val source: String, val globals: List<String>) |  | 5 |
| `JsEngine` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | class JsEngine(private val context: Context) | JavaScript 引擎 - 通过 QuickJS 执行 JavaScript 脚本并提供与 Android 原生代码的交互机制 | 55 |
| `JsEngine.ExecutionDispatch` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | class ExecutionDispatch(val session: ExecutionSession, val timeoutSec: Long?, val timeoutMillis: Long?) |  | 108 |
| `JsEngine.ExecutionSession` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | class ExecutionSession(val callId: String, val future: CompletableFuture<Any?>, val intermediateResultCallback: ((Any?) -> Unit)?, val dispatchIntermediateOnMain: Boolean, val envOv… |  | 93 |
| `JsEngine.PendingJsBridgeCallback` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | class PendingJsBridgeCallback(val requestId: String, val jsObjectId: String, val methodName: String, val argsJson: String, val future: CompletableFuture<String>) |  | 114 |
| `JsExecutionFailure` | `JsExecutionFailure` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionResultProtocol.kt` | class JsExecutionFailure(val message: String, val dataText: String) |  | 6 |
| `JsExecutionListener` | `JsExecutionListener` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | interface JsExecutionListener |  | 13 |
| `JsExecutionTraceRecorder` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | class JsExecutionTraceRecorder(private val scriptPath: String, private val functionName: String, private val paramsJson: String, private val envFilePath: String?) : JsExecutionListener |  | 23 |
| `JsExternalJavaCodeLoader` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | class JsExternalJavaCodeLoader(private val context: Context) |  | 59 |
| `JsExternalJavaCodeLoader.LoadedArtifact` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | class LoadedArtifact(val sourceType: SourceType, val sourcePath: String, val nativeLibraryDir: String?, val childFirstPrefixes: List<String>, val classLoader: ClassLoader) |  | 70 |
| `JsExternalJavaCodeLoader.LoadOptions` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | class LoadOptions(val nativeLibraryDir: String?, val childFirstPrefixes: List<String>) |  | 65 |
| `JsExternalJavaCodeLoader.SourceType` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | class SourceType(val wireName: String) |  | 60 |
| `JsInterfaceCallbackInvoker` | `JsInterfaceCallbackInvoker` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | typealias JsInterfaceCallbackInvoker |  | 27 |
| `JsJavaBridgeDelegates` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | object JsJavaBridgeDelegates |  | 30 |
| `JsJavaBridgeDelegates.BridgeResponse` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | class BridgeResponse(val success: Boolean, val dataRaw: Any?, val error: String?) |  | 76 |
| `JsJavaBridgeDelegates.ConstructedJavaObject` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | class ConstructedJavaObject(val value: Any) |  | 67 |
| `JsJavaBridgeDelegates.ConstructorMatch` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | class ConstructorMatch(val constructor: Constructor<*>, val args: Array<Any?>, val score: Int) |  | 61 |
| `JsJavaBridgeDelegates.ConvertedArg` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | class ConvertedArg(val value: Any?, val score: Int) |  | 50 |
| `JsJavaBridgeDelegates.JsInterfaceBinding` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | class JsInterfaceBinding(val jsObjectId: String, val interfaceNames: List<String>) |  | 71 |
| `JsJavaBridgeDelegates.JsInterfaceProxyReference` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | class JsInterfaceProxyReference(referent: Any, val callbackInvoker: JsInterfaceCallbackInvoker, val jsObjectIds: Set<String>) : PhantomReference<Any> |  | 82 |
| `JsJavaBridgeDelegates.MethodMatch` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | class MethodMatch(val method: Method, val args: Array<Any?>, val score: Int) |  | 55 |
| `JsJavaBridgeSuspendLifecycleTest` | `JsJavaBridgeSuspendLifecycleTest` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeSuspendLifecycleTest.kt` | class JsJavaBridgeSuspendLifecycleTest |  | 34 |
| `JsNativeInterfaceDelegates` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | object JsNativeInterfaceDelegates |  | 52 |
| `JsNativeInterfaceDelegates.ParsedToolCall` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | class ParsedToolCall(val params: Map<String, String>, val fullToolName: String, val aiTool: AITool) |  | 60 |
| `JsNativeInterfaceDelegates.ParsedWasmArgs` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | class ParsedWasmArgs(val types: IntArray, val bits: LongArray) |  | 71 |
| `JsNativeInterfaceDelegates.SerializedToolResultData` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | class SerializedToolResultData(val data: JsonElement, val dataType: String?) |  | 66 |
| `JsRuntimeToolCallTest` | `JsRuntimeToolCallTest` | `com.ai.assistance.operit.core.tools.javascript` | `JsRuntimeToolCallTest.kt` | class JsRuntimeToolCallTest |  | 7 |
| `JsTimeoutConfig` | `JsTimeoutConfig` | `com.ai.assistance.operit.core.tools.javascript` | `JsTimeoutConfig.kt` | object JsTimeoutConfig |  | 3 |
| `JsToolCallInterface` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | class JsToolCallInterface | JavaScript 接口，提供 Native 调用方法 | 1579 |
| `JsToolManager` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | class JsToolManager(private val context: Context, private val packageManager: PackageManager) |  | 18 |
| `JsToolManager.ToolParameterConversionException` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | class ToolParameterConversionException(message: String) : IllegalArgumentException |  | 23 |
| `JsToolPkgExecutionContext` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | class JsToolPkgExecutionContext |  | 3 |
| `JsToolPkgExecutionContext.LogSnapshot` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | class LogSnapshot(val pluginTag: String, val functionName: String, val codeSnippet: String) |  | 5 |
| `JsToolPkgRegistrationSession` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | class JsToolPkgRegistrationSession |  | 65 |
| `JsToolPkgRegistrationTest` | `JsToolPkgRegistrationTest` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistrationTest.kt` | class JsToolPkgRegistrationTest |  | 9 |
| `OperitQuickJsEngine` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | class OperitQuickJsEngine : Closeable |  | 16 |
| `PrefixIsolatedDexClassLoader` | `PrefixIsolatedDexClassLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | class PrefixIsolatedDexClassLoader(dexPath: String, optimizedDirectory: String, librarySearchPath: String?, parent: ClassLoader, childFirstPrefixes: List<String>) : DexClassLoader |  | 16 |
| `QuickJsMemoryUsage` | `QuickJsMemoryUsage` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | class QuickJsMemoryUsage(val mallocSizeBytes: Long, val memoryUsedBytes: Long, val peakMallocSizeBytes: Long) |  | 42 |
| `QuickJsNativeBridge` | `QuickJsNativeBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | object QuickJsNativeBridge |  | 7 |
| `QuickJsNativeHostDispatcher` | `QuickJsNativeHostDispatcher` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeHostDispatcher.kt` | class QuickJsNativeHostDispatcher(private val dispatchTimer: (Int) -> Unit, private val forwardCall: (String, String?) -> String?) : QuickJsNativeRuntime.HostBridge, Closeable |  | 11 |
| `QuickJsNativeRuntime` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | class QuickJsNativeRuntime(private val handle: Long, private val hostBridge: HostBridge) : Closeable |  | 48 |
| `QuickJsNativeRuntime.EvalResult` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | class EvalResult(val success: Boolean, val valueJson: String?, val errorMessage: String?, val errorStack: String?, val errorDetailsJson: String?) |  | 57 |
| `QuickJsNativeRuntime.HostBridge` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | interface HostBridge |  | 53 |
| `RegistrationBucket` | `RegistrationBucket` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | class RegistrationBucket(val nativeRegistrationName: String?) |  | 37 |
| `ScriptExecutionReceiver` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | class ScriptExecutionReceiver : BroadcastReceiver |  | 22 |
| `ToolPkgMainRegistrationCapture` | `ToolPkgMainRegistrationCapture` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | class ToolPkgMainRegistrationCapture(val toolboxUiModules: List<String>, val uiRoutes: List<String>, val navigationEntries: List<String>, val desktopWidgets: List<String>, val appLifecycleHooks: … |  | 10 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `readJavaScriptAsset` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsAssetLoader.kt` | context: Context<br>assetPath: String<br>label: String | String |  | 8 |
| `loadUINodeJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsAssetLoader.kt` | context: Context | String |  | 21 |
| `loadAndroidUtilsJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsAssetLoader.kt` | context: Context | String |  | 24 |
| `loadOkHttp3Js` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsAssetLoader.kt` | context: Context | String |  | 27 |
| `buildComposeDslContextBridgeDefinition` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` |  | String |  | 3 |
| `buildComposeDslRuntimeWrappedScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | script: String | String |  | 3 |
| `loadPakoJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEmbeddedLibraryLoader.kt` | context: Context | String |  | 5 |
| `loadCryptoJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEmbeddedLibraryLoader.kt` | context: Context | String |  | 7 |
| `loadJimpJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEmbeddedLibraryLoader.kt` | context: Context | String |  | 9 |
| `loadEmbeddedLibrary` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEmbeddedLibraryLoader.kt` | context: Context<br>assetPath: String | String |  | 11 |
| `JsEngine.canScheduleQuickJsWork` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Boolean |  | 130 |
| `JsEngine.withTemporaryToolPkgTextResourceResolver` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | resolver: (String, String) -> String?<br>block: () -> T | T |  | 134 |
| `JsEngine.resolveTemporaryToolPkgTextResource` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageNameOrSubpackageId: String<br>resourcePath: String | String? |  | 141 |
| `JsEngine.hasTemporaryToolPkgTextResourceResolver` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Boolean |  | 158 |
| `JsEngine.getJavaBridgeBaseClassLoader` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | ClassLoader |  | 162 |
| `JsEngine.getJavaBridgeClassLoader` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | ClassLoader |  | 168 |
| `JsEngine.runOnQuickJsThreadBlocking` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | allowWhenDestroyed: Boolean?<br>block: () -> T | T |  | 172 |
| `JsEngine.ensureQuickJs` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Unit |  | 186 |
| `JsEngine.quickJsMemorySample` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | resetPeak: Boolean | ToolPkgRuntimeMonitor.MemorySample? |  | 210 |
| `JsEngine.getQuickJsMemoryUsage` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | QuickJsMemoryUsage? |  | 224 |
| `JsEngine.getQuickJsRuntimeTid` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Long? | QuickJS 运行线程的内核 tid，供 /proc/self/task 采样 CPU 用；引擎未创建时为 null。 | 229 |
| `JsEngine.interruptQuickJs` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | reason: String | Unit |  | 234 |
| `JsEngine.disposeQuickJsForReinit` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | reason: String | Unit |  | 243 |
| `JsEngine.evaluateQuickJsBlocking` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | script: String<br>fileName: String? | T? |  | 266 |
| `JsEngine.launchQuickJsEvaluation` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | script: String<br>fileName: String?<br>onError: ((Exception) -> Unit)?? | Unit |  | 280 |
| `JsEngine.launchQuickJsFunctionCall` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | functionName: String<br>argsJson: String<br>callSite: String?<br>onError: ((Exception) -> Unit)?? | Unit |  | 308 |
| `JsEngine.nextExecutionCallId` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |  | 338 |
| `JsEngine.createExecutionSession` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>script: String<br>functionName: String<br>params: Map<String, Any?><br>envOverrides: Map<String, String><br>onIntermediateResult: ((Any?) -> Unit)?<br>dispatchIntermediateOnMain: Boolean<br>toolPkgApiVersion: ToolPkgApiVe… | ExecutionSession |  | 342 |
| `JsEngine.resolveToolPkgApiVersionForExecution` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | params: Map<String, Any?><br>explicitApiVersion: String? | ToolPkgApiVersion? |  | 374 |
| `JsEngine.buildToolPkgApiContextJson` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | apiVersion: ToolPkgApiVersion? | Any |  | 396 |
| `JsEngine.resolveExecutionSession` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String | ExecutionSession? |  | 405 |
| `JsEngine.removeExecutionSession` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String | ExecutionSession? |  | 409 |
| `JsEngine.clearPendingJsBridgeCallbacks` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | reason: String | Unit |  | 416 |
| `JsEngine.requestPendingJsBridgeCallbackPump` | `JsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Unit |  | 432 |
| `pollPendingJsBridgeCallbackPayload` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String? |  | 473 |
| `resolvePendingJsBridgeCallback` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | requestId: String<br>responseJson: String | Unit |  | 490 |
| `drainExecutionSessions` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | reason: String | List<ExecutionSession> |  | 501 |
| `cancelAllExecutionSessions` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | reason: String | Unit |  | 518 |
| `cancelExecutionSessionInJs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>reason: String | Unit |  | 527 |
| `withToolPkgPluginTag` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | message: String | String |  | 553 |
| `withToolPkgPluginTag` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | session: ExecutionSession?<br>message: String | String |  | 557 |
| `withToolPkgCodeContext` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | session: ExecutionSession?<br>message: String | String |  | 561 |
| `runtimeBootstrapModules` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | List<JsBootstrapModule> |  | 565 |
| `evaluateBootstrapModule` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | module: JsBootstrapModule | Unit |  | 573 |
| `summarizeJavaScriptForLog` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | source: String<br>maxLength: Int? | String |  | 591 |
| `exposeBootstrapGlobals` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | module: JsBootstrapModule | Unit |  | 613 |
| `buildBootstrapGlobalExposureScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | globalNames: List<String> | String |  | 623 |
| `invokeJavaBridgeJsObjectCallbackSync` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | jsObjectId: String<br>methodName: String<br>argsJson: String | String |  | 650 |
| `releaseJavaBridgeJsObjectSync` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | jsObjectId: String | Boolean |  | 701 |
| `splitBridgeResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | raw: String | Pair<String?, Any?> |  | 748 |
| `initJavaScriptEnvironment` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Unit | 初始化 JavaScript 环境，加上 QuickJS 兼容层、核心运行时与工具桥 | 772 |
| `executeScriptFunction` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | script: String<br>functionName: String<br>params: Map<String, Any?><br>envOverrides: Map<String, String>?<br>onIntermediateResult: ((Any?) -> Unit)??<br>dispatchIntermediateOnMain: Boolean?<br>timeoutSec: Long??<br>timeoutMillis: Long??<br… | Any? | 执行 JavaScript 脚本并调用其中的特定函数 | 801 |
| `executeScriptCode` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | script: String<br>params: Map<String, Any?>?<br>envOverrides: Map<String, String>?<br>onIntermediateResult: ((Any?) -> Unit)??<br>dispatchIntermediateOnMain: Boolean?<br>timeoutSec: Long?<br>executionListener: JsExecutionListener?? | Any? |  | 1049 |
| `buildDirectScriptExecutionSource` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | script: String | String |  | 1073 |
| `normalizeToolPkgModulePath` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | modulePath: String | String? |  | 1113 |
| `executeToolPkgMainRegistrationFunction` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | script: String<br>functionName: String<br>apiVersion: String?<br>params: Map<String, Any?>? | ToolPkgMainRegistrationCapture |  | 1121 |
| `executeComposeDslScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | script: String<br>runtimeOptions: Map<String, Any?>?<br>envOverrides: Map<String, String>? | Any? |  | 1145 |
| `executeComposeDslAction` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | actionId: String<br>payload: Any??<br>runtimeOptions: Map<String, Any?>?<br>envOverrides: Map<String, String>?<br>onIntermediateResult: ((Any?) -> Unit)?? | Any? |  | 1159 |
| `rerenderComposeDslTree` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | runtimeOptions: Map<String, Any?>?<br>envOverrides: Map<String, String>? | Any? |  | 1185 |
| `dispatchComposeDslActionAsync` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | actionId: String<br>payload: Any??<br>runtimeOptions: Map<String, Any?>?<br>envOverrides: Map<String, String>?<br>onIntermediateResult: ((Any?) -> Unit)??<br>onFinalResult: ((Any?) -> Unit)??<br>onComplete: (() -> Unit)??<br>onError: ((Str… | Boolean |  | 1198 |
| `exposeNativeInterfaceBridgeObject` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |  | 1253 |
| `callExposedBridgeObject` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String<br>methodName: String<br>argsJson: String | String |  | 1275 |
| `releaseExposedBridgeObject` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String | String |  | 1296 |
| `buildToolPkgIpcFailure` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | message: String | String |  | 1303 |
| `inferToolPkgIpcRuntimeFromContextKey` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | contextKey: String | String |  | 1309 |
| `invokeToolPkgIpc` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageTarget: String<br>callerContextKey: String<br>targetContextKey: String<br>targetRuntime: String<br>channel: String<br>payloadJson: String | String |  | 1320 |
| `cancelCurrentExecution` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | reason: String? | Unit |  | 1513 |
| `cancelExecutionsForChat` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | chatId: String<br>reason: String? | Boolean |  | 1517 |
| `resetState` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | cancellationMessage: String? | Unit | 重置引擎状态，避免多次调用时的状态干扰 | 1547 |
| `JsToolCallInterface.detachJavaBridgeLifecycle` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Unit |  | 1597 |
| `JsToolCallInterface.requireToolPkgRegistrationOperationAllowed` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | operation: String | Unit |  | 1601 |
| `JsToolCallInterface.decompress` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | data: String<br>algorithm: String | String |  | 1608 |
| `JsToolCallInterface.getEnvForCall` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>key: String | String? |  | 1618 |
| `JsToolCallInterface.setEnv` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | key: String<br>value: String? | Unit |  | 1628 |
| `JsToolCallInterface.setEnvs` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | valuesJson: String | Unit |  | 1633 |
| `JsToolCallInterface.isPackageImported` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String | Boolean |  | 1638 |
| `JsToolCallInterface.importPackage` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String | String |  | 1646 |
| `JsToolCallInterface.removePackage` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String | String |  | 1654 |
| `JsToolCallInterface.usePackage` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String | String |  | 1662 |
| `JsToolCallInterface.listImportedPackagesJson` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |  | 1670 |
| `JsToolCallInterface.resolveToolName` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageName: String<br>subpackageId: String<br>toolName: String<br>preferImported: String | String |  | 1677 |
| `JsToolCallInterface.readToolPkgResource` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageNameOrSubpackageId: String<br>resourceKey: String<br>outputFileName: String<br>internal: String | String |  | 1693 |
| `JsToolCallInterface.readToolPkgTextResource` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageNameOrSubpackageId: String<br>resourcePath: String | String |  | 1711 |
| `JsToolCallInterface.callToolPkgWasm` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | packageNameOrSubpackageId: String<br>moduleId: String<br>exportName: String<br>argsJson: String | String |  | 1733 |
| `JsToolCallInterface.getPluginConfigDir` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | pluginId: String | String |  | 1750 |
| `JsToolCallInterface.invokeToolPkgIpcAsync` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>packageTarget: String<br>callerContextKey: String<br>targetContextKey: String<br>targetRuntime: String<br>channel: String<br>payloadJson: String | Unit |  | 1758 |
| `JsToolCallInterface.invokeToolPkgFloatingWindowCommand` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>owner: String<br>operation: String<br>argsJson: String | Unit |  | 1795 |
| `JsToolCallInterface.measureComposeText` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | payloadJson: String | String |  | 1835 |
| `JsToolCallInterface.navigateToRoute` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | routeId: String<br>argsJson: String | Unit |  | 1843 |
| `JsToolCallInterface.listRoutes` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |  | 1856 |
| `JsToolCallInterface.listHostRoutes` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |  | 1861 |
| `JsToolCallInterface.composeWebViewControllerCommand` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | payloadJson: String | String |  | 1866 |
| `JsToolCallInterface.composeWebViewControllerCommandSuspend` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | payloadJson: String<br>callbackId: String | Unit |  | 1871 |
| `JsToolCallInterface.composeOpenFilePickerSuspend` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | payloadJson: String<br>callbackId: String | Unit |  | 1900 |
| `JsToolCallInterface.buildRoutesJson` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | includeOnlyNative: Boolean | String |  | 1922 |
| `JsToolCallInterface.captureToolPkgMarketOrigin` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1945 |
| `JsToolCallInterface.registerToolPkgToolboxUiModule` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1950 |
| `JsToolCallInterface.registerToolPkgUiRoute` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1955 |
| `JsToolCallInterface.registerToolPkgNavigationEntry` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1960 |
| `JsToolCallInterface.registerToolPkgDesktopWidget` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1965 |
| `JsToolCallInterface.registerToolPkgAppLifecycleHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1970 |
| `JsToolCallInterface.registerToolPkgMessageProcessingPlugin` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1975 |
| `JsToolCallInterface.registerToolPkgXmlRenderPlugin` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1980 |
| `JsToolCallInterface.registerToolPkgInputMenuTogglePlugin` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1985 |
| `JsToolCallInterface.registerToolPkgChatInputHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1990 |
| `JsToolCallInterface.registerToolPkgChatViewHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 1995 |
| `JsToolCallInterface.registerToolPkgChatMessageHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2000 |
| `JsToolCallInterface.registerToolPkgChatMessageMenuItem` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2005 |
| `JsToolCallInterface.registerToolPkgChatRuntimeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2010 |
| `JsToolCallInterface.registerToolPkgToolLifecycleHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2015 |
| `JsToolCallInterface.registerToolPkgPromptInputHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2020 |
| `JsToolCallInterface.registerToolPkgPromptHistoryHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2025 |
| `JsToolCallInterface.registerToolPkgPromptEstimateHistoryHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2030 |
| `JsToolCallInterface.registerToolPkgSystemPromptComposeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2035 |
| `JsToolCallInterface.registerToolPkgToolPromptComposeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2040 |
| `JsToolCallInterface.registerToolPkgPromptFinalizeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2045 |
| `JsToolCallInterface.registerToolPkgPromptEstimateFinalizeHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2050 |
| `JsToolCallInterface.registerToolPkgSummaryGenerateHook` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2055 |
| `JsToolCallInterface.registerToolPkgAiProvider` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | specJson: String | Unit |  | 2060 |
| `JsToolCallInterface.bridgeClassLoader` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | ClassLoader |  | 2064 |
| `JsToolCallInterface.parseJsonObjectToMap` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | raw: String | Map<String, Any?> |  | 2066 |
| `JsToolCallInterface.exposeJavaObject` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | target: Any<br>failureLabel: String | String |  | 2070 |
| `JsToolCallInterface.launchSuspendJavaBridgeCall` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>callId: String??<br>block: (coroutineContext: CoroutineContext… | Unit |  | 2092 |
| `JsToolCallInterface.isSuspendJavaBridgeOwnerActive` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | session: ExecutionSession? | Boolean |  | 2138 |
| `JsToolCallInterface.createSuspendJavaBridgeResultCallback` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>session: ExecutionSession?<br>expectedEngine: OperitQuickJsEngine? | (String) -> Unit |  | 2145 |
| `JsToolCallInterface.buildSuspendJavaBridgeCallbackScript` | `JsToolCallInterface` | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>resultJson: String | String |  | 2180 |
| `javaClassExists` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String | Boolean |  | 2223 |
| `javaLoadDex` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | path: String<br>optionsJson: String | String |  | 2231 |
| `javaLoadJar` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | path: String<br>optionsJson: String | String |  | 2240 |
| `javaListLoadedCodePaths` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |  | 2249 |
| `javaGetApplicationContext` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |  | 2254 |
| `javaGetCurrentActivity` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |  | 2262 |
| `javaNewInstance` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String<br>argsJson: String | String |  | 2275 |
| `javaCallStatic` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String<br>methodName: String<br>argsJson: String | String |  | 2286 |
| `javaCallInstance` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String<br>methodName: String<br>argsJson: String | String |  | 2298 |
| `javaCallStaticSuspend` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String<br>methodName: String<br>argsJson: String<br>callbackId: String | Unit |  | 2310 |
| `javaCallStaticSuspendForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>className: String<br>methodName: String<br>argsJson: String<br>callbackId: String | Unit |  | 2320 |
| `dispatchJavaStaticSuspend` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String?<br>className: String<br>methodName: String<br>argsJson: String<br>callbackId: String | Unit |  | 2330 |
| `javaCallInstanceSuspend` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String<br>methodName: String<br>argsJson: String<br>callbackId: String | Unit |  | 2352 |
| `javaCallInstanceSuspendForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>instanceHandle: String<br>methodName: String<br>argsJson: String<br>callbackId: String | Unit |  | 2362 |
| `dispatchJavaInstanceSuspend` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String?<br>instanceHandle: String<br>methodName: String<br>argsJson: String<br>callbackId: String | Unit |  | 2372 |
| `javaGetStaticField` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String<br>fieldName: String | String |  | 2394 |
| `javaSetStaticField` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | className: String<br>fieldName: String<br>valueJson: String | String |  | 2404 |
| `javaGetInstanceField` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String<br>fieldName: String | String |  | 2416 |
| `javaHasInstanceMethod` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String<br>methodName: String | String |  | 2425 |
| `javaSetInstanceField` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String<br>fieldName: String<br>valueJson: String | String |  | 2434 |
| `javaPollPendingJsCallback` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | String |  | 2446 |
| `javaResolvePendingJsCallback` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | requestId: String<br>responseJson: String | Unit |  | 2451 |
| `javaSleepMillis` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | durationText: String? | Unit |  | 2459 |
| `__javaReleaseInstanceInternal` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | instanceHandle: String | String |  | 2474 |
| `registerImageFromBase64` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | base64: String<br>mimeType: String | String |  | 2482 |
| `registerImageFromPath` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | path: String | String |  | 2498 |
| `image_processing` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>operation: String<br>argsJson: String | Unit |  | 2513 |
| `crypto` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | algorithm: String<br>operation: String<br>argsJson: String | String |  | 2527 |
| `sendCallIntermediateResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>result: String | Unit |  | 2536 |
| `callTool` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | toolType: String<br>toolName: String<br>paramsJson: String | String | 同步工具调用 | 2554 |
| `callToolAsync` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>toolType: String<br>toolName: String<br>paramsJson: String | Unit | 异步工具调用（新版本，使用Promise） | 2568 |
| `callToolAsyncStreaming` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>intermediateCallbackId: String<br>toolType: String<br>toolName: String<br>paramsJson: String | Unit |  | 2590 |
| `sendToolResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>result: String<br>isError: Boolean | Unit | 向JavaScript发送工具调用结果 | 2617 |
| `sendToolPkgIpcResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>result: String<br>isError: Boolean | Unit | ToolPkg.ipc uses a JSON string envelope, so its callback must receive a string. | 2641 |
| `sendToolPkgFloatingWindowResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callbackId: String<br>result: String<br>isError: Boolean | Unit | ToolPkg.ui.floatingWindows 复用 ipc 的 JSON 信封与字符串回调脚本模式。 | 2665 |
| `setCallResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>result: String | Unit |  | 2689 |
| `setCallError` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>error: String | Unit |  | 2713 |
| `completeCallFuture` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | session: ExecutionSession<br>value: String<br>failureMessage: String | Unit |  | 2751 |
| `extractErrorLogMessage` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | error: String | String |  | 2771 |
| `logInfo` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | message: String | Unit |  | 2789 |
| `logInfoForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>message: String | Unit |  | 2794 |
| `logWarnForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>message: String | Unit |  | 2802 |
| `logError` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | message: String | Unit |  | 2810 |
| `logErrorForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>message: String | Unit |  | 2815 |
| `logDebug` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | message: String<br>data: String | Unit |  | 2823 |
| `reportError` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | errorType: String<br>errorMessage: String<br>errorLine: Int<br>errorStack: String | Unit |  | 2827 |
| `reportErrorForCall` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` | callId: String<br>errorType: String<br>errorMessage: String<br>errorLine: Int<br>errorStack: String | Unit |  | 2842 |
| `destroy` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsEngine.kt` |  | Unit | 销毁引擎资源 | 2866 |
| `buildJsExecutionErrorPayload` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionResultProtocol.kt` | message: String | String |  | 11 |
| `extractJsExecutionFailure` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionResultProtocol.kt` | raw: Any? | JsExecutionFailure? |  | 17 |
| `extractJsExecutionErrorMessage` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionResultProtocol.kt` | raw: Any? | String? |  | 41 |
| `decodeJsExecutionResultValue` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionResultProtocol.kt` | raw: Any? | Any? |  | 45 |
| `buildExecutionPreludeSource` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` |  | String |  | 7 |
| `buildExecutionRuntimeBridgeScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` |  | String |  | 86 |
| `JsExecutionListener.onCallLog` | `JsExecutionListener` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | callId: String<br>level: String<br>message: String | Unit |  | 14 |
| `JsExecutionListener.onIntermediateResult` | `JsExecutionListener` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | callId: String<br>value: Any? | Unit |  | 16 |
| `JsExecutionListener.onCompleted` | `JsExecutionListener` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | callId: String<br>result: String | Unit |  | 18 |
| `JsExecutionListener.onFailed` | `JsExecutionListener` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | callId: String<br>error: String | Unit |  | 20 |
| `JsExecutionTraceRecorder.onCallLog` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | callId: String<br>level: String<br>message: String | Unit |  | 33 |
| `JsExecutionTraceRecorder.onIntermediateResult` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | callId: String<br>value: Any? | Unit |  | 47 |
| `JsExecutionTraceRecorder.onCompleted` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | callId: String<br>result: String | Unit |  | 55 |
| `JsExecutionTraceRecorder.onFailed` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | callId: String<br>error: String | Unit |  | 63 |
| `JsExecutionTraceRecorder.buildPayload` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | success: Boolean<br>result: Any?<br>error: String?? | SandboxScriptExecutionResultData |  | 71 |
| `JsExecutionTraceRecorder.buildResultData` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | success: Boolean<br>result: Any?<br>error: String??<br>executionMode: String??<br>scriptLabel: String??<br>requestedWaitMs: Long?? | SandboxScriptExecutionResultData |  | 84 |
| `JsExecutionTraceRecorder.writeTo` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | file: File<br>payload: SandboxScriptExecutionResultData | Unit |  | 111 |
| `JsExecutionTraceRecorder.parseJsonText` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | text: String | JsonElement? |  | 125 |
| `JsExecutionTraceRecorder.toJsonElement` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | value: Any? | JsonElement? |  | 137 |
| `JsExecutionTraceRecorder.summarizeValue` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | value: Any?<br>maxLength: Int?<br>depth: Int? | String |  | 158 |
| `JsExecutionTraceRecorder.summarizeJsonElement` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | element: JsonElement<br>maxLength: Int<br>depth: Int | String |  | 172 |
| `JsExecutionTraceRecorder.summarizeIterable` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | values: List<Any?><br>maxLength: Int<br>depth: Int | String |  | 193 |
| `JsExecutionTraceRecorder.summarizeMap` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | values: Map<*, *><br>maxLength: Int<br>depth: Int | String |  | 210 |
| `JsExecutionTraceRecorder.collapseWhitespace` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | text: String | String |  | 246 |
| `JsExecutionTraceRecorder.truncateText` | `JsExecutionTraceRecorder` | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionTrace.kt` | text: String<br>maxLength: Int | String |  | 250 |
| `PrefixIsolatedDexClassLoader.loadClass` | `PrefixIsolatedDexClassLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | name: String<br>resolve: Boolean | Class<*> |  | 29 |
| `PrefixIsolatedDexClassLoader.shouldLoadChildFirst` | `PrefixIsolatedDexClassLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | className: String | Boolean |  | 54 |
| `JsExternalJavaCodeLoader.LoadedArtifact.toJson` | `LoadedArtifact` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | index: Int<br>alreadyLoaded: Boolean | JSONObject |  | 77 |
| `JsExternalJavaCodeLoader.getEffectiveClassLoader` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | baseClassLoader: ClassLoader | ClassLoader |  | 99 |
| `JsExternalJavaCodeLoader.loadDex` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | path: String<br>optionsJson: String<br>baseClassLoader: ClassLoader | String |  | 104 |
| `JsExternalJavaCodeLoader.loadJar` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | path: String<br>optionsJson: String<br>baseClassLoader: ClassLoader | String |  | 109 |
| `JsExternalJavaCodeLoader.listLoadedArtifacts` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` |  | String |  | 114 |
| `JsExternalJavaCodeLoader.load` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | sourceType: SourceType<br>path: String<br>optionsJson: String<br>baseClassLoader: ClassLoader | String |  | 122 |
| `JsExternalJavaCodeLoader.validateSourceFile` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | sourceType: SourceType<br>sourceFile: File<br>canonicalPath: String | Unit |  | 196 |
| `JsExternalJavaCodeLoader.normalizeSourcePath` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | path: String | String |  | 219 |
| `JsExternalJavaCodeLoader.parseOptions` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | optionsJson: String | LoadOptions |  | 225 |
| `JsExternalJavaCodeLoader.resolveNativeLibraryDir` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | nativeLibraryDir: String? | String? |  | 255 |
| `JsExternalJavaCodeLoader.prepareLoadableSourceFile` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | sourceType: SourceType<br>sourceFile: File<br>canonicalPath: String | File |  | 263 |
| `JsExternalJavaCodeLoader.ensureJvmCompatibilitySystemProperties` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` |  | Unit |  | 300 |
| `JsExternalJavaCodeLoader.ensureSystemProperty` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | key: String<br>value: String | Unit |  | 320 |
| `JsExternalJavaCodeLoader.ensureOptimizedDir` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` |  | File |  | 330 |
| `JsExternalJavaCodeLoader.ensurePreparedSourceDir` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` |  | File |  | 334 |
| `JsExternalJavaCodeLoader.ensureManagedDirectory` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | childName: String | File |  | 338 |
| `JsExternalJavaCodeLoader.buildPreparedSourceFileName` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | sourceType: SourceType<br>canonicalPath: String | String |  | 351 |
| `JsExternalJavaCodeLoader.buildArtifactKey` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | sourceType: SourceType<br>canonicalPath: String<br>nativeLibraryDir: String?<br>childFirstPrefixes: List<String> | String |  | 359 |
| `JsExternalJavaCodeLoader.indexOf` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | artifactKey: String | Int |  | 373 |
| `JsExternalJavaCodeLoader.success` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | data: Any? | String |  | 377 |
| `JsExternalJavaCodeLoader.failure` | `JsExternalJavaCodeLoader` | `com.ai.assistance.operit.core.tools.javascript` | `JsExternalJavaCodeLoader.kt` | message: String | String |  | 384 |
| `buildInitRuntimeModules` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsInitRuntimeScriptBuilder.kt` | operitDownloadDir: String<br>operitCleanOnExitDir: String | List<JsBootstrapModule> |  | 5 |
| `buildRuntimeExposeScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsInitRuntimeScriptBuilder.kt` |  | String |  | 41 |
| `buildRuntimeConstantsScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsInitRuntimeScriptBuilder.kt` | operitDownloadDir: String<br>operitCleanOnExitDir: String | String |  | 56 |
| `buildRuntimeCallRegistryScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsInitRuntimeScriptBuilder.kt` |  | String |  | 74 |
| `buildRuntimeErrorScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsInitRuntimeScriptBuilder.kt` |  | String |  | 220 |
| `buildRuntimeToolCallScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsInitRuntimeScriptBuilder.kt` |  | String |  | 306 |
| `buildJavaClassBridgeDefinition` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` |  | String |  | 3 |
| `JsJavaBridgeDelegates.parseJsonObject` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | raw: Any? | JSONObject? |  | 98 |
| `JsJavaBridgeDelegates.parsePlainJsonObjectToMap` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | raw: String | Map<String, Any?> |  | 121 |
| `JsJavaBridgeDelegates.parsePlainJsonValueOrRawString` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | raw: String? | Any? |  | 126 |
| `JsJavaBridgeDelegates.parsePlainJsonArray` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | raw: String | List<Any?>? |  | 138 |
| `JsJavaBridgeDelegates.decodePlainJsonValue` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | raw: Any? | Any? |  | 148 |
| `JsJavaBridgeDelegates.toPlainJsonValue` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | value: Any? | Any |  | 156 |
| `JsJavaBridgeDelegates.toPlainJsonText` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | value: Any? | String |  | 164 |
| `JsJavaBridgeDelegates.containsBridgeMarkers` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | raw: Any? | Boolean |  | 177 |
| `JsJavaBridgeDelegates.registerJsInterfaceReleaseInvoker` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | callbackInvoker: JsInterfaceCallbackInvoker<br>releaseInvoker: JsInterfaceReleaseInvoker | Unit |  | 214 |
| `JsJavaBridgeDelegates.unregisterJsInterfaceReleaseInvoker` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | callbackInvoker: JsInterfaceCallbackInvoker | Unit |  | 224 |
| `JsJavaBridgeDelegates.classExists` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | className: String<br>bridgeClassLoader: ClassLoader?? | Boolean |  | 231 |
| `JsJavaBridgeDelegates.newInstance` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | className: String<br>argsJson: String<br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker??<br>bridgeClassLoader: ClassLoader?? | String |  | 240 |
| `JsJavaBridgeDelegates.callStatic` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | className: String<br>methodName: String<br>argsJson: String<br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker??<br>bridgeClassLoader: ClassLoader?? | String |  | 262 |
| `JsJavaBridgeDelegates.callInstance` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | instanceHandle: String<br>methodName: String<br>argsJson: String<br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker??<br>bridgeClassLoader: ClassLoader?? | String |  | 311 |
| `JsJavaBridgeDelegates.callStaticSuspend` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | className: String<br>methodName: String<br>argsJson: String<br>objectRegistry: ConcurrentHashMap<String, Any><br>callback: (String) -> Unit<br>coroutineContext: CoroutineContext<br>jsCallbackInvoker: JsInterfaceCallbackInvoker??<br>bridgeC… | Unit |  | 340 |
| `JsJavaBridgeDelegates.callInstanceSuspend` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | instanceHandle: String<br>methodName: String<br>argsJson: String<br>objectRegistry: ConcurrentHashMap<String, Any><br>callback: (String) -> Unit<br>coroutineContext: CoroutineContext<br>jsCallbackInvoker: JsInterfaceCallbackInvoker??<br>br… | Unit |  | 365 |
| `JsJavaBridgeDelegates.getStaticField` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | className: String<br>fieldName: String<br>objectRegistry: ConcurrentHashMap<String, Any><br>bridgeClassLoader: ClassLoader?? | String |  | 390 |
| `JsJavaBridgeDelegates.setStaticField` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | className: String<br>fieldName: String<br>valueJson: String<br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker??<br>bridgeClassLoader: ClassLoader?? | String |  | 429 |
| `JsJavaBridgeDelegates.getInstanceField` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | instanceHandle: String<br>fieldName: String<br>objectRegistry: ConcurrentHashMap<String, Any> | String |  | 515 |
| `JsJavaBridgeDelegates.hasInstanceMethod` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | instanceHandle: String<br>methodName: String<br>objectRegistry: ConcurrentHashMap<String, Any> | String |  | 540 |
| `JsJavaBridgeDelegates.setInstanceField` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | instanceHandle: String<br>fieldName: String<br>valueJson: String<br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker??<br>bridgeClassLoader: ClassLoader?? | String |  | 554 |
| `JsJavaBridgeDelegates.releaseInstance` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | instanceHandle: String<br>objectRegistry: ConcurrentHashMap<String, Any> | String |  | 604 |
| `JsJavaBridgeDelegates.ensureJsInterfaceLifecycleWorker` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` |  | Unit |  | 612 |
| `JsJavaBridgeDelegates.trackJsInterfaceProxy` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | proxy: Any<br>callbackInvoker: JsInterfaceCallbackInvoker<br>jsObjectIds: Collection<String> | Unit |  | 636 |
| `JsJavaBridgeDelegates.releaseCollectedJsInterfaceProxy` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | reference: JsInterfaceProxyReference | Unit |  | 670 |
| `JsJavaBridgeDelegates.collectJsInterfaceObjectIds` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | value: Any?<br>output: MutableSet<String> | Unit |  | 711 |
| `JsJavaBridgeDelegates.runBridgeCall` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | objectRegistry: ConcurrentHashMap<String, Any><br>block: () -> Any? | String |  | 725 |
| `JsJavaBridgeDelegates.describeThrowable` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | error: Throwable | String |  | 747 |
| `JsJavaBridgeDelegates.callSuspendInternal` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | targetClass: Class<*><br>instance: Any?<br>methodName: String<br>argsJson: String<br>staticOnly: Boolean<br>objectRegistry: ConcurrentHashMap<String, Any><br>callback: (String) -> Unit<br>coroutineContext: CoroutineContext<br>jsCallbackInv… | Unit |  | 760 |
| `JsJavaBridgeDelegates.resumeWith` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | result: Result<Any?> | Unit |  | 845 |
| `JsJavaBridgeDelegates.success` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | value: Any?<br>objectRegistry: ConcurrentHashMap<String, Any> | String |  | 877 |
| `JsJavaBridgeDelegates.failure` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | message: String | String |  | 890 |
| `JsJavaBridgeDelegates.loadClass` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | className: String<br>classLoader: ClassLoader?? | Class<*> |  | 897 |
| `JsJavaBridgeDelegates.requireInstance` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | instanceHandle: String<br>objectRegistry: ConcurrentHashMap<String, Any> | Any |  | 924 |
| `JsJavaBridgeDelegates.parseArgsJson` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | argsJson: String<br>objectRegistry: ConcurrentHashMap<String, Any> | List<Any?> |  | 934 |
| `JsJavaBridgeDelegates.parseSingleValueJson` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | valueJson: String<br>objectRegistry: ConcurrentHashMap<String, Any> | Any? |  | 958 |
| `JsJavaBridgeDelegates.decodeJsonValue` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | raw: Any?<br>objectRegistry: ConcurrentHashMap<String, Any><br>interpretBridgeMarkers: Boolean | Any? |  | 974 |
| `JsJavaBridgeDelegates.toJsonCompatibleValue` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | value: Any?<br>objectRegistry: ConcurrentHashMap<String, Any><br>bridgeAware: Boolean? | Any |  | 1048 |
| `JsJavaBridgeDelegates.exposeConstructedJavaObject` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | value: Any<br>objectRegistry: ConcurrentHashMap<String, Any> | JSONObject |  | 1131 |
| `JsJavaBridgeDelegates.toStructuredJsonValue` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | value: Any?<br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader: ClassLoader? | Any |  | 1142 |
| `JsJavaBridgeDelegates.selectConstructor` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*><br>rawArgs: List<Any?><br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader: ClassLoader? | ConstructorMatch |  | 1241 |
| `JsJavaBridgeDelegates.buildConstructorUnavailableMessage` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*> | String |  | 1277 |
| `JsJavaBridgeDelegates.buildConstructorMismatchMessage` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*><br>rawArgs: List<Any?> | String |  | 1289 |
| `JsJavaBridgeDelegates.selectMethod` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*><br>methodName: String<br>rawArgs: List<Any?><br>staticOnly: Boolean<br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader: ClassLoader? | MethodMatch |  | 1300 |
| `JsJavaBridgeDelegates.convertArguments` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | parameterTypes: Array<Class<*>><br>isVarArgs: Boolean<br>rawArgs: List<Any?><br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader: ClassLoader? | Pair<Array<Any?>, Int>? |  | 1343 |
| `JsJavaBridgeDelegates.convertArg` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | rawValue: Any?<br>targetType: Class<*><br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader: ClassLoader? | ConvertedArg? |  | 1425 |
| `JsJavaBridgeDelegates.createJsInterfaceProxy` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | binding: JsInterfaceBinding<br>targetType: Class<*><br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader: ClassLoader? | Any? |  | 1609 |
| `JsJavaBridgeDelegates.createJsInterfaceProxyFromMap` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | rawValue: Map<*, *><br>targetType: Class<*><br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader: ClassLoader? | Any? |  | 1675 |
| `JsJavaBridgeDelegates.resolveMapInterfaceMember` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | memberMap: MutableMap<String, Any?><br>method: Method<br>args: Array<out Any?> | Pair<Boolean, Any?> |  | 1755 |
| `JsJavaBridgeDelegates.accessorPropertyName` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | methodName: String | String? |  | 1779 |
| `JsJavaBridgeDelegates.isVoidLikeReturnType` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | returnType: Class<*> | Boolean |  | 1797 |
| `JsJavaBridgeDelegates.invokeJsInterfaceBinding` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | binding: JsInterfaceBinding<br>method: Method<br>args: Array<out Any?><br>objectRegistry: ConcurrentHashMap<String, Any><br>callbackInvoker: JsInterfaceCallbackInvoker<br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader:… | Any? |  | 1803 |
| `JsJavaBridgeDelegates.serializeCallbackArgs` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | args: Array<out Any?><br>objectRegistry: ConcurrentHashMap<String, Any> | String |  | 1847 |
| `JsJavaBridgeDelegates.parseBridgeResponse` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | raw: String | BridgeResponse |  | 1858 |
| `JsJavaBridgeDelegates.adaptReturnValue` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | value: Any?<br>targetType: Class<*><br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader: ClassLoader? | Any? |  | 1887 |
| `JsJavaBridgeDelegates.defaultPrimitiveValue` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | type: Class<*> | Any |  | 1927 |
| `JsJavaBridgeDelegates.convertToBoolean` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | rawValue: Any | ConvertedArg? |  | 1941 |
| `JsJavaBridgeDelegates.convertToChar` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | rawValue: Any | ConvertedArg? |  | 1956 |
| `JsJavaBridgeDelegates.convertToEnum` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | rawValue: Any<br>enumType: Class<*> | ConvertedArg? |  | 1972 |
| `JsJavaBridgeDelegates.convertToNumber` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | rawValue: Any<br>numberType: Class<*> | ConvertedArg? |  | 1993 |
| `JsJavaBridgeDelegates.findField` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*><br>fieldName: String<br>staticOnly: Boolean | Field? |  | 2020 |
| `JsJavaBridgeDelegates.hasMethod` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*><br>methodName: String<br>staticOnly: Boolean | Boolean |  | 2026 |
| `JsJavaBridgeDelegates.findStaticFallbackInstance` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*> | Any? |  | 2032 |
| `JsJavaBridgeDelegates.findNamedStaticInstance` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*><br>fieldName: String | Any? |  | 2037 |
| `JsJavaBridgeDelegates.findGetter` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*><br>fieldName: String<br>staticOnly: Boolean | Method? |  | 2044 |
| `JsJavaBridgeDelegates.findSetter` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | clazz: Class<*><br>fieldName: String<br>rawValue: Any?<br>staticOnly: Boolean<br>objectRegistry: ConcurrentHashMap<String, Any><br>jsCallbackInvoker: JsInterfaceCallbackInvoker?<br>bridgeClassLoader: ClassLoader? | Pair<Method, Any?>? |  | 2063 |
| `JsJavaBridgeDelegates.describeValueType` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | value: Any? | String |  | 2110 |
| `buildRuntimeBootstrapModules` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsLibraries.kt` | context: Context<br>operitDownloadDir: String<br>operitCleanOnExitDir: String | List<JsBootstrapModule> |  | 11 |
| `module` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsLibraries.kt` | fileName: String<br>source: String<br>globals: List<String>? | JsBootstrapModule |  | 94 |
| `getJsThirdPartyLibraries` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsLibraries.kt` |  | String |  | 106 |
| `JsNativeInterfaceDelegates.buildToolErrorJson` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | message: String | String |  | 76 |
| `JsNativeInterfaceDelegates.parseToolCall` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | toolType: String<br>toolName: String<br>paramsJson: String | ParsedToolCall |  | 86 |
| `JsNativeInterfaceDelegates.serializeToolExecutionResult` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | result: ToolResult<br>binaryDataRegistry: ConcurrentHashMap<String, ByteArray><br>binaryHandlePrefix: String<br>binaryDataThreshold: Int | String |  | 118 |
| `JsNativeInterfaceDelegates.serializeToolResultData` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | resultData: ToolResultData<br>binaryDataRegistry: ConcurrentHashMap<String, ByteArray><br>binaryHandlePrefix: String<br>binaryDataThreshold: Int | SerializedToolResultData |  | 145 |
| `JsNativeInterfaceDelegates.guard` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | defaultValue: T<br>failureMessage: String<br>block: () -> T | T |  | 202 |
| `JsNativeInterfaceDelegates.normalizeNonBlank` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | value: String | String? |  | 215 |
| `JsNativeInterfaceDelegates.parseBooleanFlag` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | value: String | Boolean |  | 219 |
| `JsNativeInterfaceDelegates.applyEnvValue` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | preferences: EnvPreferences<br>key: String<br>value: String? | Unit |  | 226 |
| `JsNativeInterfaceDelegates.setEnv` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | context: Context<br>key: String<br>value: String? | Unit |  | 240 |
| `JsNativeInterfaceDelegates.getEnv` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | context: Context<br>key: String<br>envOverrides: Map<String, String> | String |  | 246 |
| `JsNativeInterfaceDelegates.setEnvs` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | context: Context<br>valuesJson: String | Unit |  | 259 |
| `JsNativeInterfaceDelegates.isPackageImported` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | packageManager: PackageManager<br>packageName: String | Boolean |  | 272 |
| `JsNativeInterfaceDelegates.importPackage` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | packageManager: PackageManager<br>packageName: String | String |  | 278 |
| `JsNativeInterfaceDelegates.removePackage` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | packageManager: PackageManager<br>packageName: String | String |  | 285 |
| `JsNativeInterfaceDelegates.usePackage` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | packageManager: PackageManager<br>packageName: String | String |  | 292 |
| `JsNativeInterfaceDelegates.listImportedPackagesJson` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | packageManager: PackageManager | String |  | 299 |
| `JsNativeInterfaceDelegates.resolveToolName` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | packageManager: PackageManager<br>packageName: String<br>subpackageId: String<br>toolName: String<br>preferImported: String | String |  | 308 |
| `JsNativeInterfaceDelegates.readToolPkgResource` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | context: Context<br>packageManager: PackageManager<br>packageNameOrSubpackageId: String<br>resourceKey: String<br>outputFileName: String<br>internal: String | String |  | 346 |
| `JsNativeInterfaceDelegates.readToolPkgTextResource` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | packageManager: PackageManager<br>packageNameOrSubpackageId: String<br>resourcePath: String | String |  | 388 |
| `JsNativeInterfaceDelegates.parseWasmArgs` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | argsJson: String | ParsedWasmArgs |  | 406 |
| `JsNativeInterfaceDelegates.parseWasmI32` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | value: Any<br>label: String | Long |  | 449 |
| `JsNativeInterfaceDelegates.parseWasmI64` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | value: Any<br>label: String | Long |  | 462 |
| `JsNativeInterfaceDelegates.parseWasmF32Bits` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | value: Any<br>label: String | Long |  | 476 |
| `JsNativeInterfaceDelegates.parseWasmF64Bits` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | value: Any<br>label: String | Long |  | 485 |
| `JsNativeInterfaceDelegates.parseIntegralNumber` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | value: Double<br>label: String | Long |  | 490 |
| `JsNativeInterfaceDelegates.parseSignedIntegerText` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | value: String<br>label: String | Long |  | 500 |
| `JsNativeInterfaceDelegates.parseFiniteDouble` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | value: Any<br>label: String | Double |  | 509 |
| `JsNativeInterfaceDelegates.callToolPkgWasm` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | packageManager: PackageManager<br>packageNameOrSubpackageId: String<br>moduleId: String<br>exportName: String<br>argsJson: String | String |  | 523 |
| `JsNativeInterfaceDelegates.getPluginConfigDir` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | packageManager: PackageManager<br>pluginId: String | String |  | 564 |
| `JsNativeInterfaceDelegates.measureComposeText` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | context: Context<br>payloadJson: String | String |  | 577 |
| `JsNativeInterfaceDelegates.decompress` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | data: String<br>algorithm: String<br>binaryDataRegistry: ConcurrentHashMap<String, ByteArray><br>binaryHandlePrefix: String | String |  | 640 |
| `callToolSync` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | toolHandler: AIToolHandler<br>toolType: String<br>toolName: String<br>paramsJson: String<br>binaryDataRegistry: ConcurrentHashMap<String, ByteArray><br>binaryHandlePrefix: String<br>binaryDataThreshold: Int | String |  | 687 |
| `callToolAsync` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | toolHandler: AIToolHandler<br>callbackId: String<br>toolType: String<br>toolName: String<br>paramsJson: String<br>binaryDataRegistry: ConcurrentHashMap<String, ByteArray><br>binaryHandlePrefix: String<br>binaryDataThreshold: Int<br>sendToo… | Unit |  | 720 |
| `callToolAsyncStreaming` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | toolHandler: AIToolHandler<br>callbackId: String<br>intermediateCallbackId: String<br>toolType: String<br>toolName: String<br>paramsJson: String<br>binaryDataRegistry: ConcurrentHashMap<String, ByteArray><br>binaryHandlePrefix: String<br>b… | Unit |  | 771 |
| `buildToolResultCallbackScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | callbackId: String<br>result: String<br>isError: Boolean | String |  | 845 |
| `buildStringResultCallbackScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | callbackId: String<br>result: String<br>isError: Boolean | String |  | 876 |
| `imageProcessing` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | callbackId: String<br>operation: String<br>argsJson: String<br>binaryDataRegistry: ConcurrentHashMap<String, ByteArray><br>bitmapRegistry: ConcurrentHashMap<String, Bitmap><br>binaryHandlePrefix: String<br>sendToolResult: (callbackId: Stri… | Unit |  | 894 |
| `crypto` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | algorithm: String<br>operation: String<br>argsJson: String | String |  | 1056 |
| `JsToolManager.getInstance` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | context: Context<br>packageManager: PackageManager | JsToolManager |  | 34 |
| `JsToolManager.withEngine` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | block: suspend (JsEngine) -> T | T |  | 50 |
| `JsToolManager.withEngineBlocking` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | block: (JsEngine) -> T | T |  | 59 |
| `JsToolManager.parseDotCall` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | toolName: String | Pair<String, String>? |  | 65 |
| `JsToolManager.parsePackageToolName` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | toolName: String | Pair<String, String>? |  | 73 |
| `JsToolManager.buildRuntimeParams` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | packageName: String<br>params: Map<String, Any?> | MutableMap<String, Any?> |  | 81 |
| `JsToolManager.withExecutionEngineForPackage` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | packageName: String<br>block: suspend (JsEngine) -> T | T |  | 125 |
| `JsToolManager.withExecutionEngineForPackageBlocking` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | packageName: String<br>block: (JsEngine) -> T | T |  | 142 |
| `JsToolManager.convertToolParameters` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | tool: AITool<br>packageName: String<br>functionName: String | MutableMap<String, Any?> |  | 151 |
| `JsToolManager.convertToolParameterValue` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | toolName: String<br>parameterName: String<br>rawValue: String<br>type: String | Any? |  | 188 |
| `JsToolManager.parseNumberValue` | `JsToolManager` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | value: String | Number? |  | 210 |
| `parseBooleanValue` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | value: String | Boolean? |  | 220 |
| `invalidParameterType` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | toolName: String<br>parameterName: String<br>expectedType: String<br>rawValue: String<br>cause: Throwable?? | ToolParameterConversionException |  | 228 |
| `jsonObjectToKotlin` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | jsonObject: JSONObject | Map<String, Any?> |  | 246 |
| `jsonArrayToKotlin` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | jsonArray: JSONArray | List<Any?> |  | 256 |
| `jsonValueToKotlin` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | value: Any? | Any? |  | 264 |
| `success` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | toolName: String<br>value: Any? | ToolResult |  | 274 |
| `failure` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | toolName: String<br>message: String | ToolResult |  | 282 |
| `failure` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | toolName: String<br>failure: JsExecutionFailure | ToolResult |  | 291 |
| `trace` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | toolName: String<br>kind: String<br>message: String<br>level: String??<br>callId: String?? | ToolResult |  | 300 |
| `executeScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | toolName: String<br>params: Map<String, String> | String |  | 319 |
| `executeScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | script: String<br>tool: AITool | Flow<ToolResult> |  | 351 |
| `onCallLog` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | callId: String<br>level: String<br>message: String | Unit |  | 369 |
| `onIntermediateResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | callId: String<br>value: Any? | Unit |  | 381 |
| `executeComposeDsl` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` | script: String<br>packageName: String?<br>uiModuleId: String?<br>toolPkgId: String?<br>state: Map<String, Any?>?<br>memo: Map<String, Any?>?<br>moduleSpec: Map<String, Any?>?<br>envOverrides: Map<String, String>? | String |  | 423 |
| `destroy` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolManager.kt` |  | Unit |  | 473 |
| `buildToolPkgApiRuntimeScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgApiRuntime.kt` |  | String |  | 3 |
| `JsToolPkgExecutionContext.capture` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | script: String<br>functionName: String<br>params: Map<String, Any?> | LogSnapshot |  | 16 |
| `JsToolPkgExecutionContext.hasActivePluginIdForLogs` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | snapshot: LogSnapshot? | Boolean |  | 24 |
| `JsToolPkgExecutionContext.withPluginTag` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | snapshot: LogSnapshot?<br>message: String | String |  | 28 |
| `JsToolPkgExecutionContext.withCodeContext` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | snapshot: LogSnapshot?<br>message: String | String |  | 33 |
| `JsToolPkgExecutionContext.withTemporaryTextResourceResolver` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | resolver: (String, String) -> String?<br>block: () -> T | T |  | 50 |
| `JsToolPkgExecutionContext.resolveTemporaryTextResource` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | packageNameOrSubpackageId: String<br>resourcePath: String<br>onResolverFailure: (Exception) -> Unit | String? |  | 65 |
| `JsToolPkgExecutionContext.hasTemporaryTextResourceResolver` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` |  | Boolean |  | 79 |
| `JsToolPkgExecutionContext.resolvePluginTag` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | functionName: String<br>params: Map<String, Any?> | String |  | 81 |
| `JsToolPkgExecutionContext.buildSnippet` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | script: String<br>functionName: String | String |  | 103 |
| `JsToolPkgExecutionContext.compactTag` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | raw: String? | String |  | 139 |
| `JsToolPkgExecutionContext.firstNonBlank` | `JsToolPkgExecutionContext` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgExecutionContext.kt` | values: Any? | String? |  | 152 |
| `JsToolPkgRegistrationSession.begin` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` |  | Unit |  | 69 |
| `JsToolPkgRegistrationSession.isActive` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` |  | Boolean |  | 76 |
| `JsToolPkgRegistrationSession.appendToolboxUiModule` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 82 |
| `JsToolPkgRegistrationSession.appendUiRoute` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 83 |
| `JsToolPkgRegistrationSession.appendNavigationEntry` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 84 |
| `JsToolPkgRegistrationSession.appendDesktopWidget` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 85 |
| `JsToolPkgRegistrationSession.appendAppLifecycleHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 86 |
| `JsToolPkgRegistrationSession.appendMessageProcessingPlugin` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 87 |
| `JsToolPkgRegistrationSession.appendXmlRenderPlugin` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 90 |
| `JsToolPkgRegistrationSession.appendInputMenuTogglePlugin` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 91 |
| `JsToolPkgRegistrationSession.appendChatInputHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 94 |
| `JsToolPkgRegistrationSession.appendChatViewHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 97 |
| `JsToolPkgRegistrationSession.appendChatMessageHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 100 |
| `JsToolPkgRegistrationSession.appendChatMessageMenuItem` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 103 |
| `JsToolPkgRegistrationSession.appendChatRuntimeHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 106 |
| `JsToolPkgRegistrationSession.appendToolLifecycleHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 109 |
| `JsToolPkgRegistrationSession.appendPromptInputHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 112 |
| `JsToolPkgRegistrationSession.appendPromptHistoryHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 113 |
| `JsToolPkgRegistrationSession.appendPromptEstimateHistoryHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 115 |
| `JsToolPkgRegistrationSession.appendSystemPromptComposeHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 118 |
| `JsToolPkgRegistrationSession.appendToolPromptComposeHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 121 |
| `JsToolPkgRegistrationSession.appendPromptFinalizeHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 124 |
| `JsToolPkgRegistrationSession.appendPromptEstimateFinalizeHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 126 |
| `JsToolPkgRegistrationSession.appendSummaryGenerateHook` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 128 |
| `JsToolPkgRegistrationSession.appendAiProvider` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 130 |
| `JsToolPkgRegistrationSession.captureMarketOrigin` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | Unit |  | 133 |
| `JsToolPkgRegistrationSession.finish` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | executionResult: Any? | ToolPkgMainRegistrationCapture |  | 144 |
| `JsToolPkgRegistrationSession.read` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | bucket: RegistrationBucket | List<String> |  | 151 |
| `JsToolPkgRegistrationSession.end` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` |  | Unit |  | 181 |
| `JsToolPkgRegistrationSession.append` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | bucket: RegistrationBucket<br>specJson: String | Unit |  | 188 |
| `JsToolPkgRegistrationSession.normalizeRegistrationSpec` | `JsToolPkgRegistrationSession` | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | specJson: String | String |  | 199 |
| `buildToolPkgRegistrationBridgeScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` |  | String |  | 208 |
| `getJsToolsDefinition` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsTools.kt` |  | String | JavaScript Tools 对象定义 提供了一组便捷的工具调用方法，用于在JavaScript脚本中调用Android工具 | 4 |
| `ScriptExecutionReceiver.onReceive` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | context: Context<br>intent: Intent | Unit |  | 45 |
| `ScriptExecutionReceiver.execute` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | context: Context<br>executionMode: String<br>filePath: String?<br>codeText: String?<br>functionName: String<br>rawParamsJson: String?<br>paramsFilePath: String?<br>tempScript: Boolean<br>tempParamsFile: Boolean<br>envFilePath: String?<br>t… | Unit |  | 104 |
| `ScriptExecutionReceiver.resolveResultFile` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | rawPath: String?<br>scriptIdentityPath: String<br>functionName: String<br>executionMode: String | File |  | 283 |
| `ScriptExecutionReceiver.resolveParamsJson` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | rawParamsJson: String?<br>paramsFilePath: String? | String |  | 311 |
| `ScriptExecutionReceiver.normalizeParamsJson` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | rawPayload: String | String |  | 329 |
| `ScriptExecutionReceiver.canParseJsonObject` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | raw: String | Boolean |  | 347 |
| `ScriptExecutionReceiver.parseParams` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | paramsJson: String | Map<String, Any?> |  | 352 |
| `ScriptExecutionReceiver.parseEnvFile` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | envFilePath: String? | Map<String, String> |  | 368 |
| `ScriptExecutionReceiver.removeWrappingQuotes` | `ScriptExecutionReceiver` | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` |  | String |  | 404 |
| `deleteIfNeeded` | — | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | file: File<br>enabled: Boolean<br>label: String | Unit |  | 417 |
| `jsonElementToValue` | — | `com.ai.assistance.operit.core.tools.javascript` | `ScriptExecutionReceiver.kt` | element: JsonElement | Any? |  | 430 |
| `JavaSuspendLifecycleProbe.collectUntilCancelled` | `JavaSuspendLifecycleProbe` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeSuspendLifecycleTest.kt` |  | String |  | 22 ⚑ |
| `JavaSuspendLifecycleProbe.echo` | `JavaSuspendLifecycleProbe` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeSuspendLifecycleTest.kt` | value: String | String |  | 31 ⚑ |
| `OperitQuickJsEngine.bindNativeInterface` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | instance: Any | Unit |  | 46 |
| `OperitQuickJsEngine.evaluate` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | script: String<br>fileName: String? | T? |  | 53 |
| `OperitQuickJsEngine.callFunction` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | functionName: String<br>argsJson: String<br>callSite: String? | T? |  | 66 |
| `OperitQuickJsEngine.interrupt` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` |  | Unit |  | 82 |
| `OperitQuickJsEngine.getRuntimeTid` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` |  | Long | 运行线程的内核 tid；线程尚未启动或已关闭时返回 -1。 | 87 |
| `OperitQuickJsEngine.getMemoryUsage` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` |  | QuickJsMemoryUsage |  | 91 |
| `OperitQuickJsEngine.resetMemoryPeak` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` |  | Unit |  | 96 |
| `OperitQuickJsEngine.close` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` |  | Unit |  | 101 |
| `OperitQuickJsEngine.dispatchTimerOnRuntimeThread` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | timerId: Int | Unit |  | 117 |
| `OperitQuickJsEngine.runOnRuntimeThread` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | block: () -> T | T |  | 144 |
| `OperitQuickJsEngine.dispatchNativeCall` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | methodName: String<br>argsJson: String? | String? |  | 156 |
| `OperitQuickJsEngine.resolveMethod` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | target: Any<br>methodName: String<br>argCount: Int | Method |  | 166 |
| `OperitQuickJsEngine.decodeArgs` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | argsJson: String? | List<Any?> |  | 175 |
| `OperitQuickJsEngine.decodeJsonValue` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | valueJson: String? | Any? |  | 186 |
| `OperitQuickJsEngine.normalizeJsonValue` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | value: Any? | Any? |  | 193 |
| `OperitQuickJsEngine.convertArg` | `OperitQuickJsEngine` | `com.ai.assistance.operit.core.tools.javascript` | `OperitQuickJsEngine.kt` | value: Any?<br>parameterType: Class<*> | Any? |  | 202 |
| `buildQuickJsCompatScript` | — | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeCompatScriptBuilder.kt` |  | String |  | 3 |
| `QuickJsNativeHostDispatcher.onCall` | `QuickJsNativeHostDispatcher` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeHostDispatcher.kt` | method: String<br>argsJson: String? | String? |  | 21 |
| `QuickJsNativeHostDispatcher.close` | `QuickJsNativeHostDispatcher` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeHostDispatcher.kt` |  | Unit |  | 36 |
| `QuickJsNativeHostDispatcher.schedule` | `QuickJsNativeHostDispatcher` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeHostDispatcher.kt` | argsJson: String? | Unit |  | 42 |
| `QuickJsNativeHostDispatcher.cancel` | `QuickJsNativeHostDispatcher` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeHostDispatcher.kt` | argsJson: String? | Unit |  | 71 |
| `QuickJsNativeHostDispatcher.parseArgs` | `QuickJsNativeHostDispatcher` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeHostDispatcher.kt` | argsJson: String? | List<String> |  | 76 |
| `QuickJsNativeHostDispatcher.parseBoolean` | `QuickJsNativeHostDispatcher` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeHostDispatcher.kt` | value: String | Boolean |  | 88 |
| `QuickJsNativeBridge.nativeCreate` | `QuickJsNativeBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | hostBridge: QuickJsNativeRuntime.HostBridge | Long |  | 13 |
| `QuickJsNativeBridge.nativeDestroy` | `QuickJsNativeBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | handle: Long | Unit |  | 16 |
| `QuickJsNativeBridge.nativeEvaluate` | `QuickJsNativeBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | handle: Long<br>script: String<br>fileName: String | String |  | 19 |
| `QuickJsNativeBridge.nativeCallFunction` | `QuickJsNativeBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | handle: Long<br>functionName: String<br>argsJson: String<br>callSite: String | String |  | 22 |
| `QuickJsNativeBridge.nativeExecutePendingJobs` | `QuickJsNativeBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | handle: Long<br>maxJobs: Int | Int |  | 30 |
| `QuickJsNativeBridge.nativeGetMemoryUsage` | `QuickJsNativeBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | handle: Long | String |  | 33 |
| `QuickJsNativeBridge.nativeResetMemoryPeak` | `QuickJsNativeBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | handle: Long | Unit |  | 36 |
| `QuickJsNativeBridge.nativeInterrupt` | `QuickJsNativeBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | handle: Long | Unit |  | 39 |
| `QuickJsNativeRuntime.HostBridge.onCall` | `HostBridge` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | method: String<br>argsJson: String? | String? |  | 54 |
| `QuickJsNativeRuntime.create` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | hostBridge: HostBridge | QuickJsNativeRuntime |  | 66 |
| `QuickJsNativeRuntime.eval` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | script: String<br>fileName: String? | EvalResult |  | 76 |
| `QuickJsNativeRuntime.callFunction` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | functionName: String<br>argsJson: String<br>callSite: String? | EvalResult |  | 81 |
| `QuickJsNativeRuntime.installCompatLayerOrThrow` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` |  | Unit |  | 96 |
| `QuickJsNativeRuntime.executePendingJobs` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | maxJobs: Int? | Int |  | 107 |
| `QuickJsNativeRuntime.getMemoryUsage` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` |  | QuickJsMemoryUsage |  | 112 |
| `QuickJsNativeRuntime.resetMemoryPeak` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` |  | Unit |  | 121 |
| `QuickJsNativeRuntime.dispatchTimer` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | timerId: Int | EvalResult |  | 125 |
| `QuickJsNativeRuntime.clearAllTimers` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` |  | EvalResult |  | 132 |
| `QuickJsNativeRuntime.interrupt` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` |  | Unit |  | 139 |
| `QuickJsNativeRuntime.close` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` |  | Unit |  | 147 |
| `QuickJsNativeRuntime.requireHandle` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` |  | Long |  | 155 |
| `QuickJsNativeRuntime.parseEvalResult` | `QuickJsNativeRuntime` | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | resultJson: String | EvalResult |  | 160 |
| `optNullableString` | — | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeRuntime.kt` | name: String | String? |  | 184 |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `__actionId` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 163 |
| `__actionSettled` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 188 |
| `__activeCallRuntime` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 79 |
| `__activeCallRuntime` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 113 |
| `__activeCallRuntime` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 144 |
| `__bundle` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 89 |
| `__entry` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 90 |
| `__intermediateRenderInFlight` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 190 |
| `__intermediateRenderQueued` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 189 |
| `__javaBridgeJsObjectStore` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 50 |
| `__javaHandleRegistrations` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 51 |
| `__javaInstanceFinalizer` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 52 |
| `__noRender` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 174 |
| `__options` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 83 |
| `__options` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 117 |
| `__payload` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 170 |
| `__request` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 149 |
| `__root` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 76 |
| `__root` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 346 |
| `__runtimeOptions` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 153 |
| `__unsubscribeStateChange` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslRuntimeScript.kt` | inferred |  | 191 |
| `api` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 691 |
| `args` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 671 |
| `callState` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 430 |
| `controller` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 506 |
| `ctx` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 644 |
| `currentId` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 302 |
| `fieldValue` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 397 |
| `finalUrl` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 511 |
| `first` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsInitRuntimeScriptBuilder.kt` | inferred |  | 459 |
| `floatingWindowsApi` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred | 嵌套命名空间必须先经 namespace() 构建版本化方法，再挂到外层 ToolPkg.ui。 | 660 |
| `fn` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 401 |
| `functionRef` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 385 |
| `functionRef` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 405 |
| `hasTimeout` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 425 |
| `interfaceName` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 552 |
| `interfaceName` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 565 |
| `Java` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 1307 |
| `JavaApi` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 1192 |
| `JsJavaBridgeDelegates.CLASS_KEY` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 33 |
| `JsJavaBridgeDelegates.HANDLE_KEY` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 32 |
| `JsJavaBridgeDelegates.JS_INTERFACE_KEY` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 34 |
| `JsJavaBridgeDelegates.JS_INTERFACES_KEY` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 36 |
| `JsJavaBridgeDelegates.JS_OBJECT_ID_KEY` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 35 |
| `JsJavaBridgeDelegates.jsInterfaceLifecycleLock` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 91 |
| `JsJavaBridgeDelegates.jsInterfaceLifecycleWorkerStarted` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 96 |
| `JsJavaBridgeDelegates.jsInterfaceProxyReferenceQueue` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 88 |
| `JsJavaBridgeDelegates.jsInterfaceProxyReferences` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 89 |
| `JsJavaBridgeDelegates.jsInterfaceReferenceCounts` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 94 |
| `JsJavaBridgeDelegates.jsInterfaceReleaseInvokers` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 92 |
| `JsJavaBridgeDelegates.primitiveWrapperMap` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | Map<Class<*>, Class<*>> |  | 38 |
| `JsJavaBridgeDelegates.TAG` | `JsJavaBridgeDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridgeDelegates.kt` | inferred |  | 31 |
| `JsNativeInterfaceDelegates.MAX_SAFE_JS_INTEGER` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | inferred |  | 58 |
| `JsNativeInterfaceDelegates.TAG` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | inferred |  | 53 |
| `JsNativeInterfaceDelegates.WASM_TYPE_F32` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | inferred |  | 56 |
| `JsNativeInterfaceDelegates.WASM_TYPE_F64` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | inferred |  | 57 |
| `JsNativeInterfaceDelegates.WASM_TYPE_I32` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | inferred |  | 54 |
| `JsNativeInterfaceDelegates.WASM_TYPE_I64` | `JsNativeInterfaceDelegates` | `com.ai.assistance.operit.core.tools.javascript` | `JsNativeInterfaceDelegates.kt` | inferred |  | 55 |
| `JsTimeoutConfig.MAIN_TIMEOUT_SECONDS` | `JsTimeoutConfig` | `com.ai.assistance.operit.core.tools.javascript` | `JsTimeoutConfig.kt` | inferred |  | 4 |
| `JsTimeoutConfig.PRE_TIMEOUT_LEAD_SECONDS` | `JsTimeoutConfig` | `com.ai.assistance.operit.core.tools.javascript` | `JsTimeoutConfig.kt` | inferred |  | 5 |
| `JsTimeoutConfig.SCRIPT_TIMEOUT_MS` | `JsTimeoutConfig` | `com.ai.assistance.operit.core.tools.javascript` | `JsTimeoutConfig.kt` | inferred |  | 6 |
| `JsTimeoutConfig.TOOL_CALL_TIMEOUT_MS` | `JsTimeoutConfig` | `com.ai.assistance.operit.core.tools.javascript` | `JsTimeoutConfig.kt` | inferred |  | 7 |
| `jsValue` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 311 |
| `loaded` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 1321 |
| `MaterialTheme` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 624 |
| `nextId` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 320 |
| `normalized` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 293 |
| `normalized` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 151 |
| `normalized` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 756 |
| `normalized` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 438 |
| `normalizedField` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 408 |
| `normalizedPayload` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 900 |
| `out` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 415 |
| `out` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 439 |
| `output` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgApiRuntime.kt` | inferred |  | 181 |
| `path` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 440 |
| `previousActiveExports` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 1399 |
| `previousActiveModule` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 1398 |
| `previousCallId` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 431 |
| `previousCallRuntime` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 432 |
| `previousExports` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 1397 |
| `previousModule` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 1396 |
| `prototype` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 1235 |
| `proxy` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 871 |
| `resolvedPath` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 1312 |
| `runtimeContext` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 1419 |
| `safePreTimeoutMs` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 427 |
| `safeTimeoutSec` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 426 |
| `screen` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 439 |
| `sendIntermediateResult` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 38 |
| `since` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgApiRuntime.kt` | inferred |  | 109 |
| `start` | — | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeCompatScriptBuilder.kt` | inferred |  | 75 |
| `startedAt` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 646 |
| `TAG` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsAssetLoader.kt` | inferred |  | 6 |
| `targetFunction` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 1384 |
| `timerState` | — | `com.ai.assistance.operit.core.tools.javascript` | `QuickJsNativeCompatScriptBuilder.kt` | inferred |  | 79 |
| `token` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 92 |
| `tokenSet` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 93 |
| `tokenSet` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsJavaBridge.kt` | inferred |  | 156 |
| `TOOLPKG_EXECUTION_ENTRY_FUNCTION` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsExecutionScriptBuilder.kt` | inferred |  | 5 |
| `toolPkgApi` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsToolPkgRegistration.kt` | inferred |  | 590 |
| `trimmed` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 145 |
| `uiProxy` | — | `com.ai.assistance.operit.core.tools.javascript` | `JsComposeDslBridge.kt` | inferred |  | 635 |
