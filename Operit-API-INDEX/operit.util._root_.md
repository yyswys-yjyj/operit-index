# operit.util.(root)

> 函数 834 · 类型 150 · 顶层常量 216 · 共 1200 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `AndroidUserPathUtils` | `AndroidUserPathUtils` | `com.ai.assistance.operit.util` | `AndroidUserPathUtils.kt` | object AndroidUserPathUtils |  | 5 |
| `AnrCaptureBudget` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | object AnrCaptureBudget | Memory and frequency budget for the diagnostics collected by [AnrMonitor]. The watchdog s… | 11 |
| `AnrCaptureBudgetTest` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` | class AnrCaptureBudgetTest | Regression coverage for the ANR capture budget that keeps [AnrMonitor] from allocating an… | 13 |
| `AnrCaptureThrottle` | `AnrCaptureThrottle` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | class AnrCaptureThrottle(private val cooldownMs: Long) | Rate limiter for ANR captures. A blocked main thread stays blocked across many 100 ms sam… | 121 |
| `AnrCaptureThrottleTest` | `AnrCaptureThrottleTest` | `com.ai.assistance.operit.util` | `AnrCaptureThrottleTest.kt` | class AnrCaptureThrottleTest | Regression coverage for the capture rate limit that stops a long main-thread stall from s… | 12 |
| `AnrMonitor` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` | class AnrMonitor(private val context: Context, private val coroutineScope: CoroutineScope, private val tag: String) | ANR监控器，用于跟踪和记录可能导致ANR的主线程阻塞 | 41 |
| `AnrMonitor.MainThreadStack` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` | class MainThreadStack(val signature: String, val dump: String) : String |  | 385 |
| `AppLogger` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | object AppLogger | App-wide logger with an API closely mirroring [com.ai.assistance.operit.util.AppLogger]. … | 22 |
| `ArchiveUtil` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | object ArchiveUtil | Utility class for archive operations | 19 |
| `AssetCopyUtils` | `AssetCopyUtils` | `com.ai.assistance.operit.util` | `AssetCopyUtils.kt` | object AssetCopyUtils |  | 9 |
| `ChatMarkupRegex` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | object ChatMarkupRegex |  | 5 |
| `ChatMarkupRegexAttachmentTest` | `ChatMarkupRegexAttachmentTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexAttachmentTest.kt` | class ChatMarkupRegexAttachmentTest |  | 7 |
| `ChatMarkupRegexContainsTest` | `ChatMarkupRegexContainsTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexContainsTest.kt` | class ChatMarkupRegexContainsTest |  | 7 |
| `ChatMarkupRegexMetaTest` | `ChatMarkupRegexMetaTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexMetaTest.kt` | class ChatMarkupRegexMetaTest |  | 7 |
| `ChatMarkupRegexOpeningTagTest` | `ChatMarkupRegexOpeningTagTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexOpeningTagTest.kt` | class ChatMarkupRegexOpeningTagTest |  | 7 |
| `ChatMarkupRegexPatternTest` | `ChatMarkupRegexPatternTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexPatternTest.kt` | class ChatMarkupRegexPatternTest |  | 7 |
| `ChatMarkupRegexRandomTagTest` | `ChatMarkupRegexRandomTagTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexRandomTagTest.kt` | class ChatMarkupRegexRandomTagTest |  | 7 |
| `ChatMarkupRegexSearchTest` | `ChatMarkupRegexSearchTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexSearchTest.kt` | class ChatMarkupRegexSearchTest |  | 7 |
| `ChatMarkupRegexStatusTest` | `ChatMarkupRegexStatusTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexStatusTest.kt` | class ChatMarkupRegexStatusTest |  | 7 |
| `ChatMarkupRegexTest` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` | class ChatMarkupRegexTest |  | 10 |
| `ChatMarkupRegexToolNameTest` | `ChatMarkupRegexToolNameTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolNameTest.kt` | class ChatMarkupRegexToolNameTest |  | 8 |
| `ChatMarkupRegexToolResultTest` | `ChatMarkupRegexToolResultTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolResultTest.kt` | class ChatMarkupRegexToolResultTest |  | 8 |
| `ChatTrace` | `ChatTrace` | `com.ai.assistance.operit.util` | `ChatTrace.kt` | object ChatTrace | Formatting helpers for diagnosing message truncation without writing user content to logs… | 13 |
| `ChatUtils` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | object ChatUtils | Utility functions for chat message handling | 7 |
| `ChatUtilsExtractJsonEdgeTest` | `ChatUtilsExtractJsonEdgeTest` | `com.ai.assistance.operit.util` | `ChatUtilsExtractJsonEdgeTest.kt` | class ChatUtilsExtractJsonEdgeTest |  | 6 |
| `ChatUtilsJsonExtractionTest` | `ChatUtilsJsonExtractionTest` | `com.ai.assistance.operit.util` | `ChatUtilsJsonExtractionTest.kt` | class ChatUtilsJsonExtractionTest |  | 6 |
| `ChatUtilsProviderModelTest` | `ChatUtilsProviderModelTest` | `com.ai.assistance.operit.util` | `ChatUtilsProviderModelTest.kt` | class ChatUtilsProviderModelTest |  | 7 |
| `ChatUtilsStripMetaCollectionsTest` | `ChatUtilsStripMetaCollectionsTest` | `com.ai.assistance.operit.util` | `ChatUtilsStripMetaCollectionsTest.kt` | class ChatUtilsStripMetaCollectionsTest |  | 8 |
| `ChatUtilsTest` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` | class ChatUtilsTest |  | 10 |
| `ChatUtilsThinkingEdgeTest` | `ChatUtilsThinkingEdgeTest` | `com.ai.assistance.operit.util` | `ChatUtilsThinkingEdgeTest.kt` | class ChatUtilsThinkingEdgeTest |  | 6 |
| `ChatUtilsThinkingTest` | `ChatUtilsThinkingTest` | `com.ai.assistance.operit.util` | `ChatUtilsThinkingTest.kt` | class ChatUtilsThinkingTest |  | 6 |
| `ChatUtilsTokenEstimateTest` | `ChatUtilsTokenEstimateTest` | `com.ai.assistance.operit.util` | `ChatUtilsTokenEstimateTest.kt` | class ChatUtilsTokenEstimateTest |  | 6 |
| `ColorQrCodeUtil` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | object ColorQrCodeUtil |  | 29 |
| `ColorQrCodeUtil.BitReader` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | class BitReader(private val data: ByteArray) |  | 652 |
| `ColorQrCodeUtil.ColorQrException` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | class ColorQrException(message: String, cause: Throwable?) : Exception |  | 37 |
| `ColorQrCodeUtil.DecodeResult` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | class DecodeResult(val payload: ByteArray, val colorCount: Int, val qrVersion: Int, val crc32: Int) |  | 30 |
| `ColorQrCodeUtil.DetectedQr` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | class DetectedQr(val dimension: Int, val points: Array<com.google.zxing.Result…) : DetectedQr |  | 275 |
| `ColorQrCodeUtilAndroidTest` | `ColorQrCodeUtilAndroidTest` | `com.ai.assistance.operit.util` | `ColorQrCodeUtilAndroidTest.kt` | class ColorQrCodeUtilAndroidTest |  | 10 |
| `CrashRecoveryState` | `CrashRecoveryState` | `com.ai.assistance.operit.util` | `CrashRecoveryState.kt` | object CrashRecoveryState |  | 5 |
| `CrashRecoveryStateAndroidTest` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` | class CrashRecoveryStateAndroidTest |  | 13 |
| `CrashRecoveryStateLifecycleAndroidTest` | `CrashRecoveryStateLifecycleAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateLifecycleAndroidTest.kt` | class CrashRecoveryStateLifecycleAndroidTest |  | 13 |
| `CrashRecoveryStatePrefsAndroidTest` | `CrashRecoveryStatePrefsAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStatePrefsAndroidTest.kt` | class CrashRecoveryStatePrefsAndroidTest |  | 12 |
| `CrashRecoveryStateRepeatAndroidTest` | `CrashRecoveryStateRepeatAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateRepeatAndroidTest.kt` | class CrashRecoveryStateRepeatAndroidTest |  | 13 |
| `DocumentConversionUtil` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | object DocumentConversionUtil | Utility class for document conversion operations | 35 |
| `DocumentConversionUtilNullCharacterTest` | `DocumentConversionUtilNullCharacterTest` | `com.ai.assistance.operit.util` | `DocumentConversionUtilNullCharacterTest.kt` | class DocumentConversionUtilNullCharacterTest |  | 6 |
| `FFmpegUtil` | `FFmpegUtil` | `com.ai.assistance.operit.util` | `FFmpegUtil.kt` | object FFmpegUtil | Utility class for FFmpeg operations | 12 |
| `FileUtils` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | object FileUtils |  | 15 |
| `GithubReleaseDigestTest` | `GithubReleaseDigestTest` | `com.ai.assistance.operit.util` | `GithubReleaseDigestTest.kt` | class GithubReleaseDigestTest | The published asset digest is the only integrity anchor the updater has: the patch meta c… | 14 |
| `GithubReleaseUtil` | `GithubReleaseUtil` | `com.ai.assistance.operit.util` | `GithubReleaseUtil.kt` | class GithubReleaseUtil(private val context: Context) | GitHub Release 工具类 使用统一的 GitHubApiService 来获取 Release 信息 支持自动添加认证头以提高 API 配额 | 19 |
| `GithubReleaseUtil.ProbeResult` | `GithubReleaseUtil` | `com.ai.assistance.operit.util` | `GithubReleaseUtil.kt` | class ProbeResult(val ok: Boolean, val latencyMs: Long?, val bytesPerSec: Long?, val sampledBytes: Long?, val httpStatus: Int?, val contentType: String?, val error: String?) |  | 39 |
| `GithubReleaseUtil.ReleaseInfo` | `GithubReleaseUtil` | `com.ai.assistance.operit.util` | `GithubReleaseUtil.kt` | class ReleaseInfo(val version: String, val downloadUrl: String, val releaseNotes: String, val releasePageUrl: String, /** * SHA-256 that GitHub publishes for the APK asset (`di… |  | 23 |
| `GlobalExceptionHandler` | `GlobalExceptionHandler` | `com.ai.assistance.operit.util` | `GlobalExceptionHandler.kt` | class GlobalExceptionHandler(private val context: Context) : Thread.UncaughtExceptionHandler |  | 8 |
| `HtmlParserUtil` | `HtmlParserUtil` | `com.ai.assistance.operit.util` | `HtmlParserUtil.kt` | object HtmlParserUtil |  | 8 |
| `HtmlParserUtil.ExtractionResult` | `HtmlParserUtil` | `com.ai.assistance.operit.util` | `HtmlParserUtil.kt` | class ExtractionResult(val tree: List<ComputerPageInfoNode>?, val map: Map<String, String>) |  | 213 |
| `HttpLogSanitizer` | `HttpLogSanitizer` | `com.ai.assistance.operit.util` | `HttpLogSanitizer.kt` | object HttpLogSanitizer |  | 6 |
| `HttpMultiPartDownloader` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | object HttpMultiPartDownloader |  | 13 |
| `HttpMultiPartDownloader.ProbeResult` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | class ProbeResult(val contentLength: Long, val acceptRanges: Boolean) |  | 14 |
| `HttpMultiPartDownloader.SegmentPlan` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | class SegmentPlan(val index: Int, val startInclusive: Long, val endInclusive: Long) |  | 19 |
| `ImageBitmapLimiter` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | object ImageBitmapLimiter |  | 8 |
| `ImageBitmapLimiter.ImageBounds` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | class ImageBounds(val width: Int, val height: Int) |  | 20 |
| `ImageBitmapLimiter.LimitedImage` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | class LimitedImage(val base64: String, val mimeType: String) |  | 15 |
| `ImageOutputFormat` | `ImageOutputFormat` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | class ImageOutputFormat |  | 16 |
| `ImagePoolManager` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | object ImagePoolManager | 全局图片池管理器 支持内存缓存和本地持久化缓存，使用LRU策略。 图片在注册入池时会被统一解码、方向归一、缩放、格式转换， 池中仅保存最终发送用的唯一标准图。 | 37 |
| `ImagePoolManager.ImageData` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | class ImageData(val base64: String, val mimeType: String, val width: Int, val height: Int) |  | 63 |
| `ImagePoolManager.NormalizedBase64Input` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | class NormalizedBase64Input(val base64: String, val mimeType: String) |  | 78 |
| `ImagePoolManager.ResolvedRegistrationOptions` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | class ResolvedRegistrationOptions(val scalePercent: Int, val outputFormat: ImageOutputFormat, val jpegQuality: Int, val normalizeExif: Boolean, val maxLongEdge: Int?) |  | 70 |
| `ImageRegistrationOptions` | `ImageRegistrationOptions` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | class ImageRegistrationOptions(val scalePercent: Int?, val outputFormat: ImageOutputFormat, val jpegQuality: Int?, val normalizeExif: Boolean, val maxLongEdge: Int?) |  | 22 |
| `IntRangeSerializer` | `IntRangeSerializer` | `com.ai.assistance.operit.util` | `IntRangeSerializer.kt` | object IntRangeSerializer : KSerializer<IntRange> | Custom serializer for IntRange | 12 |
| `IntRangeSerializerAndroidTest` | `IntRangeSerializerAndroidTest` | `com.ai.assistance.operit.util` | `IntRangeSerializerAndroidTest.kt` | class IntRangeSerializerAndroidTest |  | 10 |
| `IntRangeSerializerShapeAndroidTest` | `IntRangeSerializerShapeAndroidTest` | `com.ai.assistance.operit.util` | `IntRangeSerializerShapeAndroidTest.kt` | class IntRangeSerializerShapeAndroidTest |  | 10 |
| `LatexMathMlConverter` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | object LatexMathMlConverter |  | 8 |
| `LocalDateTimeSerializer` | `LocalDateTimeSerializer` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializer.kt` | object LocalDateTimeSerializer : KSerializer<LocalDateTime> |  | 12 |
| `LocalDateTimeSerializerAndroidTest` | `LocalDateTimeSerializerAndroidTest` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializerAndroidTest.kt` | class LocalDateTimeSerializerAndroidTest |  | 11 |
| `LocalDateTimeSerializerFormatAndroidTest` | `LocalDateTimeSerializerFormatAndroidTest` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializerFormatAndroidTest.kt` | class LocalDateTimeSerializerFormatAndroidTest |  | 11 |
| `LocaleUtils` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | object LocaleUtils | 语言工具类，用于管理应用的国际化设置 | 16 |
| `LocaleUtils.Language` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | class Language(val code: String, val displayName: String, val nativeName: String) | 语言信息数据类 | 40 |
| `LocaleUtils.LanguageCodes` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | object LanguageCodes |  | 18 |
| `LocaleUtilsConfigurationAndroidTest` | `LocaleUtilsConfigurationAndroidTest` | `com.ai.assistance.operit.util` | `LocaleUtilsConfigurationAndroidTest.kt` | class LocaleUtilsConfigurationAndroidTest |  | 13 |
| `LocationUtils` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | object LocationUtils |  | 26 |
| `MathMlPlainTextConverter` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | object MathMlPlainTextConverter |  | 8 |
| `MathMlPlainTextConverterTest` | `MathMlPlainTextConverterTest` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverterTest.kt` | class MathMlPlainTextConverterTest |  | 6 |
| `MediaBase64Limiter` | `MediaBase64Limiter` | `com.ai.assistance.operit.util` | `MediaBase64Limiter.kt` | object MediaBase64Limiter |  | 5 |
| `MediaBase64Limiter.LimitedMedia` | `MediaBase64Limiter` | `com.ai.assistance.operit.util` | `MediaBase64Limiter.kt` | class LimitedMedia(val base64: String, val mimeType: String) |  | 8 |
| `MediaPoolManager` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | object MediaPoolManager |  | 11 |
| `MediaPoolManager.AsciiStringInputStream` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | class AsciiStringInputStream(private val data: String) : InputStream |  | 104 |
| `MediaPoolManager.MediaData` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | class MediaData(val base64: String, val mimeType: String) |  | 133 |
| `MediaPoolManager.TranscodedMedia` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | class TranscodedMedia(val file: File, val mimeType: String) |  | 18 |
| `MetadataBlock` | `MetadataBlock` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | class MetadataBlock(val comment: String, val content: String, val range: IntRange) |  | 369 |
| `NetworkUtils` | `NetworkUtils` | `com.ai.assistance.operit.util` | `NetworkUtils.kt` | object NetworkUtils |  | 8 |
| `OCRUtils` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | object OCRUtils | OCR工具类，封装ML Kit的文本识别功能 | 28 |
| `OCRUtils.Language` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | class Language | 文本识别语言选项 | 38 |
| `OCRUtils.OCRResult` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | class OCRResult | OCR识别结果 | 385 |
| `OCRUtils.OCRResult.Error` | `OCRResult` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | class Error(val message: String) : OCRResult | 识别失败 | 408 |
| `OCRUtils.OCRResult.Success` | `OCRResult` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | class Success(val text: Text) : OCRResult | 识别成功 | 387 |
| `OCRUtils.Quality` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | class Quality | 识别质量选项 | 46 |
| `OperitPaths` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | object OperitPaths |  | 7 |
| `PathMapper` | `PathMapper` | `com.ai.assistance.operit.util` | `PathMapper.kt` | object PathMapper | 路径映射工具类 用于在Android环境和Linux（Ubuntu终端）环境之间转换文件路径 | 10 |
| `PathMapperAndroidTest` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` | class PathMapperAndroidTest |  | 13 |
| `PathMapperLinuxEnvAndroidTest` | `PathMapperLinuxEnvAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperLinuxEnvAndroidTest.kt` | class PathMapperLinuxEnvAndroidTest |  | 10 |
| `PathMapperLinuxPathAndroidTest` | `PathMapperLinuxPathAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperLinuxPathAndroidTest.kt` | class PathMapperLinuxPathAndroidTest |  | 11 |
| `PathMapperResolveAndroidTest` | `PathMapperResolveAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperResolveAndroidTest.kt` | class PathMapperResolveAndroidTest |  | 11 |
| `PortProcessKiller` | `PortProcessKiller` | `com.ai.assistance.operit.util` | `PortProcessKiller.kt` | object PortProcessKiller |  | 6 |
| `Segment` | `Segment` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | class Segment(val content: String, val isProtected: Boolean, val blockType: MarkdownProcessorType) |  | 902 |
| `SerializationSetup` | `SerializationSetup` | `com.ai.assistance.operit.util` | `SerializationSetup.kt` | object SerializationSetup | Configures the serialization module with custom serializers | 9 |
| `SerializerAndroidTest` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` | class SerializerAndroidTest |  | 13 |
| `SerializerRoundTripAndroidTest` | `SerializerRoundTripAndroidTest` | `com.ai.assistance.operit.util` | `SerializerRoundTripAndroidTest.kt` | class SerializerRoundTripAndroidTest |  | 12 |
| `SkillRepoZipPoolManager` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | object SkillRepoZipPoolManager |  | 9 |
| `StreamingJsonXmlConverter` | `StreamingJsonXmlConverter` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` | class StreamingJsonXmlConverter | 流式 JSON 到 XML 的转换器 专门用于将 Tool Call 的 arguments JSON 流增量转换为 XML 格式 例如: {"arg1": "val"} -> … | 8 |
| `StreamingJsonXmlConverter.Event` | `StreamingJsonXmlConverter` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` | class Event | XML 流事件 | 13 |
| `StreamingJsonXmlConverter.Event.State` | `Event` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` | class State |  | 18 |
| `StreamingJsonXmlConverter.Event.Tag` | `Event` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` | class Tag(val text: String) : Event |  | 14 |
| `StreamingJsonXmlConverterChunkTest` | `StreamingJsonXmlConverterChunkTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterChunkTest.kt` | class StreamingJsonXmlConverterChunkTest |  | 6 |
| `StreamingJsonXmlConverterEscapeTest` | `StreamingJsonXmlConverterEscapeTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterEscapeTest.kt` | class StreamingJsonXmlConverterEscapeTest |  | 6 |
| `StreamingJsonXmlConverterFlushTest` | `StreamingJsonXmlConverterFlushTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterFlushTest.kt` | class StreamingJsonXmlConverterFlushTest |  | 7 |
| `StreamingJsonXmlConverterObjectTest` | `StreamingJsonXmlConverterObjectTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterObjectTest.kt` | class StreamingJsonXmlConverterObjectTest |  | 6 |
| `StreamingJsonXmlConverterPrimitiveTest` | `StreamingJsonXmlConverterPrimitiveTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterPrimitiveTest.kt` | class StreamingJsonXmlConverterPrimitiveTest |  | 6 |
| `StreamingJsonXmlConverterStringTest` | `StreamingJsonXmlConverterStringTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterStringTest.kt` | class StreamingJsonXmlConverterStringTest |  | 6 |
| `StreamingJsonXmlConverterTest` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` | class StreamingJsonXmlConverterTest |  | 8 |
| `StructuredAssistantContentParser` | `StructuredAssistantContentParser` | `com.ai.assistance.operit.util` | `StructuredAssistantContentParser.kt` | object StructuredAssistantContentParser |  | 5 |
| `StructuredAssistantContentParser.Block` | `StructuredAssistantContentParser` | `com.ai.assistance.operit.util` | `StructuredAssistantContentParser.kt` | class Block(val kind: BlockKind, val rawContent: String, val content: String, val tagName: String?, val rawTagName: String?, val attrs: Map<String, String>, val closed: B… |  | 12 |
| `StructuredAssistantContentParser.BlockKind` | `StructuredAssistantContentParser` | `com.ai.assistance.operit.util` | `StructuredAssistantContentParser.kt` | class BlockKind |  | 7 |
| `TextSegmenter` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | object TextSegmenter | 文本分词工具类 - 提供中文和多语言文本的分词功能 | 13 |
| `ThrowableTextFormatter` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | object ThrowableTextFormatter |  | 6 |
| `TokenCacheManager` | `TokenCacheManager` | `com.ai.assistance.operit.util` | `TokenCacheManager.kt` | class TokenCacheManager | Token缓存管理器，用于优化重复对话历史的token计算 通过缓存之前计算过的对话历史token数量，避免重复计算相同的内容 | 10 |
| `ToolingRegressionTest` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` | class ToolingRegressionTest |  | 7 |
| `ToolPkgArtifactMinifier` | `ToolPkgArtifactMinifier` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | object ToolPkgArtifactMinifier | Produces publish artifacts with optional AST minification and mandatory market provenance. | 19 |
| `ToolPkgJsAstMinifier` | `ToolPkgJsAstMinifier` | `com.ai.assistance.operit.util` | `ToolPkgJsAstMinifier.kt` | class ToolPkgJsAstMinifier(context: Context) : Closeable |  | 9 |
| `ToolPkgWasmNative` | `ToolPkgWasmNative` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | object ToolPkgWasmNative |  | 94 |
| `ToolPkgWasmRuntime` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | object ToolPkgWasmRuntime |  | 6 |
| `ToolPkgWasmRuntime.LoadedModule` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | class LoadedModule(val handle: Long, val fingerprint: String) |  | 7 |
| `TtsCleaner` | `TtsCleaner` | `com.ai.assistance.operit.util` | `TtsCleaner.kt` | object TtsCleaner |  | 5 |
| `TtsCleanerSpeechPipelineTest` | `TtsCleanerSpeechPipelineTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechPipelineTest.kt` | class TtsCleanerSpeechPipelineTest | End to end coverage for reading messages aloud with the built-in "Remove XML tags" cleane… | 23 |
| `TtsCleanerSpeechTest` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` | class TtsCleanerSpeechTest | Regression coverage for reading messages aloud when the user enabled the built-in "Remove… | 16 |
| `TtsSegmenter` | `TtsSegmenter` | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | object TtsSegmenter |  | 3 |
| `TtsSegmenterTest` | `TtsSegmenterTest` | `com.ai.assistance.operit.util` | `TtsSegmenterTest.kt` | class TtsSegmenterTest |  | 6 |
| `UpdateSourceProbeTest` | `UpdateSourceProbeTest` | `com.ai.assistance.operit.util` | `UpdateSourceProbeTest.kt` | class UpdateSourceProbeTest | The speed probe decides which sources the updater is allowed to download from, so it has … | 21 |
| `UriSerializer` | `UriSerializer` | `com.ai.assistance.operit.util` | `UriSerializer.kt` | object UriSerializer |  | 11 |
| `UriSerializerAndroidTest` | `UriSerializerAndroidTest` | `com.ai.assistance.operit.util` | `UriSerializerAndroidTest.kt` | class UriSerializerAndroidTest |  | 11 |
| `UriSerializerNullAndroidTest` | `UriSerializerNullAndroidTest` | `com.ai.assistance.operit.util` | `UriSerializerNullAndroidTest.kt` | class UriSerializerNullAndroidTest |  | 11 |
| `UriSerializerSchemeAndroidTest` | `UriSerializerSchemeAndroidTest` | `com.ai.assistance.operit.util` | `UriSerializerSchemeAndroidTest.kt` | class UriSerializerSchemeAndroidTest |  | 11 |
| `WaifuMessageProcessor` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | object WaifuMessageProcessor | Waifu模式消息处理器 负责将AI回复按句号分割并模拟逐句发送 | 20 |
| `WaifuMessageProcessor.StreamingSession` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | class StreamingSession(private val removePunctuation: Boolean) |  | 68 |
| `WaifuMessageProcessorTest` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` | class WaifuMessageProcessorTest |  | 17 |
| `WaifuMessageProcessorTest.FixedTagXmlRenderPlugin` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` | class FixedTagXmlRenderPlugin(override val id: String, private val supportedTags: Set<String>) : XmlRenderPlugin | ---- Plugins registered through ToolPkg 的 XML 渲染标签（如 voice）必须穿过 Waifu 过滤链路。 | 214 |
| `WaifuRenderableSnapshotTest` | `WaifuRenderableSnapshotTest` | `com.ai.assistance.operit.util` | `WaifuRenderableSnapshotTest.kt` | class WaifuRenderableSnapshotTest |  | 7 |
| `WaifuSegmentMessageStore` | `WaifuSegmentMessageStore` | `com.ai.assistance.operit.util` | `WaifuStreamUpdates.kt` | class WaifuSegmentMessageStore(private val messages: MutableList<T>, private val createMessage: (String) -> T, private val appendMessage: suspend (message: T, interrup…, private val removeM… : suspend | Applies the same segment changes to this turn's message identities and its persisted bubb… | 223 |
| `WaifuSegmentUpdate` | `WaifuSegmentUpdate` | `com.ai.assistance.operit.util` | `WaifuStreamUpdates.kt` | interface WaifuSegmentUpdate |  | 22 |
| `WaifuSegmentUpdate.Append` | `WaifuSegmentUpdate` | `com.ai.assistance.operit.util` | `WaifuStreamUpdates.kt` | class Append(val content: String) : WaifuSegmentUpdate data class Retain |  | 23 |
| `WaifuStreamUpdatesTest` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` | class WaifuStreamUpdatesTest |  | 36 |
| `WaifuStreamUpdatesTest.Bubble` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` | class Bubble(val id: Int, val text: String) |  | 91 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `ColorQrCodeUtilAndroidTest.roundTrip_2_4_8_16_colors` | `ColorQrCodeUtilAndroidTest` | `com.ai.assistance.operit.util` | `ColorQrCodeUtilAndroidTest.kt` |  | Unit |  | 13 ⚑ |
| `ColorQrCodeUtilAndroidTest.roundTrip_autoDetectColorCount` | `ColorQrCodeUtilAndroidTest` | `com.ai.assistance.operit.util` | `ColorQrCodeUtilAndroidTest.kt` |  | Unit |  | 31 ⚑ |
| `CrashRecoveryStateAndroidTest.resetState` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 18 ⚑ |
| `CrashRecoveryStateAndroidTest.consumeWithoutMark_returnsFalse` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 26 ⚑ |
| `CrashRecoveryStateAndroidTest.markThenConsume_returnsTrue` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 30 ⚑ |
| `CrashRecoveryStateAndroidTest.consumeClearsPendingFlag` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 35 ⚑ |
| `CrashRecoveryStateAndroidTest.multipleMarksRemainSinglePendingFlag` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 41 ⚑ |
| `CrashRecoveryStateAndroidTest.applicationContextPath_isUsedSafely` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 47 ⚑ |
| `CrashRecoveryStateAndroidTest.unrelatedPreferenceKeys_arePreserved` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 52 ⚑ |
| `CrashRecoveryStateAndroidTest.repeatedConsumeAfterClear_staysFalse` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 60 ⚑ |
| `CrashRecoveryStateAndroidTest.markAfterConsume_becomesPendingAgain` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 66 ⚑ |
| `CrashRecoveryStateAndroidTest.separateContextReferences_shareSameState` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 73 ⚑ |
| `CrashRecoveryStateAndroidTest.pendingFlagUsesCommitAndPersistsImmediately` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 80 ⚑ |
| `CrashRecoveryStateAndroidTest.consumeRemovesStoredKey` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 86 ⚑ |
| `CrashRecoveryStateAndroidTest.doubleConsumeAfterSingleMark_onlyFirstIsTrue` | `CrashRecoveryStateAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateAndroidTest.kt` |  | Unit |  | 93 ⚑ |
| `CrashRecoveryStateLifecycleAndroidTest.clearPrefs` | `CrashRecoveryStateLifecycleAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateLifecycleAndroidTest.kt` |  | Unit |  | 18 ⚑ |
| `CrashRecoveryStateLifecycleAndroidTest.markPending_setsFlagVisibleToDirectPrefsRead` | `CrashRecoveryStateLifecycleAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateLifecycleAndroidTest.kt` |  | Unit |  | 22 ⚑ |
| `CrashRecoveryStateLifecycleAndroidTest.consumeWithoutMark_doesNotCreateFlag` | `CrashRecoveryStateLifecycleAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateLifecycleAndroidTest.kt` |  | Unit |  | 28 ⚑ |
| `CrashRecoveryStateLifecycleAndroidTest.secondMark_afterConsume_setsFlagAgain` | `CrashRecoveryStateLifecycleAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateLifecycleAndroidTest.kt` |  | Unit |  | 34 ⚑ |
| `CrashRecoveryStatePrefsAndroidTest.setup` | `CrashRecoveryStatePrefsAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStatePrefsAndroidTest.kt` |  | Unit |  | 17 ⚑ |
| `CrashRecoveryStatePrefsAndroidTest.otherPreferenceKey_survivesMarkAndConsume` | `CrashRecoveryStatePrefsAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStatePrefsAndroidTest.kt` |  | Unit |  | 21 ⚑ |
| `CrashRecoveryStateRepeatAndroidTest.clear` | `CrashRecoveryStateRepeatAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateRepeatAndroidTest.kt` |  | Unit |  | 18 ⚑ |
| `CrashRecoveryStateRepeatAndroidTest.consumeTwiceAfterMark_onlyFirstReturnsTrue` | `CrashRecoveryStateRepeatAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateRepeatAndroidTest.kt` |  | Unit |  | 22 ⚑ |
| `CrashRecoveryStateRepeatAndroidTest.consumeBeforeMarkThenAfterMark_behavesCorrectly` | `CrashRecoveryStateRepeatAndroidTest` | `com.ai.assistance.operit.util` | `CrashRecoveryStateRepeatAndroidTest.kt` |  | Unit |  | 28 ⚑ |
| `IntRangeSerializerAndroidTest.singlePointRange_roundTrips` | `IntRangeSerializerAndroidTest` | `com.ai.assistance.operit.util` | `IntRangeSerializerAndroidTest.kt` |  | Unit |  | 12 ⚑ |
| `IntRangeSerializerAndroidTest.descendingValues_preserveStoredBounds` | `IntRangeSerializerAndroidTest` | `com.ai.assistance.operit.util` | `IntRangeSerializerAndroidTest.kt` |  | Unit |  | 18 ⚑ |
| `IntRangeSerializerShapeAndroidTest.serializedRangeContainsStartField` | `IntRangeSerializerShapeAndroidTest` | `com.ai.assistance.operit.util` | `IntRangeSerializerShapeAndroidTest.kt` |  | Unit |  | 12 ⚑ |
| `IntRangeSerializerShapeAndroidTest.serializedRangeContainsEndInclusiveField` | `IntRangeSerializerShapeAndroidTest` | `com.ai.assistance.operit.util` | `IntRangeSerializerShapeAndroidTest.kt` |  | Unit |  | 17 ⚑ |
| `LocalDateTimeSerializerAndroidTest.midnight_roundTrips` | `LocalDateTimeSerializerAndroidTest` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializerAndroidTest.kt` |  | Unit |  | 13 ⚑ |
| `LocalDateTimeSerializerAndroidTest.endOfDay_roundTrips` | `LocalDateTimeSerializerAndroidTest` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializerAndroidTest.kt` |  | Unit |  | 20 ⚑ |
| `LocalDateTimeSerializerFormatAndroidTest.serializedDateTimeUsesIsoSeparatorT` | `LocalDateTimeSerializerFormatAndroidTest` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializerFormatAndroidTest.kt` |  | Unit |  | 13 ⚑ |
| `LocalDateTimeSerializerFormatAndroidTest.serializedDateTimeContainsYearPrefix` | `LocalDateTimeSerializerFormatAndroidTest` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializerFormatAndroidTest.kt` |  | Unit |  | 18 ⚑ |
| `LocaleUtilsConfigurationAndroidTest.localeOverride_onlyDefinesLocaleFields` | `LocaleUtilsConfigurationAndroidTest` | `com.ai.assistance.operit.util` | `LocaleUtilsConfigurationAndroidTest.kt` |  | Unit |  | 15 ⚑ |
| `LocaleUtilsConfigurationAndroidTest.localizedContext_inheritsBaseWindowDimensions` | `LocaleUtilsConfigurationAndroidTest` | `com.ai.assistance.operit.util` | `LocaleUtilsConfigurationAndroidTest.kt` |  | Unit |  | 28 ⚑ |
| `LocaleUtilsConfigurationAndroidTest.japaneseOverride_usesEnglishAfterJapanese` | `LocaleUtilsConfigurationAndroidTest` | `com.ai.assistance.operit.util` | `LocaleUtilsConfigurationAndroidTest.kt` |  | Unit |  | 46 ⚑ |
| `LocaleUtilsConfigurationAndroidTest.japaneseContext_usesJapaneseThenEnglishResources` | `LocaleUtilsConfigurationAndroidTest` | `com.ai.assistance.operit.util` | `LocaleUtilsConfigurationAndroidTest.kt` |  | Unit |  | 53 ⚑ |
| `PathMapperAndroidTest.mapLinuxPath_rootSlash_returnsUbuntuRoot` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 18 ⚑ |
| `PathMapperAndroidTest.mapLinuxPath_emptyString_returnsUbuntuRoot` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 22 ⚑ |
| `PathMapperAndroidTest.mapLinuxPath_simpleFile_joinsUnderUbuntuRoot` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 26 ⚑ |
| `PathMapperAndroidTest.mapLinuxPath_nestedFile_joinsUnderUbuntuRoot` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 30 ⚑ |
| `PathMapperAndroidTest.mapLinuxPath_relativePath_stillJoinsUnderUbuntuRoot` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 34 ⚑ |
| `PathMapperAndroidTest.mapLinuxPath_multipleLeadingSlashes_areTrimmed` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 38 ⚑ |
| `PathMapperAndroidTest.mapLinuxPath_trailingSlash_isPreservedByFileJoin` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 42 ⚑ |
| `PathMapperAndroidTest.mapLinuxPath_pathWithSpaces_isSupported` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 46 ⚑ |
| `PathMapperAndroidTest.isLinuxEnvironment_acceptsLowercaseLinux` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 50 ⚑ |
| `PathMapperAndroidTest.isLinuxEnvironment_acceptsUppercaseLinux` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 54 ⚑ |
| `PathMapperAndroidTest.isLinuxEnvironment_rejectsAndroid` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 58 ⚑ |
| `PathMapperAndroidTest.isLinuxEnvironment_rejectsNull` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 62 ⚑ |
| `PathMapperAndroidTest.resolvePath_linuxEnvironment_mapsPath` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 66 ⚑ |
| `PathMapperAndroidTest.resolvePath_androidEnvironment_returnsOriginalPath` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 70 ⚑ |
| `PathMapperAndroidTest.resolvePath_unknownEnvironment_returnsOriginalPath` | `PathMapperAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperAndroidTest.kt` |  | Unit |  | 74 ⚑ |
| `PathMapperLinuxEnvAndroidTest.isLinuxEnvironment_acceptsMixedCase` | `PathMapperLinuxEnvAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperLinuxEnvAndroidTest.kt` |  | Unit |  | 12 ⚑ |
| `PathMapperLinuxEnvAndroidTest.isLinuxEnvironment_rejectsEmptyString` | `PathMapperLinuxEnvAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperLinuxEnvAndroidTest.kt` |  | Unit |  | 16 ⚑ |
| `PathMapperLinuxEnvAndroidTest.isLinuxEnvironment_rejectsWhitespaceString` | `PathMapperLinuxEnvAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperLinuxEnvAndroidTest.kt` |  | Unit |  | 20 ⚑ |
| `PathMapperLinuxPathAndroidTest.mapLinuxPath_binPath_mapsUnderUbuntuRoot` | `PathMapperLinuxPathAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperLinuxPathAndroidTest.kt` |  | Unit |  | 16 ⚑ |
| `PathMapperLinuxPathAndroidTest.mapLinuxPath_usrPath_mapsUnderUbuntuRoot` | `PathMapperLinuxPathAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperLinuxPathAndroidTest.kt` |  | Unit |  | 20 ⚑ |
| `PathMapperResolveAndroidTest.resolvePath_linuxCaseInsensitive_mapsPath` | `PathMapperResolveAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperResolveAndroidTest.kt` |  | Unit |  | 16 ⚑ |
| `PathMapperResolveAndroidTest.resolvePath_nullEnvironment_returnsOriginal` | `PathMapperResolveAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperResolveAndroidTest.kt` |  | Unit |  | 20 ⚑ |
| `PathMapperResolveAndroidTest.resolvePath_blankEnvironment_returnsOriginal` | `PathMapperResolveAndroidTest` | `com.ai.assistance.operit.util` | `PathMapperResolveAndroidTest.kt` |  | Unit |  | 24 ⚑ |
| `SerializerAndroidTest.uriSerializer_serializesNonNullUri` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 15 ⚑ |
| `SerializerAndroidTest.uriSerializer_serializesNullAsEmptyString` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 20 ⚑ |
| `SerializerAndroidTest.uriSerializer_deserializesEmptyStringToNull` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 25 ⚑ |
| `SerializerAndroidTest.uriSerializer_deserializesHttpUri` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 29 ⚑ |
| `SerializerAndroidTest.intRangeSerializer_serializesRange` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 34 ⚑ |
| `SerializerAndroidTest.intRangeSerializer_deserializesRange` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 39 ⚑ |
| `SerializerAndroidTest.intRangeSerializer_deserializesNegativeRange` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 44 ⚑ |
| `SerializerAndroidTest.localDateTimeSerializer_serializesIsoString` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 49 ⚑ |
| `SerializerAndroidTest.localDateTimeSerializer_deserializesIsoString` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 54 ⚑ |
| `SerializerAndroidTest.localDateTimeSerializer_roundTripsFractionalSeconds` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 59 ⚑ |
| `SerializerAndroidTest.uriSerializer_roundTripsContentUri` | `SerializerAndroidTest` | `com.ai.assistance.operit.util` | `SerializerAndroidTest.kt` |  | Unit |  | 66 ⚑ |
| `SerializerRoundTripAndroidTest.uriSerializer_roundTripsHttpUri` | `SerializerRoundTripAndroidTest` | `com.ai.assistance.operit.util` | `SerializerRoundTripAndroidTest.kt` |  | Unit |  | 14 ⚑ |
| `SerializerRoundTripAndroidTest.intRangeSerializer_roundTripsNegativeRange` | `SerializerRoundTripAndroidTest` | `com.ai.assistance.operit.util` | `SerializerRoundTripAndroidTest.kt` |  | Unit |  | 19 ⚑ |
| `SerializerRoundTripAndroidTest.localDateTimeSerializer_roundTripsSimpleValue` | `SerializerRoundTripAndroidTest` | `com.ai.assistance.operit.util` | `SerializerRoundTripAndroidTest.kt` |  | Unit |  | 24 ⚑ |
| `TtsCleanerSpeechPipelineTest.disableAndroidLogging` | `TtsCleanerSpeechPipelineTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechPipelineTest.kt` |  | Unit |  | 37 ⚑ |
| `TtsCleanerSpeechPipelineTest.restoreAndroidLogging` | `TtsCleanerSpeechPipelineTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechPipelineTest.kt` |  | Unit |  | 45 ⚑ |
| `TtsCleanerSpeechPipelineTest.speechPipeline` | `TtsCleanerSpeechPipelineTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechPipelineTest.kt` | message: String<br>cleanerRegexs: List<String> | String |  | 50 ⚑ |
| `TtsCleanerSpeechPipelineTest.manualRead_readsReplyBodyOnlyUnderBothFilterStates` | `TtsCleanerSpeechPipelineTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechPipelineTest.kt` |  | Unit |  | 56 ⚑ |
| `TtsCleanerSpeechPipelineTest.autoReadStream_neverSpeaksReasoning` | `TtsCleanerSpeechPipelineTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechPipelineTest.kt` |  | Unit |  | 70 ⚑ |
| `TtsCleanerSpeechPipelineTest.markdownReplyBody_survivesBothFilterStates` | `TtsCleanerSpeechPipelineTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechPipelineTest.kt` |  | Unit |  | 101 ⚑ |
| `UriSerializerAndroidTest.fileUri_roundTrips` | `UriSerializerAndroidTest` | `com.ai.assistance.operit.util` | `UriSerializerAndroidTest.kt` |  | Unit |  | 13 ⚑ |
| `UriSerializerAndroidTest.customScheme_roundTrips` | `UriSerializerAndroidTest` | `com.ai.assistance.operit.util` | `UriSerializerAndroidTest.kt` |  | Unit |  | 20 ⚑ |
| `UriSerializerNullAndroidTest.serializeNull_returnsEmptyStringPayload` | `UriSerializerNullAndroidTest` | `com.ai.assistance.operit.util` | `UriSerializerNullAndroidTest.kt` |  | Unit |  | 13 ⚑ |
| `UriSerializerNullAndroidTest.deserializeEmptyString_returnsNull` | `UriSerializerNullAndroidTest` | `com.ai.assistance.operit.util` | `UriSerializerNullAndroidTest.kt` |  | Unit |  | 17 ⚑ |
| `UriSerializerSchemeAndroidTest.contentScheme_isPreserved` | `UriSerializerSchemeAndroidTest` | `com.ai.assistance.operit.util` | `UriSerializerSchemeAndroidTest.kt` |  | Unit |  | 13 ⚑ |
| `UriSerializerSchemeAndroidTest.fileScheme_isPreserved` | `UriSerializerSchemeAndroidTest` | `com.ai.assistance.operit.util` | `UriSerializerSchemeAndroidTest.kt` |  | Unit |  | 18 ⚑ |
| `AndroidUserPathUtils.currentUserId` | `AndroidUserPathUtils` | `com.ai.assistance.operit.util` | `AndroidUserPathUtils.kt` |  | Int |  | 8 |
| `AndroidUserPathUtils.currentUserDataRootPath` | `AndroidUserPathUtils` | `com.ai.assistance.operit.util` | `AndroidUserPathUtils.kt` |  | String |  | 10 |
| `AndroidUserPathUtils.currentUserPackageDataPath` | `AndroidUserPathUtils` | `com.ai.assistance.operit.util` | `AndroidUserPathUtils.kt` | packageName: String | String |  | 12 |
| `AndroidUserPathUtils.currentUserPackageFilesPath` | `AndroidUserPathUtils` | `com.ai.assistance.operit.util` | `AndroidUserPathUtils.kt` | packageName: String | String |  | 15 |
| `AndroidUserPathUtils.isCurrentUserPackageDataPath` | `AndroidUserPathUtils` | `com.ai.assistance.operit.util` | `AndroidUserPathUtils.kt` | path: String<br>packageName: String | Boolean |  | 18 |
| `AnrCaptureBudget.formatFrames` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | frames: Array<StackTraceElement><br>skipFrames: Int?<br>maxDepth: Int?<br>maxFrameChars: Int?<br>maxChars: Int? | String | Renders [frames] as indented stack lines within the given budget. Rendering stops at [max… | 43 |
| `AnrCaptureBudget.clampDump` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | dump: CharSequence<br>maxChars: Int? | String | Cuts an assembled thread dump to [maxChars] characters, marking the cut. Returns at most … | 83 |
| `AnrCaptureBudget.stackSignature` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | frames: Array<StackTraceElement><br>depth: Int? | String | Builds the identity of a stalled stack, used to recognise a repeated ANR. Only the leadin… | 101 |
| `AnrCaptureThrottle.tryAcquire` | `AnrCaptureThrottle` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | nowMs: Long | Boolean |  | 126 |
| `AnrMonitor.start` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | Unit | 开始ANR监控 | 91 |
| `AnrMonitor.startUsingExecutor` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | Unit | 使用ScheduledExecutorService开始监控（备选方案） | 128 |
| `AnrMonitor.stop` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | Unit | 停止ANR监控 | 150 |
| `AnrMonitor.reportThreadHealthy` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | Unit | 报告主线程正常响应 | 168 |
| `AnrMonitor.reportSlowResponse` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` | responseTime: Long | Unit | 报告主线程响应缓慢 | 175 |
| `AnrMonitor.addCallerInfo` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` | key: String<br>info: String | Unit | 添加调用者信息，帮助跟踪ANR来源 | 195 |
| `AnrMonitor.checkMainThreadHealth` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | Unit | 检查主线程健康状态 | 202 |
| `AnrMonitor.captureMainThreadStack` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | Unit | 捕获主线程堆栈 | 245 |
| `AnrMonitor.getMainThread` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | Thread? | 获取主线程实例的引用 | 274 |
| `AnrMonitor.captureFullThreadDump` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | Unit | 捕获完整的线程转储信息，包括主线程和其他重要线程 | 295 |
| `AnrMonitor.readMainThreadStack` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | MainThreadStack? | 一次性读取主线程堆栈：同一次采样只取一份 stackTrace 数组，供去重签名和转储共用。 | 364 |
| `AnrMonitor.saveAnrReport` | `AnrMonitor` | `com.ai.assistance.operit.util` | `AnrMonitor.kt` |  | Unit | 保存ANR报告到文件 | 423 |
| `AppLogger.bindContext` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | context: Context | Unit |  | 91 |
| `AppLogger.resolveLogFile` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` |  | File? |  | 97 |
| `AppLogger.resolvePackageLogFile` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` |  | File? |  | 119 |
| `AppLogger.prunePackageLogFiles` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | dir: File | Unit |  | 147 |
| `AppLogger.v` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String | Int | --- Public API mirroring com.ai.assistance.operit.util.AppLogger --- | 166 |
| `AppLogger.v` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String<br>tr: Throwable | Int |  | 172 |
| `AppLogger.d` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String | Int |  | 178 |
| `AppLogger.d` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String<br>tr: Throwable | Int |  | 184 |
| `AppLogger.i` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String | Int |  | 190 |
| `AppLogger.i` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String<br>tr: Throwable | Int |  | 196 |
| `AppLogger.w` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String | Int |  | 202 |
| `AppLogger.w` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String<br>tr: Throwable | Int |  | 208 |
| `AppLogger.w` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>tr: Throwable | Int |  | 214 |
| `AppLogger.e` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String | Int |  | 220 |
| `AppLogger.e` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String<br>tr: Throwable | Int |  | 226 |
| `AppLogger.wtf` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String | Int |  | 232 |
| `AppLogger.wtf` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String<br>tr: Throwable | Int |  | 238 |
| `AppLogger.wtf` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>tr: Throwable | Int |  | 244 |
| `AppLogger.isLoggable` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>level: Int | Boolean |  | 250 |
| `AppLogger.println` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | priority: Int<br>tag: String<br>msg: String | Int |  | 255 |
| `AppLogger.getStackTraceString` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tr: Throwable | String |  | 261 |
| `AppLogger.getLogFile` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` |  | File? | Returns the current log file (if available) so that callers can export it. | 269 |
| `AppLogger.resetLogFile` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` |  | Unit |  | 272 |
| `AppLogger.writeToFile` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | priority: Int<br>tag: String<br>msg: String<br>tr: Throwable? | Unit | --- Internal helpers --- | 289 |
| `AppLogger.writeToFileSync` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | priority: Int<br>tag: String<br>msg: String<br>tr: Throwable? | Unit |  | 299 |
| `AppLogger.writeToPackageLogIfNeeded` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String<br>throwableText: String?<br>time: String<br>levelChar: Char | Unit |  | 348 |
| `shouldMirrorToPackageLog` | — | `com.ai.assistance.operit.util` | `AppLogger.kt` | tag: String<br>msg: String | Boolean |  | 405 |
| `normalizeLogMessage` | — | `com.ai.assistance.operit.util` | `AppLogger.kt` | msg: String | String |  | 412 |
| `extractFirstMatch` | — | `com.ai.assistance.operit.util` | `AppLogger.kt` | text: String<br>patterns: List<Pattern> | String? |  | 416 |
| `ArchiveUtil.convertArchive` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | context: Context<br>sourceFile: File<br>targetFile: File<br>sourceExt: String<br>targetExt: String<br>extraParams: String??<br>password: String?? | Boolean | Convert between archive formats or extract | 24 |
| `ArchiveUtil.ensureDirectoryExists` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | directory: File | Boolean | Create directory if it doesn't exist | 102 |
| `ArchiveUtil.extractArchive` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | archiveFile: File<br>extractDir: File<br>archiveExt: String<br>password: String?? | Boolean | Extract an archive file | 111 |
| `ArchiveUtil.extractZip` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | zipFile: File<br>targetDir: File<br>password: String?? | Boolean | Extract a zip file | 136 |
| `ArchiveUtil.extractTar` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | tarFile: File<br>targetDir: File | Boolean | Extract a tar file | 206 |
| `ArchiveUtil.extract7z` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | sevenZFile: File<br>targetDir: File<br>password: String?? | Boolean | Extract a 7z file | 259 |
| `ArchiveUtil.extractRar` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | rarFile: File<br>targetDir: File<br>password: String?? | Boolean | Extract a RAR file | 349 |
| `ArchiveUtil.createArchive` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | sourceDir: File<br>targetFile: File<br>archiveExt: String | Boolean | Create an archive from a directory | 435 |
| `ArchiveUtil.createZip` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | sourceDir: File<br>zipFile: File | Boolean | Create a zip file from a directory | 451 |
| `ArchiveUtil.addToZip` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | baseDir: File<br>currentDir: File<br>zos: ZipOutputStream | Unit | Add files to a zip archive recursively | 464 |
| `ArchiveUtil.createTar` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | sourceDir: File<br>tarFile: File | Boolean | Create a tar file from a directory | 492 |
| `ArchiveUtil.addToTar` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | baseDir: File<br>currentDir: File<br>tos: TarArchiveOutputStream | Unit | Add files to a TAR archive recursively | 507 |
| `ArchiveUtil.create7z` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | sourceDir: File<br>sevenZFile: File | Boolean | Create a 7z file from a directory | 536 |
| `ArchiveUtil.addTo7z` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | baseDir: File<br>currentDir: File<br>szof: SevenZOutputFile | Unit | Add files to a 7z archive recursively | 547 |
| `AssetCopyUtils.copyAssetToCache` | `AssetCopyUtils` | `com.ai.assistance.operit.util` | `AssetCopyUtils.kt` | context: Context<br>assetPath: String<br>overwrite: Boolean? | File |  | 10 |
| `AssetCopyUtils.copyAssetToFile` | `AssetCopyUtils` | `com.ai.assistance.operit.util` | `AssetCopyUtils.kt` | context: Context<br>assetPath: String<br>outputFile: File<br>overwrite: Boolean? | File |  | 19 |
| `AssetCopyUtils.copyAssetDirToCache` | `AssetCopyUtils` | `com.ai.assistance.operit.util` | `AssetCopyUtils.kt` | context: Context<br>assetDir: String<br>targetDir: File<br>overwrite: Boolean? | File |  | 47 |
| `AssetCopyUtils.copyAssetDirRecursive` | `AssetCopyUtils` | `com.ai.assistance.operit.util` | `AssetCopyUtils.kt` | context: Context<br>assetDir: String<br>targetDir: File<br>overwrite: Boolean? | File |  | 79 |
| `ChatMarkupRegex.isToolTagName` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | tagName: String? | Boolean |  | 202 |
| `ChatMarkupRegex.isToolResultTagName` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | tagName: String? | Boolean |  | 206 |
| `ChatMarkupRegex.normalizeToolLikeTagName` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | tagName: String? | String? |  | 210 |
| `ChatMarkupRegex.containsToolTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | Boolean |  | 218 |
| `ChatMarkupRegex.containsToolResultTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | Boolean |  | 222 |
| `ChatMarkupRegex.containsAnyToolLikeTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | Boolean |  | 226 |
| `ChatMarkupRegex.extractOpeningTagName` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | xml: String | String? |  | 230 |
| `ChatMarkupRegex.generateRandomToolTagName` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` |  | String |  | 234 |
| `ChatMarkupRegex.generateRandomToolResultTagName` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` |  | String |  | 236 |
| `ChatMarkupRegex.geminiThoughtSignatureMetaTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | signatureBase64: String | String |  | 238 |
| `ChatMarkupRegex.openAiResponsesReasoningMetaTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | payloadBase64: String | String |  | 242 |
| `ChatMarkupRegex.openAiResponsesOutputItemMetaTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | payloadBase64: String | String |  | 246 |
| `ChatMarkupRegex.extractGeminiThoughtSignature` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | String? |  | 250 |
| `ChatMarkupRegex.extractOpenAiResponsesReasoningPayloads` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | List<String> |  | 267 |
| `ChatMarkupRegex.extractOpenAiResponsesOutputItemPayloads` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | List<String> |  | 271 |
| `ChatMarkupRegex.extractMetaPayloads` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String<br>expectedProvider: String | List<String> |  | 275 |
| `ChatMarkupRegex.removeGeminiThoughtSignatureMeta` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | String |  | 292 |
| `ChatMarkupRegex.removeOpenAiResponsesReasoningMeta` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | String |  | 296 |
| `ChatMarkupRegex.removeOpenAiResponsesOutputItemMeta` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | String |  | 300 |
| `ChatMarkupRegex.removeOpenAiResponsesProtocolMeta` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String | String |  | 304 |
| `ChatMarkupRegex.removeMetaByProvider` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | content: String<br>expectedProvider: String | String |  | 308 |
| `ChatMarkupRegex.extractMetaProvider` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | metaTagContent: String | String? |  | 322 |
| `ChatMarkupRegex.generateRandomTagCode` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | length: Int? | String |  | 329 |
| `ChatTrace.sha256` | `ChatTrace` | `com.ai.assistance.operit.util` | `ChatTrace.kt` | text: String | String | Returns the lowercase hex SHA-256 of [text] encoded as UTF-8. | 18 |
| `ChatTrace.describe` | `ChatTrace` | `com.ai.assistance.operit.util` | `ChatTrace.kt` | text: String<br>byteLength: Int??<br>previewChars: Int? | String | Describes [text] for a log line: character length, optional byte length, digest prefix an… | 27 |
| `ChatTrace.preview` | `ChatTrace` | `com.ai.assistance.operit.util` | `ChatTrace.kt` | text: String<br>from: Int<br>count: Int | String |  | 37 |
| `ChatUtils.stripGeminiThoughtSignatureMeta` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | content: String | String |  | 20 |
| `ChatUtils.stripGeminiThoughtSignatureMeta` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | messages: List<Pair<String, String>> | List<Pair<String, String>> |  | 24 |
| `ChatUtils.stripGeminiThoughtSignatureMetaTurns` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | messages: List<PromptTurn> | List<PromptTurn> |  | 30 |
| `ChatUtils.stripOpenAiResponsesReasoningMeta` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | content: String | String |  | 36 |
| `ChatUtils.stripOpenAiResponsesReasoningMetaTurns` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | messages: List<PromptTurn> | List<PromptTurn> |  | 40 |
| `ChatUtils.stripOpenAiResponsesProtocolMeta` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | content: String | String |  | 46 |
| `ChatUtils.stripOpenAiResponsesProtocolMarkup` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | content: String | String |  | 50 |
| `ChatUtils.stripOpenAiResponsesProtocolMarkupTurns` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | messages: List<PromptTurn> | List<PromptTurn> |  | 57 |
| `ChatUtils.isGeminiProviderModel` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | providerModel: String | Boolean |  | 63 |
| `ChatUtils.removeThinkingContent` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | content: String | String | 过滤掉内容中的思考部分和搜索来源 移除<think></think>、<thinking></thinking>和<search></search>标签及其中的内容，并处理未闭合… | 71 |
| `ChatUtils.extractThinkingContent` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | content: String | Pair<String, String> | 提取think标签内的内容（用于DeepSeek的reasoning_content） | 83 |
| `ChatUtils.containsThinkOrSearchMarkup` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | content: String | Boolean |  | 94 |
| `ChatUtils.estimateTokenCount` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | text: String | Long | 估算给定文本的token数量 | 104 |
| `ChatUtils.extractJson` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | response: String | String | 从 AI 响应中提取 JSON 对象部分 AI 可能会在 JSON 前后添加说明文字或使用 ```json 代码块，需要提取出纯净的 JSON | 115 |
| `ChatUtils.extractJsonArray` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | response: String | String | 从 AI 响应中提取 JSON 数组部分 AI 可能会在 JSON 前后添加说明文字或使用 ```json 代码块，需要提取出纯净的 JSON | 140 |
| `ColorQrCodeUtil.generate` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | payload: ByteArray<br>colorCount: Int<br>moduleSizePx: Int?<br>marginModules: Int? | Bitmap |  | 43 |
| `ColorQrCodeUtil.generate` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | text: String<br>colorCount: Int<br>charset: Charset?<br>moduleSizePx: Int?<br>marginModules: Int? | Bitmap |  | 93 |
| `ColorQrCodeUtil.decode` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | bitmap: Bitmap<br>expectedColorCount: Int?? | DecodeResult |  | 105 |
| `ColorQrCodeUtil.decodeToString` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | bitmap: Bitmap<br>expectedColorCount: Int??<br>charset: Charset? | String |  | 202 |
| `ColorQrCodeUtil.isGzip` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | bytes: ByteArray | Boolean |  | 216 |
| `ColorQrCodeUtil.gzipIfBeneficial` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | bytes: ByteArray | ByteArray |  | 220 |
| `ColorQrCodeUtil.gunzip` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | bytes: ByteArray | ByteArray |  | 231 |
| `ColorQrCodeUtil.cropToQrRegion` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | bitmap: Bitmap<br>paddingRatio: Float? | Bitmap? |  | 245 |
| `ColorQrCodeUtil.createTransformFromDetectorPoints` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | points: Array<com.google.zxing.ResultPoint><br>dimension: Int | PerspectiveTransform |  | 301 |
| `ColorQrCodeUtil.readSymbols` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | bitmap: Bitmap<br>transform: PerspectiveTransform<br>functionPattern: com.google.zxing.common.BitMatrix<br>palette: IntArray<br>hueOffsetDegrees: Float?<br>maxSymbols: Int?? | IntArray |  | 349 |
| `ColorQrCodeUtil.requiredSymbolCount` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | byteCount: Int<br>bitsPerSymbol: Int | Int |  | 408 |
| `ColorQrCodeUtil.sampleColor` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | bitmap: Bitmap<br>x: Int<br>y: Int | Int |  | 413 |
| `ColorQrCodeUtil.decodeBytesFromSymbols` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | symbols: IntArray<br>bitsPerSymbol: Int<br>byteCount: Int | ByteArray |  | 433 |
| `ColorQrCodeUtil.readBit` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` |  | Int |  | 446 |
| `ColorQrCodeUtil.buildHeader` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | payload: ByteArray<br>colorCount: Int | ByteArray |  | 469 |
| `ColorQrCodeUtil.chooseVersion` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | totalBytes: Int<br>bitsPerSymbol: Int | Version |  | 479 |
| `ColorQrCodeUtil.buildFunctionPattern` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | version: Version | com.google.zxing.common.BitMatrix |  | 492 |
| `ColorQrCodeUtil.countSetBits` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | matrix: com.google.zxing.common.BitMatrix | Int |  | 534 |
| `ColorQrCodeUtil.buildSkeletonQr` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | version: Version | com.google.zxing.qrcode.encoder.QRCode |  | 546 |
| `ColorQrCodeUtil.bitsPerSymbol` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | colorCount: Int | Int |  | 553 |
| `ColorQrCodeUtil.paletteFor` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | colorCount: Int | IntArray |  | 563 |
| `ColorQrCodeUtil.paletteForLegacy` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | colorCount: Int | IntArray |  | 575 |
| `ColorQrCodeUtil.nearestPaletteIndex` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | color: Int<br>palette: IntArray<br>hueOffsetDegrees: Float? | Int |  | 587 |
| `ColorQrCodeUtil.fillModule` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | pixels: IntArray<br>imageWidth: Int<br>moduleX: Int<br>moduleY: Int<br>moduleSize: Int<br>color: Int | Unit |  | 621 |
| `ColorQrCodeUtil.crc32` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | bytes: ByteArray | Int |  | 632 |
| `ColorQrCodeUtil.writeIntBE` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | buf: ByteArray<br>offset: Int<br>value: Int | Unit |  | 638 |
| `ColorQrCodeUtil.readIntBE` | `ColorQrCodeUtil` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | buf: ByteArray<br>offset: Int | Int |  | 645 |
| `ColorQrCodeUtil.BitReader.readBits` | `BitReader` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` | n: Int | Int |  | 656 |
| `ColorQrCodeUtil.BitReader.readBit` | `BitReader` | `com.ai.assistance.operit.util` | `ColorQrCodeUtil.kt` |  | Int |  | 664 |
| `CrashRecoveryState.markPendingCrashReportLaunch` | `CrashRecoveryState` | `com.ai.assistance.operit.util` | `CrashRecoveryState.kt` | context: Context | Unit |  | 9 |
| `CrashRecoveryState.consumePendingCrashReportLaunch` | `CrashRecoveryState` | `com.ai.assistance.operit.util` | `CrashRecoveryState.kt` | context: Context | Boolean |  | 17 |
| `DocumentConversionUtil.convertTextToPdf` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | context: Context<br>sourceFile: File<br>targetFile: File | Boolean | Convert text to PDF | 39 |
| `DocumentConversionUtil.extractTextFromPdf` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | context: Context<br>sourceFile: File<br>targetFile: File | Boolean | Extract text from PDF, with OCR fallback for image-based PDFs. | 77 |
| `DocumentConversionUtil.convertPdfToTextWithOcr` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | context: Context<br>sourceFile: File<br>targetFile: File | Boolean | Converts each page of a PDF to an image and uses OCR to extract text. | 118 |
| `DocumentConversionUtil.convertPdfToImage` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | sourceFile: File<br>targetFile: File<br>targetExt: String | Boolean | Convert PDF to image | 169 |
| `DocumentConversionUtil.convertBetweenDocFormats` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | context: Context<br>sourceFile: File<br>targetFile: File<br>sourceExt: String<br>targetExt: String | Boolean | Convert between DOC and DOCX formats using Apache POI | 241 |
| `DocumentConversionUtil.convertFromHtml` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | context: Context<br>sourceFile: File<br>targetFile: File<br>targetExt: String | Boolean | Convert HTML to other formats | 360 |
| `DocumentConversionUtil.convertToHtml` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | context: Context<br>sourceFile: File<br>targetFile: File<br>sourceExt: String | Boolean | Convert various document formats to HTML | 454 |
| `DocumentConversionUtil.convertSpreadsheetToHtml` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | sourceFile: File<br>targetFile: File | Boolean | Convert XLS/XLSX spreadsheet documents to HTML | 645 |
| `copyTextFile` | — | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | sourceFile: File<br>targetFile: File | Boolean | Copy text file with format conversion | 774 |
| `extractTextFromDoc` | — | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | sourceFile: File<br>targetFile: File | Boolean | Convert DOC file directly to plain text | 786 |
| `extractTextFromDocx` | — | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | sourceFile: File<br>targetFile: File | Boolean | Convert DOCX file directly to plain text | 809 |
| `optimizeTextFormat` | — | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | text: String | String | 优化提取出的文本格式，压缩连续空行 | 832 |
| `extractTextFromWord` | — | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | sourceFile: File<br>targetFile: File<br>sourceExt: String | Boolean | General method to convert Word documents to text | 861 |
| `convertPdfToDocx` | — | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | context: Context<br>sourceFile: File<br>targetFile: File | Boolean | Convert PDF to DOCX | 870 |
| `convertWordToPdf` | — | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | context: Context<br>sourceFile: File<br>targetFile: File<br>sourceExt: String | Boolean | Convert Word (DOC/DOCX) to PDF | 918 |
| `columnName` | — | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | index: Int | String |  | 951 |
| `stripNullCharacters` | — | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | text: String | String | 移除提取文本中的 U+0000。 PDF 字体映射缺字时 PDFBox 会输出 NUL，SQLite 的 LENGTH/SUBSTR 会把 TEXT 在第一个 NUL 处截断，导… | 968 |
| `FFmpegUtil.scaleFilterMaxWidth` | `FFmpegUtil` | `com.ai.assistance.operit.util` | `FFmpegUtil.kt` | maxWidth: Int | String | Build a scale filter string that survives FFmpegKit argument parsing. FFmpeg expressions … | 19 |
| `FFmpegUtil.executeCommand` | `FFmpegUtil` | `com.ai.assistance.operit.util` | `FFmpegUtil.kt` | command: String | Boolean | Execute an FFmpeg command and return if it was successful | 24 |
| `FFmpegUtil.getMediaInfo` | `FFmpegUtil` | `com.ai.assistance.operit.util` | `FFmpegUtil.kt` | filePath: String | MediaInformation? | Get media information for a file | 49 |
| `FileUtils.isTextBasedExtension` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | extension: String | Boolean | Checks if a file extension corresponds to a text-based file format. | 62 |
| `FileUtils.isTextBasedFileName` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | fileName: String | Boolean |  | 66 |
| `FileUtils.isTextLike` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | file: File<br>sampleSize: Int? | Boolean | Checks if a file appears to be text-like by reading its first few bytes. This is more rel… | 86 |
| `FileUtils.isTextLike` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | path: String<br>sampleSize: Int? | Boolean | Checks if a file appears to be text-like by reading its first few bytes from a path. This… | 121 |
| `FileUtils.isTextLike` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | bytes: ByteArray | Boolean | Check if the given byte array appears to be text content. This is useful when you already… | 132 |
| `FileUtils.isTextLikeBytes` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | bytes: ByteArray<br>length: Int | Boolean | Analyzes a byte array to determine if it contains text-like content. Algorithm: - Checks … | 149 |
| `FileUtils.isTextBasedFile` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | file: File | Boolean | Checks if a file is a text-based file, considering both extension and filename. | 220 |
| `FileUtils.isWorkspaceFile` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | file: File<br>workspaceRoot: File<br>gitignoreRules: List<String> | Boolean | Checks if a file is a valid workspace file to be shown or backed up. This combines severa… | 242 |
| `FileUtils.isVideoFile` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | context: Context<br>uri: Uri | Boolean | Check if a URI points to a video file | 260 |
| `FileUtils.getFileExtension` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | context: Context<br>uri: Uri | String? | Get the file extension from a URI | 276 |
| `FileUtils.copyFileToInternalStorage` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | context: Context<br>uri: Uri<br>uniqueName: String | Uri? | Copies a file from a given URI to the app's internal storage. This makes the file private… | 296 |
| `FileUtils.getFileExtensionFromUri` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | context: Context<br>uri: Uri | String? | Get the file extension from a URI | 341 |
| `cleanOldBackgroundFiles` | — | `com.ai.assistance.operit.util` | `FileUtils.kt` | directory: File<br>currentFileName: String | Unit | Clean up old background media files to prevent using too much storage Keeps only the most… | 381 |
| `checkVideoSize` | — | `com.ai.assistance.operit.util` | `FileUtils.kt` | context: Context<br>uri: Uri<br>maxSizeMB: Int? | Boolean | 检查视频文件大小是否超过限制 | 404 |
| `GithubReleaseUtil.parseAssetDigest` | `GithubReleaseUtil` | `com.ai.assistance.operit.util` | `GithubReleaseUtil.kt` | digest: String? | String? | Normalise the GitHub asset `digest` field (`sha256:<hex>`) to a bare lowercase hex string… | 58 |
| `GithubReleaseUtil.getMirroredUrls` | `GithubReleaseUtil` | `com.ai.assistance.operit.util` | `GithubReleaseUtil.kt` | originalUrl: String | Map<String, String> | 获取镜像加速 URL 用于加速 GitHub 下载 | 110 |
| `GithubReleaseUtil.getDownloadSources` | `GithubReleaseUtil` | `com.ai.assistance.operit.util` | `GithubReleaseUtil.kt` | originalUrl: String | Map<String, String> | Every source an artifact can be fetched from, keyed by source name: the official GitHub U… | 129 |
| `GithubReleaseUtil.probeMirrorUrls` | `GithubReleaseUtil` | `com.ai.assistance.operit.util` | `GithubReleaseUtil.kt` | urls: Map<String, String><br>timeoutMs: Int? | Map<String, ProbeResult> |  | 132 |
| `GithubReleaseUtil.probeOneUrl` | `GithubReleaseUtil` | `com.ai.assistance.operit.util` | `GithubReleaseUtil.kt` | url: String<br>timeoutMs: Int | ProbeResult | Probe one candidate source by sampling its first bytes. The probe must apply exactly the … | 162 |
| `GithubReleaseUtil.fetchLatestReleaseInfo` | `GithubReleaseUtil` | `com.ai.assistance.operit.util` | `GithubReleaseUtil.kt` | repoOwner: String<br>repoName: String | ReleaseInfo? | 获取最新的 Release 信息 如果用户已登录，会自动带上认证头以提高 API 配额 | 264 |
| `GlobalExceptionHandler.uncaughtException` | `GlobalExceptionHandler` | `com.ai.assistance.operit.util` | `GlobalExceptionHandler.kt` | thread: Thread<br>ex: Throwable | Unit |  | 10 |
| `HtmlParserUtil.getExtractionScript` | `HtmlParserUtil` | `com.ai.assistance.operit.util` | `HtmlParserUtil.kt` |  | String |  | 10 |
| `HtmlParserUtil.parseAndSimplify` | `HtmlParserUtil` | `com.ai.assistance.operit.util` | `HtmlParserUtil.kt` | jsonString: String<br>updateInteractionMap: (Map<Int, String>) -> Unit | ComputerPageInfoNode? |  | 218 |
| `HttpLogSanitizer.urlForLog` | `HttpLogSanitizer` | `com.ai.assistance.operit.util` | `HttpLogSanitizer.kt` | url: HttpUrl | String |  | 7 |
| `HttpLogSanitizer.headersForLog` | `HttpLogSanitizer` | `com.ai.assistance.operit.util` | `HttpLogSanitizer.kt` | headers: Headers | String |  | 38 |
| `HttpMultiPartDownloader.download` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | url: String<br>dest: File<br>headers: Map<String, String>?<br>threadCount: Int?<br>onProgress: ((downloadedBytes: Long, totalBytes…? | Unit |  | 25 |
| `HttpMultiPartDownloader.probeDownload` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | url: String<br>headers: Map<String, String>? | ProbeResult |  | 46 |
| `HttpMultiPartDownloader.buildSegmentPlan` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | totalBytes: Long<br>threadCount: Int | List<SegmentPlan> |  | 101 |
| `HttpMultiPartDownloader.downloadSegment` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | url: String<br>dest: File<br>headers: Map<String, String>?<br>startInclusive: Long?<br>endInclusive: Long??<br>append: Boolean?<br>onChunk: ((chunkBytes: Int) -> Unit)??<br>isCancelled: (() -> Boolean)?? | Unit |  | 124 |
| `HttpMultiPartDownloader.parseTotalFromContentRange` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | contentRange: String? | Long |  | 185 |
| `HttpMultiPartDownloader.downloadSingle` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | url: String<br>dest: File<br>headers: Map<String, String><br>totalBytes: Long<br>onProgress: ((Long, Long) -> Unit)? | Unit |  | 193 |
| `HttpMultiPartDownloader.downloadMulti` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | url: String<br>dest: File<br>headers: Map<String, String><br>totalBytes: Long<br>threadCount: Int<br>onProgress: ((Long, Long) -> Unit)? | Unit |  | 216 |
| `HttpMultiPartDownloader.applyHeaders` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | conn: HttpURLConnection<br>headers: Map<String, String> | Unit |  | 303 |
| `HttpMultiPartDownloader.sanitizeHeaderName` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | name: String? | String? |  | 312 |
| `HttpMultiPartDownloader.sanitizeHeaderValue` | `HttpMultiPartDownloader` | `com.ai.assistance.operit.util` | `HttpMultiPartDownloader.kt` | value: String? | String |  | 320 |
| `ImageBitmapLimiter.decodeDownsampledBitmap` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | bytes: ByteArray<br>maxPixels: Long?<br>maxDimension: Int? | Bitmap? |  | 25 |
| `ImageBitmapLimiter.limitBase64ForAi` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | base64: String<br>mimeType: String | LimitedImage? |  | 62 |
| `ImageBitmapLimiter.encodeBitmap` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | bitmap: Bitmap<br>format: Bitmap.CompressFormat<br>quality: Int | ByteArray |  | 127 |
| `ImageBitmapLimiter.compressFormatForMimeType` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | mimeType: String | Bitmap.CompressFormat? |  | 135 |
| `ImageBitmapLimiter.decodeImageBounds` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | bytes: ByteArray | ImageBounds? |  | 145 |
| `ImageBitmapLimiter.calculateSampleSize` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | srcWidth: Int<br>srcHeight: Int<br>maxPixels: Long<br>maxDimension: Int | Int |  | 159 |
| `ImagePoolManager.removeEldestEntry` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | eldest: Map.Entry<String, ImageData>? | Boolean |  | 85 |
| `ImagePoolManager.defaultRegistrationOptions` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` |  | ImageRegistrationOptions |  | 95 |
| `ImagePoolManager.initialize` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | cacheDirPath: File<br>preloadNow: Boolean? | Unit |  | 97 |
| `ImagePoolManager.addImage` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | filePath: String<br>options: ImageRegistrationOptions?? | String |  | 123 |
| `ImagePoolManager.addImageFromBase64` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | base64: String<br>mimeType: String<br>options: ImageRegistrationOptions?? | String |  | 151 |
| `ImagePoolManager.addImageFromBitmap` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | bitmap: Bitmap<br>mimeType: String<br>options: ImageRegistrationOptions?? | String |  | 177 |
| `ImagePoolManager.getImage` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | id: String | ImageData? |  | 196 |
| `ImagePoolManager.getImageMimeType` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | id: String | String? |  | 223 |
| `ImagePoolManager.removeImage` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | id: String | Unit |  | 226 |
| `ImagePoolManager.clear` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` |  | Unit |  | 234 |
| `ImagePoolManager.size` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` |  | Int |  | 241 |
| `ImagePoolManager.preloadFromDisk` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` |  | Unit |  | 244 |
| `ImagePoolManager.registerBitmap` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | sourceBitmap: Bitmap<br>sourceMimeType: String<br>options: ImageRegistrationOptions?<br>sourcePath: String??<br>recycleSource: Boolean | String |  | 248 |
| `ImagePoolManager.resolveOptions` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | options: ImageRegistrationOptions? | ResolvedRegistrationOptions |  | 360 |
| `ImagePoolManager.normalizeBase64Input` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | base64: String<br>mimeType: String | NormalizedBase64Input |  | 380 |
| `ImagePoolManager.decodeBitmapFromFile` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | filePath: String | Bitmap? |  | 399 |
| `ImagePoolManager.decodeBitmapFromBytes` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | bytes: ByteArray | Bitmap? |  | 411 |
| `ImagePoolManager.detectImageMimeTypeFromBytes` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | bytes: ByteArray | String? |  | 423 |
| `ImagePoolManager.normalizeImageDataMimeTypeIfNeeded` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | id: String<br>imageData: ImageData | ImageData |  | 436 |
| `ImagePoolManager.normalizeBitmapOrientationIfNeeded` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | bitmap: Bitmap<br>filePath: String | Bitmap |  | 456 |
| `ImagePoolManager.scaleBitmapIfNeeded` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | bitmap: Bitmap<br>scalePercent: Int | Bitmap |  | 498 |
| `ImagePoolManager.limitBitmapLongEdgeIfNeeded` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | bitmap: Bitmap<br>maxLongEdge: Int? | Bitmap |  | 513 |
| `ImagePoolManager.resolveOutputFormat` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | bitmap: Bitmap<br>outputFormat: ImageOutputFormat | ImageOutputFormat |  | 530 |
| `ImagePoolManager.flattenAlphaForJpeg` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | bitmap: Bitmap | Bitmap |  | 542 |
| `ImagePoolManager.encodeBitmap` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | bitmap: Bitmap<br>outputFormat: ImageOutputFormat<br>jpegQuality: Int | ByteArray |  | 553 |
| `ImagePoolManager.getMimeTypeFromFile` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | file: File | String? |  | 579 |
| `ImagePoolManager.saveToDisk` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | id: String<br>imageData: ImageData | Unit |  | 601 |
| `ImagePoolManager.loadFromDisk` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | id: String | ImageData? |  | 624 |
| `ImagePoolManager.loadAllFromDisk` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` |  | Unit |  | 650 |
| `ImagePoolManager.deleteFromDisk` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | id: String | Unit |  | 669 |
| `ImagePoolManager.clearDiskCache` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` |  | Unit |  | 681 |
| `IntRangeSerializer.serialize` | `IntRangeSerializer` | `com.ai.assistance.operit.util` | `IntRangeSerializer.kt` | encoder: Encoder<br>value: IntRange | Unit |  | 18 |
| `IntRangeSerializer.deserialize` | `IntRangeSerializer` | `com.ai.assistance.operit.util` | `IntRangeSerializer.kt` | decoder: Decoder | IntRange |  | 25 |
| `LatexMathMlConverter.convertAll` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | context: Context<br>formulas: List<String> | List<String> |  | 18 |
| `LatexMathMlConverter.getEngine` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | context: Context | OperitQuickJsEngine |  | 50 |
| `LatexMathMlConverter.createEngine` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | context: Context | OperitQuickJsEngine |  | 57 |
| `LocalDateTimeSerializer.serialize` | `LocalDateTimeSerializer` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializer.kt` | encoder: Encoder<br>value: LocalDateTime | Unit |  | 17 |
| `LocalDateTimeSerializer.deserialize` | `LocalDateTimeSerializer` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializer.kt` | decoder: Decoder | LocalDateTime |  | 21 |
| `LocaleUtils.getSupportedLanguages` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` |  | List<Language> | 获取支持的语言列表 | 64 |
| `LocaleUtils.getLocaleForLanguageCode` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | languageCode: String<br>context: Context?? | Locale |  | 68 |
| `LocaleUtils.createLocaleOverrideConfiguration` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | locale: Locale | Configuration |  | 82 |
| `LocaleUtils.createCompatLocaleList` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | locale: Locale | LocaleListCompat | 日本語で未翻訳の項目は英語リソースを使用し、中国語の既定リソースを表示しない。 | 97 |
| `LocaleUtils.createPlatformLocaleList` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | locale: Locale | LocaleList |  | 105 |
| `LocaleUtils.setDefaultLocales` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | locale: Locale | Unit |  | 113 |
| `LocaleUtils.usesChineseContent` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | context: Context | Boolean | 中国語専用コンテンツを選ぶ必要がある場合だけtrueを返す。 | 121 |
| `LocaleUtils.getLocalizedContext` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | context: Context | Context | 获取包含当前应用语言设置的上下文。 对于使用applicationContext的单例或服务，这非常有用， 因为它可以确保获取到最新的本地化资源。 | 135 |
| `LocaleUtils.getCurrentLanguage` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | context: Context | String | 获取当前应用设置的语言 | 146 |
| `LocaleUtils.getCurrentSystemLanguage` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | context: Context | String | 获取系统当前语言 | 161 |
| `LocaleUtils.setAppLanguage` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | context: Context<br>languageCode: String | Unit | 设置应用语言 | 170 |
| `LocaleUtils.getCurrentSystemLocale` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | context: Context | Locale |  | 230 |
| `LocaleUtils.getCurrentSystemLanguageCode` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | context: Context | String |  | 239 |
| `LocaleUtils.normalizeStoredLanguageCode` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | languageCode: String | String |  | 243 |
| `LocaleUtils.resolveSupportedLanguageCode` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | languageCode: String | String |  | 258 |
| `LocationUtils.isDeviceInMainlandChina` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | context: Context | Boolean | 使用安卓原生API，检测设备是否在中国大陆。 此方法不依赖任何Google Play Services。 | 35 |
| `LocationUtils.getCurrentLocationNative` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | context: Context<br>locationManager: LocationManager | Location | 封装原生API的回调，以协程方式获取当前位置。 | 68 |
| `LocationUtils.onLocationChanged` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | location: Location | Unit |  | 90 |
| `LocationUtils.onProviderDisabled` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | provider: String | Unit |  | 94 |
| `LocationUtils.getCountryFromLocation` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | context: Context<br>location: Location | Boolean | 将Location对象通过Geocoder转换为国家代码并进行判断。 | 108 |
| `LocationUtils.onGeocode` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | results: MutableList<Address> | Unit |  | 120 |
| `LocationUtils.onError` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | errorMessage: String? | Unit |  | 124 |
| `LocationUtils.isWithinMainlandChinaBounds` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | lat: Double<br>lon: Double | Boolean |  | 160 |
| `LocationUtils.getCountryIsoByTelephony` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | context: Context | String? |  | 170 |
| `LocationUtils.isChinaTimezone` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` |  | Boolean |  | 183 |
| `LocationUtils.hasLocationPermission` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | context: Context | Boolean | 检查应用是否具有粗略或精细位置权限。 | 195 |
| `MathMlPlainTextConverter.convert` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | mathMl: String | String |  | 9 |
| `MathMlPlainTextConverter.render` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | node: Node | String |  | 22 |
| `MathMlPlainTextConverter.renderChildren` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | element: Element | String |  | 100 |
| `MathMlPlainTextConverter.renderOperator` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | operator: String | String |  | 103 |
| `MathMlPlainTextConverter.appendLargeOperatorSpacing` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | base: String<br>expression: String | String |  | 112 |
| `MathMlPlainTextConverter.toSuperscript` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | value: String | String? |  | 115 |
| `MathMlPlainTextConverter.toSubscript` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | value: String | String? |  | 118 |
| `MediaBase64Limiter.estimateDecodedSizeBytes` | `MediaBase64Limiter` | `com.ai.assistance.operit.util` | `MediaBase64Limiter.kt` | base64: String | Int? |  | 13 |
| `limitBase64ForAi` | — | `com.ai.assistance.operit.util` | `MediaBase64Limiter.kt` | base64: String<br>mimeType: String<br>maxDecodedBytes: Int? | LimitedMedia? |  | 41 |
| `MediaPoolManager.q` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | path: String | String |  | 16 |
| `MediaPoolManager.transcodeToFit` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | source: File<br>mimeType: String<br>targetBytes: Long | TranscodedMedia? |  | 23 |
| `MediaPoolManager.ok` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | out: File | Boolean |  | 28 |
| `MediaPoolManager.extForMimeType` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | mimeType: String | String |  | 76 |
| `MediaPoolManager.decodeBase64ToFile` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | base64: String<br>outFile: File | Unit |  | 90 |
| `MediaPoolManager.AsciiStringInputStream.read` | `AsciiStringInputStream` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` |  | Int |  | 107 |
| `MediaPoolManager.AsciiStringInputStream.read` | `AsciiStringInputStream` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | b: ByteArray<br>off: Int<br>len: Int | Int |  | 112 |
| `MediaPoolManager.initialize` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | cacheDirPath: File<br>preloadNow: Boolean? | Unit |  | 138 |
| `MediaPoolManager.preloadFromDisk` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` |  | Unit |  | 150 |
| `MediaPoolManager.removeEldestEntry` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | eldest: MutableMap.MutableEntry<String, Med… | Boolean |  | 155 |
| `MediaPoolManager.addMedia` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | filePath: String<br>mimeType: String | String |  | 166 |
| `MediaPoolManager.addMediaFromBase64` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | base64: String<br>mimeType: String | String |  | 220 |
| `MediaPoolManager.getMedia` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | id: String | MediaData? |  | 303 |
| `MediaPoolManager.loadOneFromDisk` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | id: String | MediaData? |  | 312 |
| `MediaPoolManager.removeMedia` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | id: String | Unit |  | 333 |
| `MediaPoolManager.saveToDisk` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | id: String<br>data: MediaData | Unit |  | 338 |
| `MediaPoolManager.deleteFromDisk` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | id: String | Unit |  | 350 |
| `MediaPoolManager.loadAllFromDisk` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` |  | Unit |  | 360 |
| `NetworkUtils.isNetworkAvailable` | `NetworkUtils` | `com.ai.assistance.operit.util` | `NetworkUtils.kt` | context: Context | Boolean | 检查设备是否连接到网络 | 12 |
| `NetworkUtils.getNetworkType` | `NetworkUtils` | `com.ai.assistance.operit.util` | `NetworkUtils.kt` | context: Context | String | 获取网络连接类型 | 26 |
| `OCRUtils.getRecognizer` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | language: Language | TextRecognizer | 初始化识别器 | 54 |
| `OCRUtils.preprocessBitmap` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | bitmap: Bitmap | Bitmap | 对Bitmap进行预处理以提高OCR识别率 | 97 |
| `OCRUtils.recognizeTextFromBitmap` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | bitmap: Bitmap<br>language: Language?<br>quality: Quality? | OCRResult | 从Bitmap识别文本（同步方法） | 139 |
| `OCRUtils.recognizeTextFromUri` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | context: Context<br>uri: Uri<br>language: Language?<br>quality: Quality? | OCRResult | 从Uri识别文本（同步方法） | 176 |
| `OCRUtils.processImage` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | image: InputImage<br>language: Language | Text | 处理图像并识别文本 | 219 |
| `OCRUtils.recognizeText` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | context: Context<br>bitmap: Bitmap<br>quality: Quality? | String | 识别图像中的文本（同时识别拉丁文和中文） | 242 |
| `OCRUtils.recognizeText` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | context: Context<br>bitmap: Bitmap<br>language: Language<br>quality: Quality? | String | 识别图像中的文本（指定语言） | 273 |
| `OCRUtils.recognizeText` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | context: Context<br>uri: Uri<br>quality: Quality? | String | 从文件Uri识别文本（同时识别拉丁文和中文） | 298 |
| `OCRUtils.extractTextBlocks` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | bitmap: Bitmap<br>languages: List<Language>?<br>quality: Quality? | List<String> | 扫描并提取图像中所有的文本块 | 324 |
| `OCRUtils.saveBitmapToTempFile` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | context: Context<br>bitmap: Bitmap | File? | 保存Bitmap到临时文件，用于OCR处理 | 353 |
| `OCRUtils.closeRecognizers` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` |  | Unit | 清理资源 | 370 |
| `OCRUtils.OCRResult.Success.getFullText` | `Success` | `com.ai.assistance.operit.util` | `OCRUtils.kt` |  | String | 获取识别到的完整文本 | 389 |
| `OCRUtils.OCRResult.Success.getTextBlocks` | `Success` | `com.ai.assistance.operit.util` | `OCRUtils.kt` |  | List<Text.TextBlock> | 获取所有文本块 | 392 |
| `OCRUtils.OCRResult.Success.getStructuredText` | `Success` | `com.ai.assistance.operit.util` | `OCRUtils.kt` |  | String | 获取结构化文本信息 | 395 |
| `OperitPaths.downloadsDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 27 |
| `OperitPaths.operitRootDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 31 |
| `OperitPaths.cleanOnExitDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 35 |
| `OperitPaths.pluginsDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 39 |
| `OperitPaths.pluginConfigDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | pluginId: String | File |  | 43 |
| `OperitPaths.cleanOnExitInternalDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | context: Context | File |  | 59 |
| `OperitPaths.mcpPluginsDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 63 |
| `OperitPaths.bridgeDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 67 |
| `OperitPaths.exportsDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 71 |
| `OperitPaths.workspaceDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 75 |
| `OperitPaths.testDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 79 |
| `OperitPaths.webSessionDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 83 |
| `OperitPaths.webSessionUserscriptsDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | File |  | 87 |
| `OperitPaths.sherpaNcnnModelsDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | context: Context | File |  | 91 |
| `OperitPaths.vectorIndexDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | context: Context | File |  | 95 |
| `OperitPaths.imagePoolDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | baseDir: File | File |  | 99 |
| `OperitPaths.mediaPoolDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | baseDir: File | File |  | 103 |
| `OperitPaths.skillRepoZipPoolDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | baseDir: File | File |  | 107 |
| `OperitPaths.rawSnapshotExcludedFilesTopLevelDirNames` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | Set<String> |  | 111 |
| `OperitPaths.operitRootPathSdcard` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | String |  | 121 |
| `OperitPaths.cleanOnExitPathSdcard` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | String |  | 125 |
| `OperitPaths.pluginsPathSdcard` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | String |  | 129 |
| `OperitPaths.bridgePathSdcard` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | String |  | 133 |
| `OperitPaths.exportsPathSdcard` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | String |  | 137 |
| `OperitPaths.workspacePathSdcard` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | chatId: String | String |  | 141 |
| `OperitPaths.testPathSdcard` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | String |  | 145 |
| `OperitPaths.webSessionUserscriptsPathSdcard` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` |  | String |  | 149 |
| `OperitPaths.ensureDir` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | dir: File | File |  | 153 |
| `PathMapper.mapLinuxPath` | `PathMapper` | `com.ai.assistance.operit.util` | `PathMapper.kt` | context: Context<br>linuxPath: String | String | 将Linux路径转换为Android文件系统中的实际路径 | 19 |
| `PathMapper.isLinuxEnvironment` | `PathMapper` | `com.ai.assistance.operit.util` | `PathMapper.kt` | environment: String? | Boolean | 判断是否为Linux环境 | 43 |
| `PathMapper.resolvePath` | `PathMapper` | `com.ai.assistance.operit.util` | `PathMapper.kt` | context: Context<br>path: String<br>environment: String? | String | 根据environment参数转换路径 | 55 |
| `PortProcessKiller.killListeners` | `PortProcessKiller` | `com.ai.assistance.operit.util` | `PortProcessKiller.kt` | port: Int | List<Int> |  | 9 |
| `SkillRepoZipPoolManager.initialize` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | baseDir: File | Unit |  | 26 |
| `SkillRepoZipPoolManager.sha256Hex16` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | value: String | String |  | 33 |
| `SkillRepoZipPoolManager.zipFileFor` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | dir: File<br>key: String | File |  | 47 |
| `SkillRepoZipPoolManager.partFileFor` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | dir: File<br>key: String | File |  | 49 |
| `SkillRepoZipPoolManager.touch` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | file: File | Unit |  | 51 |
| `SkillRepoZipPoolManager.evictIfNeededLocked` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | dir: File | Unit |  | 55 |
| `SkillRepoZipPoolManager.getOrDownloadZip` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | key: String<br>downloadTo: suspend (outFile: File) -> Boolean | File? |  | 67 |
| `StreamingJsonXmlConverter.resetPrimitiveTracking` | `StreamingJsonXmlConverter` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` |  | Unit |  | 41 |
| `StreamingJsonXmlConverter.emitPrimitiveParam` | `StreamingJsonXmlConverter` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` | events: MutableList<Event> | Unit |  | 48 |
| `StreamingJsonXmlConverter.canFinalizePrimitiveOnFlush` | `StreamingJsonXmlConverter` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` |  | Boolean |  | 56 |
| `StreamingJsonXmlConverter.hasUnfinishedParam` | `StreamingJsonXmlConverter` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` |  | Boolean | 当前是否存在未闭合的 <param>。 若为 true，说明参数内容仍可能是半截，调用方不应补 </tool>。 | 66 |
| `StreamingJsonXmlConverter.feed` | `StreamingJsonXmlConverter` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` | chunk: String | List<Event> | 处理 JSON 块并返回 XML 事件列表 | 71 |
| `flush` | — | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` |  | List<Event> | 刷新缓冲区，处理剩余的原始值 | 222 |
| `escapeXml` | — | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverter.kt` | text: String | String | XML 转义辅助函数 | 233 |
| `StructuredAssistantContentParser.parse` | `StructuredAssistantContentParser` | `com.ai.assistance.operit.util` | `StructuredAssistantContentParser.kt` | content: String | List<Block> |  | 22 |
| `StructuredAssistantContentParser.buildBlock` | `StructuredAssistantContentParser` | `com.ai.assistance.operit.util` | `StructuredAssistantContentParser.kt` | segment: List<String> | Block? |  | 41 |
| `StructuredAssistantContentParser.extractXmlInnerContent` | `StructuredAssistantContentParser` | `com.ai.assistance.operit.util` | `StructuredAssistantContentParser.kt` | xml: String<br>rawTagName: String?<br>normalizedTagName: String? | String |  | 69 |
| `StructuredAssistantContentParser.extractXmlAttributes` | `StructuredAssistantContentParser` | `com.ai.assistance.operit.util` | `StructuredAssistantContentParser.kt` | xml: String | Map<String, String> |  | 102 |
| `StructuredAssistantContentParser.isXmlFullyClosed` | `StructuredAssistantContentParser` | `com.ai.assistance.operit.util` | `StructuredAssistantContentParser.kt` | xml: String<br>rawTagName: String? | Boolean |  | 123 |
| `TextSegmenter.initialize` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | context: Context<br>customDictPath: String?? | Unit | 初始化分词器，可选加载自定义词典 | 39 |
| `TextSegmenter.loadCustomDictionaryIfNeeded` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | dictionary: WordDictionary<br>customDictPath: String | Unit |  | 67 |
| `TextSegmenter.segment` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | text: String<br>useCached: Boolean? | List<String> | 对文本进行分词 | 85 |
| `TextSegmenter.clearCache` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` |  | Unit | 清除分词缓存 | 121 |
| `TextSegmenter.calculateRelevance` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | text: String<br>keywords: List<String> | Double | 计算文本与关键词的相关性得分 | 131 |
| `ThrowableTextFormatter.format` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | throwable: Throwable?<br>maxChars: Int? | String |  | 16 |
| `ThrowableTextFormatter.truncateText` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | text: String?<br>maxChars: Int? | String |  | 34 |
| `ThrowableTextFormatter.buildMinimalText` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | throwable: Throwable<br>maxChars: Int | String |  | 48 |
| `ThrowableTextFormatter.appendThrowable` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | builder: StringBuilder<br>throwable: Throwable<br>seen: MutableSet<Throwable><br>maxChars: Int<br>depth: Int | Boolean |  | 60 |
| `ThrowableTextFormatter.appendBounded` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | builder: StringBuilder<br>text: String<br>maxChars: Int | Boolean |  | 105 |
| `TokenCacheManager.resetTokenCounts` | `TokenCacheManager` | `com.ai.assistance.operit.util` | `TokenCacheManager.kt` |  | Unit | 重置所有token计数和缓存 | 52 |
| `TokenCacheManager.addOutputTokens` | `TokenCacheManager` | `com.ai.assistance.operit.util` | `TokenCacheManager.kt` | tokens: Long | Unit | 增加输出token数量 | 63 |
| `TokenCacheManager.setOutputTokens` | `TokenCacheManager` | `com.ai.assistance.operit.util` | `TokenCacheManager.kt` | tokens: Long | Unit | 使用API返回的实际输出token数量覆盖当前估算值 | 70 |
| `TokenCacheManager.updateActualTokens` | `TokenCacheManager` | `com.ai.assistance.operit.util` | `TokenCacheManager.kt` | actualInput: Long<br>cachedInput: Long | Unit | 使用API返回的实际token数据更新计数 用于Gemini等支持服务端缓存统计的API | 81 |
| `TokenCacheManager.calculateInputTokens` | `TokenCacheManager` | `com.ai.assistance.operit.util` | `TokenCacheManager.kt` | chatHistory: List<Pair<String, String>><br>toolsJson: String??<br>updateState: Boolean? | Long | 计算输入token数量，利用缓存优化重复计算 | 93 |
| `TokenCacheManager.findCommonPrefixLength` | `TokenCacheManager` | `com.ai.assistance.operit.util` | `TokenCacheManager.kt` | current: List<Pair<String, String>><br>previous: List<Pair<String, String>> | Int | 找到两个聊天历史列表的公共前缀长度 | 179 |
| `TokenCacheManager.calculateTokensForHistory` | `TokenCacheManager` | `com.ai.assistance.operit.util` | `TokenCacheManager.kt` | history: List<Pair<String, String>> | Long | 计算聊天历史的token数量 | 200 |
| `ToolPkgArtifactMinifier.readToolPkgLogoAsset` | `ToolPkgArtifactMinifier` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | sourceFile: File | ToolPkgLogoAsset? |  | 20 |
| `ToolPkgArtifactMinifier.processArtifactFile` | `ToolPkgArtifactMinifier` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | context: Context<br>sourceFile: File<br>isToolPkg: Boolean<br>marketOrigin: ToolPkgMarketOrigin<br>minify: Boolean | ByteArray |  | 61 |
| `ToolPkgArtifactMinifier.processScriptFile` | `ToolPkgArtifactMinifier` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | sourceFile: File<br>minifier: ToolPkgJsAstMinifier<br>marketOrigin: ToolPkgMarketOrigin<br>minify: Boolean | ByteArray |  | 77 |
| `ToolPkgArtifactMinifier.processToolPkgArchive` | `ToolPkgArtifactMinifier` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | sourceFile: File<br>minifier: ToolPkgJsAstMinifier<br>marketOrigin: ToolPkgMarketOrigin<br>minify: Boolean | ByteArray |  | 95 |
| `ToolPkgArtifactMinifier.collectReachableToolPkgEntries` | `ToolPkgArtifactMinifier` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | archive: ZipFile<br>entries: List<ZipEntry><br>manifestEntryName: String<br>executableEntryNames: Set<String><br>resourceEntryRoots: Set<String> | Set<String> |  | 225 |
| `ToolPkgArtifactMinifier.resolveToolPkgModuleEntry` | `ToolPkgArtifactMinifier` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | currentName: String<br>specifier: String<br>entryNames: Set<String> | String? |  | 263 |
| `isJavaScriptEntry` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | name: String | Boolean |  | 292 |
| `injectToolPkgMarketOrigin` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | bytes: ByteArray<br>marketOrigin: ToolPkgMarketOrigin | ByteArray |  | 297 |
| `minifyJavaScriptBytes` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | bytes: ByteArray<br>entryName: String<br>minifier: ToolPkgJsAstMinifier<br>marketOrigin: ToolPkgMarketOrigin?? | ByteArray |  | 306 |
| `minifyJavaScriptSourcePreservingMetadata` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | source: String<br>entryName: String<br>minifier: ToolPkgJsAstMinifier | String |  | 321 |
| `findMetadataBlock` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | source: String | MetadataBlock? |  | 335 |
| `injectScriptMarketOriginIntoMetadata` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | source: String<br>marketOrigin: ToolPkgMarketOrigin | String |  | 344 |
| `shouldMinifyToolPkgEntry` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | normalizedName: String<br>executableEntryNames: Set<String><br>resourceEntryRoots: Set<String> | Boolean |  | 356 |
| `logoContentType` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | mime: String<br>fileName: String | String |  | 380 |
| `ToolPkgJsAstMinifier.minify` | `ToolPkgJsAstMinifier` | `com.ai.assistance.operit.util` | `ToolPkgJsAstMinifier.kt` | source: String<br>entryName: String | String |  | 24 |
| `ToolPkgJsAstMinifier.close` | `ToolPkgJsAstMinifier` | `com.ai.assistance.operit.util` | `ToolPkgJsAstMinifier.kt` |  | Unit |  | 45 |
| `ToolPkgWasmRuntime.call` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | cacheKey: String<br>wasmBytes: ByteArray<br>exportName: String<br>argTypes: IntArray<br>argBits: LongArray | String |  | 16 |
| `ToolPkgWasmRuntime.close` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | cacheKey: String | Unit |  | 32 |
| `ToolPkgWasmRuntime.closeAllForPackage` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | packageName: String | Unit |  | 41 |
| `ToolPkgWasmRuntime.closeAll` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` |  | Unit |  | 50 |
| `ToolPkgWasmRuntime.resolveLoadedModule` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | cacheKey: String<br>wasmBytes: ByteArray | LoadedModule |  | 55 |
| `ToolPkgWasmRuntime.sha256Hex` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | bytes: ByteArray | String |  | 82 |
| `ToolPkgWasmNative.load` | `ToolPkgWasmNative` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | bytes: ByteArray | Long |  | 99 |
| `ToolPkgWasmNative.call` | `ToolPkgWasmNative` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | handle: Long<br>functionName: String<br>argTypes: IntArray<br>argBits: LongArray | String |  | 101 |
| `ToolPkgWasmNative.close` | `ToolPkgWasmNative` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | handle: Long | Unit |  | 108 |
| `TtsCleaner.clean` | `TtsCleaner` | `com.ai.assistance.operit.util` | `TtsCleaner.kt` | text: String<br>regexPattern: String | String | Cleans a given text by removing all parts that match the provided regex pattern. | 16 |
| `TtsCleaner.clean` | `TtsCleaner` | `com.ai.assistance.operit.util` | `TtsCleaner.kt` | text: String<br>regexPatterns: List<String> | String | Cleans a given text by removing all parts that match any of the provided regex patterns. | 40 |
| `TtsCleaner.cleanForSpeech` | `TtsCleaner` | `com.ai.assistance.operit.util` | `TtsCleaner.kt` | text: String<br>regexPatterns: List<String> | String | Resolves the spoken reply body of a stored message, then applies the user's cleaner patte… | 90 |
| `TtsCleaner.extractReplyBody` | `TtsCleaner` | `com.ai.assistance.operit.util` | `TtsCleaner.kt` | text: String | String | Drops the blocks that are never part of the spoken reply: provider protocol metadata, rea… | 114 |
| `TtsSegmenter.findFirstEndCharIndex` | `TtsSegmenter` | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | text: CharSequence | Int |  | 7 |
| `TtsSegmenter.nextSegmentEnd` | `TtsSegmenter` | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | buffer: CharSequence | Int |  | 14 |
| `TtsSegmenter.split` | `TtsSegmenter` | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | text: String | List<String> |  | 27 |
| `TtsSegmenter.isSegmentEndingChar` | `TtsSegmenter` | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | text: CharSequence<br>index: Int | Boolean |  | 45 |
| `isTrailingEndingChar` | — | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | text: CharSequence<br>index: Int | Boolean |  | 59 |
| `getOrNull` | — | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | index: Int | Char? |  | 73 |
| `UriSerializer.serialize` | `UriSerializer` | `com.ai.assistance.operit.util` | `UriSerializer.kt` | encoder: Encoder<br>value: Uri? | Unit |  | 14 |
| `UriSerializer.deserialize` | `UriSerializer` | `com.ai.assistance.operit.util` | `UriSerializer.kt` | decoder: Decoder | Uri? |  | 18 |
| `WaifuMessageProcessor.StreamingSession.collectStableSegments` | `StreamingSession` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | List<String> |  | 73 |
| `WaifuMessageProcessor.StreamingSession.collectFinalSegments` | `StreamingSession` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | List<String> |  | 83 |
| `WaifuMessageProcessor.StreamingSession.collectSegments` | `StreamingSession` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | segments: List<String> | List<String> |  | 93 |
| `WaifuMessageProcessor.streamSegments` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | sourceStream: Stream<String><br>removePunctuation: Boolean? | Stream<String> |  | 124 |
| `WaifuMessageProcessor.ensureBlockLatexDelimiters` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | rawContent: String | String | Ensure a BLOCK_LATEX body carries a recognized block delimiter pair. `StreamMarkdownBlock… | 145 |
| `WaifuMessageProcessor.calculateTypingDelayMs` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | segmentLength: Int<br>charDelayMs: Int<br>isFirstSegment: Boolean | Long |  | 163 |
| `WaifuMessageProcessor.streamSegmentsWithTypingQueue` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | sourceStream: Stream<String><br>removePunctuation: Boolean?<br>charDelayMs: Int | Stream<String> |  | 175 |
| `WaifuMessageProcessor.streamSegmentUpdatesWithTypingQueue` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | sourceStream: Stream<String><br>removePunctuation: Boolean?<br>charDelayMs: Int | Stream<WaifuSegmentUpdate> |  | 191 |
| `WaifuMessageProcessor.buildRenderableSnapshot` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String<br>final: Boolean<br>nativeSegments: IntArray | String | Replays native block events without treating the current live snapshot as an EOF. | 219 |
| `WaifuMessageProcessor.closeBlock` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` |  | Unit |  | 228 |
| `WaifuMessageProcessor.streamTtsText` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | sourceStream: Stream<String> | Stream<Char> |  | 270 |
| `WaifuMessageProcessor.emitText` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | text: String | Unit |  | 273 |
| `WaifuMessageProcessor.removeSentenceEndPunctuation` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | sentence: String | String |  | 311 |
| `WaifuMessageProcessor.initialize` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | appContext: Context | Unit | 初始化处理器（需要在应用启动时调用） | 323 |
| `WaifuMessageProcessor.splitMessageBySentences` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String<br>removePunctuation: Boolean? | List<String> | 将完整的消息按句号分割成句子 | 334 |
| `WaifuMessageProcessor.splitStableMessageSegments` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String<br>removePunctuation: Boolean? | List<String> |  | 342 |
| `WaifuMessageProcessor.splitMessageBySentencesInternal` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String<br>removePunctuation: Boolean<br>includeTrailingIncomplete: Boolean | List<String> |  | 350 |
| `WaifuMessageProcessor.createPlaceholder` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | value: String | String |  | 359 |
| `WaifuMessageProcessor.protectMatches` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | source: String<br>regex: Regex | String |  | 365 |
| `WaifuMessageProcessor.splitTrailingProtectedText` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | value: String | Pair<String, String> |  | 494 |
| `WaifuMessageProcessor.splitPlainTextIntoSentences` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | cleanedContent: String<br>removePunctuation: Boolean | List<String> |  | 507 |
| `WaifuMessageProcessor.mergePunctuationOnlySegments` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | segments: List<String> | MutableList<String> |  | 536 |
| `shouldSplitStructuredMarkdownLines` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String<br>sentences: List<String> | Boolean |  | 562 |
| `splitStructuredMarkdownLines` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String<br>removePunctuation: Boolean | List<String> |  | 585 |
| `cleanStructuredMarkdownLine` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | line: String | String |  | 609 |
| `getLastVisibleLine` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | String |  | 620 |
| `lineAllowsStableWithoutSentenceEnding` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | line: String | Boolean |  | 627 |
| `isUrlOrEmailLine` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | line: String | Boolean |  | 645 |
| `hasStableSentenceEnding` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | Boolean |  | 657 |
| `splitStableSentencesForRawContent` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | rawContent: String<br>cleanedContent: String<br>removePunctuation: Boolean<br>segment: Segment<br>hasFollowingStableBoundarySegment: Boolean | List<String> |  | 661 |
| `shouldHoldLastStableSentence` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | rawContent: String<br>cleanedContent: String<br>segment: Segment<br>hasFollowingStableBoundarySegment: Boolean | Boolean |  | 695 |
| `findLastUnclosedInlineMarkdownStart` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | Int? |  | 708 |
| `findLastUnclosedDelimiterStart` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String<br>delimiter: String | Int? |  | 719 |
| `isEscaped` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String<br>index: Int | Boolean |  | 741 |
| `segmentProducesOutput` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | segment: Segment | Boolean |  | 752 |
| `isRenderablePluginTagName` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | rawTagName: String | Boolean | 判断某个标签名是否由插件渲染器接管，同时排除内部控制标签。 这里复用 [XmlRenderPluginRegistry] 的注册信息，而不是在消息链路上另立一份白名单： Tool… | 774 |
| `isRenderablePluginXmlContent` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | rawContent: String | Boolean | 判断一段原始 XML 文本是否是"已注册渲染标签"的完整块。 未闭合的标签不算：流式期间标签可能只到达一半，此时把它当成分段内容会固化成 不完整的标签；等标签闭合后的下一次分段快… | 791 |
| `isRenderablePluginXmlBlock` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | block: StructuredAssistantContentParser.Bl… | Boolean |  | 806 |
| `buildRenderableContentForWaifu` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | String |  | 814 |
| `cleanContentForWaifu` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | String | 清理内容中的状态标签和XML标签，只保留纯文本 | 847 |
| `Segment.canUseBlockBoundaryAsStableEnding` | `Segment` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | hasFollowingStableBoundarySegment: Boolean | Boolean |  | 907 |
| `canCloseStableTextAtBlockBoundary` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` |  | Boolean |  | 912 |
| `splitIntoSegments` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | List<Segment> |  | 941 |
| `processEmotionTags` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | String | 处理表情包标签，将<emotion>标签替换为对应的表情图片 | 1003 |
| `separateEmotionAndText` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | content: String | List<String> | 分离表情包和文本内容 | 1037 |
| `getRandomEmojiPath` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | emotion: String | String? | 根据情绪名称获取随机的表情图片路径 | 1094 |
| `WaifuSegmentUpdate.streamWaifuUpdates` | `WaifuSegmentUpdate` | `com.ai.assistance.operit.util` | `WaifuStreamUpdates.kt` | sourceStream: Stream<String><br>splitSnapshot: (content: String, final: Boolean) -…<br>typingDelayMs: (segmentLength: Int, first: Boolean…<br>nowMillis: () -> Long? | Stream<WaifuSegmentUpdate> | Keeps typing work relative to the latest revision-applied sentence snapshot. The splitter… | 32 |
| `WaifuSegmentUpdate.publish` | `WaifuSegmentUpdate` | `com.ai.assistance.operit.util` | `WaifuStreamUpdates.kt` | final: Boolean | Unit |  | 50 |
| `WaifuSegmentUpdate.scheduleNext` | `WaifuSegmentUpdate` | `com.ai.assistance.operit.util` | `WaifuStreamUpdates.kt` |  | Unit |  | 106 |
| `WaifuSegmentUpdate.accept` | `WaifuSegmentUpdate` | `com.ai.assistance.operit.util` | `WaifuStreamUpdates.kt` | snapshot: List<String> | Unit |  | 115 |
| `WaifuSegmentUpdate.appendNext` | `WaifuSegmentUpdate` | `com.ai.assistance.operit.util` | `WaifuStreamUpdates.kt` |  | Unit |  | 131 |
| `WaifuSegmentMessageStore.apply` | `WaifuSegmentMessageStore` | `com.ai.assistance.operit.util` | `WaifuStreamUpdates.kt` | update: WaifuSegmentUpdate | Unit |  | 231 |
| `AnrCaptureBudgetTest.deepStack` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` | depth: Int<br>prefix: String? | Array<StackTraceElement> |  | 15 ⚑ |
| `AnrCaptureBudgetTest.formatFrames_capsDepthForVeryDeepStacks` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 19 ⚑ |
| `AnrCaptureBudgetTest.formatFrames_staysWithinCharBudget` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 28 ⚑ |
| `AnrCaptureBudgetTest.formatFrames_truncatesSingleOverlongFrame` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 42 ⚑ |
| `AnrCaptureBudgetTest.formatFrames_keepsShortStacksIntact` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 54 ⚑ |
| `AnrCaptureBudgetTest.formatFrames_skipsLeadingFramesWhenAsked` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 68 ⚑ |
| `AnrCaptureBudgetTest.formatFrames_doesNotEmitMarkerWhenNothingIsCut` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 76 ⚑ |
| `AnrCaptureBudgetTest.clampDump_boundsOversizedDumpAndMarksTheCut` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 83 ⚑ |
| `AnrCaptureBudgetTest.clampDump_leavesSmallDumpUntouched` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 93 ⚑ |
| `AnrCaptureBudgetTest.stackSignature_isStableForTheSameFrames` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 100 ⚑ |
| `AnrCaptureBudgetTest.stackSignature_ignoresFramesBelowSignatureDepth` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 108 ⚑ |
| `AnrCaptureBudgetTest.stackSignature_separatesDifferentStalls` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 120 ⚑ |
| `AnrCaptureBudgetTest.stackSignature_staysSmallForDeepStacks` | `AnrCaptureBudgetTest` | `com.ai.assistance.operit.util` | `AnrCaptureBudgetTest.kt` |  | Unit |  | 128 ⚑ |
| `AnrCaptureThrottleTest.firstCaptureIsAlwaysAllowed` | `AnrCaptureThrottleTest` | `com.ai.assistance.operit.util` | `AnrCaptureThrottleTest.kt` |  | Unit |  | 15 ⚑ |
| `AnrCaptureThrottleTest.samplesInsideTheCooldownAreRejected` | `AnrCaptureThrottleTest` | `com.ai.assistance.operit.util` | `AnrCaptureThrottleTest.kt` |  | Unit |  | 22 ⚑ |
| `AnrCaptureThrottleTest.captureIsAllowedAgainAfterTheCooldownElapses` | `AnrCaptureThrottleTest` | `com.ai.assistance.operit.util` | `AnrCaptureThrottleTest.kt` |  | Unit |  | 34 ⚑ |
| `AnrCaptureThrottleTest.cooldownIsMeasuredFromTheLastAllowedCapture` | `AnrCaptureThrottleTest` | `com.ai.assistance.operit.util` | `AnrCaptureThrottleTest.kt` |  | Unit |  | 43 ⚑ |
| `AnrCaptureThrottleTest.aSixtySecondStallProducesABoundedNumberOfCaptures` | `AnrCaptureThrottleTest` | `com.ai.assistance.operit.util` | `AnrCaptureThrottleTest.kt` |  | Unit |  | 54 ⚑ |
| `ChatMarkupRegexAttachmentTest.attachmentTag_matchesExplicitAttachmentBlock` | `ChatMarkupRegexAttachmentTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexAttachmentTest.kt` |  | Unit |  | 9 ⚑ |
| `ChatMarkupRegexAttachmentTest.attachmentSelfClosingTag_matchesSelfClosingAttachment` | `ChatMarkupRegexAttachmentTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexAttachmentTest.kt` |  | Unit |  | 13 ⚑ |
| `ChatMarkupRegexAttachmentTest.workspaceAttachmentTag_matchesWorkspaceBlock` | `ChatMarkupRegexAttachmentTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexAttachmentTest.kt` |  | Unit |  | 17 ⚑ |
| `ChatMarkupRegexAttachmentTest.proxySenderTag_extractsName` | `ChatMarkupRegexAttachmentTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexAttachmentTest.kt` |  | Unit |  | 21 ⚑ |
| `ChatMarkupRegexContainsTest.containsAnyToolLikeTag_detectsToolTag` | `ChatMarkupRegexContainsTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexContainsTest.kt` |  | Unit |  | 9 ⚑ |
| `ChatMarkupRegexContainsTest.containsAnyToolLikeTag_detectsToolResultTag` | `ChatMarkupRegexContainsTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexContainsTest.kt` |  | Unit |  | 13 ⚑ |
| `ChatMarkupRegexContainsTest.containsAnyToolLikeTag_returnsFalseForPlainText` | `ChatMarkupRegexContainsTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexContainsTest.kt` |  | Unit |  | 17 ⚑ |
| `ChatMarkupRegexMetaTest.extractSignature_ignoresEmptyBody` | `ChatMarkupRegexMetaTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexMetaTest.kt` |  | Unit |  | 9 ⚑ |
| `ChatMarkupRegexMetaTest.removeSignature_preservesTrailingText` | `ChatMarkupRegexMetaTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexMetaTest.kt` |  | Unit |  | 13 ⚑ |
| `ChatMarkupRegexMetaTest.removeSignature_removesMultipleMatchingTags` | `ChatMarkupRegexMetaTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexMetaTest.kt` |  | Unit |  | 17 ⚑ |
| `ChatMarkupRegexMetaTest.extractSignature_returnsLastAmongMixedMetaTags` | `ChatMarkupRegexMetaTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexMetaTest.kt` |  | Unit |  | 21 ⚑ |
| `ChatMarkupRegexMetaTest.removeOpenAiReasoning_preservesVoidMetaBeforeMatchingTag` | `ChatMarkupRegexMetaTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexMetaTest.kt` |  | Unit |  | 30 ⚑ |
| `ChatMarkupRegexMetaTest.removeOpenAiReasoning_ignoresProviderTextInMetaBody` | `ChatMarkupRegexMetaTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexMetaTest.kt` |  | Unit |  | 41 ⚑ |
| `ChatMarkupRegexMetaTest.extractOpenAiResponsesOutputItem_returnsMatchingPayloads` | `ChatMarkupRegexMetaTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexMetaTest.kt` |  | Unit |  | 47 ⚑ |
| `ChatMarkupRegexMetaTest.removeOpenAiResponsesProtocolMeta_removesReasoningAndOutputItemsOnly` | `ChatMarkupRegexMetaTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexMetaTest.kt` |  | Unit |  | 59 ⚑ |
| `ChatMarkupRegexOpeningTagTest.extractOpeningTagName_readsStatusTag` | `ChatMarkupRegexOpeningTagTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexOpeningTagTest.kt` |  | Unit |  | 9 ⚑ |
| `ChatMarkupRegexOpeningTagTest.extractOpeningTagName_readsTagAfterLeadingWhitespace` | `ChatMarkupRegexOpeningTagTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexOpeningTagTest.kt` |  | Unit |  | 13 ⚑ |
| `ChatMarkupRegexOpeningTagTest.extractOpeningTagName_returnsNullForBrokenTag` | `ChatMarkupRegexOpeningTagTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexOpeningTagTest.kt` |  | Unit |  | 17 ⚑ |
| `ChatMarkupRegexPatternTest.namePattern_extractsToolName` | `ChatMarkupRegexPatternTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexPatternTest.kt` |  | Unit |  | 9 ⚑ |
| `ChatMarkupRegexPatternTest.toolParamPattern_extractsParamNameAndBody` | `ChatMarkupRegexPatternTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexPatternTest.kt` |  | Unit |  | 13 ⚑ |
| `ChatMarkupRegexPatternTest.anyXmlTag_matchesSimpleTag` | `ChatMarkupRegexPatternTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexPatternTest.kt` |  | Unit |  | 19 ⚑ |
| `ChatMarkupRegexPatternTest.pruneToolResultContentPattern_matchesStatusPayload` | `ChatMarkupRegexPatternTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexPatternTest.kt` |  | Unit |  | 23 ⚑ |
| `ChatMarkupRegexRandomTagTest.generatedToolTag_hasExpectedPrefixLength` | `ChatMarkupRegexRandomTagTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexRandomTagTest.kt` |  | Unit |  | 9 ⚑ |
| `ChatMarkupRegexRandomTagTest.generatedToolResultTag_hasExpectedPrefixLength` | `ChatMarkupRegexRandomTagTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexRandomTagTest.kt` |  | Unit |  | 15 ⚑ |
| `ChatMarkupRegexSearchTest.searchTag_isCaseInsensitive` | `ChatMarkupRegexSearchTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexSearchTest.kt` |  | Unit |  | 9 ⚑ |
| `ChatMarkupRegexSearchTest.thinkTag_isCaseInsensitive` | `ChatMarkupRegexSearchTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexSearchTest.kt` |  | Unit |  | 13 ⚑ |
| `ChatMarkupRegexSearchTest.metaTag_doesNotMatchPlainText` | `ChatMarkupRegexSearchTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexSearchTest.kt` |  | Unit |  | 17 ⚑ |
| `ChatMarkupRegexStatusTest.xmlStatusPattern_extractsUuidWhenPresent` | `ChatMarkupRegexStatusTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexStatusTest.kt` |  | Unit |  | 9 ⚑ |
| `ChatMarkupRegexStatusTest.xmlStatusPattern_extractsTitleWhenPresent` | `ChatMarkupRegexStatusTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexStatusTest.kt` |  | Unit |  | 15 ⚑ |
| `ChatMarkupRegexStatusTest.xmlStatusPattern_extractsSubtitleWhenPresent` | `ChatMarkupRegexStatusTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexStatusTest.kt` |  | Unit |  | 21 ⚑ |
| `ChatMarkupRegexTest.toolTagName_acceptsBaseTool` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 12 ⚑ |
| `ChatMarkupRegexTest.toolTagName_acceptsSuffix` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 16 ⚑ |
| `ChatMarkupRegexTest.toolTagName_rejectsToolResult` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 20 ⚑ |
| `ChatMarkupRegexTest.toolResultTagName_acceptsBaseToolResult` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 24 ⚑ |
| `ChatMarkupRegexTest.toolResultTagName_acceptsSuffix` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 28 ⚑ |
| `ChatMarkupRegexTest.toolResultTagName_rejectsPlainTool` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 32 ⚑ |
| `ChatMarkupRegexTest.normalizeToolLikeTagName_normalizesToolSuffix` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 36 ⚑ |
| `ChatMarkupRegexTest.normalizeToolLikeTagName_normalizesToolResultSuffix` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 40 ⚑ |
| `ChatMarkupRegexTest.normalizeToolLikeTagName_preservesUnknownTag` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 44 ⚑ |
| `ChatMarkupRegexTest.containsToolTag_detectsOpeningTag` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 48 ⚑ |
| `ChatMarkupRegexTest.containsToolTag_rejectsToolResult` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 52 ⚑ |
| `ChatMarkupRegexTest.containsToolResultTag_detectsOpeningTag` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 56 ⚑ |
| `ChatMarkupRegexTest.containsAnyToolLikeTag_detectsEitherVariant` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 60 ⚑ |
| `ChatMarkupRegexTest.extractOpeningTagName_readsFirstTag` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 64 ⚑ |
| `ChatMarkupRegexTest.extractOpeningTagName_returnsNullForPlainText` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 68 ⚑ |
| `ChatMarkupRegexTest.generateRandomToolTagName_usesToolPrefix` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 72 ⚑ |
| `ChatMarkupRegexTest.generateRandomToolResultTagName_usesToolResultPrefix` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 76 ⚑ |
| `ChatMarkupRegexTest.geminiMetaTag_wrapsSignature` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 80 ⚑ |
| `ChatMarkupRegexTest.extractGeminiThoughtSignature_readsSingleSignature` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 87 ⚑ |
| `ChatMarkupRegexTest.extractGeminiThoughtSignature_usesLastMatchingSignature` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 94 ⚑ |
| `ChatMarkupRegexTest.extractGeminiThoughtSignature_ignoresOtherProviders` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 104 ⚑ |
| `ChatMarkupRegexTest.extractGeminiThoughtSignature_trimsBodyWhitespace` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 108 ⚑ |
| `ChatMarkupRegexTest.removeGeminiThoughtSignatureMeta_removesMatchingTag` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 115 ⚑ |
| `ChatMarkupRegexTest.removeGeminiThoughtSignatureMeta_keepsOtherMeta` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 119 ⚑ |
| `ChatMarkupRegexTest.removeGeminiThoughtSignatureMeta_isCaseInsensitiveOnProvider` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 124 ⚑ |
| `ChatMarkupRegexTest.toolCallPattern_extractsNameAndBody` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 128 ⚑ |
| `ChatMarkupRegexTest.toolTag_matchesSuffixVariant` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 135 ⚑ |
| `ChatMarkupRegexTest.toolSelfClosingTag_matchesSuffixVariant` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 139 ⚑ |
| `ChatMarkupRegexTest.toolResultTagWithAttrs_extractsStatusBlock` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 143 ⚑ |
| `ChatMarkupRegexTest.xmlToolRequestPattern_extractsDescriptionWhenPresent` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 149 ⚑ |
| `ChatMarkupRegexTest.xmlToolResultPattern_extractsContentAndStatus` | `ChatMarkupRegexTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexTest.kt` |  | Unit |  | 157 ⚑ |
| `ChatMarkupRegexToolNameTest.toolTag_acceptsUppercaseVariant` | `ChatMarkupRegexToolNameTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolNameTest.kt` |  | Unit |  | 10 ⚑ |
| `ChatMarkupRegexToolNameTest.toolTag_rejectsNull` | `ChatMarkupRegexToolNameTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolNameTest.kt` |  | Unit |  | 14 ⚑ |
| `ChatMarkupRegexToolNameTest.toolResultTag_acceptsUppercaseVariant` | `ChatMarkupRegexToolNameTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolNameTest.kt` |  | Unit |  | 18 ⚑ |
| `ChatMarkupRegexToolNameTest.toolResultTag_rejectsNull` | `ChatMarkupRegexToolNameTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolNameTest.kt` |  | Unit |  | 22 ⚑ |
| `ChatMarkupRegexToolNameTest.normalizeNullTagName_returnsNull` | `ChatMarkupRegexToolNameTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolNameTest.kt` |  | Unit |  | 26 ⚑ |
| `ChatMarkupRegexToolResultTest.toolResultTag_matchesSuffixVariant` | `ChatMarkupRegexToolResultTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolResultTest.kt` |  | Unit |  | 10 ⚑ |
| `ChatMarkupRegexToolResultTest.toolResultSelfClosingTag_matchesSuffixVariant` | `ChatMarkupRegexToolResultTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolResultTest.kt` |  | Unit |  | 14 ⚑ |
| `ChatMarkupRegexToolResultTest.toolResultAnyPattern_extractsBody` | `ChatMarkupRegexToolResultTest` | `com.ai.assistance.operit.util` | `ChatMarkupRegexToolResultTest.kt` |  | Unit |  | 18 ⚑ |
| `ChatUtilsExtractJsonEdgeTest.extractJson_returnsOriginalWhenBracesOutOfOrder` | `ChatUtilsExtractJsonEdgeTest` | `com.ai.assistance.operit.util` | `ChatUtilsExtractJsonEdgeTest.kt` |  | Unit |  | 8 ⚑ |
| `ChatUtilsExtractJsonEdgeTest.extractJsonArray_returnsOriginalWhenBracketsOutOfOrder` | `ChatUtilsExtractJsonEdgeTest` | `com.ai.assistance.operit.util` | `ChatUtilsExtractJsonEdgeTest.kt` |  | Unit |  | 12 ⚑ |
| `ChatUtilsExtractJsonEdgeTest.extractJson_handlesMarkdownFenceWithoutLanguage` | `ChatUtilsExtractJsonEdgeTest` | `com.ai.assistance.operit.util` | `ChatUtilsExtractJsonEdgeTest.kt` |  | Unit |  | 16 ⚑ |
| `ChatUtilsJsonExtractionTest.extractJson_keepsNestedObject` | `ChatUtilsJsonExtractionTest` | `com.ai.assistance.operit.util` | `ChatUtilsJsonExtractionTest.kt` |  | Unit |  | 8 ⚑ |
| `ChatUtilsJsonExtractionTest.extractJson_returnsTrimmedMarkdownBody` | `ChatUtilsJsonExtractionTest` | `com.ai.assistance.operit.util` | `ChatUtilsJsonExtractionTest.kt` |  | Unit |  | 12 ⚑ |
| `ChatUtilsJsonExtractionTest.extractJsonArray_keepsNestedArray` | `ChatUtilsJsonExtractionTest` | `com.ai.assistance.operit.util` | `ChatUtilsJsonExtractionTest.kt` |  | Unit |  | 16 ⚑ |
| `ChatUtilsJsonExtractionTest.extractJsonArray_returnsTrimmedMarkdownBody` | `ChatUtilsJsonExtractionTest` | `com.ai.assistance.operit.util` | `ChatUtilsJsonExtractionTest.kt` |  | Unit |  | 20 ⚑ |
| `ChatUtilsProviderModelTest.providerModel_acceptsGoogleWithoutSuffix` | `ChatUtilsProviderModelTest` | `com.ai.assistance.operit.util` | `ChatUtilsProviderModelTest.kt` |  | Unit |  | 9 ⚑ |
| `ChatUtilsProviderModelTest.providerModel_acceptsGeminiGenericWithoutSuffix` | `ChatUtilsProviderModelTest` | `com.ai.assistance.operit.util` | `ChatUtilsProviderModelTest.kt` |  | Unit |  | 13 ⚑ |
| `ChatUtilsProviderModelTest.providerModel_rejectsEmptyString` | `ChatUtilsProviderModelTest` | `com.ai.assistance.operit.util` | `ChatUtilsProviderModelTest.kt` |  | Unit |  | 17 ⚑ |
| `ChatUtilsProviderModelTest.providerModel_rejectsAnthropic` | `ChatUtilsProviderModelTest` | `com.ai.assistance.operit.util` | `ChatUtilsProviderModelTest.kt` |  | Unit |  | 21 ⚑ |
| `ChatUtilsStripMetaCollectionsTest.stripMeta_pairs_preserveRoles` | `ChatUtilsStripMetaCollectionsTest` | `com.ai.assistance.operit.util` | `ChatUtilsStripMetaCollectionsTest.kt` |  | Unit |  | 10 ⚑ |
| `ChatUtilsStripMetaCollectionsTest.stripMeta_turns_preserveKinds` | `ChatUtilsStripMetaCollectionsTest` | `com.ai.assistance.operit.util` | `ChatUtilsStripMetaCollectionsTest.kt` |  | Unit |  | 16 ⚑ |
| `ChatUtilsTest.stripGeminiThoughtSignatureMeta_removesMatchingMeta` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 12 ⚑ |
| `ChatUtilsTest.stripGeminiThoughtSignatureMeta_preservesPlainText` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 16 ⚑ |
| `ChatUtilsTest.stripGeminiThoughtSignatureMeta_pairsOnlyChangeContent` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 20 ⚑ |
| `ChatUtilsTest.stripGeminiThoughtSignatureMeta_turnsOnlyChangeContent` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 25 ⚑ |
| `ChatUtilsTest.geminiProviderModel_recognizesGooglePrefix` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 31 ⚑ |
| `ChatUtilsTest.geminiProviderModel_recognizesGenericPrefix` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 35 ⚑ |
| `ChatUtilsTest.geminiProviderModel_rejectsOtherPrefix` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 39 ⚑ |
| `ChatUtilsTest.stripOpenAiResponsesProtocolMarkup_removesMetaAndSearchDisplay` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 43 ⚑ |
| `ChatUtilsTest.removeThinkingContent_removesThinkBlock` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 52 ⚑ |
| `ChatUtilsTest.removeThinkingContent_removesThinkingBlock` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 56 ⚑ |
| `ChatUtilsTest.removeThinkingContent_removesSearchBlock` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 60 ⚑ |
| `ChatUtilsTest.removeThinkingContent_removesSearchBlockWithAttributes` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 64 ⚑ |
| `ChatUtilsTest.removeThinkingContent_handlesUnclosedThink` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 71 ⚑ |
| `ChatUtilsTest.removeThinkingContent_handlesUnclosedSearch` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 75 ⚑ |
| `ChatUtilsTest.extractThinkingContent_returnsCleanContent` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 79 ⚑ |
| `ChatUtilsTest.extractThinkingContent_mergesMultipleBlocks` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 85 ⚑ |
| `ChatUtilsTest.extractThinkingContent_alsoRemovesSearchBlocks` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 91 ⚑ |
| `ChatUtilsTest.extractThinkingContent_alsoRemovesSearchBlocksWithAttributes` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 97 ⚑ |
| `ChatUtilsTest.estimateTokenCount_countsEnglishApproximately` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 105 ⚑ |
| `ChatUtilsTest.estimateTokenCount_countsChineseApproximately` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 109 ⚑ |
| `ChatUtilsTest.estimateTokenCount_countsMixedText` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 113 ⚑ |
| `ChatUtilsTest.extractJson_returnsEmbeddedObject` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 117 ⚑ |
| `ChatUtilsTest.extractJson_handlesMarkdownFence` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 121 ⚑ |
| `ChatUtilsTest.extractJson_returnsOriginalWhenNoObjectFound` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 125 ⚑ |
| `ChatUtilsTest.extractJsonArray_returnsEmbeddedArray` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 129 ⚑ |
| `ChatUtilsTest.extractJsonArray_handlesMarkdownFence` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 133 ⚑ |
| `ChatUtilsTest.extractJsonArray_returnsOriginalWhenNoArrayFound` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 137 ⚑ |
| `ChatUtilsTest.stripGeminiThoughtSignatureMeta_turnObjectIsReusedWhenUnchanged` | `ChatUtilsTest` | `com.ai.assistance.operit.util` | `ChatUtilsTest.kt` |  | Unit |  | 141 ⚑ |
| `ChatUtilsThinkingEdgeTest.removeThinkingContent_handlesThinkingTagVariant` | `ChatUtilsThinkingEdgeTest` | `com.ai.assistance.operit.util` | `ChatUtilsThinkingEdgeTest.kt` |  | Unit |  | 8 ⚑ |
| `ChatUtilsThinkingEdgeTest.extractThinkingContent_handlesNoSearchTag` | `ChatUtilsThinkingEdgeTest` | `com.ai.assistance.operit.util` | `ChatUtilsThinkingEdgeTest.kt` |  | Unit |  | 12 ⚑ |
| `ChatUtilsThinkingEdgeTest.removeThinkingContent_handlesSearchOnlyContent` | `ChatUtilsThinkingEdgeTest` | `com.ai.assistance.operit.util` | `ChatUtilsThinkingEdgeTest.kt` |  | Unit |  | 18 ⚑ |
| `ChatUtilsThinkingTest.removeThinkingContent_trimsWhitespaceAroundRemovedBlocks` | `ChatUtilsThinkingTest` | `com.ai.assistance.operit.util` | `ChatUtilsThinkingTest.kt` |  | Unit |  | 8 ⚑ |
| `ChatUtilsThinkingTest.extractThinkingContent_returnsEmptyThinkingWhenAbsent` | `ChatUtilsThinkingTest` | `com.ai.assistance.operit.util` | `ChatUtilsThinkingTest.kt` |  | Unit |  | 12 ⚑ |
| `ChatUtilsThinkingTest.extractThinkingContent_trimsEachThinkingSegment` | `ChatUtilsThinkingTest` | `com.ai.assistance.operit.util` | `ChatUtilsThinkingTest.kt` |  | Unit |  | 18 ⚑ |
| `ChatUtilsThinkingTest.removeThinkingContent_preservesMiddleText` | `ChatUtilsThinkingTest` | `com.ai.assistance.operit.util` | `ChatUtilsThinkingTest.kt` |  | Unit |  | 24 ⚑ |
| `ChatUtilsTokenEstimateTest.estimateTokenCount_emptyText_isZero` | `ChatUtilsTokenEstimateTest` | `com.ai.assistance.operit.util` | `ChatUtilsTokenEstimateTest.kt` |  | Unit |  | 8 ⚑ |
| `ChatUtilsTokenEstimateTest.estimateTokenCount_asciiOnlyRoundsDown` | `ChatUtilsTokenEstimateTest` | `com.ai.assistance.operit.util` | `ChatUtilsTokenEstimateTest.kt` |  | Unit |  | 12 ⚑ |
| `ChatUtilsTokenEstimateTest.estimateTokenCount_chineseOnlyUsesHigherWeight` | `ChatUtilsTokenEstimateTest` | `com.ai.assistance.operit.util` | `ChatUtilsTokenEstimateTest.kt` |  | Unit |  | 16 ⚑ |
| `DocumentConversionUtilNullCharacterTest.stripNullCharactersRemovesEveryNulAndKeepsOtherText` | `DocumentConversionUtilNullCharacterTest` | `com.ai.assistance.operit.util` | `DocumentConversionUtilNullCharacterTest.kt` |  | Unit |  | 9 ⚑ |
| `DocumentConversionUtilNullCharacterTest.stripNullCharactersKeepsTextWithoutNulUnchanged` | `DocumentConversionUtilNullCharacterTest` | `com.ai.assistance.operit.util` | `DocumentConversionUtilNullCharacterTest.kt` |  | Unit |  | 16 ⚑ |
| `DocumentConversionUtilNullCharacterTest.stripNullCharactersHandlesEmptyText` | `DocumentConversionUtilNullCharacterTest` | `com.ai.assistance.operit.util` | `DocumentConversionUtilNullCharacterTest.kt` |  | Unit |  | 23 ⚑ |
| `assertPropagatedException` | — | `com.ai.assistance.operit.util` | `ExceptionAssertions.kt` | expected: Throwable<br>actual: Throwable | Unit |  | 6 ⚑ |
| `MathMlPlainTextConverterTest.convert_rendersFractionsRootsAndSuperscripts` | `MathMlPlainTextConverterTest` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverterTest.kt` |  | Unit |  | 7 ⚑ |
| `MathMlPlainTextConverterTest.convert_rendersSubscriptsAndSummationLimits` | `MathMlPlainTextConverterTest` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverterTest.kt` |  | Unit |  | 39 ⚑ |
| `MathMlPlainTextConverterTest.convert_rendersMatricesAsRowsAndColumns` | `MathMlPlainTextConverterTest` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverterTest.kt` |  | Unit |  | 60 ⚑ |
| `StreamingJsonXmlConverterChunkTest.chunkedKeyName_isAccumulatedAcrossFeeds` | `StreamingJsonXmlConverterChunkTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterChunkTest.kt` |  | Unit |  | 8 ⚑ |
| `StreamingJsonXmlConverterChunkTest.chunkedUnicodeEscape_isAccumulatedAcrossFeeds` | `StreamingJsonXmlConverterChunkTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterChunkTest.kt` |  | Unit |  | 14 ⚑ |
| `StreamingJsonXmlConverterChunkTest.render` | `StreamingJsonXmlConverterChunkTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterChunkTest.kt` | events: List<StreamingJsonXmlConverter.Even… | String |  | 20 ⚑ |
| `StreamingJsonXmlConverterEscapeTest.apostropheInString_isEscapedForXml` | `StreamingJsonXmlConverterEscapeTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterEscapeTest.kt` |  | Unit |  | 8 ⚑ |
| `StreamingJsonXmlConverterEscapeTest.quoteInString_isEscapedForXml` | `StreamingJsonXmlConverterEscapeTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterEscapeTest.kt` |  | Unit |  | 13 ⚑ |
| `StreamingJsonXmlConverterEscapeTest.render` | `StreamingJsonXmlConverterEscapeTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterEscapeTest.kt` | events: List<StreamingJsonXmlConverter.Even… | String |  | 18 ⚑ |
| `StreamingJsonXmlConverterFlushTest.flush_afterCompletedString_emitsNothing` | `StreamingJsonXmlConverterFlushTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterFlushTest.kt` |  | Unit |  | 9 ⚑ |
| `StreamingJsonXmlConverterFlushTest.flush_afterPrimitiveEmitsClosingContent` | `StreamingJsonXmlConverterFlushTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterFlushTest.kt` |  | Unit |  | 15 ⚑ |
| `StreamingJsonXmlConverterFlushTest.render` | `StreamingJsonXmlConverterFlushTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterFlushTest.kt` | events: List<StreamingJsonXmlConverter.Even… | String |  | 22 ⚑ |
| `StreamingJsonXmlConverterObjectTest.nestedObjectWithString_preservesQuotesInsideBody` | `StreamingJsonXmlConverterObjectTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterObjectTest.kt` |  | Unit |  | 8 ⚑ |
| `StreamingJsonXmlConverterObjectTest.nestedArrayWithString_preservesQuotesInsideBody` | `StreamingJsonXmlConverterObjectTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterObjectTest.kt` |  | Unit |  | 14 ⚑ |
| `StreamingJsonXmlConverterObjectTest.render` | `StreamingJsonXmlConverterObjectTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterObjectTest.kt` | events: List<StreamingJsonXmlConverter.Even… | String |  | 20 ⚑ |
| `StreamingJsonXmlConverterPrimitiveTest.primitiveFalse_followedByObjectEnd_isClosed` | `StreamingJsonXmlConverterPrimitiveTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterPrimitiveTest.kt` |  | Unit |  | 8 ⚑ |
| `StreamingJsonXmlConverterPrimitiveTest.primitiveWithWhitespaceBeforeComma_isClosed` | `StreamingJsonXmlConverterPrimitiveTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterPrimitiveTest.kt` |  | Unit |  | 13 ⚑ |
| `StreamingJsonXmlConverterPrimitiveTest.nestedComplexPrimitive_flushesOnlyAfterClosure` | `StreamingJsonXmlConverterPrimitiveTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterPrimitiveTest.kt` |  | Unit |  | 21 ⚑ |
| `StreamingJsonXmlConverterPrimitiveTest.render` | `StreamingJsonXmlConverterPrimitiveTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterPrimitiveTest.kt` | events: List<StreamingJsonXmlConverter.Even… | String |  | 27 ⚑ |
| `StreamingJsonXmlConverterStringTest.stringValue_withSlashEscape_isDecoded` | `StreamingJsonXmlConverterStringTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterStringTest.kt` |  | Unit |  | 8 ⚑ |
| `StreamingJsonXmlConverterStringTest.stringValue_withFormFeedEscape_isDecoded` | `StreamingJsonXmlConverterStringTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterStringTest.kt` |  | Unit |  | 13 ⚑ |
| `StreamingJsonXmlConverterStringTest.stringValue_withBackspaceEscape_isDecoded` | `StreamingJsonXmlConverterStringTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterStringTest.kt` |  | Unit |  | 18 ⚑ |
| `StreamingJsonXmlConverterStringTest.render` | `StreamingJsonXmlConverterStringTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterStringTest.kt` | events: List<StreamingJsonXmlConverter.Even… | String |  | 23 ⚑ |
| `StreamingJsonXmlConverterTest.stringValue_emitsParamTagAndContent` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 10 ⚑ |
| `StreamingJsonXmlConverterTest.multipleValues_emitMultipleParams` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 15 ⚑ |
| `StreamingJsonXmlConverterTest.numericValue_isCapturedAsPrimitive` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 23 ⚑ |
| `StreamingJsonXmlConverterTest.booleanValue_isCapturedAsPrimitive` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 28 ⚑ |
| `StreamingJsonXmlConverterTest.nullValue_isCapturedAsPrimitive` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 33 ⚑ |
| `StreamingJsonXmlConverterTest.arrayValue_isCapturedAsSinglePrimitiveBlock` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 38 ⚑ |
| `StreamingJsonXmlConverterTest.objectValue_isCapturedAsSinglePrimitiveBlock` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 43 ⚑ |
| `StreamingJsonXmlConverterTest.escapedXmlCharacters_areEncoded` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 51 ⚑ |
| `StreamingJsonXmlConverterTest.unicodeEscape_isDecoded` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 59 ⚑ |
| `StreamingJsonXmlConverterTest.escapedNewline_isDecoded` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 64 ⚑ |
| `StreamingJsonXmlConverterTest.escapedQuote_isDecodedAndEscapedForXml` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 69 ⚑ |
| `StreamingJsonXmlConverterTest.escapedBackslash_isDecoded` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 74 ⚑ |
| `StreamingJsonXmlConverterTest.chunkedStringInput_accumulatesAcrossFeeds` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 79 ⚑ |
| `StreamingJsonXmlConverterTest.chunkedPrimitiveInput_flushesAtEnd` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 85 ⚑ |
| `StreamingJsonXmlConverterTest.chunkedComplexValue_staysOpenUntilClosed` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 91 ⚑ |
| `StreamingJsonXmlConverterTest.flushWithoutPendingPrimitive_returnsNoEvents` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 99 ⚑ |
| `StreamingJsonXmlConverterTest.unfinishedString_keepsParamOpen` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 104 ⚑ |
| `StreamingJsonXmlConverterTest.finishedString_closesParam` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 110 ⚑ |
| `StreamingJsonXmlConverterTest.nestedObjectInsideArray_isPreserved` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 116 ⚑ |
| `StreamingJsonXmlConverterTest.whitespaceAroundValue_isIgnoredForPrimitiveParsing` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` |  | Unit |  | 124 ⚑ |
| `StreamingJsonXmlConverterTest.render` | `StreamingJsonXmlConverterTest` | `com.ai.assistance.operit.util` | `StreamingJsonXmlConverterTest.kt` | events: List<StreamingJsonXmlConverter.Even… | String |  | 129 ⚑ |
| `ToolingRegressionTest.toolResultAnyPattern_matchesToolResult` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 9 ⚑ |
| `ToolingRegressionTest.toolResultWithNameAnyPattern_extractsNameAndBody` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 13 ⚑ |
| `ToolingRegressionTest.toolOrToolResultBlock_matchesToolBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 19 ⚑ |
| `ToolingRegressionTest.statusPattern_extractsBody` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 23 ⚑ |
| `ToolingRegressionTest.nameAttr_extractsNameAttribute` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 29 ⚑ |
| `ToolingRegressionTest.statusAttr_extractsStatusAttribute` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 33 ⚑ |
| `ToolingRegressionTest.typeAttr_extractsTypeAttribute` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 37 ⚑ |
| `ToolingRegressionTest.titleAttr_extractsTitleAttribute` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 41 ⚑ |
| `ToolingRegressionTest.subtitleAttr_extractsSubtitleAttribute` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 45 ⚑ |
| `ToolingRegressionTest.toolAttr_extractsToolAttribute` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 49 ⚑ |
| `ToolingRegressionTest.uuidAttr_extractsUuidAttribute` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 53 ⚑ |
| `ToolingRegressionTest.contentTag_extractsInnerContent` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 57 ⚑ |
| `ToolingRegressionTest.errorTag_extractsInnerContent` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 61 ⚑ |
| `ToolingRegressionTest.statusTag_matchesStatusBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 65 ⚑ |
| `ToolingRegressionTest.statusSelfClosingTag_matchesBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 69 ⚑ |
| `ToolingRegressionTest.thinkTag_matchesThinkBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 73 ⚑ |
| `ToolingRegressionTest.thinkSelfClosingTag_matchesThinkBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 77 ⚑ |
| `ToolingRegressionTest.searchTag_matchesSearchBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 81 ⚑ |
| `ToolingRegressionTest.searchSelfClosingTag_matchesSearchBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 85 ⚑ |
| `ToolingRegressionTest.metaTag_matchesMetaBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 89 ⚑ |
| `ToolingRegressionTest.emotionTag_matchesEmotionBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 93 ⚑ |
| `ToolingRegressionTest.memoryTag_matchesMemoryBlock` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 97 ⚑ |
| `ToolingRegressionTest.replyToTag_extractsSenderAndTimestamp` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 101 ⚑ |
| `ToolingRegressionTest.attachmentDataTag_extractsAttachmentPayload` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 108 ⚑ |
| `ToolingRegressionTest.attachmentDataSelfClosingTag_extractsAttachmentPayload` | `ToolingRegressionTest` | `com.ai.assistance.operit.util` | `ToolingRegressionTest.kt` |  | Unit |  | 116 ⚑ |
| `TtsCleanerSpeechTest.disableAndroidLogging` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 30 ⚑ |
| `TtsCleanerSpeechTest.restoreAndroidLogging` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 38 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_withXmlTagFilter_readsOnlyReplyBody` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 44 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_withoutXmlTagFilter_readsOnlyReplyBody` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 52 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_filterStateDoesNotChangeSpokenBody` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 60 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_thinkingVariant_alsoSkipped` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 72 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_unclosedReasoning_isDroppedToEnd` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 80 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_reasoningWithAttributes_isDropped` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 88 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_uppercaseReasoning_isDropped` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 96 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_searchSources_areSkipped` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 104 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_toolCallsAndResults_areSkipped` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 112 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_statusAndEmotionTags_areSkipped` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 123 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_markdownBody_keepsTextUnderBothFilterStates` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit | ---- Auto read: the streamed segments and the final flush both flow through the same ----… | 137 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_userPatternStillAppliesToReplyBody` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 150 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_providerMetadataPayload_isSkipped` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 164 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_plainReplyWithoutMarkup_isUnchanged` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 177 ⚑ |
| `TtsCleanerSpeechTest.cleanForSpeech_reasoningOnly_yieldsBlankSoPlaybackIsSkipped` | `TtsCleanerSpeechTest` | `com.ai.assistance.operit.util` | `TtsCleanerSpeechTest.kt` |  | Unit |  | 183 ⚑ |
| `TtsSegmenterTest.decimalNumber_isNotSplitByDot` | `TtsSegmenterTest` | `com.ai.assistance.operit.util` | `TtsSegmenterTest.kt` |  | Unit |  | 8 ⚑ |
| `TtsSegmenterTest.versionNumber_isNotSplitByDot` | `TtsSegmenterTest` | `com.ai.assistance.operit.util` | `TtsSegmenterTest.kt` |  | Unit |  | 13 ⚑ |
| `TtsSegmenterTest.sentenceEndingDot_stillSplitsNormally` | `TtsSegmenterTest` | `com.ai.assistance.operit.util` | `TtsSegmenterTest.kt` |  | Unit |  | 18 ⚑ |
| `UpdateSourceProbeTest.setUp` | `UpdateSourceProbeTest` | `com.ai.assistance.operit.util` | `UpdateSourceProbeTest.kt` |  | Unit |  | 26 ⚑ |
| `UpdateSourceProbeTest.tearDown` | `UpdateSourceProbeTest` | `com.ai.assistance.operit.util` | `UpdateSourceProbeTest.kt` |  | Unit |  | 35 ⚑ |
| `UpdateSourceProbeTest.probe` | `UpdateSourceProbeTest` | `com.ai.assistance.operit.util` | `UpdateSourceProbeTest.kt` | timeoutMs: Int? | GithubReleaseUtil.ProbeResult |  | 39 ⚑ |
| `WaifuMessageProcessorTest.calculateTypingDelayMs_firstSegmentIsImmediate` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 19 ⚑ |
| `WaifuMessageProcessorTest.calculateTypingDelayMs_usesCurrentSegmentLengthForShortTail` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 31 ⚑ |
| `WaifuMessageProcessorTest.calculateTypingDelayMs_capsLongSegmentDelay` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 43 ⚑ |
| `WaifuMessageProcessorTest.calculateTypingDelayMs_nonPositiveDelayIsImmediate` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 55 ⚑ |
| `WaifuMessageProcessorTest.ensureBlockLatexDelimiters_wrapsDollarWhenMissing` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 67 ⚑ |
| `WaifuMessageProcessorTest.ensureBlockLatexDelimiters_preservesExistingDollarDelimiters` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 76 ⚑ |
| `WaifuMessageProcessorTest.ensureBlockLatexDelimiters_preservesBracketDelimiters` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 82 ⚑ |
| `WaifuMessageProcessorTest.ensureBlockLatexDelimiters_keepsOuterWhitespace` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 88 ⚑ |
| `WaifuMessageProcessorTest.ensureBlockLatexDelimiters_returnsBlankInputUnchanged` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 97 ⚑ |
| `WaifuMessageProcessorTest.ensureBlockLatexDelimiters_doesNotDoubleWrapEmptyBody` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 103 ⚑ |
| `WaifuMessageProcessorTest.requireNativeStreamSplitter` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit | ---- Integration tests below run the native block splitter and need libstreamnative.so. -… | 112 ⚑ |
| `WaifuMessageProcessorTest.splitMessageBySentences_preservesDollarBlockLatex` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 121 ⚑ |
| `WaifuMessageProcessorTest.splitMessageBySentences_preservesBracketBlockLatex` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 138 ⚑ |
| `WaifuMessageProcessorTest.splitMessageBySentences_doesNotSplitBlockLatexInterior` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 151 ⚑ |
| `WaifuMessageProcessorTest.splitMessageBySentences_keepsOrderAroundBlockLatex` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 162 ⚑ |
| `WaifuMessageProcessorTest.streamSegments_preservesDollarBlockLatexAcrossChunks` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 170 ⚑ |
| `WaifuMessageProcessorTest.streamSegments_preservesBracketBlockLatexAcrossChunks` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 194 ⚑ |
| `WaifuMessageProcessorTest.FixedTagXmlRenderPlugin.supports` | `FixedTagXmlRenderPlugin` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` | tagName: String | Boolean |  | 218 ⚑ |
| `WaifuMessageProcessorTest.FixedTagXmlRenderPlugin.resolve` | `FixedTagXmlRenderPlugin` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` | context: Context<br>xmlContent: String<br>tagName: String<br>textColor: Color<br>xmlStream: Stream<String>? | XmlRenderResult |  | 220 ⚑ |
| `WaifuMessageProcessorTest.withRegisteredXmlTags` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` | tags: String<br>block: () -> Unit | Unit |  | 229 ⚑ |
| `WaifuMessageProcessorTest.isRenderablePluginXmlContent_acceptsRegisteredVoiceTag` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 244 ⚑ |
| `WaifuMessageProcessorTest.isRenderablePluginXmlContent_acceptsRegisteredSelfClosingTag` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 255 ⚑ |
| `WaifuMessageProcessorTest.isRenderablePluginXmlContent_rejectsUnregisteredCustomTag` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 262 ⚑ |
| `WaifuMessageProcessorTest.isRenderablePluginXmlContent_rejectsControlTagsEvenWhenPluginRegistersThem` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 269 ⚑ |
| `WaifuMessageProcessorTest.isRenderablePluginXmlContent_rejectsUnclosedTag` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 288 ⚑ |
| `WaifuMessageProcessorTest.isRenderablePluginXmlBlock_requiresClosedRegisteredTag` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 295 ⚑ |
| `WaifuMessageProcessorTest.buildRenderableContentForWaifu_keepsRegisteredTagAndDropsControlXml` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 318 ⚑ |
| `WaifuMessageProcessorTest.splitMessageBySentences_emitsRegisteredVoiceTagAsStandaloneSegment` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 337 ⚑ |
| `WaifuMessageProcessorTest.streamSegments_preservesRegisteredVoiceTagAcrossChunks` | `WaifuMessageProcessorTest` | `com.ai.assistance.operit.util` | `WaifuMessageProcessorTest.kt` |  | Unit |  | 349 ⚑ |
| `WaifuRenderableSnapshotTest.liveSnapshotHoldsOpenCodeTableAndImageBlocks` | `WaifuRenderableSnapshotTest` | `com.ai.assistance.operit.util` | `WaifuRenderableSnapshotTest.kt` |  | Unit |  | 11 ⚑ |
| `WaifuRenderableSnapshotTest.switchingBlockTypeClosesThePreviousProtectedBlock` | `WaifuRenderableSnapshotTest` | `com.ai.assistance.operit.util` | `WaifuRenderableSnapshotTest.kt` |  | Unit |  | 42 ⚑ |
| `WaifuRenderableSnapshotTest.latexDelimitersAreRestoredOnlyWhenTheBlockCloses` | `WaifuRenderableSnapshotTest` | `com.ai.assistance.operit.util` | `WaifuRenderableSnapshotTest.kt` |  | Unit |  | 52 ⚑ |
| `WaifuRenderableSnapshotTest.internalXmlIsFilteredAfterItsNativeBlockCloses` | `WaifuRenderableSnapshotTest` | `com.ai.assistance.operit.util` | `WaifuRenderableSnapshotTest.kt` |  | Unit |  | 64 ⚑ |
| `WaifuRenderableSnapshotTest.emptySnapshotProducesNoContent` | `WaifuRenderableSnapshotTest` | `com.ai.assistance.operit.util` | `WaifuRenderableSnapshotTest.kt` |  | Unit |  | 76 ⚑ |
| `WaifuStreamUpdatesTest.disableAndroidLog` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 40 ⚑ |
| `WaifuStreamUpdatesTest.restoreAndroidLog` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 46 ⚑ |
| `WaifuStreamUpdatesTest.updates` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` | source: Stream<String><br>charDelayMs: Int? | Unit | The production revision/typing pipeline is exercised directly. A separator stands in for … | 52 ⚑ |
| `WaifuStreamUpdatesTest.rollbackRetractsAnAlreadyDisplayedSentence` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 66 ⚑ |
| `WaifuStreamUpdatesTest.retryPreservesPrefixIdentityDeletesOldBubbleAndClearsPendingTyping` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 90 ⚑ |
| `WaifuStreamUpdatesTest.finalHistoryWinsWhenAllEventsAreStillQueued` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 144 ⚑ |
| `WaifuStreamUpdatesTest.rollbackBeforeItsRawChunkDoesNotDisplayTheDiscardedChunk` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 162 ⚑ |
| `WaifuStreamUpdatesTest.repeatedRetriesRetractEachFailedAttempt` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 179 ⚑ |
| `WaifuStreamUpdatesTest.addingLaterSentencesDoesNotRestartTheCurrentTypingDelay` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 212 ⚑ |
| `WaifuStreamUpdatesTest.rollbackAtTypingDeadlinePreventsSendingTheAbandonedSentence` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 240 ⚑ |
| `WaifuStreamUpdatesTest.cancellationRetractsFinalizerRollbackAndDoesNotDrainTypingQueue` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 261 ⚑ |
| `WaifuStreamUpdatesTest.cancellationDuringBubblePersistenceRetractsThePartiallySavedMessage` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 289 ⚑ |
| `WaifuStreamUpdatesTest.providerFailureRetractsInvalidBubbleAndPropagatesOriginalException` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 324 ⚑ |
| `WaifuStreamUpdatesTest.finalSnapshotIncludesUnfinishedSentenceOnce` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 353 ⚑ |
| `WaifuStreamUpdatesTest.typingDelayStillCapsAtThreeSeconds` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 372 ⚑ |
| `WaifuStreamUpdatesTest.emptyStreamProducesNoBubbles` | `WaifuStreamUpdatesTest` | `com.ai.assistance.operit.util` | `WaifuStreamUpdatesTest.kt` |  | Unit |  | 381 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `AndroidUserPathUtils.PER_USER_RANGE` | `AndroidUserPathUtils` | `com.ai.assistance.operit.util` | `AndroidUserPathUtils.kt` | inferred |  | 6 |
| `AnrCaptureBudget.CAPTURE_COOLDOWN_MS` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | inferred | Minimum delay between two captures, enforced by [AnrCaptureThrottle]. | 25 |
| `AnrCaptureBudget.DUMP_TRUNCATION_MARKER` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | inferred |  | 32 |
| `AnrCaptureBudget.FRAME_PREFIX` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | inferred |  | 30 |
| `AnrCaptureBudget.MAX_DUMP_CHARS` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | inferred | Characters kept for a complete thread dump. | 22 |
| `AnrCaptureBudget.MAX_FRAME_CHARS` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | inferred | Characters kept for a single rendered frame line. | 16 |
| `AnrCaptureBudget.MAX_STACK_CHARS` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | inferred | Characters kept for one rendered stack section. | 19 |
| `AnrCaptureBudget.MAX_STACK_DEPTH` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | inferred | Frames rendered per capture. Deeper stacks are cut off instead of walked in ful… | 13 |
| `AnrCaptureBudget.SIGNATURE_DEPTH` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | inferred | Frames that identify a stall. Frames below this are not compared between captur… | 28 |
| `AnrCaptureBudget.STACK_TRUNCATION_MARKER` | `AnrCaptureBudget` | `com.ai.assistance.operit.util` | `AnrCaptureBudget.kt` | inferred |  | 31 |
| `AppLogger.ASSERT` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | Int |  | 30 |
| `AppLogger.boundContext` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | Context? |  | 83 |
| `AppLogger.dateFormat` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred | Simple date formatter for log lines | 42 |
| `AppLogger.DEBUG` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | Int |  | 26 |
| `AppLogger.enableFileLogging` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | Boolean | Optional external switch to completely disable file logging if needed. System A… | 68 |
| `AppLogger.enableSystemLog` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | Boolean | JVM 单元测试开关：关闭对 [android.util.Log] 的调用（返回 0/false），避免 纯 JVM 环境抛 "not mocked" 异常。… | 75 |
| `AppLogger.ERROR` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | Int |  | 29 |
| `AppLogger.fileLogExecutor` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 84 |
| `AppLogger.INFO` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | Int |  | 27 |
| `AppLogger.LOG_DIR_NAME` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred | Log file configuration | 33 |
| `AppLogger.LOG_FILE_NAME` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 34 |
| `AppLogger.logFile` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | File? |  | 78 |
| `AppLogger.MAX_LOG_MESSAGE_CHARS` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 38 |
| `AppLogger.MAX_LOG_THROWABLE_CHARS` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 39 |
| `AppLogger.MAX_PACKAGE_LOG_FILES` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 36 |
| `AppLogger.PACKAGE_LOG_DIR_NAME` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 35 |
| `AppLogger.packageIdRegexes` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 45 |
| `AppLogger.packageLogFile` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | File? |  | 80 |
| `AppLogger.packageLogFileNamePattern` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 44 |
| `AppLogger.pluginRegexes` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 57 |
| `AppLogger.scriptRegexes` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 51 |
| `AppLogger.startupFileDateFormat` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 43 |
| `AppLogger.TOOLPKG_LOG_TAG` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | inferred |  | 37 |
| `AppLogger.VERBOSE` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | Int | Mirror com.ai.assistance.operit.util.AppLogger priority constants | 25 |
| `AppLogger.WARN` | `AppLogger` | `com.ai.assistance.operit.util` | `AppLogger.kt` | Int |  | 28 |
| `ArchiveUtil.BUFFER_SIZE` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | inferred |  | 21 |
| `ArchiveUtil.TAG` | `ArchiveUtil` | `com.ai.assistance.operit.util` | `ArchiveUtil.kt` | inferred |  | 20 |
| `ChatMarkupRegex.anyXmlTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 195 |
| `ChatMarkupRegex.attachmentDataSelfClosingTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 170 |
| `ChatMarkupRegex.attachmentDataTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 166 |
| `ChatMarkupRegex.attachmentSelfClosingTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 180 |
| `ChatMarkupRegex.attachmentTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 175 |
| `ChatMarkupRegex.contentTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 107 |
| `ChatMarkupRegex.emotionTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 152 |
| `ChatMarkupRegex.errorTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 112 |
| `ChatMarkupRegex.GEMINI_THOUGHT_SIGNATURE_PROVIDER` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 7 |
| `ChatMarkupRegex.memoryTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 157 |
| `ChatMarkupRegex.metaBodyRegex` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 20 |
| `ChatMarkupRegex.metaProviderAttrRegex` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 19 |
| `ChatMarkupRegex.metaTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 147 |
| `ChatMarkupRegex.nameAttr` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 93 |
| `ChatMarkupRegex.namePattern` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 86 |
| `ChatMarkupRegex.OPENAI_RESPONSES_OUTPUT_ITEM_PROVIDER` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 9 |
| `ChatMarkupRegex.OPENAI_RESPONSES_REASONING_PROVIDER` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 8 |
| `ChatMarkupRegex.openingTagNameRegex` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 16 |
| `ChatMarkupRegex.proxySenderTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 190 |
| `ChatMarkupRegex.pruneToolResultContentPattern` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 197 |
| `ChatMarkupRegex.randomTagCodeChars` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 24 |
| `ChatMarkupRegex.randomTagCodeSource` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 25 |
| `ChatMarkupRegex.replyToTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 162 |
| `ChatMarkupRegex.searchSelfClosingTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 142 |
| `ChatMarkupRegex.searchTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 137 |
| `ChatMarkupRegex.statusAttr` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 95 |
| `ChatMarkupRegex.statusSelfClosingTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 122 |
| `ChatMarkupRegex.statusTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 117 |
| `ChatMarkupRegex.subtitleAttr` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 101 |
| `ChatMarkupRegex.thinkSelfClosingTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 132 |
| `ChatMarkupRegex.thinkTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 127 |
| `ChatMarkupRegex.titleAttr` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 99 |
| `ChatMarkupRegex.TOOL_RESULT_TAG_NAME_REGEX_SOURCE` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 12 |
| `ChatMarkupRegex.TOOL_TAG_NAME_REGEX_SOURCE` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 10 |
| `ChatMarkupRegex.TOOL_TAG_SUFFIX_REGEX_SOURCE` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 6 |
| `ChatMarkupRegex.toolAttr` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 103 |
| `ChatMarkupRegex.toolCallPattern` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 27 |
| `ChatMarkupRegex.toolOrToolResultBlock` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 67 |
| `ChatMarkupRegex.toolParamPattern` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 91 |
| `ChatMarkupRegex.toolResultAnyPattern` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 57 |
| `ChatMarkupRegex.toolResultSelfClosingTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 47 |
| `ChatMarkupRegex.toolResultStartTagRegex` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 18 |
| `ChatMarkupRegex.toolResultTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 42 |
| `ChatMarkupRegex.toolResultTagNameRegex` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 15 |
| `ChatMarkupRegex.toolResultTagWithAttrs` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 52 |
| `ChatMarkupRegex.toolResultWithNameAnyPattern` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 62 |
| `ChatMarkupRegex.toolSelfClosingTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 37 |
| `ChatMarkupRegex.toolStartTagRegex` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 17 |
| `ChatMarkupRegex.toolTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 32 |
| `ChatMarkupRegex.toolTagNameRegex` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 14 |
| `ChatMarkupRegex.typeAttr` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 97 |
| `ChatMarkupRegex.uuidAttr` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 105 |
| `ChatMarkupRegex.workspaceAttachmentTag` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 185 |
| `ChatMarkupRegex.xmlStatusPattern` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 72 |
| `ChatMarkupRegex.xmlToolRequestPattern` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 81 |
| `ChatMarkupRegex.xmlToolResultPattern` | `ChatMarkupRegex` | `com.ai.assistance.operit.util` | `ChatMarkupRegex.kt` | inferred |  | 76 |
| `ChatTrace.DEFAULT_PREVIEW_CHARS` | `ChatTrace` | `com.ai.assistance.operit.util` | `ChatTrace.kt` | inferred |  | 15 |
| `ChatUtils.searchContentPattern` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | inferred |  | 12 |
| `ChatUtils.thinkCapturePattern` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | inferred |  | 17 |
| `ChatUtils.thinkContentPattern` | `ChatUtils` | `com.ai.assistance.operit.util` | `ChatUtils.kt` | inferred | getMemoryFromMessages 会对每条 AI 消息调用 removeThinkingContent。 每次 toRegex() 都会走 ICU … | 10 |
| `CrashRecoveryState.KEY_PRESERVE_LOGS_FOR_CRASH_REPORT` | `CrashRecoveryState` | `com.ai.assistance.operit.util` | `CrashRecoveryState.kt` | inferred |  | 7 |
| `CrashRecoveryState.PREFS_NAME` | `CrashRecoveryState` | `com.ai.assistance.operit.util` | `CrashRecoveryState.kt` | inferred |  | 6 |
| `DocumentConversionUtil.TAG` | `DocumentConversionUtil` | `com.ai.assistance.operit.util` | `DocumentConversionUtil.kt` | inferred |  | 36 |
| `FFmpegUtil.TAG` | `FFmpegUtil` | `com.ai.assistance.operit.util` | `FFmpegUtil.kt` | inferred |  | 13 |
| `FileUtils.BACKGROUND_IMAGES_DIR` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | inferred |  | 18 |
| `FileUtils.BACKGROUND_VIDEOS_DIR` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | inferred |  | 19 |
| `FileUtils.mimeType` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | inferred | Try to get from content resolver | 352 |
| `FileUtils.TAG` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | inferred |  | 17 |
| `FileUtils.TEXT_BASED_EXTENSIONS` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | inferred |  | 24 |
| `FileUtils.TEXT_BASED_FILENAMES` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | inferred | Common text files without extensions | 51 |
| `FileUtils.VIDEO_EXTENSIONS` | `FileUtils` | `com.ai.assistance.operit.util` | `FileUtils.kt` | inferred | List of common video file extensions | 22 |
| `ImageBitmapLimiter.AI_MAX_DIMENSION` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | inferred |  | 13 |
| `ImageBitmapLimiter.AI_MAX_PIXELS` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | inferred |  | 12 |
| `ImageBitmapLimiter.UI_MAX_DIMENSION` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | inferred |  | 10 |
| `ImageBitmapLimiter.UI_MAX_PIXELS` | `ImageBitmapLimiter` | `com.ai.assistance.operit.util` | `ImageBitmapLimiter.kt` | inferred |  | 9 |
| `ImagePoolManager.cacheDir` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | File? |  | 60 |
| `ImagePoolManager.DEFAULT_JPEG_QUALITY` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | inferred |  | 40 |
| `ImagePoolManager.DEFAULT_MAX_LONG_EDGE` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | inferred |  | 41 |
| `ImagePoolManager.DEFAULT_REGISTRATION_OPTIONS` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | inferred |  | 43 |
| `ImagePoolManager.DEFAULT_SCALE_PERCENT` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | inferred |  | 39 |
| `ImagePoolManager.hasResetCacheOnInitialize` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | inferred |  | 61 |
| `ImagePoolManager.imagePool` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | inferred |  | 83 |
| `ImagePoolManager.maxPoolSize` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | inferred |  | 52 |
| `ImagePoolManager.TAG` | `ImagePoolManager` | `com.ai.assistance.operit.util` | `ImagePoolManager.kt` | inferred |  | 38 |
| `IntRangeSerializer.descriptor` | `IntRangeSerializer` | `com.ai.assistance.operit.util` | `IntRangeSerializer.kt` | SerialDescriptor |  | 13 |
| `LatexMathMlConverter.ASSET_PATH` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | inferred |  | 10 |
| `LatexMathMlConverter.BOOTSTRAP` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | inferred |  | 73 |
| `LatexMathMlConverter.engine` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | OperitQuickJsEngine? |  | 16 |
| `LatexMathMlConverter.FUNCTION_NAME` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | inferred |  | 11 |
| `LatexMathMlConverter.lock` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | inferred |  | 13 |
| `LatexMathMlConverter.TAG` | `LatexMathMlConverter` | `com.ai.assistance.operit.util` | `LatexMathMlConverter.kt` | inferred |  | 9 |
| `LocalDateTimeSerializer.descriptor` | `LocalDateTimeSerializer` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializer.kt` | SerialDescriptor |  | 15 |
| `LocalDateTimeSerializer.formatter` | `LocalDateTimeSerializer` | `com.ai.assistance.operit.util` | `LocalDateTimeSerializer.kt` | inferred |  | 13 |
| `LocaleUtils.legacyLanguageCodeAliases` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | inferred |  | 31 |
| `LocaleUtils.supportedLanguageCodes` | `LocaleUtils` | `com.ai.assistance.operit.util` | `LocaleUtils.kt` | inferred |  | 60 |
| `LocationUtils.TAG` | `LocationUtils` | `com.ai.assistance.operit.util` | `LocationUtils.kt` | inferred |  | 28 |
| `MathMlPlainTextConverter.FUNCTION_NAMES` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | inferred |  | 121 |
| `MathMlPlainTextConverter.LARGE_OPERATORS` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | inferred |  | 127 |
| `MathMlPlainTextConverter.SUBSCRIPTS` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | inferred |  | 136 |
| `MathMlPlainTextConverter.SUPERSCRIPTS` | `MathMlPlainTextConverter` | `com.ai.assistance.operit.util` | `MathMlPlainTextConverter.kt` | inferred |  | 129 |
| `MediaBase64Limiter.decoded` | `MediaBase64Limiter` | `com.ai.assistance.operit.util` | `MediaBase64Limiter.kt` | inferred |  | 37 |
| `MediaBase64Limiter.DEFAULT_MAX_DECODED_BYTES` | `MediaBase64Limiter` | `com.ai.assistance.operit.util` | `MediaBase64Limiter.kt` | inferred |  | 6 |
| `MediaPoolManager.cacheDir` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | File? |  | 131 |
| `MediaPoolManager.MAX_INPUT_BYTES` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | inferred |  | 14 |
| `MediaPoolManager.maxPoolSize` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | inferred |  | 123 |
| `MediaPoolManager.mediaPool` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | inferred |  | 154 |
| `MediaPoolManager.TAG` | `MediaPoolManager` | `com.ai.assistance.operit.util` | `MediaPoolManager.kt` | inferred |  | 12 |
| `metadataContentPattern` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | inferred |  | 376 |
| `OCRUtils.chineseRecognizer` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | TextRecognizer? |  | 33 |
| `OCRUtils.japaneseRecognizer` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | TextRecognizer? |  | 34 |
| `OCRUtils.koreanRecognizer` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | TextRecognizer? |  | 35 |
| `OCRUtils.latinRecognizer` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | TextRecognizer? | 识别器缓存 | 32 |
| `OCRUtils.TAG` | `OCRUtils` | `com.ai.assistance.operit.util` | `OCRUtils.kt` | inferred |  | 29 |
| `OperitPaths.BRIDGE_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 13 |
| `OperitPaths.CLEAN_ON_EXIT_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 10 |
| `OperitPaths.EXPORTS_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 14 |
| `OperitPaths.IMAGE_POOL_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 23 |
| `OperitPaths.MCP_PLUGINS_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 12 |
| `OperitPaths.MEDIA_POOL_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 24 |
| `OperitPaths.OPERIT_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 9 |
| `OperitPaths.PLUGINS_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 11 |
| `OperitPaths.SHERPA_NCNN_MODELS_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 20 |
| `OperitPaths.SKILL_REPO_ZIP_POOL_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 25 |
| `OperitPaths.TEST_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 16 |
| `OperitPaths.USERSCRIPTS_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 18 |
| `OperitPaths.VECTOR_INDEX_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 21 |
| `OperitPaths.WEBSESSION_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 17 |
| `OperitPaths.WORKSPACE_DIR_NAME` | `OperitPaths` | `com.ai.assistance.operit.util` | `OperitPaths.kt` | inferred |  | 15 |
| `PortProcessKiller.TAG` | `PortProcessKiller` | `com.ai.assistance.operit.util` | `PortProcessKiller.kt` | inferred |  | 7 |
| `previous` | — | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | inferred |  | 69 |
| `SCRIPT_MARKET_ORIGIN_METADATA_KEY` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | inferred |  | 375 |
| `SerializationSetup.module` | `SerializationSetup` | `com.ai.assistance.operit.util` | `SerializationSetup.kt` | inferred | Creates and returns a SerializersModule with all custom serializers registered | 13 |
| `SkillRepoZipPoolManager.cacheDir` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | File? |  | 20 |
| `SkillRepoZipPoolManager.evictionMutex` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | inferred |  | 23 |
| `SkillRepoZipPoolManager.keyMutexes` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | inferred |  | 22 |
| `SkillRepoZipPoolManager.maxPoolSize` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | inferred |  | 12 |
| `SkillRepoZipPoolManager.TAG` | `SkillRepoZipPoolManager` | `com.ai.assistance.operit.util` | `SkillRepoZipPoolManager.kt` | inferred |  | 10 |
| `staticModuleReferencePattern` | — | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | inferred |  | 377 |
| `TextSegmenter.baseInitialized` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | inferred |  | 23 |
| `TextSegmenter.initLock` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | inferred |  | 20 |
| `TextSegmenter.loadedUserDictPaths` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | inferred |  | 25 |
| `TextSegmenter.MAX_CACHE_SIZE` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | inferred | 最大缓存大小 | 31 |
| `TextSegmenter.PREWARM_TEXT` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | inferred |  | 15 |
| `TextSegmenter.segmentCache` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | inferred | 关键词缓存，提高性能 | 28 |
| `TextSegmenter.TAG` | `TextSegmenter` | `com.ai.assistance.operit.util` | `TextSegmenter.kt` | inferred |  | 14 |
| `ThrowableTextFormatter.DEFAULT_MAX_CHARS` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | inferred |  | 8 |
| `ThrowableTextFormatter.FORMAT_FAILURE_MARKER` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | inferred |  | 13 |
| `ThrowableTextFormatter.MAX_CAUSE_DEPTH` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | inferred |  | 11 |
| `ThrowableTextFormatter.MAX_FRAMES_PER_THROWABLE` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | inferred |  | 10 |
| `ThrowableTextFormatter.MIN_MAX_CHARS` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | inferred |  | 9 |
| `ThrowableTextFormatter.TRUNCATED_MARKER` | `ThrowableTextFormatter` | `com.ai.assistance.operit.util` | `ThrowableTextFormatter.kt` | inferred |  | 12 |
| `ToolPkgArtifactMinifier.candidates` | `ToolPkgArtifactMinifier` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | inferred |  | 281 |
| `ToolPkgArtifactMinifier.modulePath` | `ToolPkgArtifactMinifier` | `com.ai.assistance.operit.util` | `ToolPkgArtifactMinifier.kt` | inferred |  | 280 |
| `ToolPkgWasmRuntime.hexDigits` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | inferred |  | 14 |
| `ToolPkgWasmRuntime.moduleLock` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | inferred |  | 13 |
| `ToolPkgWasmRuntime.modules` | `ToolPkgWasmRuntime` | `com.ai.assistance.operit.util` | `ToolPkgWasmRuntime.kt` | inferred |  | 12 |
| `TRAILING_PROTECTED_TEXT_CHARS` | — | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 938 |
| `TtsCleaner.TAG` | `TtsCleaner` | `com.ai.assistance.operit.util` | `TtsCleaner.kt` | inferred |  | 6 |
| `TtsSegmenter.END_CHARS` | `TtsSegmenter` | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | inferred |  | 5 |
| `TtsSegmenter.MAX_SEGMENT_LENGTH` | `TtsSegmenter` | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | inferred |  | 4 |
| `TtsSegmenter.next` | `TtsSegmenter` | `com.ai.assistance.operit.util` | `TtsSegmenter.kt` | inferred |  | 55 |
| `UriSerializer.descriptor` | `UriSerializer` | `com.ai.assistance.operit.util` | `UriSerializer.kt` | SerialDescriptor |  | 12 |
| `WaifuMessageProcessor.activePromptManager` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | ActivePromptManager? |  | 66 |
| `WaifuMessageProcessor.BARE_URL_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 33 |
| `WaifuMessageProcessor.customEmojiRepository` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | CustomEmojiRepository? |  | 65 |
| `WaifuMessageProcessor.DOMAIN_URL_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 35 |
| `WaifuMessageProcessor.EMAIL_ADDRESS_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 34 |
| `WaifuMessageProcessor.ENTITY_PLACEHOLDER_PREFIX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 22 |
| `WaifuMessageProcessor.ENTITY_PLACEHOLDER_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 37 |
| `WaifuMessageProcessor.ENTITY_PLACEHOLDER_SUFFIX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 23 |
| `WaifuMessageProcessor.FENCED_CODE_BLOCK_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 25 |
| `WaifuMessageProcessor.HORIZONTAL_RULE_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 31 |
| `WaifuMessageProcessor.MARKDOWN_ENTITY_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 32 |
| `WaifuMessageProcessor.MAX_TYPING_DELAY_MS` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 24 |
| `WaifuMessageProcessor.nonRenderableXmlTags` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred | 不能按"插件渲染标签"放行的内部标签：控制信息、上下文包装标签，以及仍由 表情转换链路单独处理的 emotion。即使插件注册了同名渲染器，这些标签也必须 继… | 45 |
| `WaifuMessageProcessor.SENTENCE_END_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 29 |
| `WaifuMessageProcessor.SENTENCE_SPLIT_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 27 |
| `WaifuMessageProcessor.UNCLOSED_FENCED_CODE_BLOCK_REGEX` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 26 |
| `WaifuMessageProcessor.URL_CHARS` | `WaifuMessageProcessor` | `com.ai.assistance.operit.util` | `WaifuMessageProcessor.kt` | inferred |  | 21 |
