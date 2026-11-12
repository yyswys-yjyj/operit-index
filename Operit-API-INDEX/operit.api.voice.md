# operit.api.voice

> 函数 239 · 类型 34 · 顶层常量 4 · 共 277 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `DoubaoVoiceProvider` | `DoubaoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `DoubaoVoiceProvider.kt` | class DoubaoVoiceProvider(context: Context, private val config: SpeechServicesPreferences.Tts…) : HttpVoiceProvider |  | 6 |
| `HttpTtsResponsePipelineStep` | `HttpTtsResponsePipelineStep` | `com.ai.assistance.operit.api.voice` | `HttpTtsResponsePipelineStep.kt` | class HttpTtsResponsePipelineStep(val type: String, val path: String, val headers: Map<String, String>) |  | 9 |
| `HttpVoiceProvider` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | class HttpVoiceProvider(private val context: Context) : VoiceService | 基于HTTP请求的TTS语音服务实现 此实现通过HTTP请求获取TTS音频数据，支持配置不同的TTS服务端点 | 46 |
| `HttpVoiceProvider.BinaryPayload` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | class BinaryPayload(val bytes: ByteArray, val contentType: String?, val charset: Charset) |  | 98 |
| `HttpVoiceProvider.PipelineValue` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | interface PipelineValue |  | 104 |
| `HttpVoiceProvider.PipelineValue.Binary` | `PipelineValue` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | class Binary(val payload: BinaryPayload) : PipelineValue data class Text |  | 105 |
| `HttpVoiceProvider.PipelineValue.JsonPathToken` | `PipelineValue` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | interface JsonPathToken |  | 110 |
| `HttpVoiceProvider.PipelineValue.JsonPathToken.Key` | `JsonPathToken` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | class Key(val name: String) : JsonPathToken data class Index |  | 111 |
| `MimoVoiceProvider` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` | class MimoVoiceProvider(private val context: Context, private val config: SpeechServicesPreferences.Tts…) : VoiceService |  | 8 |
| `MiniMaxVoiceProvider` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` | class MiniMaxVoiceProvider(private val context: Context, private val config: SpeechServicesPreferences.Tts…) : VoiceService |  | 8 |
| `OpenAIRealtimeVoiceProvider` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | class OpenAIRealtimeVoiceProvider(private val context: Context, private val endpointUrl: String, private val apiKey: String, private val model: String, initialVoiceId: String) : VoiceService |  | 33 |
| `OpenAIVoiceProvider` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` | class OpenAIVoiceProvider(private val context: Context, private val endpointUrl: String, private val apiKey: String, private val model: String, initialVoiceId: String) : VoiceService |  | 31 |
| `OpenAIVoiceProvider.OpenAiSpeechRequest` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` | class OpenAiSpeechRequest(val model: String, val input: String, val voice: String, val response_format: String?, val speed: Double?) |  | 54 |
| `QueuedTtsPlayback` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` | class QueuedTtsPlayback(private val tag: String, private val prepareAudioFile: suspend (Request) -> File?) : suspend |  | 23 |
| `QueuedTtsPlayback.PreparedRequest` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` | class PreparedRequest(val request: Request, val audioFile: File) |  | 36 |
| `QueuedTtsPlayback.Request` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` | class Request(val text: String, val rate: Float?, val pitch: Float?, val extraParams: Map<String, String>, val generation: Long, val completion: CompletableDeferred<Boolean… |  | 27 |
| `SiliconFlowVoiceProvider` | `SiliconFlowVoiceProvider` | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | class SiliconFlowVoiceProvider(private val context: Context, private val apiKey: String, initialVoiceId: String, private val initialModelName: String) : VoiceService | 硅基流动TTS语音服务实现 | 35 |
| `SiliconFlowVoiceProvider.PreparedRequest` | `SiliconFlowVoiceProvider` | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | class PreparedRequest(val request: SpeakRequest, val audioFile: File) |  | 106 |
| `SiliconFlowVoiceProvider.SpeakRequest` | `SiliconFlowVoiceProvider` | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | class SpeakRequest(val text: String, val interrupt: Boolean, val rate: Float?, val pitch: Float?, val extraParams: Map<String, String>, val generation: Long, val completion: Com… |  | 96 |
| `SimpleVoiceProvider` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | class SimpleVoiceProvider(private val context: Context, initialLocaleTag: String, initialVoiceId: String) : VoiceService | 基于Android系统TextToSpeech API的语音服务实现 此实现利用Android的TextToSpeech API进行文本转语音 | 27 |
| `SimpleVoiceProvider.PendingUtterance` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | class PendingUtterance(val utteranceId: String, val text: String) |  | 41 |
| `TtsException` | `TtsException` | `com.ai.assistance.operit.api.voice` | `TtsException.kt` | class TtsException(message: String, val httpStatusCode: Int?, val errorBody: String?, cause: Throwable?) : Exception | TTS服务相关的自定义异常 | 10 |
| `VitsVoiceProvider` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | class VitsVoiceProvider(private val context: Context, private val config: SpeechServicesPreferences.Vit…) : VoiceService |  | 47 |
| `VitsVoiceProvider.InputBindings` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | class InputBindings(val idsInputName: String, val lengthInputName: String?, val scalesInputName: String?, val sidInputName: String?) |  | 81 |
| `VitsVoiceProvider.PackageFiles` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | class PackageFiles(val root: File, val modelFile: File, val configFile: File, val lexiconFile: File?) |  | 74 |
| `VitsVoiceProvider.PackageLexicon` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | class PackageLexicon(private val entries: Map<String, LongArray>, private val tokenMap: Map<String, List<Long>>) |  | 103 |
| `VitsVoiceProvider.PreparedSpeech` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | class PreparedSpeech(val request: SpeakRequest, val pcm: ShortArray, val sampleRate: Int) |  | 97 |
| `VitsVoiceProvider.RuntimeConfig` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | class RuntimeConfig(val sampleRate: Int, val tokenMap: Map<String, List<Long>>, val lexicon: PackageLexicon?, val frontend: String, val addBlank: Boolean, val blankId: Long?, val… |  | 59 |
| `VitsVoiceProvider.SpeakRequest` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | class SpeakRequest(val text: String, val rate: Float?, val pitch: Float?, val extraParams: Map<String, String>, val generation: Long, val completion: CompletableDeferred<Boolean… |  | 88 |
| `VoiceListFetcher` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | object VoiceListFetcher |  | 13 |
| `VoiceService` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` | interface VoiceService | 语音服务接口，定义与不同语音引擎进行交互的标准方法 | 6 |
| `VoiceService.Voice` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` | class Voice(val id: String, val name: String, val locale: String, val gender: String) | 表示TTS语音的数据类 | 88 |
| `VoiceServiceFactory` | `VoiceServiceFactory` | `com.ai.assistance.operit.api.voice` | `VoiceServiceFactory.kt` | object VoiceServiceFactory | 语音服务工厂，用于创建不同类型的语音服务实例 | 8 |
| `VoiceServiceFactory.VoiceServiceType` | `VoiceServiceFactory` | `com.ai.assistance.operit.api.voice` | `VoiceServiceFactory.kt` | class VoiceServiceType | 语音服务类型枚举 | 10 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `SimpleVoiceProvider.speechPreview` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | text: String | String |  | 37 |
| `SimpleVoiceProvider.logQueueState` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | event: String<br>extra: String? | Unit |  | 76 |
| `SimpleVoiceProvider.updateSpeakingStateLocked` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | event: String | Unit |  | 84 |
| `SimpleVoiceProvider.removeQueuedUtteranceLocked` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | utteranceId: String | PendingUtterance? |  | 89 |
| `SimpleVoiceProvider.buildPausedSegmentsLocked` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` |  | List<String> |  | 101 |
| `SimpleVoiceProvider.submitUtterance` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | textToSpeech: TextToSpeech<br>entry: PendingUtterance<br>queueMode: Int | Boolean |  | 130 |
| `SimpleVoiceProvider.initialize` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` |  | Boolean | 初始化TTS引擎 | 149 |
| `SimpleVoiceProvider.onStart` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | utteranceId: String | Unit |  | 169 |
| `SimpleVoiceProvider.onDone` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | utteranceId: String | Unit |  | 193 |
| `SimpleVoiceProvider.onError` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | utteranceId: String | Unit |  | 211 |
| `SimpleVoiceProvider.onError` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | utteranceId: String<br>errorCode: Int | Unit |  | 227 |
| `SimpleVoiceProvider.onRangeStart` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | utteranceId: String<br>start: Int<br>end: Int<br>frame: Int | Unit |  | 247 |
| `SimpleVoiceProvider.speak` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean | 将文本转换为语音并播放 | 293 |
| `SimpleVoiceProvider.stop` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` |  | Boolean | 停止当前正在播放的语音 | 396 |
| `SimpleVoiceProvider.pause` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` |  | Boolean | 暂停当前正在播放的语音 | 423 |
| `SimpleVoiceProvider.resume` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` |  | Boolean | 继续播放暂停的语音 | 476 |
| `SimpleVoiceProvider.shutdown` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` |  | Unit | 释放TTS引擎资源 | 555 |
| `SimpleVoiceProvider.getAvailableVoices` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` |  | List<VoiceService.Voice> | 获取可用的语音列表 | 580 |
| `SimpleVoiceProvider.setVoice` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | voiceId: String | Boolean | 设置当前使用的语音 | 622 |
| `SimpleVoiceProvider.ensureVoiceAndLocaleReady` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | textToSpeech: TextToSpeech | Unit |  | 656 |
| `SimpleVoiceProvider.resolveBestLocale` | `SimpleVoiceProvider` | `com.ai.assistance.operit.api.voice` | `AccessibilityVoiceProvider.kt` | textToSpeech: TextToSpeech<br>requestedTag: String | Locale? |  | 687 |
| `DoubaoVoiceProvider.initialize` | `DoubaoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `DoubaoVoiceProvider.kt` |  | Boolean |  | 39 |
| `DoubaoVoiceProvider.speak` | `DoubaoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `DoubaoVoiceProvider.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean |  | 44 |
| `DoubaoVoiceProvider.getAvailableVoices` | `DoubaoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `DoubaoVoiceProvider.kt` |  | List<VoiceService.Voice> |  | 63 |
| `DoubaoVoiceProvider.setVoice` | `DoubaoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `DoubaoVoiceProvider.kt` | voiceId: String | Boolean |  | 65 |
| `DoubaoVoiceProvider.buildHttpConfig` | `DoubaoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `DoubaoVoiceProvider.kt` |  | SpeechServicesPreferences.TtsHttpConfig |  | 70 |
| `HttpTtsResponsePipelineStep.parseList` | `HttpTtsResponsePipelineStep` | `com.ai.assistance.operit.api.voice` | `HttpTtsResponsePipelineStep.kt` | raw: String | List<HttpTtsResponsePipelineStep> |  | 41 |
| `HttpTtsResponsePipelineStep.encodeList` | `HttpTtsResponsePipelineStep` | `com.ai.assistance.operit.api.voice` | `HttpTtsResponsePipelineStep.kt` | steps: List<HttpTtsResponsePipelineStep> | String |  | 47 |
| `HttpVoiceProvider.speechPreview` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | text: String | String |  | 58 |
| `HttpVoiceProvider.setConfiguration` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | config: SpeechServicesPreferences.TtsHttpCo… | Unit | 设置HTTP TTS服务的配置 | 124 |
| `HttpVoiceProvider.initialize` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` |  | Boolean | 初始化TTS引擎 | 135 |
| `HttpVoiceProvider.speak` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean | 将文本转换为语音并播放 | 188 |
| `HttpVoiceProvider.fetchAudioFile` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | request: QueuedTtsPlayback.Request | File? |  | 208 |
| `HttpVoiceProvider.stop` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` |  | Boolean | 停止当前正在播放的语音 | 264 |
| `HttpVoiceProvider.pause` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` |  | Boolean | 暂停当前正在播放的语音 | 270 |
| `HttpVoiceProvider.resume` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` |  | Boolean | 继续播放暂停的语音 | 276 |
| `HttpVoiceProvider.shutdown` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` |  | Unit | 释放TTS引擎资源 | 282 |
| `HttpVoiceProvider.getAvailableVoices` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` |  | List<VoiceService.Voice> | 获取可用的语音列表 | 293 |
| `HttpVoiceProvider.setVoice` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | voiceId: String | Boolean | 设置当前使用的语音 | 299 |
| `HttpVoiceProvider.fetchAudioFromServer` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | text: String<br>rate: Float<br>pitch: Float<br>voiceId: String?<br>extraParams: Map<String, String> | File? | 从服务器获取音频数据 | 313 |
| `HttpVoiceProvider.replaceBodyPlaceholders` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | template: String<br>replacements: Map<String, String><br>contentType: String | String |  | 444 |
| `HttpVoiceProvider.replacePlainPlaceholders` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | template: String<br>replacements: Map<String, String> | String |  | 465 |
| `HttpVoiceProvider.replacePlaceholders` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | template: String<br>replacements: Map<String, String><br>transform: (rawValue: String, matchRange: IntR… | String |  | 472 |
| `HttpVoiceProvider.encodeJsonPlaceholderValue` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | template: String<br>matchRange: IntRange<br>rawValue: String | String |  | 489 |
| `HttpVoiceProvider.isWrappedInJsonQuotes` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | template: String<br>matchRange: IntRange | Boolean |  | 503 |
| `HttpVoiceProvider.toJsonLiteralOrNull` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` |  | String? |  | 512 |
| `HttpVoiceProvider.isJsonContentType` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | contentType: String | Boolean |  | 525 |
| `HttpVoiceProvider.isFormUrlEncodedContentType` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | contentType: String | Boolean |  | 530 |
| `HttpVoiceProvider.validateResponsePipeline` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | steps: List<HttpTtsResponsePipelineStep> | Unit |  | 535 |
| `HttpVoiceProvider.executeRequest` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | request: Request | Response |  | 563 |
| `HttpVoiceProvider.onFailure` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | call: Call<br>e: IOException | Unit |  | 566 |
| `HttpVoiceProvider.onResponse` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | call: Call<br>response: Response | Unit |  | 570 |
| `HttpVoiceProvider.executeBinaryRequest` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | request: Request<br>requestLabel: String | BinaryPayload |  | 576 |
| `HttpVoiceProvider.resolvePipelineAudio` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | initialPayload: BinaryPayload<br>steps: List<HttpTtsResponsePipelineStep> | BinaryPayload |  | 604 |
| `HttpVoiceProvider.parseJsonPayload` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | current: PipelineValue<br>stepIndex: Int | JsonElement |  | 655 |
| `HttpVoiceProvider.pickJsonValue` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | current: PipelineValue<br>path: String<br>stepIndex: Int | JsonElement |  | 682 |
| `HttpVoiceProvider.parseJsonStringValue` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | current: PipelineValue<br>stepIndex: Int | JsonElement |  | 701 |
| `HttpVoiceProvider.followHttpUrl` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | current: PipelineValue<br>step: HttpTtsResponsePipelineStep<br>stepIndex: Int | BinaryPayload |  | 715 |
| `HttpVoiceProvider.followHttpRequestObject` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | current: PipelineValue<br>stepIndex: Int | BinaryPayload |  | 741 |
| `HttpVoiceProvider.decodeBase64Value` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | current: PipelineValue<br>stepIndex: Int | BinaryPayload |  | 820 |
| `HttpVoiceProvider.asScalarString` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | stepIndex: Int<br>stepType: String | String |  | 839 |
| `HttpVoiceProvider.readJsonPath` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | root: JsonElement<br>rawPath: String<br>stepIndex: Int | JsonElement |  | 876 |
| `HttpVoiceProvider.buildJsonPathReadException` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | root: JsonElement<br>rawPath: String<br>stepIndex: Int | TtsException |  | 904 |
| `HttpVoiceProvider.parseJsonPath` | `HttpVoiceProvider` | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | rawPath: String | List<JsonPathToken> |  | 921 |
| `generateCacheKey` | — | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` | text: String<br>rate: Float<br>pitch: Float<br>voiceId: String?<br>extraParams: Map<String, String> | String | 生成缓存键 | 968 |
| `clearCache` | — | `com.ai.assistance.operit.api.voice` | `HttpVoiceProvider.kt` |  | Unit | 清除缓存文件 | 982 |
| `MimoVoiceProvider.initialize` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` |  | Boolean |  | 59 |
| `MimoVoiceProvider.speak` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean |  | 68 |
| `MimoVoiceProvider.stop` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` |  | Boolean |  | 101 |
| `MimoVoiceProvider.pause` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` |  | Boolean |  | 103 |
| `MimoVoiceProvider.resume` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` |  | Boolean |  | 105 |
| `MimoVoiceProvider.shutdown` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` |  | Unit |  | 107 |
| `MimoVoiceProvider.getAvailableVoices` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` |  | List<VoiceService.Voice> |  | 111 |
| `MimoVoiceProvider.setVoice` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` | voiceId: String | Boolean |  | 113 |
| `MimoVoiceProvider.buildHttpConfig` | `MimoVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MimoVoiceProvider.kt` |  | SpeechServicesPreferences.TtsHttpConfig |  | 118 |
| `MiniMaxVoiceProvider.initialize` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` |  | Boolean |  | 51 |
| `MiniMaxVoiceProvider.speak` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean |  | 60 |
| `MiniMaxVoiceProvider.stop` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` |  | Boolean |  | 93 |
| `MiniMaxVoiceProvider.pause` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` |  | Boolean |  | 95 |
| `MiniMaxVoiceProvider.resume` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` |  | Boolean |  | 97 |
| `MiniMaxVoiceProvider.shutdown` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` |  | Unit |  | 99 |
| `MiniMaxVoiceProvider.getAvailableVoices` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` |  | List<VoiceService.Voice> |  | 103 |
| `MiniMaxVoiceProvider.setVoice` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` | voiceId: String | Boolean |  | 105 |
| `MiniMaxVoiceProvider.buildHttpConfig` | `MiniMaxVoiceProvider` | `com.ai.assistance.operit.api.voice` | `MiniMaxVoiceProvider.kt` |  | SpeechServicesPreferences.TtsHttpConfig |  | 110 |
| `OpenAIRealtimeVoiceProvider.initialize` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` |  | Boolean |  | 92 |
| `OpenAIRealtimeVoiceProvider.speak` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean |  | 120 |
| `OpenAIRealtimeVoiceProvider.requestAudio` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | text: String<br>requestModel: String<br>requestVoice: String<br>speed: Float | ByteArray |  | 169 |
| `OpenAIRealtimeVoiceProvider.onOpen` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | webSocket: WebSocket<br>response: Response | Unit |  | 184 |
| `OpenAIRealtimeVoiceProvider.onMessage` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | webSocket: WebSocket<br>text: String | Unit |  | 201 |
| `OpenAIRealtimeVoiceProvider.onFailure` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | webSocket: WebSocket<br>t: Throwable<br>response: Response? | Unit |  | 253 |
| `OpenAIRealtimeVoiceProvider.onClosed` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | webSocket: WebSocket<br>code: Int<br>reason: String | Unit |  | 283 |
| `OpenAIRealtimeVoiceProvider.completeAudioResponse` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | deferred: CompletableDeferred<ByteArray><br>audioBuffer: ByteArrayOutputStream | Unit |  | 323 |
| `OpenAIRealtimeVoiceProvider.failResponse` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | deferred: CompletableDeferred<ByteArray><br>message: String | Unit |  | 338 |
| `OpenAIRealtimeVoiceProvider.buildRealtimeUrl` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | baseUrl: String<br>model: String | String |  | 347 |
| `OpenAIRealtimeVoiceProvider.buildConversationItemCreateEvent` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | text: String | JSONObject |  | 362 |
| `OpenAIRealtimeVoiceProvider.buildResponseCreateEvent` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | voice: String<br>speed: Float | JSONObject |  | 384 |
| `OpenAIRealtimeVoiceProvider.buildVoiceValue` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | voice: String | Any |  | 409 |
| `OpenAIRealtimeVoiceProvider.wrapPcm16AsWav` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | pcmData: ByteArray | ByteArray |  | 417 |
| `OpenAIRealtimeVoiceProvider.writeIntLE` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | output: ByteArrayOutputStream<br>value: Int | Unit |  | 442 |
| `OpenAIRealtimeVoiceProvider.writeShortLE` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | output: ByteArrayOutputStream<br>value: Int | Unit |  | 449 |
| `OpenAIRealtimeVoiceProvider.playAudioFileAndAwait` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | file: File | Boolean |  | 454 |
| `OpenAIRealtimeVoiceProvider.finishPlayback` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | success: Boolean<br>done: CompletableDeferred<Boolean><br>file: File | Unit |  | 507 |
| `OpenAIRealtimeVoiceProvider.stop` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` |  | Boolean |  | 536 |
| `OpenAIRealtimeVoiceProvider.pause` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` |  | Boolean |  | 580 |
| `OpenAIRealtimeVoiceProvider.resume` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` |  | Boolean |  | 593 |
| `OpenAIRealtimeVoiceProvider.shutdown` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` |  | Unit |  | 606 |
| `OpenAIRealtimeVoiceProvider.getAvailableVoices` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` |  | List<VoiceService.Voice> |  | 636 |
| `OpenAIRealtimeVoiceProvider.setVoice` | `OpenAIRealtimeVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIRealtimeVoiceProvider.kt` | voiceId: String | Boolean |  | 640 |
| `OpenAIVoiceProvider.initialize` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` |  | Boolean |  | 89 |
| `OpenAIVoiceProvider.speak` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean |  | 120 |
| `OpenAIVoiceProvider.playAudioFileAndAwait` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` | file: File | Boolean |  | 203 |
| `OpenAIVoiceProvider.finishPlayback` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` | success: Boolean<br>done: CompletableDeferred<Boolean><br>file: File | Unit |  | 256 |
| `OpenAIVoiceProvider.stop` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` |  | Boolean |  | 290 |
| `OpenAIVoiceProvider.pause` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` |  | Boolean |  | 319 |
| `OpenAIVoiceProvider.resume` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` |  | Boolean |  | 332 |
| `OpenAIVoiceProvider.shutdown` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` |  | Unit |  | 345 |
| `OpenAIVoiceProvider.getAvailableVoices` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` |  | List<VoiceService.Voice> |  | 356 |
| `OpenAIVoiceProvider.setVoice` | `OpenAIVoiceProvider` | `com.ai.assistance.operit.api.voice` | `OpenAIVoiceProvider.kt` | voiceId: String | Boolean |  | 360 |
| `QueuedTtsPlayback.speak` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean |  | 81 |
| `QueuedTtsPlayback.stop` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` |  | Boolean |  | 105 |
| `QueuedTtsPlayback.pause` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` |  | Boolean |  | 113 |
| `QueuedTtsPlayback.resume` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` |  | Boolean |  | 130 |
| `QueuedTtsPlayback.shutdown` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` |  | Unit |  | 147 |
| `QueuedTtsPlayback.isCurrent` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` | request: Request | Boolean |  | 164 |
| `QueuedTtsPlayback.clearPendingRequests` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` |  | Unit |  | 168 |
| `QueuedTtsPlayback.clearPendingPlayback` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` |  | Unit |  | 175 |
| `QueuedTtsPlayback.clearForInterrupt` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` |  | Unit |  | 182 |
| `QueuedTtsPlayback.stopPlaybackOnly` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` |  | Boolean |  | 190 |
| `QueuedTtsPlayback.playPreparedRequest` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` | prepared: PreparedRequest | Boolean |  | 207 |
| `QueuedTtsPlayback.playAudioFile` | `QueuedTtsPlayback` | `com.ai.assistance.operit.api.voice` | `QueuedTtsPlayback.kt` | audioFile: File | Unit |  | 215 |
| `SiliconFlowVoiceProvider.getAvailableVoices` | `SiliconFlowVoiceProvider` | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | context: Context | List<VoiceService.Voice> | 可用音色列表 - 根据硅基流动官方文档 注意：现在只列出音色名称，模型在设置中独立配置 | 52 |
| `SiliconFlowVoiceProvider.speechPreview` | `SiliconFlowVoiceProvider` | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | text: String | String |  | 65 |
| `SiliconFlowVoiceProvider.initialize` | `SiliconFlowVoiceProvider` | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` |  | Boolean |  | 139 |
| `SiliconFlowVoiceProvider.speak` | `SiliconFlowVoiceProvider` | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean |  | 159 |
| `SiliconFlowVoiceProvider.fetchAudioFile` | `SiliconFlowVoiceProvider` | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | request: SpeakRequest | PreparedRequest? |  | 184 |
| `playPreparedRequest` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | prepared: PreparedRequest | Boolean |  | 317 |
| `clearPendingRequests` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` |  | Unit |  | 326 |
| `clearPendingPlayback` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` |  | Unit |  | 333 |
| `stopPlaybackOnly` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` |  | Boolean |  | 341 |
| `playAudioFileAndAwait` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | file: File | Boolean |  | 363 |
| `stop` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` |  | Boolean |  | 420 |
| `pause` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` |  | Boolean |  | 431 |
| `resume` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` |  | Boolean |  | 445 |
| `shutdown` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` |  | Unit |  | 459 |
| `getAvailableVoices` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` |  | List<VoiceService.Voice> |  | 470 |
| `setVoice` | — | `com.ai.assistance.operit.api.voice` | `SiliconFlowVoiceProvider.kt` | voiceId: String | Boolean |  | 474 |
| `VitsVoiceProvider.PackageLexicon.tokenize` | `PackageLexicon` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | text: String | LongArray |  | 109 |
| `VitsVoiceProvider.PackageLexicon.longestEntryAt` | `PackageLexicon` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | text: String<br>start: Int | Pair<String, LongArray>? |  | 153 |
| `VitsVoiceProvider.PackageLexicon.isAsciiWordChar` | `PackageLexicon` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | codePoint: Int | Boolean |  | 173 |
| `VitsVoiceProvider.initialize` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | Boolean |  | 251 |
| `VitsVoiceProvider.speak` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | text: String<br>interrupt: Boolean<br>rate: Float?<br>pitch: Float?<br>extraParams: Map<String, String> | Boolean |  | 295 |
| `VitsVoiceProvider.prepareSpeech` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | request: SpeakRequest | PreparedSpeech? |  | 319 |
| `VitsVoiceProvider.runModel` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | activeSession: OrtSession<br>activeConfig: RuntimeConfig<br>bindings: InputBindings<br>ids: LongArray<br>effectiveRate: Float | ShortArray |  | 365 |
| `VitsVoiceProvider.playPcm16` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | pcm: ShortArray<br>sampleRate: Int<br>generation: Long | Boolean |  | 434 |
| `VitsVoiceProvider.clearPendingRequests` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | Unit |  | 526 |
| `VitsVoiceProvider.clearPendingPlayback` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | Unit |  | 533 |
| `VitsVoiceProvider.clearForInterrupt` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | Unit |  | 540 |
| `VitsVoiceProvider.stopPlaybackOnly` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | Boolean |  | 547 |
| `VitsVoiceProvider.stop` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | Boolean |  | 574 |
| `VitsVoiceProvider.pause` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | Boolean |  | 582 |
| `VitsVoiceProvider.resume` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | Boolean |  | 597 |
| `VitsVoiceProvider.shutdown` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | Unit |  | 612 |
| `VitsVoiceProvider.getAvailableVoices` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` |  | List<VoiceService.Voice> |  | 640 |
| `VitsVoiceProvider.setVoice` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | voiceId: String | Boolean |  | 648 |
| `VitsVoiceProvider.resolvePackageRoot` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | raw: String | File |  | 653 |
| `VitsVoiceProvider.extractZipPackage` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | zipFile: File | File |  | 672 |
| `VitsVoiceProvider.resolvePackageFiles` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | root: File | PackageFiles |  | 726 |
| `VitsVoiceProvider.parseRuntimeConfig` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | packageFiles: PackageFiles | RuntimeConfig |  | 759 |
| `VitsVoiceProvider.tokenize` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | text: String<br>activeConfig: RuntimeConfig<br>extraParams: Map<String, String> | LongArray |  | 816 |
| `VitsVoiceProvider.loadLexicon` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | file: File<br>tokenMap: Map<String, List<Long>> | PackageLexicon |  | 869 |
| `VitsVoiceProvider.resolveInputBindings` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | activeSession: OrtSession | InputBindings |  | 899 |
| `VitsVoiceProvider.resolveInputName` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | inputNames: Set<String><br>explicitOptionKeys: List<String><br>candidates: List<String><br>requiredLabel: String | String |  | 931 |
| `VitsVoiceProvider.resolveOptionalInputName` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | inputNames: Set<String><br>explicitOptionKeys: List<String><br>candidates: List<String> | String? |  | 956 |
| `VitsVoiceProvider.tensorInfo` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | activeSession: OrtSession<br>name: String | TensorInfo |  | 972 |
| `VitsVoiceProvider.createIntegerTensor` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | name: String<br>values: LongArray<br>shape: LongArray<br>info: TensorInfo | OnnxTensor |  | 977 |
| `VitsVoiceProvider.createFloatTensor` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | name: String<br>values: FloatArray<br>shape: LongArray<br>info: TensorInfo | OnnxTensor |  | 1001 |
| `VitsVoiceProvider.shapeForValues` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | info: TensorInfo<br>valueCount: Int<br>inputName: String | LongArray |  | 1019 |
| `VitsVoiceProvider.extractPcm16` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | value: Any? | ShortArray |  | 1056 |
| `VitsVoiceProvider.floatsToPcm16` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | samples: FloatArray | ShortArray |  | 1075 |
| `VitsVoiceProvider.doublesToPcm16` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | samples: DoubleArray | ShortArray |  | 1083 |
| `VitsVoiceProvider.flattenFloats` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | value: Any? | FloatArray |  | 1091 |
| `VitsVoiceProvider.walk` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | v: Any? | Unit |  | 1093 |
| `VitsVoiceProvider.flattenDoubles` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | value: Any? | DoubleArray |  | 1103 |
| `VitsVoiceProvider.walk` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | v: Any? | Unit |  | 1105 |
| `VitsVoiceProvider.flattenShorts` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | value: Any? | ShortArray |  | 1115 |
| `VitsVoiceProvider.walk` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | v: Any? | Unit |  | 1117 |
| `VitsVoiceProvider.flattenInts` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | value: Any? | IntArray |  | 1127 |
| `VitsVoiceProvider.walk` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | v: Any? | Unit |  | 1129 |
| `VitsVoiceProvider.flattenBytes` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | value: Any? | ByteArray |  | 1140 |
| `VitsVoiceProvider.walk` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | v: Any? | Unit |  | 1142 |
| `VitsVoiceProvider.firstTokenMapObject` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | root: JSONObject | Pair<String, JSONObject>? |  | 1152 |
| `VitsVoiceProvider.firstTokenArray` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | root: JSONObject | JSONArray? |  | 1160 |
| `VitsVoiceProvider.parseTokenMap` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | obj: JSONObject | Map<String, List<Long>> |  | 1166 |
| `VitsVoiceProvider.parseTokenArray` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | arr: JSONArray | Map<String, List<Long>> |  | 1182 |
| `VitsVoiceProvider.readFirstTokenId` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | obj: JSONObject<br>key: String | Long? |  | 1193 |
| `VitsVoiceProvider.readTokenIds` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | obj: JSONObject<br>key: String | List<Long> |  | 1197 |
| `VitsVoiceProvider.parseJsonIds` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | value: Any?<br>label: String | List<Long> |  | 1202 |
| `VitsVoiceProvider.parseJsonId` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | value: Any?<br>label: String | Long |  | 1215 |
| `VitsVoiceProvider.parseIds` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | raw: String<br>label: String | List<Long> |  | 1223 |
| `VitsVoiceProvider.parseLong` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | raw: String<br>label: String | Long |  | 1230 |
| `VitsVoiceProvider.optionalIds` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | key: String | List<Long>? |  | 1235 |
| `VitsVoiceProvider.optionalString` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | key: String | String |  | 1240 |
| `VitsVoiceProvider.optionalLong` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | key: String | Long? |  | 1244 |
| `VitsVoiceProvider.optionalInt` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | key: String | Int? |  | 1250 |
| `VitsVoiceProvider.optionalFloat` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | key: String | Float? |  | 1256 |
| `VitsVoiceProvider.optionalBool` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | key: String | Boolean? |  | 1262 |
| `VitsVoiceProvider.optionalInt` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | key: String | Int? |  | 1271 |
| `VitsVoiceProvider.optionalFloat` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | key: String | Float? |  | 1281 |
| `VitsVoiceProvider.manifestPath` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | root: File<br>manifest: JSONObject?<br>key: String | File? |  | 1291 |
| `VitsVoiceProvider.optionPath` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | root: File<br>key: String | File? |  | 1296 |
| `VitsVoiceProvider.resolveRelativeFile` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | root: File<br>raw: String | File |  | 1301 |
| `VitsVoiceProvider.singleCandidate` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | files: List<File><br>missingRes: Int<br>ambiguousRes: Int | File |  | 1318 |
| `VitsVoiceProvider.optionalSingleCandidate` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | files: List<File><br>ambiguousRes: Int | File? |  | 1324 |
| `VitsVoiceProvider.isTtsConfigJson` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | file: File | Boolean |  | 1330 |
| `VitsVoiceProvider.normalizeLocalPath` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | raw: String | String |  | 1337 |
| `VitsVoiceProvider.tokenizeSymbolsByMap` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | text: String<br>tokenMap: Map<String, List<Long>> | LongArray |  | 1341 |
| `VitsVoiceProvider.sha256` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | raw: String | String |  | 1362 |
| `VitsVoiceProvider.isCurrentPlayback` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | generation: Long | Boolean |  | 1367 |
| `VitsVoiceProvider.isPlaybackPaused` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | generation: Long | Boolean |  | 1371 |
| `VitsVoiceProvider.printableSymbol` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | symbol: String | String |  | 1375 |
| `VitsVoiceProvider.speechPreview` | `VitsVoiceProvider` | `com.ai.assistance.operit.api.voice` | `VitsVoiceProvider.kt` | text: String | String |  | 1385 |
| `VoiceListFetcher.getVoicesListUrl` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | endpointUrl: String | List<String> |  | 23 |
| `VoiceListFetcher.extractBaseUrl` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | fullUrl: String | String |  | 32 |
| `VoiceListFetcher.getVoicesList` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | apiKey: String<br>ttsEndpointUrl: String | Result<List<VoiceService.Voice>> |  | 50 |
| `VoiceListFetcher.parseVoices` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | json: String | List<VoiceService.Voice> |  | 99 |
| `VoiceListFetcher.dedupeVoicesById` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | voices: List<VoiceService.Voice> | List<VoiceService.Voice> |  | 126 |
| `VoiceListFetcher.preferRicherVoice` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | current: VoiceService.Voice<br>incoming: VoiceService.Voice | VoiceService.Voice |  | 153 |
| `VoiceListFetcher.score` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | voice: VoiceService.Voice | Int |  | 157 |
| `VoiceService.initialize` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` |  | Boolean | 初始化语音引擎 | 21 |
| `VoiceService.speak` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` | text: String<br>interrupt: Boolean?<br>rate: Float??<br>pitch: Float??<br>extraParams: Map<String, String>? | Boolean | 文本转语音，将文本通过TTS引擎转换为语音并播放 | 33 |
| `VoiceService.stop` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` |  | Boolean | 停止当前正在播放的语音 | 46 |
| `VoiceService.pause` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` |  | Boolean | 暂停当前正在播放的语音 | 53 |
| `VoiceService.resume` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` |  | Boolean | 继续播放暂停的语音 | 60 |
| `VoiceService.shutdown` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` |  | Unit | 释放语音引擎资源 | 63 |
| `VoiceService.getAvailableVoices` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` |  | List<Voice> | 获取当前可用的语音列表 | 70 |
| `VoiceService.setVoice` | `VoiceService` | `com.ai.assistance.operit.api.voice` | `VoiceService.kt` | voiceId: String | Boolean | 设置当前使用的语音 | 78 |
| `VoiceServiceFactory.createVoiceService` | `VoiceServiceFactory` | `com.ai.assistance.operit.api.voice` | `VoiceServiceFactory.kt` | context: Context | VoiceService | 创建语音服务实例 (现在从Preferences中读取配置) | 36 |
| `VoiceServiceFactory.getInstance` | `VoiceServiceFactory` | `com.ai.assistance.operit.api.voice` | `VoiceServiceFactory.kt` | context: Context | VoiceService | 获取语音服务单例实例 | 121 |
| `VoiceServiceFactory.resetInstance` | `VoiceServiceFactory` | `com.ai.assistance.operit.api.voice` | `VoiceServiceFactory.kt` |  | Unit | 重置单例实例 在需要更改语音服务类型或释放资源时调用 | 134 |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `VoiceListFetcher.client` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | inferred |  | 16 |
| `VoiceListFetcher.TAG` | `VoiceListFetcher` | `com.ai.assistance.operit.api.voice` | `VoiceListFetcher.kt` | inferred |  | 14 |
| `VoiceServiceFactory.currentProfileId` | `VoiceServiceFactory` | `com.ai.assistance.operit.api.voice` | `VoiceServiceFactory.kt` | String? |  | 113 |
| `VoiceServiceFactory.instance` | `VoiceServiceFactory` | `com.ai.assistance.operit.api.voice` | `VoiceServiceFactory.kt` | VoiceService? | 单例实例缓存 | 112 |
