# operit.api.（其余零散）

> 函数 351 · 类型 51 · 顶层常量 28 · 共 430 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `AIForegroundService` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | class AIForegroundService : Service | 前台服务，用于在AI进行长时间处理时保持应用活跃，防止被系统杀死。 该服务不执行实际工作，仅通过显示一个持久通知来提升应用的进程优先级。 | 101 |
| `ChatMemoryRebuildManager` | `ChatMemoryRebuildManager` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildManager.kt` | class ChatMemoryRebuildManager(private val context: Context) |  | 30 |
| `ChatMemoryRebuildManager.PlannedChat` | `ChatMemoryRebuildManager` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildManager.kt` | class PlannedChat(val history: ChatHistory, val windows: List<ChatMemoryWindowPlanner.…, val memoryProfileId: String) |  | 246 |
| `ChatMemoryRebuildManager.Progress` | `ChatMemoryRebuildManager` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildManager.kt` | class Progress(val status: Status, val totalChats: Int, val completedChats: Int, val currentChatTitle: String, val totalWindows: Int, val completedWindows: Int, val totalSou… |  | 44 |
| `ChatMemoryRebuildManager.Status` | `ChatMemoryRebuildManager` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildManager.kt` | class Status |  | 62 |
| `ChatMemoryRebuildTimeScope` | `ChatMemoryRebuildTimeScope` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildTimeScope.kt` | class ChatMemoryRebuildTimeScope |  | 8 |
| `ChatMemoryRebuildTimeScope.EntireChat` | `ChatMemoryRebuildTimeScope` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildTimeScope.kt` | object EntireChat : ChatMemoryRebuildTimeScope |  | 9 |
| `ChatMemoryRebuildTimeScopeTest` | `ChatMemoryRebuildTimeScopeTest` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildTimeScopeTest.kt` | class ChatMemoryRebuildTimeScopeTest |  | 11 |
| `ChatMemoryWindowPlanner` | `ChatMemoryWindowPlanner` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlanner.kt` | object ChatMemoryWindowPlanner |  | 5 |
| `ChatMemoryWindowPlanner.Window` | `ChatMemoryWindowPlanner` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlanner.kt` | class Window(val messages: List<ChatMessage>, val sourceMessageCount: Int) |  | 11 |
| `ChatMemoryWindowPlannerTest` | `ChatMemoryWindowPlannerTest` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlannerTest.kt` | class ChatMemoryWindowPlannerTest |  | 10 |
| `ChatRuntimeHolder` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` | class ChatRuntimeHolder(context: Context) |  | 22 |
| `ChatRuntimeHolder.RuntimeHookObservation` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` | class RuntimeHookObservation(val stateByChatId: Map<String, InputProcessingSt…, val activeChatIds: Set<String>, val toolInvocationCountByChatId: Map<String, Int>) |  | 83 |
| `ChatRuntimeSlot` | `ChatRuntimeSlot` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeSlot.kt` | class ChatRuntimeSlot |  | 3 |
| `DeepgramSttProvider` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | class DeepgramSttProvider(private val context: Context, private val endpointUrl: String, private val apiKey: String, private val model: String) : SpeechService |  | 36 |
| `EnhancedAIService` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | class EnhancedAIService(private val context: Context) | Enhanced AI service that provides advanced conversational capabilities by integrating var… | 96 |
| `EnhancedAIService.MessageExecutionContext` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | class MessageExecutionContext(val executionId: Int, val streamBuffer: StringBuilder, val roundManager: ConversationRoundManager, val isConversationActive: AtomicBoolean, val conversationHi… |  | 436 |
| `EnhancedAIService.ModelExecutionSnapshot` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | class ModelExecutionSnapshot(val lease: MultiServiceManager.ServiceLe…) | Execution context for a single sendMessage call to achieve concurrency | 425 |
| `EnhancedAIService.SendMessageCallbacks` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | interface SendMessageCallbacks |  | 322 |
| `EnhancedAIService.SendMessageOptions` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | class SendMessageOptions(var message: String, var maxTokens: Int, var tokenUsageThreshold: Double, var chatId: String?, var chatHistory: List<PromptTurn>, var workspacePath: String?, … : suspend |  | 334 |
| `EnhancedAIService.TruncatedToolRoundRecovery` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | class TruncatedToolRoundRecovery(val repairedContent: String, val appendedSuffix: String, val invalidatedToolNames: List<String>) |  | 1491 |
| `EnhancedAIService.TurnTokenSnapshot` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | class TurnTokenSnapshot(val inputTokens: Long, val outputTokens: Long, val cachedInputTokens: Long) |  | 97 |
| `MemoryAnalysisProtocolTest` | `MemoryAnalysisProtocolTest` | `com.ai.assistance.operit.api.chat.library` | `MemoryAnalysisProtocolTest.kt` | class MemoryAnalysisProtocolTest |  | 11 |
| `MemoryAutoSaveScheduler` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` | class MemoryAutoSaveScheduler(private val context: Context, private val scope: CoroutineScope) |  | 24 |
| `MemoryLibrary` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | object MemoryLibrary | 记忆库管理类 - 提供分析对话内容并存储为结构化记忆图谱的功能。 | 35 |
| `MemoryLibrary.ParsedAnalysis` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | class ParsedAnalysis(val mainProblem: ParsedEntity?, val extractedEntities: List<ParsedEntity>, val links: List<ParsedLink>, val updatedEntities: List<ParsedUpdate>, val mergedEnt… |  | 77 |
| `MemoryLibrary.ParsedEntity` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | class ParsedEntity(val title: String, val content: String, val tags: List<String>, val aliasFor: String?, val folderPath: String) |  | 52 |
| `MemoryLibrary.ParsedLink` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | class ParsedLink(val sourceTitle: String, val targetTitle: String, val type: String, val description: String, val weight: Float) |  | 44 |
| `MemoryLibrary.ParsedMerge` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | class ParsedMerge(val sourceTitles: List<String>, val newTitle: String, val newContent: String, val newTags: List<String>, val folderPath: String, val reason: String) |  | 68 |
| `MemoryLibrary.ParsedUpdate` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | class ParsedUpdate(val titleToUpdate: String, val newContent: String, val reason: String, val newCredibility: Float?, val newImportance: Float?) |  | 60 |
| `OnnxSileroVad` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | class OnnxSileroVad(context: Context, private val sampleRate: Int, private val frameSize: Int, private val mode: Mode, speechDurationMs: Int, silenceDurationMs: Int, modelAssetPa… : AutoCloseable |  | 15 |
| `OnnxSileroVad.Mode` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | class Mode |  | 29 |
| `OpenAISttProvider` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | class OpenAISttProvider(private val context: Context, private val endpointUrl: String, private val apiKey: String, private val model: String) : SpeechService |  | 37 |
| `PersonalWakeEnrollment` | `PersonalWakeEnrollment` | `com.ai.assistance.operit.api.speech` | `PersonalWakeEnrollment.kt` | object PersonalWakeEnrollment |  | 11 |
| `PersonalWakeFeatureExtractor` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | object PersonalWakeFeatureExtractor |  | 10 |
| `PersonalWakeFeatureExtractor.Config` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | class Config(val sampleRate: Int, val frameSize: Int, val hopSize: Int, val fftSize: Int, val melBins: Int, val numMfcc: Int, val maxFrames: Int, val fMin: Float, val fMax… |  | 13 |
| `PersonalWakeFeatureExtractor.MelFilterBank` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | class MelFilterBank(val weights: Array<FloatArray>) |  | 25 |
| `PersonalWakeListener` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | class PersonalWakeListener(private val context: Context, private val templatesProvider: () -> List<FloatArray>, private val onTriggered: (similarity: Float) -> Unit) |  | 15 |
| `PersonalWakeListener.Config` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | class Config(val sampleRate: Int, val frameSize: Int, val maxSegmentMs: Long, val minSegmentMs: Long, val endSilenceMs: Long, val similarityThreshold: Float, val dynamicTh… |  | 24 |
| `SherpaMnnSpeechProvider` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` | class SherpaMnnSpeechProvider(private val context: Context) : SpeechService | 基于sherpa-mnn的本地语音识别实现，集成VAD能力 sherpa-mnn是基于MNN的语音识别引擎，支持流式识别和VAD | 32 |
| `SherpaSpeechProvider` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` | class SherpaSpeechProvider(private val context: Context) : SpeechService | 基于sherpa-ncnn的本地语音识别实现 sherpa-ncnn是一个轻量级、高性能的语音识别引擎，比Whisper更适合移动端 参考: https://github.com… | 36 |
| `SpeechPrerollStore` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | object SpeechPrerollStore |  | 10 |
| `SpeechService` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` | interface SpeechService | 语音识别服务接口 定义与不同语音识别引擎进行交互的标准方法 | 8 |
| `SpeechService.RecognitionError` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` | class RecognitionError(val code: Int, val message: String) | 识别错误类型 | 38 |
| `SpeechService.RecognitionResult` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` | class RecognitionResult(val text: String, val isFinal: Boolean, val confidence: Float) | 识别结果类型 | 31 |
| `SpeechService.RecognitionState` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` | class RecognitionState | 当前识别引擎状态枚举 | 10 |
| `SpeechServiceFactory` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | object SpeechServiceFactory | 语音识别服务工厂类 用于创建和管理不同类型的语音识别服务 | 11 |
| `SpeechServiceFactory.LocalEntry` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | class LocalEntry(val type: SpeechServiceType, val service: SpeechService, var refCount: Int) |  | 104 |
| `SpeechServiceFactory.SpeechServiceLease` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | class SpeechServiceLease(private val delegate: SpeechService, private val onRelease: () -> Unit) : SpeechService by delegate |  | 91 |
| `SpeechServiceFactory.SpeechServiceType` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | class SpeechServiceType | 语音识别服务类型 | 15 |
| `WakePhraseSnapshot` | `WakePhraseSnapshot` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | class WakePhraseSnapshot(val phrase: String, val regexEnabled: Boolean) |  | 5 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `tryGetClientUid` | — | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Int? |  | 78 |
| `tryGetClientPackageName` | — | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | String? |  | 89 |
| `AIForegroundService.buildReplyNotificationTag` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | chatId: String? | String |  | 155 |
| `AIForegroundService.createMainActivityPendingIntent` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context<br>chatId: String? | PendingIntent |  | 160 |
| `AIForegroundService.buildReplyNotificationChannelId` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | enableSound: Boolean<br>enableVibration: Boolean | String |  | 182 |
| `AIForegroundService.getReplyNotificationChannelNameRes` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | enableSound: Boolean<br>enableVibration: Boolean | Int |  | 193 |
| `AIForegroundService.ensureReplyNotificationChannel` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context<br>enableSound: Boolean<br>enableVibration: Boolean | String |  | 204 |
| `AIForegroundService.loadBitmapFromUri` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context<br>uriString: String | Bitmap? |  | 250 |
| `AIForegroundService.notifyReplyCompleted` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context<br>chatId: String?<br>characterName: String?<br>rawReplyContent: String?<br>avatarUri: String?<br>notifyReplyOverride: Boolean?? | Unit |  | 287 |
| `AIForegroundService.setWakeListeningSuspendedForIme` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context<br>imeVisible: Boolean | Unit |  | 390 |
| `AIForegroundService.setWakeListeningSuspendedForFloatingFullscreen` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context<br>active: Boolean | Unit |  | 404 |
| `AIForegroundService.ensureMicrophoneForeground` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context<br>forceStart: Boolean? | Unit |  | 421 |
| `AIForegroundService.ensureRunningForExternalHttp` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context | Unit |  | 445 |
| `AIForegroundService.refreshBackgroundKeepAlive` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context | Unit |  | 449 |
| `AIForegroundService.stopExternalHttp` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context | Unit |  | 475 |
| `AIForegroundService.startServiceForAction` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context<br>action: String | Unit |  | 484 |
| `AIForegroundService.hasPersistentForegroundResponsibilityConfigured` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | context: Context | Boolean |  | 502 |
| `AIForegroundService.updateWakeListeningSuspendedForIme` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | imeVisible: Boolean | Unit |  | 523 |
| `AIForegroundService.updateWakeListeningSuspendedForExternalRecording` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | externalRecording: Boolean | Unit |  | 530 |
| `AIForegroundService.updateWakeListeningSuspendedForFloatingFullscreen` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | active: Boolean | Unit |  | 537 |
| `AIForegroundService.applyWakeListeningState` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 544 |
| `AIForegroundService.applyWakeListeningStateLocked` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 554 |
| `AIForegroundService.startRecordingStateMonitoring` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 572 |
| `AIForegroundService.onRecordingConfigChanged` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | configs: List<AudioRecordingConfiguration> | Unit |  | 582 |
| `AIForegroundService.isExternalConfig` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | cfg: AudioRecordingConfiguration | Boolean |  | 590 |
| `AIForegroundService.isExternalConfig` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | cfg: AudioRecordingConfiguration | Boolean |  | 662 |
| `AIForegroundService.stopRecordingStateMonitoring` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 695 |
| `AIForegroundService.ensureWakeSpeechProvider` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | SpeechService |  | 793 |
| `AIForegroundService.releaseWakeSpeechProvider` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 801 |
| `AIForegroundService.startOrRefreshExternalHttpServer` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | config: ExternalHttpApiConfig? | Unit |  | 810 |
| `AIForegroundService.stopExternalHttpServer` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | portOverride: Int??<br>lastError: String?? | Unit |  | 861 |
| `AIForegroundService.updateExternalHttpState` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | newState: ExternalChatHttpState<br>refreshNotification: Boolean? | Unit |  | 880 |
| `AIForegroundService.refreshServiceNotification` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 890 |
| `AIForegroundService.isExternalHttpEnabledNow` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Boolean |  | 898 |
| `AIForegroundService.stopSelfIfIdle` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | ignoreAppForeground: Boolean? | Unit |  | 906 |
| `AIForegroundService.onCreate` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 927 |
| `AIForegroundService.observeRuntimeTaskViewPreference` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 953 |
| `AIForegroundService.observeBackgroundKeepAlivePreference` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 969 |
| `AIForegroundService.updateAiBusyState` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | isBusy: Boolean | Unit |  | 990 |
| `AIForegroundService.updateRuntimeTaskViewVisibility` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 995 |
| `AIForegroundService.observeChatRuntimeStats` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1022 |
| `AIForegroundService.hasRecordAudioPermission` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Boolean |  | 1037 |
| `AIForegroundService.isAlwaysListeningEnabledNow` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Boolean |  | 1046 |
| `AIForegroundService.tryPromoteToMicrophoneForeground` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Boolean |  | 1054 |
| `AIForegroundService.onStartCommand` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | intent: Intent?<br>flags: Int<br>startId: Int | Int |  | 1085 |
| `AIForegroundService.onDestroy` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1279 |
| `AIForegroundService.onBind` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | intent: Intent? | IBinder? |  | 1304 |
| `AIForegroundService.createNotificationChannel` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1309 |
| `AIForegroundService.startExternalHttpMonitoring` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1326 |
| `AIForegroundService.startWakeMonitoring` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1362 |
| `AIForegroundService.updateKeepAliveOverlayVisibility` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1420 |
| `AIForegroundService.stopWakeMonitoring` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1428 |
| `AIForegroundService.runOnMainThread` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | action: () -> Unit | Unit |  | 1450 |
| `AIForegroundService.showKeepAliveOverlayIfPossible` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1464 |
| `AIForegroundService.hideKeepAliveOverlay` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1517 |
| `AIForegroundService.startWakeListening` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1535 |
| `AIForegroundService.startWakeListeningLocked` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1541 |
| `AIForegroundService.startPersonalWakeListening` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1695 |
| `AIForegroundService.stopWakeListening` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | releaseProvider: Boolean? | Unit |  | 1742 |
| `AIForegroundService.stopWakeListeningLocked` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | releaseProvider: Boolean? | Unit |  | 1748 |
| `AIForegroundService.scheduleWakeResume` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1776 |
| `AIForegroundService.triggerWakeLaunch` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Unit |  | 1813 |
| `AIForegroundService.matchWakePhrase` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | recognized: String<br>phrase: String<br>regexEnabled: Boolean | Boolean |  | 1832 |
| `AIForegroundService.normalizeWakeText` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` | text: String | String |  | 1849 |
| `AIForegroundService.createNotification` | `AIForegroundService` | `com.ai.assistance.operit.api.chat` | `AIForegroundService.kt` |  | Notification |  | 1860 |
| `ChatRuntimeHolder.getCore` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` | slot: ChatRuntimeSlot | ChatServiceCore |  | 40 |
| `ChatRuntimeHolder.observeStats` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` |  | Unit |  | 53 |
| `ChatRuntimeHolder.observeRuntimeHooks` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` |  | Unit |  | 89 |
| `ChatRuntimeHolder.countCurrentTurnToolsForActiveChats` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` | activeChatIds: Set<String><br>countMap: Map<String, Int> | Int |  | 143 |
| `ChatRuntimeHolder.setupCrossSessionSync` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` |  | Unit |  | 150 |
| `ChatRuntimeHolder.registerTurnSync` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` | sourceSlot: ChatRuntimeSlot<br>targetSlot: ChatRuntimeSlot | Unit |  | 165 |
| `ChatRuntimeHolder.syncMainChatSelectionToFloating` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` | chatId: String | Unit |  | 200 |
| `ChatRuntimeHolder.registerChatSelectionSync` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` | sourceSlot: ChatRuntimeSlot<br>targetSlot: ChatRuntimeSlot | Unit |  | 209 |
| `ChatRuntimeHolder.syncChatSelection` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` | sourceSlot: ChatRuntimeSlot<br>targetSlot: ChatRuntimeSlot<br>chatId: String | Unit |  | 226 |
| `ChatRuntimeHolder.getInstance` | `ChatRuntimeHolder` | `com.ai.assistance.operit.api.chat` | `ChatRuntimeHolder.kt` | context: Context | ChatRuntimeHolder |  | 258 |
| `EnhancedAIService.getInstance` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context | EnhancedAIService | 获取EnhancedAIService实例 | 117 |
| `EnhancedAIService.getChatInstance` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>chatId: String | EnhancedAIService |  | 127 |
| `EnhancedAIService.releaseChatInstance` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | chatId: String | Unit |  | 136 |
| `EnhancedAIService.getAIServiceForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>functionType: FunctionType | AIService | 获取指定功能类型的 AIService 实例（非实例化方式） | 151 |
| `EnhancedAIService.acquireAIServiceForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>functionType: FunctionType | MultiServiceManager.ServiceLease |  | 158 |
| `EnhancedAIService.getModelConfigForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>functionType: FunctionType | ModelConfigData |  | 164 |
| `EnhancedAIService.refreshServiceForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>functionType: FunctionType | Unit | 刷新指定功能类型的 AIService 实例（非实例化方式） | 176 |
| `EnhancedAIService.refreshAllServices` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context | Unit | 刷新所有 AIService 实例（非实例化方式） | 188 |
| `EnhancedAIService.getCurrentInputTokenCountForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>functionType: FunctionType | Long | 获取指定功能类型的当前输入token计数（非实例化方式） | 202 |
| `EnhancedAIService.getCurrentOutputTokenCountForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>functionType: FunctionType | Long | 获取指定功能类型的当前输出token计数（非实例化方式） | 218 |
| `EnhancedAIService.resetTokenCountersForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>functionType: FunctionType?? | Unit | 重置指定功能类型或所有功能类型的token计数器（非实例化方式） | 233 |
| `EnhancedAIService.resetTokenCounters` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context | Unit |  | 250 |
| `EnhancedAIService.applyFileBinding` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>originalContent: String<br>aiGeneratedCode: String<br>onProgress: ((Float, String) -> Unit)?? | Pair<String, String> | 处理文件绑定操作（非实例化方式） | 275 |
| `EnhancedAIService.applyFileBindingOperations` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>originalContent: String<br>operations: List<FileBindingService.StructuredE…<br>onProgress: ((Float, String) -> Unit)?? | Pair<String, String> |  | 292 |
| `EnhancedAIService.generatePackageDescription` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: Context<br>pluginName: String<br>toolDescriptions: List<String> | String | 自动生成工具包描述（非实例化方式） | 313 |
| `EnhancedAIService.SendMessageCallbacks.onNonFatalError` | `SendMessageCallbacks` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | error: String | Unit |  | 323 |
| `EnhancedAIService.SendMessageCallbacks.onTokenLimitExceeded` | `SendMessageCallbacks` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | Unit |  | 325 |
| `EnhancedAIService.SendMessageCallbacks.onToolInvocation` | `SendMessageCallbacks` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | toolName: String | Unit |  | 327 |
| `EnhancedAIService.SendMessageCallbacks.onSubtaskToolResult` | `SendMessageCallbacks` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | recordJson: String | Unit |  | 329 |
| `EnhancedAIService.SendMessageCallbacks.onSubtaskCompleted` | `SendMessageCallbacks` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | outcomeJson: String | Unit |  | 331 |
| `EnhancedAIService.ensureInitialized` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | Unit |  | 383 |
| `EnhancedAIService.setInputProcessingState` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | newState: com.ai.assistance.operit.data.model… | Unit | 设置当前的输入处理状态 | 403 |
| `EnhancedAIService.registerExecutionContext` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: MessageExecutionContext | Unit |  | 459 |
| `EnhancedAIService.unregisterExecutionContext` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: MessageExecutionContext | Unit |  | 463 |
| `EnhancedAIService.invalidateExecutionContext` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: MessageExecutionContext<br>reason: String | Unit |  | 467 |
| `EnhancedAIService.invalidateAllExecutionContexts` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | reason: String | Unit |  | 474 |
| `EnhancedAIService.isExecutionContextActive` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: MessageExecutionContext | Boolean |  | 480 |
| `EnhancedAIService.getModelExecutionSnapshot` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: MessageExecutionContext<br>functionType: FunctionType<br>chatModelConfigIdOverride: String?<br>chatModelIndexOverride: Int? | ModelExecutionSnapshot |  | 485 |
| `EnhancedAIService.releaseModelExecutionSnapshot` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: MessageExecutionContext | Unit |  | 508 |
| `EnhancedAIService.startAssistantResponseRound` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: MessageExecutionContext | Unit |  | 514 |
| `EnhancedAIService.getAIServiceForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType | AIService | 获取指定功能类型的 AIService 实例 | 565 |
| `EnhancedAIService.acquireAIServiceForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType<br>chatModelConfigIdOverride: String??<br>chatModelIndexOverride: Int?? | MultiServiceManager.ServiceLease |  | 574 |
| `EnhancedAIService.getAIServiceForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType<br>chatModelConfigIdOverride: String?<br>chatModelIndexOverride: Int? | AIService |  | 590 |
| `EnhancedAIService.getProviderAndModelForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType | Pair<String, String> | 获取指定功能类型的provider和model信息 | 612 |
| `EnhancedAIService.getProviderAndModelForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType<br>chatModelConfigIdOverride: String?<br>chatModelIndexOverride: Int? | Pair<String, String> |  | 620 |
| `EnhancedAIService.getDisplayProviderAndModelForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType<br>chatModelConfigIdOverride: String?<br>chatModelIndexOverride: Int? | Pair<String, String> |  | 643 |
| `EnhancedAIService.getModelConfigForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType<br>chatModelConfigIdOverride: String??<br>chatModelIndexOverride: Int?? | ModelConfigData |  | 661 |
| `EnhancedAIService.refreshServiceForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType | Unit | 刷新指定功能类型的 AIService 实例 当配置发生更改时调用 | 679 |
| `EnhancedAIService.refreshAllServices` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | Unit | 刷新所有 AIService 实例 当全局配置发生更改时调用 | 685 |
| `EnhancedAIService.getModelParametersForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType<br>chatModelConfigIdOverride: String??<br>chatModelIndexOverride: Int?? | List<com.ai.assistance.operit.data.model.ModelParameter<*>> |  | 690 |
| `EnhancedAIService.callFunctionModel` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType<br>turns: List<PromptTurn><br>enableThinking: Boolean?<br>recordTokenUsage: Boolean? | String |  | 704 |
| `EnhancedAIService.publishRequestWindowEstimate` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | windowSize: Long | Unit |  | 735 |
| `EnhancedAIService.estimatePreparedRequestWindow` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | serviceForFunction: AIService<br>preparedHistory: List<PromptTurn><br>availableTools: List<ToolPrompt>?<br>publishEstimate: Boolean | Long |  | 739 |
| `EnhancedAIService.applyPromptFinalizeHooks` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | initialContext: PromptHookContext<br>dispatchHooks: (PromptHookContext) -> PromptHookCo…? | PromptHookContext |  | 756 |
| `EnhancedAIService.bypassPromptHooks` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: PromptHookContext | PromptHookContext |  | 763 |
| `EnhancedAIService.buildPromptFinalizeMetadata` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | chatId: String?<br>roleCardId: String?<br>workspacePath: String?<br>workspaceEnv: String?<br>enableThinking: Boolean<br>stream: Boolean<br>isSubTask: Boolean | Map<String, Any?> |  | 765 |
| `EnhancedAIService.applyFinalizedCurrentUserTurn` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | preparedHistory: List<PromptTurn><br>originalCurrentMessage: String<br>finalizedCurrentMessage: String | List<PromptTurn> |  | 783 |
| `EnhancedAIService.estimateRequestWindowFromMemory` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | message: String<br>chatHistory: List<PromptTurn><br>chatId: String??<br>workspacePath: String??<br>workspaceEnv: String??<br>functionType: FunctionType?<br>promptFunctionType: PromptFunctionType?<br>enableThinking: Boolean?<br>customSystem… | Long |  | 808 |
| `EnhancedAIService.sendMessage` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | options: SendMessageOptions | Stream<String> | Send a message to the AI service | 938 |
| `EnhancedAIService.emit` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | value: String | Unit |  | 1024 |
| `EnhancedAIService.enhanceToolDetection` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | content: String | String | 使用流处理技术增强工具调用检测能力 这个方法通过流式XML解析来辅助识别工具调用，比单纯依赖正则表达式更可靠 | 1389 |
| `EnhancedAIService.normalizeToolXml` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | xml: String | String | 规范化工具XML以符合正则表达式预期 | 1465 |
| `EnhancedAIService.isToolXmlBlock` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | xml: String<br>tagName: String | Boolean |  | 1483 |
| `EnhancedAIService.detectAndRepairTruncatedToolRound` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | content: String | TruncatedToolRoundRecovery? |  | 1497 |
| `EnhancedAIService.buildTruncatedToolRepairSuffix` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | fragment: String<br>fallbackTagName: String | String |  | 1556 |
| `EnhancedAIService.extractXmlAttributeValue` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | source: String<br>attributeName: String | String? |  | 1653 |
| `EnhancedAIService.extractTrailingPartialTag` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | fragment: String | String? |  | 1662 |
| `EnhancedAIService.completePartialOpenTag` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | partialTag: String<br>tagName: String<br>defaultNameValue: String | String |  | 1671 |
| `EnhancedAIService.isPartialOpeningTagFor` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | partialTag: String<br>tagName: String | Boolean |  | 1716 |
| `EnhancedAIService.isPartialClosingTagFor` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | partialTag: String<br>tagName: String | Boolean |  | 1732 |
| `EnhancedAIService.completePartialTagName` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | partialTag: String<br>tagName: String | String |  | 1748 |
| `EnhancedAIService.completePartialClosingTag` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | partialTag: String<br>tagName: String | String |  | 1758 |
| `EnhancedAIService.processStreamCompletion` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: MessageExecutionContext<br>functionType: FunctionType?<br>promptFunctionType: PromptFunctionType?<br>collector: StreamCollector<String><br>enableThinking: Boolean?<br>enableMemoryAutoUpdate: Boolean?<br>onNonFatalError: suspend (e… | Unit | 在处理完流后调用，使用增强的工具检测功能 | 1766 |
| `EnhancedAIService.finalizeAssistantResponse` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | context: MessageExecutionContext<br>content: String<br>enableMemoryAutoUpdate: Boolean<br>onNonFatalError: suspend (error: String) -> Unit<br>isSubTask: Boolean<br>chatId: String??<br>characterName: String??<br>avatarUri: String??<br>notif… | Unit | Finalize an assistant response without relying on status-tag control flow. | 2092 |
| `EnhancedAIService.handleToolInvocation` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | toolInvocations: List<ToolInvocation><br>context: MessageExecutionContext<br>functionType: FunctionType?<br>promptFunctionType: PromptFunctionType?<br>collector: StreamCollector<String><br>enableThinking: Boolean?<br>enableMemoryAutoUpdate… | Unit | Handle tool invocation processing - simplified version without callbacks | 2159 |
| `EnhancedAIService.awaitToolJob` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | scope: CoroutineScope | Unit |  | 2278 |
| `EnhancedAIService.processToolResults` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | results: List<ToolResult><br>context: MessageExecutionContext<br>functionType: FunctionType?<br>promptFunctionType: PromptFunctionType?<br>collector: StreamCollector<String><br>enableThinking: Boolean?<br>enableMemoryAutoUpdate: Boolean?<b… | Unit | Process tool execution result - simplified version without callbacks | 2299 |
| `EnhancedAIService.getCurrentInputTokenCount` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | Long | Get the current input token count from the last API call | 2598 |
| `EnhancedAIService.getCurrentOutputTokenCount` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | Long | Get the current output token count from the last API call | 2606 |
| `EnhancedAIService.getCurrentCachedInputTokenCount` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | Long | Get the current cached input token count accumulated across the current turn | 2614 |
| `EnhancedAIService.captureCurrentTurnTokenSnapshot` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | TurnTokenSnapshot |  | 2618 |
| `EnhancedAIService.setCurrentTurnTokenCounts` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | inputTokens: Long<br>outputTokens: Long<br>cachedInputTokens: Long? | Unit |  | 2627 |
| `EnhancedAIService.resetTokenCounters` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | Unit | Reset token counters to zero Use this when starting a new conversation | 2647 |
| `EnhancedAIService.resetTokenCountersForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType?? | Unit | 重置指定功能类型或所有功能类型的token计数器 | 2655 |
| `EnhancedAIService.generateSummary` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | messages: List<Pair<String, String>><br>recordTokenUsage: Boolean? | String | 生成对话总结 | 2664 |
| `EnhancedAIService.generateSummary` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | messages: List<Pair<String, String>><br>previousSummary: String?<br>summaryConfig: ConversationSummaryConfig?<br>recordTokenUsage: Boolean? | String | 生成对话总结，并且包含上一次的总结内容 | 2677 |
| `EnhancedAIService.generateSummaryFromPromptTurns` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | messages: List<PromptTurn><br>previousSummary: String?<br>summaryConfig: ConversationSummaryConfig?<br>recordTokenUsage: Boolean? | String |  | 2691 |
| `EnhancedAIService.generateConversationTitle` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | userText: String<br>attachmentFileNames: List<String>?<br>recordTokenUsage: Boolean? | String |  | 2709 |
| `EnhancedAIService.getCurrentInputTokenCountForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType | Long | 获取指定功能类型的当前输入token计数 | 2727 |
| `EnhancedAIService.getCurrentOutputTokenCountForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType | Long | 获取指定功能类型的当前输出token计数 | 2736 |
| `EnhancedAIService.resolveToolDisplayName` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | tool: AITool | String |  | 2740 |
| `EnhancedAIService.prepareConversationHistory` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | chatHistory: List<PromptTurn><br>processedInput: String<br>chatId: String?<br>workspacePath: String?<br>workspaceEnv: String?<br>promptFunctionType: PromptFunctionType<br>customSystemPromptTemplate: String??<br>roleCardId: String?<br>enabl… | List<PromptTurn> | Prepare the conversation history with system prompt | 2753 |
| `EnhancedAIService.serializePromptHookModelParameters` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | modelParameters: List<com.ai.assistance.operit.data.… | List<Map<String, Any?>> |  | 2818 |
| `EnhancedAIService.serializePromptHookToolPrompts` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | toolPrompts: List<ToolPrompt>? | List<Map<String, Any?>> |  | 2839 |
| `EnhancedAIService.deserializePromptHookToolPrompts` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | toolItems: List<Map<String, Any?>> | List<ToolPrompt> |  | 2864 |
| `EnhancedAIService.deserializePromptHookToolParameters` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | value: Any? | List<ToolParameterSchema> |  | 2882 |
| `EnhancedAIService.applyToolPromptComposeHooksToAvailableTools` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | availableTools: List<ToolPrompt><br>chatId: String?<br>functionType: FunctionType<br>promptFunctionType: PromptFunctionType?<br>useEnglish: Boolean | List<ToolPrompt> |  | 2900 |
| `EnhancedAIService.cancelConversation` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | Unit | Cancel the current conversation | 2922 |
| `EnhancedAIService.cancelAllToolExecutions` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` |  | Unit | Cancel all tool executions | 2967 |
| `EnhancedAIService.getAvailableToolsForFunction` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | functionType: FunctionType<br>chatId: String??<br>promptFunctionType: PromptFunctionType??<br>roleCardId: String??<br>modelConfig: ModelConfigData | List<ToolPrompt>? | 获取可用工具列表（用于Tool Call API） 如果模型配置启用了Tool Call，返回工具列表；否则返回null | 2977 |
| `EnhancedAIService.startAiService` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | characterName: String??<br>avatarUri: String?? | Unit | 启动或更新前台服务为“AI 正在运行”状态，以保持应用活跃 | 3121 |
| `EnhancedAIService.notifyReplyCompleted` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | chatId: String?<br>characterName: String??<br>avatarUri: String??<br>notifyReplyOverride: Boolean?? | Unit |  | 3158 |
| `EnhancedAIService.stopAiService` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | characterName: String??<br>avatarUri: String?? | Unit | 将前台服务更新为“空闲/已完成”状态，但不真正停止服务 | 3175 |
| `EnhancedAIService.applyFileBinding` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | originalContent: String<br>aiGeneratedCode: String | Pair<String, String> | 处理文件绑定操作（实例方法） | 3225 |
| `EnhancedAIService.translateText` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | text: String<br>recordTokenUsage: Boolean? | String | 翻译文本功能 | 3240 |
| `EnhancedAIService.generatePackageDescription` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | pluginName: String<br>toolDescriptions: List<String> | String | 自动生成工具包描述 | 3250 |
| `EnhancedAIService.saveConversationToMemoryAsync` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | conversationHistory: List<Pair<String, String>><br>lastContent: String<br>memorySpaceIdOverride: String??<br>onSuccess: (suspend () -> Unit)??<br>onError: (suspend (Exception) -> Unit)?? | Unit | Manually saves the current conversation to the problem library. | 3263 |
| `EnhancedAIService.analyzeImageWithIntent` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | imagePath: String<br>userIntent: String? | String | 使用识图模型分析图片 | 3301 |
| `EnhancedAIService.analyzeAudioWithIntent` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | audioPath: String<br>userIntent: String? | String |  | 3305 |
| `EnhancedAIService.analyzeVideoWithIntent` | `EnhancedAIService` | `com.ai.assistance.operit.api.chat` | `EnhancedAIService.kt` | videoPath: String<br>userIntent: String? | String |  | 3309 |
| `ChatMemoryRebuildManager.getInstance` | `ChatMemoryRebuildManager` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildManager.kt` | context: Context | ChatMemoryRebuildManager |  | 38 |
| `ChatMemoryRebuildManager.start` | `ChatMemoryRebuildManager` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildManager.kt` | chatIds: List<String><br>windowMessageCount: Int<br>timeScope: ChatMemoryRebuildTimeScope | Unit |  | 79 |
| `ChatMemoryRebuildManager.cancel` | `ChatMemoryRebuildManager` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildManager.kt` |  | Unit |  | 95 |
| `ChatMemoryRebuildManager.rebuild` | `ChatMemoryRebuildManager` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildManager.kt` | chatIds: List<String><br>windowMessageCount: Int<br>timeScope: ChatMemoryRebuildTimeScope | Unit |  | 99 |
| `ChatMemoryRebuildManager.resolveMemoryProfileId` | `ChatMemoryRebuildManager` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildManager.kt` | history: ChatHistory<br>activeProfileId: String | String |  | 224 |
| `ChatMemoryRebuildTimeScope.EntireChat.contains` | `EntireChat` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildTimeScope.kt` | timestamp: Long | Boolean |  | 21 |
| `ChatMemoryRebuildTimeScope.utcMidnightMillisToLocalDate` | `ChatMemoryRebuildTimeScope` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildTimeScope.kt` | utcMidnightMs: Long | LocalDate |  | 26 |
| `ChatMemoryRebuildTimeScope.inclusiveDates` | `ChatMemoryRebuildTimeScope` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryRebuildTimeScope.kt` | start: LocalDate<br>end: LocalDate<br>zone: ZoneId | InclusiveLocalRange |  | 29 |
| `ChatMemoryWindowPlanner.plan` | `ChatMemoryWindowPlanner` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlanner.kt` | messages: List<ChatMessage><br>windowMessageCount: Int<br>timeScope: ChatMemoryRebuildTimeScope | List<Window> |  | 16 |
| `ChatMemoryWindowPlanner.emitWindow` | `ChatMemoryWindowPlanner` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlanner.kt` |  | Unit |  | 34 |
| `ChatMemoryWindowPlanner.beginWindow` | `ChatMemoryWindowPlanner` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlanner.kt` | contextUser: ChatMessage?? | Unit |  | 44 |
| `MemoryAutoSaveScheduler.getInstance` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` |  | MemoryAutoSaveScheduler? |  | 40 |
| `MemoryAutoSaveScheduler.start` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` |  | Unit |  | 48 |
| `MemoryAutoSaveScheduler.getMinutesUntilNextRun` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` | profileId: String<br>nowMs: Long? | Long |  | 61 |
| `MemoryAutoSaveScheduler.runOnce` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` |  | Unit |  | 70 |
| `MemoryAutoSaveScheduler.scanAndProcessCandidates` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` |  | Unit |  | 82 |
| `MemoryAutoSaveScheduler.intervalMsForProfile` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` | profileId: String | Long |  | 169 |
| `MemoryAutoSaveScheduler.getOrInitNextRunAtMs` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` | profileId: String<br>nowMs: Long? | Long |  | 174 |
| `MemoryAutoSaveScheduler.scheduleNextRun` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` | profileId: String<br>nextRunAtMs: Long | Unit |  | 186 |
| `MemoryAutoSaveScheduler.processChatCandidateGroup` | `MemoryAutoSaveScheduler` | `com.ai.assistance.operit.api.chat.library` | `MemoryAutoSaveScheduler.kt` | profileId: String<br>chatId: String<br>candidates: List<MemoryAutoSaveCandidate><br>repository: MemoryAutoSaveCandidateRepository<br>chatContentDao: com.ai.assistance.operit.data.dao.C…<br>toolHandler: AIToolHandler<br>memoryService: com.a… | Unit |  | 192 |
| `MemoryLibrary.initialize` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context | Unit |  | 87 |
| `MemoryLibrary.autoCategorizeMemoriesAsync` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>aiService: AIService | Unit | 自动为未分类的记忆分配文件夹路径 在后台异步执行，不阻塞主线程 | 101 |
| `MemoryLibrary.saveMemoryAsync` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>toolHandler: AIToolHandler<br>conversationHistory: List<Pair<String, String>><br>content: String<br>aiService: AIService<br>profileIdOverride: String??<br>onSuccess: (suspend () -> Unit)??<br>onError: (suspend (Exceptio… | Unit |  | 113 |
| `MemoryLibrary.saveMemoryNow` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>toolHandler: AIToolHandler<br>conversationHistory: List<Pair<String, String>><br>content: String<br>aiService: AIService<br>profileIdOverride: String?? | Unit |  | 145 |
| `MemoryLibrary.saveMemoryWindowNow` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>toolHandler: AIToolHandler<br>conversationHistory: List<Pair<String, String>><br>content: String<br>aiService: AIService<br>profileIdOverride: String?<br>analysisHistoryLimit: Int | Unit |  | 165 |
| `MemoryLibrary.ensureInitialized` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context | Unit |  | 188 |
| `MemoryLibrary.autoCategorizeMemories` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>aiService: AIService | Unit | 查询未分类记忆并批量调用 AI 进行分类 | 197 |
| `MemoryLibrary.categorizeBatch` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>memories: List<Memory><br>existingFolders: List<String><br>repository: MemoryRepository<br>aiService: AIService | Unit | 使用 AI 为一批记忆分类 | 236 |
| `MemoryLibrary.parseAndApplyCategorization` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | jsonString: String<br>memories: List<Memory><br>repository: MemoryRepository | Unit | 解析 AI 返回的分类结果并更新记忆 | 271 |
| `MemoryLibrary.saveMemory` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>toolHandler: AIToolHandler<br>conversationHistory: List<Pair<String, String>><br>content: String<br>aiService: AIService<br>profileIdOverride: String??<br>analysisHistoryLimit: Int<br>propagateAnalysisFailure: Boolean? | Unit | Analyzes conversation and saves it as a structured Memory graph. | 313 |
| `MemoryLibrary.generateAnalysis` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>aiService: AIService<br>query: String<br>solution: String<br>conversationHistory: List<Pair<String, String>><br>memoryRepository: MemoryRepository<br>profileId: String<br>analysisHistoryLimit: Int<br>propagateFailure: B… | ParsedAnalysis | Generates a structured analysis of the conversation for graph creation. | 556 |
| `MemoryLibrary.buildCandidateSearchQuery` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | query: String<br>solution: String<br>conversationHistory: List<Pair<String, String>> | String |  | 679 |
| `MemoryLibrary.extractCoreQuestionText` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | rawQuery: String | String |  | 702 |
| `MemoryLibrary.normalizeCandidateSearchText` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | raw: String<br>maxLen: Int | String |  | 732 |
| `MemoryLibrary.findAndDescribeDuplicates` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | candidateMemories: List<Memory><br>memoryRepository: MemoryRepository<br>useEnglish: Boolean | String | Finds duplicates within a list of candidate memories and creates a prompt instruction for… | 754 |
| `MemoryLibrary.buildAnalysisMessage` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>query: String<br>solution: String<br>conversationHistory: List<Pair<String, String>><br>useEnglish: Boolean<br>historyLimit: Int | String |  | 778 |
| `MemoryLibrary.parseAnalysisResult` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | jsonString: String | ParsedAnalysis | Parses the object-based memory graph protocol returned by the AI. | 813 |
| `MemoryLibrary.requiredNullableObject` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | key: String | JSONObject? |  | 841 |
| `MemoryLibrary.requiredObjectArray` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | key: String | List<JSONObject> |  | 847 |
| `MemoryLibrary.optionalString` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | key: String | String? |  | 853 |
| `MemoryLibrary.requiredString` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | key: String<br>context: String | String |  | 858 |
| `MemoryLibrary.requiredStringArray` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | key: String<br>context: String | List<String> |  | 862 |
| `MemoryLibrary.optionalUnitFloat` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | key: String<br>context: String | Float? |  | 870 |
| `MemoryLibrary.toParsedEntity` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: String<br>aliasAllowed: Boolean | ParsedEntity |  | 877 |
| `MemoryLibrary.toParsedUpdate` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: String | ParsedUpdate |  | 887 |
| `MemoryLibrary.toParsedMerge` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: String | ParsedMerge |  | 896 |
| `MemoryLibrary.toParsedLink` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: String | ParsedLink |  | 906 |
| `MemoryLibrary.pruneToolResultContent` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | context: Context<br>message: String | String | Replaces the content of <tool_result> tags with a placeholder to reduce token count. | 920 |
| `DeepgramSttProvider.initialize` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` |  | Boolean |  | 97 |
| `DeepgramSttProvider.startRecognition` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | languageCode: String<br>continuousMode: Boolean<br>partialResults: Boolean<br>audioSource: Int | Boolean |  | 128 |
| `DeepgramSttProvider.appendToPreRoll` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | frame: ShortArray<br>size: Int | Unit |  | 210 |
| `DeepgramSttProvider.flushPreRoll` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | streamOut: FileOutputStream | Unit |  | 222 |
| `DeepgramSttProvider.stopRecognition` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` |  | Boolean |  | 308 |
| `DeepgramSttProvider.cancelRecognition` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` |  | Unit |  | 347 |
| `DeepgramSttProvider.shutdown` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` |  | Unit |  | 357 |
| `DeepgramSttProvider.getSupportedLanguages` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` |  | List<String> |  | 375 |
| `DeepgramSttProvider.recognize` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | audioData: FloatArray | Unit |  | 380 |
| `DeepgramSttProvider.stopRecordingInternal` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | deleteFile: Boolean | File? |  | 424 |
| `DeepgramSttProvider.writePcm16le` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | stream: FileOutputStream<br>pcm: ShortArray<br>length: Int<br>offset: Int? | Unit |  | 475 |
| `DeepgramSttProvider.writeWavHeader` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | file: File<br>pcmDataSize: Long | Unit |  | 488 |
| `DeepgramSttProvider.mapLanguage` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | languageCode: String? | String? |  | 534 |
| `DeepgramSttProvider.transcribeWavFile` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | file: File<br>languageCode: String? | String |  | 544 |
| `DeepgramSttProvider.updateVolumeLevel` | `DeepgramSttProvider` | `com.ai.assistance.operit.api.speech` | `DeepgramSttProvider.kt` | buffer: ShortArray<br>length: Int | Unit |  | 588 |
| `OnnxSileroVad.getTensorInfo` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | name: String | TensorInfo? |  | 97 |
| `OnnxSileroVad.normalizeShape` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | shape: LongArray?<br>fallback: LongArray | LongArray |  | 101 |
| `OnnxSileroVad.reset` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` |  | Unit |  | 152 |
| `OnnxSileroVad.setSpeechDurationMs` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | ms: Int | Unit |  | 161 |
| `OnnxSileroVad.setSilenceDurationMs` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | ms: Int | Unit |  | 165 |
| `OnnxSileroVad.isSpeech` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | frame: ShortArray | Boolean |  | 169 |
| `OnnxSileroVad.isContinuousSpeech` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | isSpeechFrame: Boolean | Boolean |  | 195 |
| `OnnxSileroVad.predictProbability` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | audioData: FloatArray | Float |  | 216 |
| `OnnxSileroVad.extractScalarFloat` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | value: Any? | Float |  | 293 |
| `OnnxSileroVad.extractFloatArray` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | value: Any?<br>expectedSize: Int | FloatArray? |  | 301 |
| `OnnxSileroVad.walk` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | v: Any? | Unit |  | 303 |
| `OnnxSileroVad.threshold` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` |  | Float |  | 313 |
| `OnnxSileroVad.msToFrames` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` | ms: Int | Int |  | 322 |
| `OnnxSileroVad.close` | `OnnxSileroVad` | `com.ai.assistance.operit.api.speech` | `OnnxSileroVad.kt` |  | Unit |  | 328 |
| `OpenAISttProvider.initialize` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` |  | Boolean |  | 98 |
| `OpenAISttProvider.startRecognition` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | languageCode: String<br>continuousMode: Boolean<br>partialResults: Boolean<br>audioSource: Int | Boolean |  | 132 |
| `OpenAISttProvider.appendToPreRoll` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | frame: ShortArray<br>size: Int | Unit |  | 214 |
| `OpenAISttProvider.flushPreRoll` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | streamOut: FileOutputStream | Unit |  | 226 |
| `OpenAISttProvider.stopRecognition` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` |  | Boolean |  | 324 |
| `OpenAISttProvider.cancelRecognition` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` |  | Unit |  | 363 |
| `OpenAISttProvider.shutdown` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` |  | Unit |  | 373 |
| `OpenAISttProvider.getSupportedLanguages` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` |  | List<String> |  | 391 |
| `OpenAISttProvider.recognize` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | audioData: FloatArray | Unit |  | 396 |
| `OpenAISttProvider.stopRecordingInternal` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | deleteFile: Boolean | File? |  | 440 |
| `OpenAISttProvider.writePcm16le` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | stream: FileOutputStream<br>pcm: ShortArray<br>length: Int<br>offset: Int? | Unit |  | 491 |
| `OpenAISttProvider.writeWavHeader` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | file: File<br>pcmDataSize: Long | Unit |  | 504 |
| `OpenAISttProvider.mapLanguage` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | languageCode: String? | String? |  | 550 |
| `OpenAISttProvider.transcribeWavFile` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | file: File<br>languageCode: String? | String |  | 560 |
| `OpenAISttProvider.updateVolumeLevel` | `OpenAISttProvider` | `com.ai.assistance.operit.api.speech` | `OpenAISttProvider.kt` | buffer: ShortArray<br>length: Int | Unit |  | 596 |
| `PersonalWakeEnrollment.recordOneTemplate` | `PersonalWakeEnrollment` | `com.ai.assistance.operit.api.speech` | `PersonalWakeEnrollment.kt` | context: Context<br>maxRecordMs: Long?<br>minSpeechMs: Long?<br>endSilenceMs: Long? | FloatArray? |  | 14 |
| `PersonalWakeFeatureExtractor.extractFeatures` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | pcm: ShortArray<br>size: Int<br>config: Config? | FloatArray |  | 29 |
| `PersonalWakeFeatureExtractor.limitFrames` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | frames: List<FloatArray><br>maxFrames: Int | List<FloatArray> |  | 92 |
| `PersonalWakeFeatureExtractor.computeMfcc` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | logMels: List<FloatArray><br>config: Config | Array<FloatArray> |  | 117 |
| `PersonalWakeFeatureExtractor.dctCosTable` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | numMfcc: Int<br>melBins: Int | Array<FloatArray> |  | 135 |
| `PersonalWakeFeatureExtractor.computeDelta` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | x: Array<FloatArray> | Array<FloatArray> |  | 149 |
| `PersonalWakeFeatureExtractor.cmvnInPlace` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | x: Array<FloatArray> | Unit |  | 164 |
| `PersonalWakeFeatureExtractor.cosineSimilarity` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | a: FloatArray<br>b: FloatArray | Float |  | 186 |
| `PersonalWakeFeatureExtractor.normalizePcm` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | pcm: ShortArray<br>size: Int | FloatArray |  | 202 |
| `PersonalWakeFeatureExtractor.trimToMax` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | waveform: FloatArray<br>maxSamples: Int | FloatArray |  | 220 |
| `PersonalWakeFeatureExtractor.frameSignal` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | signal: FloatArray<br>frameSize: Int<br>hopSize: Int | List<FloatArray> |  | 226 |
| `PersonalWakeFeatureExtractor.preEmphasis` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | frame: FloatArray<br>coeff: Float | FloatArray |  | 241 |
| `PersonalWakeFeatureExtractor.applyHann` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | frame: FloatArray | FloatArray |  | 252 |
| `PersonalWakeFeatureExtractor.fftMagSquared` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | frame: FloatArray<br>fftSize: Int | FloatArray |  | 263 |
| `PersonalWakeFeatureExtractor.fftInPlace` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | re: FloatArray<br>im: FloatArray | Unit |  | 282 |
| `PersonalWakeFeatureExtractor.buildMelFilterBank` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | config: Config | MelFilterBank |  | 333 |
| `PersonalWakeFeatureExtractor.hzToMel` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | hz: Float | Float |  | 371 |
| `PersonalWakeFeatureExtractor.melToHz` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | mel: Float | Float |  | 375 |
| `PersonalWakeFeatureExtractor.l2NormalizeInPlace` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | x: FloatArray | Unit |  | 379 |
| `PersonalWakeListener.runLoop` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | config: Config? | Unit |  | 54 |
| `PersonalWakeListener.stop` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` |  | Unit |  | 161 |
| `PersonalWakeListener.flushSegmentIfNeeded` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | config: Config<br>segment: ArrayList<Short><br>speechMs: Long<br>noiseRms: Float | Unit |  | 165 |
| `PersonalWakeListener.meanStd` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | x: List<Float> | Pair<Float, Float> |  | 292 |
| `PersonalWakeListener.resetSegment` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | segment: ArrayList<Short> | Unit |  | 308 |
| `PersonalWakeListener.computeRms` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | pcm: ShortArray | Float |  | 312 |
| `PersonalWakeListener.computeRms` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | pcm: ShortArray<br>len: Int | Float |  | 316 |
| `PersonalWakeListener.reshapeAndNormalizePerFrame` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | flat: FloatArray<br>featureDim: Int | Array<FloatArray> |  | 328 |
| `PersonalWakeListener.dtwSimilarity` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | a: Array<FloatArray><br>b: Array<FloatArray><br>band: Int | Float |  | 344 |
| `PersonalWakeListener.cosineDistance` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | a: FloatArray<br>b: FloatArray | Float |  | 368 |
| `PersonalWakeListener.l2NormalizeInPlace` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | x: FloatArray | Unit |  | 385 |
| `PersonalWakeListener.maybeDebug` | `PersonalWakeListener` | `com.ai.assistance.operit.api.speech` | `PersonalWakeListener.kt` | message: String | Unit |  | 396 |
| `SherpaMnnSpeechProvider.initialize` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` |  | Boolean |  | 72 |
| `SherpaMnnSpeechProvider.createRecognizer` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` |  | Unit |  | 112 |
| `SherpaMnnSpeechProvider.createVad` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` |  | Unit |  | 165 |
| `SherpaMnnSpeechProvider.createSileroVad` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` |  | Unit |  | 223 |
| `SherpaMnnSpeechProvider.detectSpeechBySilero` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` | vad: OnnxSileroVad<br>pending: ShortArray<br>buffer: ShortArray<br>size: Int | Pair<Boolean, ShortArray> |  | 231 |
| `SherpaMnnSpeechProvider.calculateVolumeLevel` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` | buffer: ShortArray<br>size: Int | Float | 计算音频缓冲区的音量级别 | 263 |
| `SherpaMnnSpeechProvider.startRecognition` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` | languageCode: String<br>continuousMode: Boolean<br>partialResults: Boolean<br>audioSource: Int | Boolean |  | 282 |
| `SherpaMnnSpeechProvider.stopRecognition` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` |  | Boolean |  | 500 |
| `SherpaMnnSpeechProvider.cancelRecognition` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` |  | Unit |  | 572 |
| `SherpaMnnSpeechProvider.shutdown` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` |  | Unit |  | 611 |
| `SherpaMnnSpeechProvider.getSupportedLanguages` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` |  | List<String> |  | 646 |
| `SherpaMnnSpeechProvider.recognize` | `SherpaMnnSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaMnnSpeechProvider.kt` | audioData: FloatArray | Unit |  | 651 |
| `SherpaSpeechProvider.clearAndReleaseAudioRecord` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` |  | Unit |  | 47 |
| `SherpaSpeechProvider.initialize` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` |  | Boolean |  | 98 |
| `SherpaSpeechProvider.createRecognizer` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` |  | Unit |  | 129 |
| `SherpaSpeechProvider.calculateVolumeLevel` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` | buffer: ShortArray<br>size: Int | Float | 计算音频缓冲区的音量级别 | 200 |
| `SherpaSpeechProvider.startRecognition` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` | languageCode: String<br>continuousMode: Boolean<br>partialResults: Boolean<br>audioSource: Int | Boolean |  | 225 |
| `SherpaSpeechProvider.stopRecognition` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` |  | Boolean |  | 446 |
| `SherpaSpeechProvider.cancelRecognition` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` |  | Unit |  | 485 |
| `SherpaSpeechProvider.shutdown` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` |  | Unit |  | 507 |
| `SherpaSpeechProvider.getSupportedLanguages` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` |  | List<String> |  | 532 |
| `SherpaSpeechProvider.recognize` | `SherpaSpeechProvider` | `com.ai.assistance.operit.api.speech` | `SherpaSpeechProvider.kt` | audioData: FloatArray | Unit | This method is for non-streaming recognition, which we are not using with sherpa-ncnn's s… | 540 |
| `SpeechPrerollStore.appendPcm` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | pcm: ShortArray<br>length: Int | Unit |  | 32 |
| `SpeechPrerollStore.capturePending` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | windowMs: Int? | Unit |  | 48 |
| `SpeechPrerollStore.consumePending` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | maxAgeMs: Long? | ShortArray? |  | 81 |
| `SpeechPrerollStore.armPending` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` |  | Unit |  | 99 |
| `SpeechPrerollStore.setPendingWakePhrase` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | phrase: String<br>regexEnabled: Boolean | Unit |  | 105 |
| `SpeechPrerollStore.consumePendingWakePhrase` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | maxAgeMs: Long? | WakePhraseSnapshot? |  | 114 |
| `SpeechPrerollStore.clearPendingWakePhrase` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` |  | Unit |  | 132 |
| `SpeechPrerollStore.clear` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` |  | Unit |  | 140 |
| `SpeechService.initialize` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` |  | Boolean | 初始化语音识别引擎 | 66 |
| `SpeechService.startRecognition` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` | languageCode: String?<br>continuousMode: Boolean?<br>partialResults: Boolean?<br>audioSource: Int? | Boolean | 开始语音识别 | 77 |
| `SpeechService.stopRecognition` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` |  | Boolean | 停止语音识别 | 89 |
| `SpeechService.cancelRecognition` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` |  | Unit | 取消语音识别，不会返回任何结果 | 92 |
| `SpeechService.shutdown` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` |  | Unit | 释放语音识别引擎资源 | 95 |
| `SpeechService.getSupportedLanguages` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` |  | List<String> | 获取支持的语言列表 | 102 |
| `SpeechService.recognize` | `SpeechService` | `com.ai.assistance.operit.api.speech` | `SpeechService.kt` | audioData: FloatArray | Unit | 识别预先录制的音频数据 这个方法主要由本地语音识别引擎实现，如WhisperSpeechProvider | 110 |
| `SpeechServiceFactory.createSpeechService` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | context: Context | SpeechService | 创建语音识别服务实例 | 28 |
| `SpeechServiceFactory.createWakeSpeechService` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | context: Context | SpeechService |  | 37 |
| `SpeechServiceFactory.createSpeechService` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | context: Context<br>type: SpeechServiceType | SpeechService |  | 52 |
| `SpeechServiceFactory.createSpeechService` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | context: Context<br>type: SpeechServiceType<br>httpConfig: SttHttpConfig | SpeechService |  | 61 |
| `SpeechServiceFactory.SpeechServiceLease.shutdown` | `SpeechServiceLease` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` |  | Unit |  | 97 |
| `SpeechServiceFactory.acquireLocalSpeechService` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | context: Context<br>type: SpeechServiceType | SpeechService |  | 113 |
| `SpeechServiceFactory.releaseLocalSpeechService` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | type: SpeechServiceType | Unit |  | 147 |
| `SpeechServiceFactory.getInstance` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | context: Context | SpeechService | 获取语音识别服务单例实例 | 181 |
| `SpeechServiceFactory.resetInstance` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` |  | Unit | 重置单例实例 在需要更改语音识别服务类型或释放资源时调用 | 222 |
| `ChatMemoryWindowPlannerTest.plan` | `ChatMemoryWindowPlannerTest` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlannerTest.kt` | messages: List<ChatMessage><br>windowMessageCount: Int<br>timeScope: ChatMemoryRebuildTimeScope? | List<ChatMemoryWindowPlanner.Window> |  | 371 ⚑ |
| `ChatMemoryWindowPlannerTest.message` | `ChatMemoryWindowPlannerTest` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlannerTest.kt` | sender: String<br>content: String<br>timestamp: Long | ChatMessage |  | 378 ⚑ |
| `MemoryAnalysisProtocolTest.disableAndroidSystemLogForJvmTests` | `MemoryAnalysisProtocolTest` | `com.ai.assistance.operit.api.chat.library` | `MemoryAnalysisProtocolTest.kt` |  | Unit |  | 16 ⚑ |
| `MemoryAnalysisProtocolTest.restoreAndroidSystemLog` | `MemoryAnalysisProtocolTest` | `com.ai.assistance.operit.api.chat.library` | `MemoryAnalysisProtocolTest.kt` |  | Unit |  | 22 ⚑ |
| `MemoryAnalysisProtocolTest.parseAnalysisResult_acceptsObjectProtocolWithoutMainEvent` | `MemoryAnalysisProtocolTest` | `com.ai.assistance.operit.api.chat.library` | `MemoryAnalysisProtocolTest.kt` |  | Unit |  | 27 ⚑ |
| `MemoryAnalysisProtocolTest.parseAnalysisResult_rejectsLegacyPositionalArrayProtocol` | `MemoryAnalysisProtocolTest` | `com.ai.assistance.operit.api.chat.library` | `MemoryAnalysisProtocolTest.kt` |  | Unit |  | 74 ⚑ |
| `MemoryAnalysisProtocolTest.parseAnalysisResult_rejectsMissingRequiredOperationField` | `MemoryAnalysisProtocolTest` | `com.ai.assistance.operit.api.chat.library` | `MemoryAnalysisProtocolTest.kt` |  | Unit |  | 91 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ChatMemoryWindowPlanner.DEFAULT_WINDOW_MESSAGE_COUNT` | `ChatMemoryWindowPlanner` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlanner.kt` | inferred |  | 7 |
| `ChatMemoryWindowPlanner.MAX_WINDOW_MESSAGE_COUNT` | `ChatMemoryWindowPlanner` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlanner.kt` | inferred |  | 9 |
| `ChatMemoryWindowPlanner.MIN_WINDOW_MESSAGE_COUNT` | `ChatMemoryWindowPlanner` | `com.ai.assistance.operit.api.chat.library` | `ChatMemoryWindowPlanner.kt` | inferred |  | 8 |
| `MemoryLibrary.apiPreferences` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | ApiPreferences? |  | 39 |
| `MemoryLibrary.coroutineScope` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | inferred |  | 38 |
| `MemoryLibrary.DEFAULT_ANALYSIS_HISTORY_MESSAGE_COUNT` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | inferred |  | 37 |
| `MemoryLibrary.mutex` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | inferred |  | 40 |
| `MemoryLibrary.TAG` | `MemoryLibrary` | `com.ai.assistance.operit.api.chat.library` | `MemoryLibrary.kt` | inferred |  | 36 |
| `PersonalWakeFeatureExtractor.EPS` | `PersonalWakeFeatureExtractor` | `com.ai.assistance.operit.api.speech` | `PersonalWakeFeatureExtractor.kt` | inferred |  | 11 |
| `SpeechPrerollStore.CAPACITY_MS` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | inferred |  | 14 |
| `SpeechPrerollStore.capacitySamples` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | Int |  | 18 |
| `SpeechPrerollStore.filled` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | Int |  | 22 |
| `SpeechPrerollStore.lock` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | inferred |  | 16 |
| `SpeechPrerollStore.pending` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | ShortArray? |  | 24 |
| `SpeechPrerollStore.pendingArmed` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | Boolean |  | 26 |
| `SpeechPrerollStore.pendingCapturedAtMs` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | Long |  | 25 |
| `SpeechPrerollStore.pendingWakePhrase` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | String? |  | 28 |
| `SpeechPrerollStore.pendingWakePhraseAtMs` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | Long |  | 30 |
| `SpeechPrerollStore.pendingWakePhraseRegexEnabled` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | Boolean |  | 29 |
| `SpeechPrerollStore.ring` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | ShortArray |  | 19 |
| `SpeechPrerollStore.SAMPLE_RATE` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | inferred |  | 13 |
| `SpeechPrerollStore.TAG` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | inferred |  | 11 |
| `SpeechPrerollStore.writePos` | `SpeechPrerollStore` | `com.ai.assistance.operit.api.speech` | `SpeechPrerollStore.kt` | Int |  | 21 |
| `SpeechServiceFactory.currentProfileId` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | String? |  | 173 |
| `SpeechServiceFactory.instance` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | SpeechService? | 单例实例缓存 | 172 |
| `SpeechServiceFactory.localEntry` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | LocalEntry? |  | 111 |
| `SpeechServiceFactory.localLock` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | inferred |  | 110 |
| `SpeechServiceFactory.TAG` | `SpeechServiceFactory` | `com.ai.assistance.operit.api.speech` | `SpeechServiceFactory.kt` | inferred |  | 12 |
