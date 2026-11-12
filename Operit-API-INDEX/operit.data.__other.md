# operit.data.（其余零散）

> 函数 931 · 类型 289 · 顶层常量 87 · 共 1307 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `AiWorkRow` | `AiWorkRow` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | class AiWorkRow(val durationMs: Long, val longestReplyTokens: Long, val firstTrackedAt: Long?) |  | 43 |
| `AnnouncementContent` | `AnnouncementContent` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | class AnnouncementContent(val defaultLocale: String, val locales: Map<String, AnnouncementLocal…) |  | 58 |
| `AnnouncementLocaleContent` | `AnnouncementLocaleContent` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | class AnnouncementLocaleContent(val title: String, val body: String, val acknowledge: String) |  | 64 |
| `AnnouncementMeta` | `AnnouncementMeta` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | class AnnouncementMeta(val updatedAt: String?, val source: String?) |  | 71 |
| `AnnouncementPointer` | `AnnouncementPointer` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | class AnnouncementPointer(val schemaVersion: Int, val latestVersion: Int, val latestFile: String, val updatedAt: String?, val notes: String?) |  | 20 |
| `AnnouncementSchedule` | `AnnouncementSchedule` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | class AnnouncementSchedule(val startAt: String?, val endAt: String?) |  | 52 |
| `AnnouncementTarget` | `AnnouncementTarget` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | class AnnouncementTarget(val minAppVersionCode: Int, val maxAppVersionCode: Int?, val channels: List<String>, val locale: String) |  | 44 |
| `AnnualReportCollector` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | class AnnualReportCollector(context: Context) | 按数据契约生成年度报告的用户数据。全程只读，运行在 IO 线程。 任何一个数据源读取失败都直接抛出，由宿主把原因交给页面的错误页，不输出缺字段的报告。 | 35 |
| `AnnualReportCollector.Window` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | class Window(val zone: ZoneId, val start: ZonedDateTime, val end: ZonedDateTime) |  | 41 |
| `AnnualReportDao` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | interface AnnualReportDao |  | 55 |
| `ApiProviderConfigs` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | object ApiProviderConfigs |  | 19 |
| `AppDatabase` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | class AppDatabase : RoomDatabase |  | 39 |
| `AppDatabaseMigrationTest` | `AppDatabaseMigrationTest` | `com.ai.assistance.operit.data.db` | `AppDatabaseMigrationTest.kt` | class AppDatabaseMigrationTest |  | 9 |
| `ArtifactProjectDetailResponse` | `ArtifactProjectDetailResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class ArtifactProjectDetailResponse(val projectId: String, val type: String, val projectDisplayName: String, val projectDescription: String, val rootPublisherLogin: String, val rootPublisherAvat… |  | 137 |
| `ArtifactProjectRankDefaultVersionResponse` | `ArtifactProjectRankDefaultVersionResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class ArtifactProjectRankDefaultVersionResponse(val versionId: String, val runtimePackageId: String, val sha256: String, val version: String, val apiVersion: String?, val downloadUrl: String, val state: Str… |  | 68 |
| `ArtifactProjectRankEntryResponse` | `ArtifactProjectRankEntryResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class ArtifactProjectRankEntryResponse(val entryId: String, val projectId: String, val type: String, val projectDisplayName: String, val projectDescription: String, val rootPublisherLogin: String, … |  | 80 |
| `ArtifactProjectRankPageResponse` | `ArtifactProjectRankPageResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class ArtifactProjectRankPageResponse(val updatedAt: String?, val type: String, val metric: String, val page: Int, val pageSize: Int, val totalPages: Int, val totalItems: Int, val items: List<Arti… |  | 99 |
| `ArtifactProjectVersionResponse` | `ArtifactProjectVersionResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class ArtifactProjectVersionResponse(val projectId: String, val type: String, val projectDisplayName: String, val projectDescription: String, val runtimePackageId: String, val versionId: String, … |  | 111 |
| `BridgeMcpRuntimeSession` | `BridgeMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `BridgeMcpRuntimeSession.kt` | class BridgeMcpRuntimeSession(context: Context, private val serviceName: String) : McpRuntimeSession | Local stdio runtime backed by the Node bridge. | 11 |
| `BusiestDay` | `BusiestDay` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class BusiestDay(val date: String, val messages: Long) |  | 100 |
| `CharacterHighlight` | `CharacterHighlight` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class CharacterHighlight(val name: String, val messages: Long, val chats: Long) |  | 133 |
| `CharacterHighlightRow` | `CharacterHighlightRow` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | class CharacterHighlightRow(val name: String, val messages: Long, val chats: Long) |  | 37 |
| `ChatBoxConverter` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | class ChatBoxConverter(private val context: Context) : ChatFormatConverter | ChatBox 格式转换器 支持 ChatBox 桌面应用的导出格式 ChatBox 导出格式参考： { "sessions": [ { "id": "session-id", … | 37 |
| `ChatContentCharacterCount` | `ChatContentCharacterCount` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | class ChatContentCharacterCount(val chatId: String, val contentCharacterCount: Long) |  | 83 |
| `ChatContentDao` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | class ChatContentDao | Reads message text in bounded rows so a single large message cannot overflow CursorWindow. | 90 |
| `ChatContentDaoNulContentTest` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` | class ChatContentDaoNulContentTest | 真实 Room + JVM SQLite 驱动下的消息读取测试。 重点覆盖 U+0000：SQLite 的 LENGTH/SUBSTR 把 TEXT 当字符处理并在第一个 NUL… | 29 |
| `ChatDao` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | interface ChatDao | 聊天DAO接口，定义对聊天表的数据访问方法 | 15 |
| `ChatFormat` | `ChatFormat` | `com.ai.assistance.operit.data.converter` | `ChatFormat.kt` | class ChatFormat | 支持的聊天记录格式 | 6 |
| `ChatFormatConverter` | `ChatFormatConverter` | `com.ai.assistance.operit.data.converter` | `ChatFormatConverter.kt` | interface ChatFormatConverter | 聊天记录格式转换器接口 | 8 |
| `ChatFormatDetector` | `ChatFormatDetector` | `com.ai.assistance.operit.data.converter` | `ChatFormatDetector.kt` | object ChatFormatDetector | 聊天记录格式检测器 自动识别导入文件的格式 | 9 |
| `ChatGPTAuthor` | `ChatGPTAuthor` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | class ChatGPTAuthor(val role: String, val name: String?) |  | 194 |
| `ChatGPTContent` | `ChatGPTContent` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | class ChatGPTContent(val content_type: String, val parts: List<String>) |  | 200 |
| `ChatGPTConversation` | `ChatGPTConversation` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | class ChatGPTConversation(val id: String?, val title: String?, val create_time: Long, val update_time: Long, val mapping: Map<String, ChatGPTNode>, val current_node: String?) | ChatGPT 数据结构定义 | 167 |
| `ChatGPTConverter` | `ChatGPTConverter` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | class ChatGPTConverter : ChatFormatConverter | ChatGPT conversations.json 格式转换器 支持 OpenAI 官方导出的格式 | 16 |
| `ChatGPTMessage` | `ChatGPTMessage` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | class ChatGPTMessage(val id: String?, val author: ChatGPTAuthor, val content: ChatGPTContent?, val create_time: Long, val metadata: ChatGPTMetadata?) |  | 185 |
| `ChatGPTMetadata` | `ChatGPTMetadata` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | class ChatGPTMetadata(val model_slug: String?, val is_user_system_message: Boolean?) |  | 206 |
| `ChatGPTNode` | `ChatGPTNode` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | class ChatGPTNode(val id: String?, val message: ChatGPTMessage?, val parent: String?, val children: List<String>) |  | 177 |
| `ChatHighlight` | `ChatHighlight` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class ChatHighlight(val title: String, val messages: Long) |  | 127 |
| `ChatHighlightRow` | `ChatHighlightRow` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | class ChatHighlightRow(val title: String, val messages: Long) |  | 32 |
| `ChatHistoryCsv` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | object ChatHistoryCsv | Versioned CSV representation for Operit chat history exports. A chat is represented by on… | 14 |
| `ChatMessageCount` | `ChatMessageCount` | `com.ai.assistance.operit.data.dao` | `ChatMessageCount.kt` | class ChatMessageCount(val chatId: String, val count: Int) |  | 3 |
| `CodexAuthManager` | `CodexAuthManager` | `com.ai.assistance.operit.data.api` | `CodexAuthManager.kt` | class CodexAuthManager(context: Context) |  | 17 |
| `CodexJwtClaims` | `CodexJwtClaims` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | class CodexJwtClaims(val accountId: String?, val residency: String?, val email: String?, val expiresAtMillis: Long?) |  | 23 |
| `CodexOAuthClient` | `CodexOAuthClient` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | class CodexOAuthClient(private val client: OkHttpClient, private val issuer: String) |  | 152 |
| `CodexOAuthProtocol` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | object CodexOAuthProtocol |  | 44 |
| `CodexOAuthTokenResponse` | `CodexOAuthTokenResponse` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | class CodexOAuthTokenResponse(val idToken: String?, val accessToken: String?, val refreshToken: String?, val expiresInSeconds: Long?) |  | 30 |
| `CodexOAuthTokenResponseTest` | `CodexOAuthTokenResponseTest` | `com.ai.assistance.operit.data.api` | `CodexOAuthTokenResponseTest.kt` | class CodexOAuthTokenResponseTest |  | 6 |
| `CodexPkceCodes` | `CodexPkceCodes` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | class CodexPkceCodes(val verifier: String, val challenge: String) |  | 18 |
| `CodexUsageClient` | `CodexUsageClient` | `com.ai.assistance.operit.data.api` | `CodexUsageClient.kt` | class CodexUsageClient(private val client: OkHttpClient) |  | 30 |
| `CodexUsageClientTest` | `CodexUsageClientTest` | `com.ai.assistance.operit.data.api` | `CodexUsageClientTest.kt` | class CodexUsageClientTest |  | 13 |
| `CodexUsageSnapshot` | `CodexUsageSnapshot` | `com.ai.assistance.operit.data.api` | `CodexUsageClient.kt` | class CodexUsageSnapshot(val planType: String?, val fiveHourWindow: CodexUsageWindow?, val sevenDayWindow: CodexUsageWindow?) |  | 24 |
| `CodexUsageWindow` | `CodexUsageWindow` | `com.ai.assistance.operit.data.api` | `CodexUsageClient.kt` | class CodexUsageWindow(val usedPercent: Int, val windowDurationSeconds: Long?, val resetsAtEpochSeconds: Long?) |  | 14 |
| `ConversionException` | `ConversionException` | `com.ai.assistance.operit.data.converter` | `ChatFormatConverter.kt` | class ConversionException(message: String, cause: Throwable?) : Exception | 转换异常 | 26 |
| `CreateReleaseRequest` | `CreateReleaseRequest` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | class CreateReleaseRequest(val tag_name: String, val name: String?, val body: String?, val draft: Boolean, val prerelease: Boolean) |  | 75 |
| `CreateRepositoryContentRequest` | `CreateRepositoryContentRequest` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | class CreateRepositoryContentRequest(val message: String, val content: String, val branch: String?, val sha: String?) |  | 59 |
| `CreateRepositoryRequest` | `CreateRepositoryRequest` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | class CreateRepositoryRequest(val name: String, val description: String?, val homepage: String?, val `private`: Boolean, val has_issues: Boolean, val has_projects: Boolean, val has_wiki: B… |  | 47 |
| `DailyActivity` | `DailyActivity` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class DailyActivity(val date: String, val messages: Long, val tokens: Long) |  | 86 |
| `DayCountRow` | `DayCountRow` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | class DayCountRow(val localDate: String, val count: Long) |  | 16 |
| `DefaultModelPricingCollect` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | object DefaultModelPricingCollect |  | 22 |
| `DefaultModelPricingCollect.ScrapedPricingRow` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | class ScrapedPricingRow(val provider: String, val model: String, val defaults: ModelPricingDefaults) |  | 91 |
| `DownloadState` | `DownloadState` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | class DownloadState |  | 79 |
| `DownloadState.Completed` | `DownloadState` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | object Completed : DownloadState |  | 92 |
| `DownloadState.Idle` | `DownloadState` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | object Idle : DownloadState |  | 80 |
| `DownloadState.MnnModelDownloadManager` | `DownloadState` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | class MnnModelDownloadManager(private val context: Context) |  | 96 |
| `ExportFormat` | `ExportFormat` | `com.ai.assistance.operit.data.converter` | `ChatFormat.kt` | class ExportFormat | 导出格式 | 38 |
| `FirstMessage` | `FirstMessage` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class FirstMessage(val at: String, val text: String, val chatTitle: String) |  | 120 |
| `FirstMessageRow` | `FirstMessageRow` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | class FirstMessageRow(val timestamp: Long, val preview: String, val chatTitle: String) |  | 26 |
| `FullUpdateInstaller` | `FullUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | object FullUpdateInstaller | Downloads the full release APK and verifies it before install. GitHub publishes a SHA-256… | 21 |
| `FullUpdateInstaller.ProgressEvent` | `FullUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | class ProgressEvent |  | 27 |
| `FullUpdateInstaller.ProgressEvent.AllSourcesFailedException` | `ProgressEvent` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | class AllSourcesFailedException(val failures: List<UpdateSourceDownloader.S…) : IllegalStateException | Every candidate source failed; the per-source reasons are surfaced to the user. | 49 |
| `FullUpdateInstaller.ProgressEvent.DownloadProgress` | `ProgressEvent` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | class DownloadProgress(val readBytes: Long, val totalBytes: Long?, val speedBytesPerSec: Long) : ProgressEvent |  | 41 |
| `FullUpdateInstaller.ProgressEvent.SourceFailed` | `ProgressEvent` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | class SourceFailed(val name: String, val reason: String, val attempt: Int, val total: Int) : ProgressEvent | A source died mid-transfer; the flow moved on to the next candidate. | 34 |
| `FullUpdateInstaller.ProgressEvent.StageChanged` | `ProgressEvent` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | class StageChanged(val stage: Stage, val message: String) : ProgressEvent |  | 28 |
| `FullUpdateInstaller.Stage` | `FullUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | class Stage |  | 22 |
| `GenericJsonConverter` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` | class GenericJsonConverter : ChatFormatConverter | 通用 JSON 格式转换器 支持标准的 role-content 格式 | 16 |
| `GitHubApiService` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | class GitHubApiService(private val context: Context) | GitHub API服务类 提供GitHub用户信息、仓库操作等功能 | 128 |
| `GitHubIdentity` | `GitHubIdentity` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class GitHubIdentity(val login: String, val id: Long) |  | 44 |
| `GitHubOAuthBrokerClaimResponse` | `GitHubOAuthBrokerClaimResponse` | `com.ai.assistance.operit.data.api` | `GitHubOAuthBrokerService.kt` | class GitHubOAuthBrokerClaimResponse(val ok: Boolean, val status: String, val accessToken: String?, val tokenType: String?, val scope: String?, val expiresIn: Long?, val refreshToken: String?, va… |  | 28 |
| `GitHubOAuthBrokerClaimResult` | `GitHubOAuthBrokerClaimResult` | `com.ai.assistance.operit.data.api` | `GitHubOAuthBrokerService.kt` | class GitHubOAuthBrokerClaimResult(val accessToken: String, val tokenType: String, val scope: String, val expiresIn: Long?, val refreshToken: String?, val user: GitHubUser) |  | 39 |
| `GitHubOAuthBrokerService` | `GitHubOAuthBrokerService` | `com.ai.assistance.operit.data.api` | `GitHubOAuthBrokerService.kt` | class GitHubOAuthBrokerService |  | 48 |
| `GitHubOAuthBrokerStartResponse` | `GitHubOAuthBrokerStartResponse` | `com.ai.assistance.operit.data.api` | `GitHubOAuthBrokerService.kt` | class GitHubOAuthBrokerStartResponse(val ok: Boolean, val transactionId: String, val deliveryCredential: String, val authorizationUrl: String, val completionRedirectUri: String, val expiresAt: Lo… |  | 18 |
| `GitHubRelease` | `GitHubRelease` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | class GitHubRelease(val id: Long, val tag_name: String, val name: String?, val body: String?, val html_url: String, val upload_url: String?, val published_at: String?, val create… |  | 94 |
| `GitHubReleaseAsset` | `GitHubReleaseAsset` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | class GitHubReleaseAsset(val id: Long, val name: String, val browser_download_url: String, val size: Long, val download_count: Int, val content_type: String, /** * Checksum GitHub pub… |  | 109 |
| `GitHubRepository` | `GitHubRepository` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | class GitHubRepository(val id: Long, val name: String, val full_name: String, val description: String?, val html_url: String, val clone_url: String, val stargazers_count: Int, val f… |  | 26 |
| `GitHubRepositoryContentFile` | `GitHubRepositoryContentFile` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | class GitHubRepositoryContentFile(val name: String, val path: String, val sha: String, val type: String) |  | 67 |
| `HourCountRow` | `HourCountRow` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | class HourCountRow(val hour: Int, val count: Long) |  | 21 |
| `HtmlExporter` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | object HtmlExporter | HTML 格式导出器 | 14 |
| `InstallProgress` | `InstallProgress` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | class InstallProgress | 安装进度状态 | 1370 |
| `InstallProgress.Finished` | `InstallProgress` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | object Finished : InstallProgress |  | 1374 |
| `InstallProgress.InstallResult` | `InstallProgress` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | class InstallResult | 安装结果 | 1378 |
| `InstallProgress.InstallResult.Success` | `InstallResult` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | class Success(val pluginPath: String) : InstallResult |  | 1379 |
| `InstallProgress.Preparing` | `InstallProgress` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | object Preparing : InstallProgress |  | 1371 |
| `JdbcSQLiteConnection` | `JdbcSQLiteConnection` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | class JdbcSQLiteConnection(fileName: String) : SQLiteConnection |  | 38 |
| `JdbcSQLiteConnection.TransactionStatement` | `JdbcSQLiteConnection` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | class TransactionStatement(private val action: () -> Unit) : SQLiteStatement |  | 94 |
| `JdbcSQLiteDriver` | `JdbcSQLiteDriver` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | class JdbcSQLiteDriver : SQLiteDriver | 单元测试用纯 JVM SQLite 驱动：基于 org.xerial:sqlite-jdbc 实现 androidx.sqlite 的 KMP [SQLiteDriver]/[S… | 34 |
| `JdbcSQLiteStatement` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | class JdbcSQLiteStatement(private val statement: PreparedStatement) : SQLiteStatement |  | 118 |
| `MarkdownConverter` | `MarkdownConverter` | `com.ai.assistance.operit.data.converter` | `MarkdownConverter.kt` | class MarkdownConverter(private val context: Context) : ChatFormatConverter | Markdown 格式转换器 支持多种 Markdown 对话格式 | 16 |
| `MarkdownExporter` | `MarkdownExporter` | `com.ai.assistance.operit.data.exporter` | `MarkdownExporter.kt` | object MarkdownExporter | Markdown 格式导出器 | 12 |
| `MarketRankEntryResponse` | `MarketRankEntryResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketRankEntryResponse(val id: String, val downloads: Int, val lastDownloadAt: String?, val updatedAt: String?, val statsUpdatedAt: String?, val displayTitle: String, val summaryDes… |  | 41 |
| `MarketRankPageResponse` | `MarketRankPageResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketRankPageResponse(val updatedAt: String?, val type: String, val metric: String, val page: Int, val pageSize: Int, val totalPages: Int, val totalItems: Int, val items: List<Mark… |  | 56 |
| `MarketStatsApiService` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketStatsApiService |  | 510 |
| `MarketStatsEntryResponse` | `MarketStatsEntryResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketStatsEntryResponse(val downloads: Int, val lastDownloadAt: String?, val updatedAt: String?) |  | 28 |
| `MarketTypeStatsResponse` | `MarketTypeStatsResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketTypeStatsResponse(val updatedAt: String?, val items: Map<String, MarketStatsEntryR…) |  | 35 |
| `MarketV2Artifact` | `MarketV2Artifact` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2Artifact(val projectId: String, val runtimePkg: String?) |  | 361 |
| `MarketV2Asset` | `MarketV2Asset` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2Asset(val id: String, val versionId: String, val kind: String, val url: String, val sha256: String, val ghOwner: String, val ghRepo: String, val ghReleaseTag: Strin… |  | 367 |
| `MarketV2Author` | `MarketV2Author` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2Author(val id: String, val githubId: Long?, val login: String, val avatar: String?, val avatarUrl: String?, val status: String) |  | 345 |
| `MarketV2AuthResponse` | `MarketV2AuthResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2AuthResponse(val ok: Boolean, val session: String, val githubId: Long, val login: String, val avatarUrl: String) |  | 154 |
| `MarketV2Comment` | `MarketV2Comment` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2Comment(val id: String, val entryId: String, val parentId: String?, val author: MarketV2Author, val body: String, val createdAt: String, val updatedAt: String) |  | 406 |
| `MarketV2CommentCreateRequest` | `MarketV2CommentCreateRequest` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2CommentCreateRequest(val body: String, val parentId: String?) |  | 505 |
| `MarketV2CommentResponse` | `MarketV2CommentResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2CommentResponse(val ok: Boolean, val item: MarketV2Comment?, val comment: MarketV2Comment?) |  | 277 |
| `MarketV2CommentsPageResponse` | `MarketV2CommentsPageResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2CommentsPageResponse(val ok: Boolean, val marketVersion: Int, val entryId: String, val page: Int, val pageSize: Int, val total: Int, val items: List<MarketV2Comment>, val generate… |  | 265 |
| `MarketV2EntriesShardResponse` | `MarketV2EntriesShardResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2EntriesShardResponse(val ok: Boolean, val marketVersion: Int, val generatedAt: String?, val shard: String, val entriesById: Map<String, MarketV2Entry>) |  | 205 |
| `MarketV2Entry` | `MarketV2Entry` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2Entry(val type: String, val id: String, val title: String, val description: String, val detail: String, val logoUrl: String?, val authorId: String, val publisherId:… |  | 306 |
| `MarketV2EntryResponse` | `MarketV2EntryResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2EntryResponse(val ok: Boolean, val item: MarketV2Entry?, val entry: MarketV2Entry?) |  | 258 |
| `MarketV2EntryStats` | `MarketV2EntryStats` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2EntryStats(val downloads: Int, val likes: Int, val lastDownloadAt: String?, val updatedAt: String?) |  | 337 |
| `MarketV2EntryUpdateRequest` | `MarketV2EntryUpdateRequest` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2EntryUpdateRequest(val title: String, val description: String, val detail: String, val categoryId: String, val allowPublicUpdates: Boolean?) |  | 460 |
| `MarketV2ListResponse` | `MarketV2ListResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2ListResponse(val ok: Boolean, val marketVersion: Int, val generatedAt: String?, val sort: String, val page: Int, val pageSize: Int, val total: Int, val items: List<MarketV… |  | 163 |
| `MarketV2ManifestCategory` | `MarketV2ManifestCategory` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2ManifestCategory(val id: String, val name: String, val description: String) |  | 192 |
| `MarketV2ManifestResponse` | `MarketV2ManifestResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2ManifestResponse(val ok: Boolean, val marketVersion: Int, val generatedAt: String?, val types: List<MarketV2ManifestType>, val categories: List<MarketV2ManifestCategory>, val … |  | 175 |
| `MarketV2ManifestState` | `MarketV2ManifestState` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2ManifestState(val code: String, val publicListed: Boolean) |  | 199 |
| `MarketV2ManifestType` | `MarketV2ManifestType` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2ManifestType(val id: String, val name: String, val description: String) |  | 185 |
| `MarketV2MyEntriesResponse` | `MarketV2MyEntriesResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2MyEntriesResponse(val ok: Boolean, val entries: MarketV2PublisherEntriesRespo…) |  | 214 |
| `MarketV2NewVersionEntryPatch` | `MarketV2NewVersionEntryPatch` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2NewVersionEntryPatch(val title: String?, val description: String?, val detail: String?, val categoryId: String?, val allowPublicUpdates: Boolean?) |  | 451 |
| `MarketV2NewVersionRequest` | `MarketV2NewVersionRequest` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2NewVersionRequest(val entry: MarketV2NewVersionEntryPatch?, val version: MarketV2PublishVersion, val repoVersion: MarketV2PublishRepoVersion?, val asset: MarketV2PublishAsset?) |  | 443 |
| `MarketV2NewVersionResponse` | `MarketV2NewVersionResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2NewVersionResponse(val ok: Boolean, val entryId: String, val versionId: String) |  | 299 |
| `MarketV2Notification` | `MarketV2Notification` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2Notification(val id: String, val kind: String, val entryId: String, val commentId: String?, val actorId: String?, val title: String, val body: String, val createdAt: Strin… |  | 417 |
| `MarketV2NotificationsResponse` | `MarketV2NotificationsResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2NotificationsResponse(val ok: Boolean, val items: List<MarketV2Notification>) |  | 284 |
| `MarketV2PublishAsset` | `MarketV2PublishAsset` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2PublishAsset(val kind: String, val url: String, val ghOwner: String, val ghRepo: String, val ghReleaseTag: String, val assetName: String, val sha256: String) |  | 494 |
| `MarketV2PublisherEntriesResponse` | `MarketV2PublisherEntriesResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2PublisherEntriesResponse(val ok: Boolean, val generatedAt: String?, val shard: String, val entries: List<MarketV2PublisherEntrySu…) |  | 220 |
| `MarketV2PublisherEntrySummary` | `MarketV2PublisherEntrySummary` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2PublisherEntrySummary(val id: String, val title: String, val type: String, val relation: String, val stateCode: String, val listingState: String, val categoryId: String, val update… |  | 237 |
| `MarketV2PublisherShardResponse` | `MarketV2PublisherShardResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2PublisherShardResponse(val ok: Boolean, val marketVersion: Int, val generatedAt: String?, val shard: String, val authors: Map<String, MarketV2Publisher…) |  | 228 |
| `MarketV2PublishRepoVersion` | `MarketV2PublishRepoVersion` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2PublishRepoVersion(val refType: String, val refName: String, val installConfig: String) |  | 487 |
| `MarketV2PublishRequest` | `MarketV2PublishRequest` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2PublishRequest(val type: String, val title: String, val description: String, val detail: String, val categoryId: String, val allowPublicUpdates: Boolean, val version: Market… |  | 429 |
| `MarketV2PublishResponse` | `MarketV2PublishResponse` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2PublishResponse(val ok: Boolean, val item: MarketV2Entry?, val entry: MarketV2Entry?, val entryId: String?, val versionId: String?) |  | 290 |
| `MarketV2PublishSource` | `MarketV2PublishSource` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2PublishSource(val kind: String, val url: String) |  | 481 |
| `MarketV2PublishVersion` | `MarketV2PublishVersion` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2PublishVersion(val version: String, val formatVer: String, val minAppVer: String, val apiVersion: String?, val maxAppVer: String?, val changelog: String?, val projectId: Str… |  | 469 |
| `MarketV2Reaction` | `MarketV2Reaction` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2Reaction(val reaction: String, val content: String, val total: Int) |  | 399 |
| `MarketV2Source` | `MarketV2Source` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2Source(val kind: String, val url: String) |  | 355 |
| `MarketV2Version` | `MarketV2Version` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | class MarketV2Version(val id: String, val version: String, val formatVer: String, val apiVersion: String?, val publisherId: String, val publisher: MarketV2Author?, val minAppVer: S… |  | 381 |
| `MCPBridge` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | class MCPBridge(private val context: Context) | MCPBridge - 用于与TCP桥接器通信的插件类 支持以下命令: - spawn: 启动新的MCP服务 - shutdown: 关闭当前MCP服务 - listtools:… | 43 |
| `MCPBridgeClient` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | class MCPBridgeClient(private val context: Context, private val serviceName: String) | MCPBridgeClient - Client for communicating with MCP services through a bridge | 14 |
| `MCPCommandGenerator` | `MCPCommandGenerator` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPCommandGenerator.kt` | class MCPCommandGenerator | MCP 命令生成器 负责生成MCP插件的部署和启动命令 | 11 |
| `MCPConfigGenerator` | `MCPConfigGenerator` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPConfigGenerator.kt` | class MCPConfigGenerator | MCP 配置生成器 负责生成MCP插件的配置文件 | 14 |
| `McpConfigImport` | `McpConfigImport` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | class McpConfigImport(val servers: List<McpImportedServer>) | Parsed standard MCP configuration used by both UI and market imports. | 8 |
| `McpConfigImportParser` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | object McpConfigImportParser | Parses the public MCP configuration format without conflating HTTP transports with stdio. | 38 |
| `McpConfigImportParserTest` | `McpConfigImportParserTest` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParserTest.kt` | class McpConfigImportParserTest |  | 8 |
| `MCPDeployer` | `MCPDeployer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` | class MCPDeployer(private val context: Context) | MCP 插件部署工具类 负责协调项目分析、命令生成和配置生成等组件完成插件部署 | 25 |
| `MCPDeployer.DeploymentStatus` | `MCPDeployer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` | class DeploymentStatus | 部署状态 | 40 |
| `MCPDeployer.DeploymentStatus.NotStarted` | `DeploymentStatus` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` | object NotStarted : DeploymentStatus |  | 41 |
| `McpImportedServer` | `McpImportedServer` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | interface McpImportedServer |  | 12 |
| `MCPLocalServer` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | class MCPLocalServer(private val context: Context) | 统一的MCP配置管理中心 负责管理所有MCP相关的配置，包括： - 官方MCP配置格式的读写 - 插件配置管理 - 服务器状态管理 - 统一存储在下载/Operit/mcp_pl… | 47 |
| `MCPLocalServer.CachedToolInfo` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | class CachedToolInfo(val name: String, val description: String, val inputSchema: String, val cachedAt: Long) | 缓存的工具信息 | 214 |
| `MCPLocalServer.MCPConfig` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | class MCPConfig(val mcpServers: MutableMap<String, ServerConf…, val pluginMetadata: MutableMap<String, PluginMeta…) | 官方MCP配置格式数据结构 | 116 |
| `MCPLocalServer.MCPConfig.PluginMetadata` | `MCPConfig` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | class PluginMetadata | 插件元数据 | 145 |
| `MCPLocalServer.MCPConfig.ServerConfig` | `MCPConfig` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | class ServerConfig(val command: String, val args: List<String>?, val disabled: Boolean, val autoApprove: List<String>?, val env: Map<String, String>?, val cwd: String?) |  | 123 |
| `MCPLocalServer.SanitizedConfigResult` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | class SanitizedConfigResult(val config: MCPConfig, val removedServerIds: List<String>, val removedMetadataIds: List<String>) |  | 368 |
| `MCPLocalServer.ServerStatus` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | class ServerStatus(val serverId: String, val lastStartTime: Long, val lastStopTime: Long, val errorMessage: String?, val cachedTools: List<CachedToolInfo>?, val toolsCachedTime:… | 服务器运行状态 注意：启用/禁用状态已移至ServerConfig.disabled字段 | 195 |
| `MCPProjectAnalyzer` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | class MCPProjectAnalyzer | MCP 项目结构分析器 负责分析插件项目结构，识别项目类型和特征 | 12 |
| `MCPRepository` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | class MCPRepository(private val context: Context) | 统一的MCP仓库管理类 职责： - 管理MCP服务器的UI状态和数据 - 处理插件的安装、卸载 - 管理已安装插件的状态跟踪 - 处理远程服务器的添加和管理 配置管理由MCPLo… | 50 |
| `MCPSharedSession` | `MCPSharedSession` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPSharedSession.kt` | object MCPSharedSession | MCP 共享终端会话管理器 用于在 MCPStarter 和 MCPDeployer 之间共享同一个终端会话 避免重复创建会话，提高资源利用效率 | 15 |
| `MCPStarter` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | class MCPStarter(private val context: Context) | MCP Plugin Starter Coordinates local bridge-backed stdio plugins and Kotlin SDK remote pl… | 30 |
| `MCPStarter.PluginInitStatus` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | class PluginInitStatus | Plugin initialization status enum | 42 |
| `MCPStarter.PluginRegistration` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | class PluginRegistration(val serviceName: String?, val failureDetail: String?) | Result of registering one plugin, carrying the concrete failure when registration fails. | 646 |
| `MCPStarter.PluginStartProgressListener` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | interface PluginStartProgressListener | Plugin start progress listener interface | 51 |
| `MCPStarter.StartStatus` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | class StartStatus | Start status | 1038 |
| `MCPStarter.StartStatus.NotStarted` | `StartStatus` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | object NotStarted : StartStatus |  | 1039 |
| `MCPStarter.StartStatus.PnpmMissing` | `StartStatus` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | class PnpmMissing(val message: String) : StartStatus |  | 1047 |
| `MCPStarter.StartStatus.VerificationResult` | `StartStatus` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | class VerificationResult(val pluginId: String, val serviceName: String, val isResponding: Boolean, val responseTime: Long, val details: String) | Verification result | 1053 |
| `McpStdioConfigResolver` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | object McpStdioConfigResolver | Pure rules for a local stdio MCP server declared in `mcpServers`. A config is "self-conta… | 14 |
| `McpStdioConfigResolverTest` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` | class McpStdioConfigResolverTest |  | 8 |
| `MessageContentRow` | `MessageContentRow` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | class MessageContentRow(val message: MessageEntity, val contentByteCount: Long, val contentBytes: ByteArray) |  | 71 |
| `MessageDao` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | interface MessageDao | 消息DAO接口，定义对消息表的数据访问方法 | 13 |
| `MessageLocatorRow` | `MessageLocatorRow` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | class MessageLocatorRow(val chatId: String, val timestamp: Long) |  | 49 |
| `MessageVariantContentRow` | `MessageVariantContentRow` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | class MessageVariantContentRow(val variant: MessageVariantEntity, val contentByteCount: Long, val contentBytes: ByteArray) |  | 77 |
| `MessageVariantDao` | `MessageVariantDao` | `com.ai.assistance.operit.data.dao` | `MessageVariantDao.kt` | interface MessageVariantDao |  | 11 |
| `MnnModel` | `MnnModel` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | class MnnModel(val modelName: String, val size_gb: Double, val tags: List<String>, val sources: Map<String, String>, val description: String) |  | 29 |
| `ModelMarketData` | `ModelMarketData` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | class ModelMarketData(val models: List<MnnModel>) |  | 38 |
| `ModelPricingDefaults` | `ModelPricingDefaults` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | class ModelPricingDefaults(val billingMode: BillingMode, val inputPricePerMillion: Double, val outputPricePerMillion: Double, val cachedInputPricePerMillion: Double, val pricePerRequest… |  | 13 |
| `ModelThinkingConfigDefaults` | `ModelThinkingConfigDefaults` | `com.ai.assistance.operit.data.collects` | `ModelThinkingConfigDefaultsCollect.kt` | object ModelThinkingConfigDefaults |  | 7 |
| `ModelUsage` | `ModelUsage` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class ModelUsage(val model: String, val tokens: Long, val requests: Long) |  | 57 |
| `MsFileInfo` | `MsFileInfo` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | class MsFileInfo(val Name: String?, val Path: String?, val Size: Long, val Type: String?) |  | 57 |
| `MsRepoInfo` | `MsRepoInfo` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | class MsRepoInfo(val Code: Int, val Data: MsResponseData?, val Message: String?, val Success: Boolean) | ModelScope API 响应数据结构 | 44 |
| `MsResponseData` | `MsResponseData` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | class MsResponseData(val Files: List<MsFileInfo>?) |  | 52 |
| `ObjectBoxManager` | `ObjectBoxManager` | `com.ai.assistance.operit.data.db` | `ObjectBox.kt` | object ObjectBoxManager |  | 9 |
| `OperitBackupDirs` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` | object OperitBackupDirs |  | 6 |
| `PatchUpdateInstaller` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | object PatchUpdateInstaller |  | 27 |
| `PatchUpdateInstaller.AllSourcesFailedException` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | class AllSourcesFailedException(val failures: List<UpdateSourceDownloader.S…) : IllegalStateException | Every candidate source failed; the per-source reasons are surfaced to the user. | 108 |
| `PatchUpdateInstaller.CdEntry` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | class CdEntry(val localHeaderOffset: Long, val compressedSize: Long) |  | 666 |
| `PatchUpdateInstaller.MirrorProbeSummary` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | class MirrorProbeSummary(val ok: Boolean, val latencyMs: Long?, val speedBytesPerSec: Long?, val error: String?) | Probe result for one source in the download-source dialog. Kept here because the dialog a… | 44 |
| `PatchUpdateInstaller.PatchStep` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | class PatchStep(val patchUrl: String, val metaUrl: String, val baseSha256: String, val targetSha256: String, val toVersion: String, val toPatchIndex: Int, val targetVersionLa… | One edge of the patch chain. [metaAssetSha256] and [patchAssetSha256] are the digests Git… | 95 |
| `PatchUpdateInstaller.ProgressEvent` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | class ProgressEvent |  | 51 |
| `PatchUpdateInstaller.ProgressEvent.ChainScanProgress` | `ProgressEvent` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | class ChainScanProgress(val scanned: Int, val total: Int) : ProgressEvent |  | 69 |
| `PatchUpdateInstaller.ProgressEvent.SourceFailed` | `ProgressEvent` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | class SourceFailed(val name: String, val reason: String, val attempt: Int, val total: Int) : ProgressEvent | A source died while transferring, so the flow moved to the next one. Carrying the reason … | 62 |
| `PatchUpdateInstaller.ProgressEvent.StageChanged` | `ProgressEvent` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | class StageChanged(val stage: Stage, val message: String) : ProgressEvent |  | 52 |
| `PatchUpdateInstaller.Stage` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | class Stage |  | 31 |
| `PersistentDownloadState` | `PersistentDownloadState` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | class PersistentDownloadState(val modelName: String, val url: String, val modelFolderName: String, val totalBytes: Long, val fileTasks: List<PersistentFileTask>) |  | 65 |
| `PersistentFileTask` | `PersistentFileTask` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | class PersistentFileTask(val path: String, val size: Long) |  | 74 |
| `PersonalMarket` | `PersonalMarket` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class PersonalMarket(val entries: Int, val downloads: Long, val likes: Long, val titles: List<String>) | 登录 GitHub 的用户在插件市场的作品，打开对应场景时按需请求。 | 167 |
| `PluginDenylistEntry` | `PluginDenylistEntry` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | class PluginDenylistEntry(val sha256: String, val note: String?) |  | 41 |
| `PluginDenylistPayload` | `PluginDenylistPayload` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | class PluginDenylistPayload(val schemaVersion: Int, val version: Int, val updatedAt: String?, val hashAlgorithm: String, val match: String, val action: String, val entries: List<PluginDe… |  | 30 |
| `PluginDenylistPointer` | `PluginDenylistPointer` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | class PluginDenylistPointer(val schemaVersion: Int, val latestVersion: Int, val latestFile: String, val updatedAt: String?, val notes: String?) |  | 21 |
| `PluginDenylistRepository` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | class PluginDenylistRepository(context: Context, private val pointerUrl: String) |  | 46 |
| `PreferencesHealthManager` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | object PreferencesHealthManager | User-triggered physical validation and preservation-first repair for Preferences DataStor… | 35 |
| `PreferencesHealthManager.CheckItem` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | class CheckItem(val title: String, val detail: String, val status: ItemStatus) |  | 56 |
| `PreferencesHealthManager.CopyValidation` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | interface CopyValidation |  | 94 |
| `PreferencesHealthManager.CopyValidation.Corrupt` | `CopyValidation` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | class Corrupt(val reason: String) : CopyValidation data class Failed |  | 99 |
| `PreferencesHealthManager.CopyValidation.Readable` | `CopyValidation` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | object Readable : CopyValidation data class DomainIssues |  | 95 |
| `PreferencesHealthManager.DomainIssue` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | class DomainIssue(val storeName: String, val detail: String) |  | 72 |
| `PreferencesHealthManager.ItemStatus` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | class ItemStatus |  | 50 |
| `PreferencesHealthManager.MainProcessState` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | class MainProcessState |  | 88 |
| `PreferencesHealthManager.RepairFailedException` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | class RepairFailedException(val sourceArchive: File, cause: Throwable) : IllegalStateException |  | 83 |
| `PreferencesHealthManager.RepairResult` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | class RepairResult(val sourceArchive: File, val resetFileNames: List<String>, val report: Report) |  | 77 |
| `PreferencesHealthManager.Report` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | class Report(val status: Status, val summary: String, val checks: List<CheckItem>, val repairableFileNames: List<String>) |  | 62 |
| `PreferencesHealthManager.Status` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | class Status |  | 44 |
| `PricingCurrency` | `PricingCurrency` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | class PricingCurrency(val code: String, val symbol: String) |  | 5 |
| `ProjectStructure` | `ProjectStructure` | `com.ai.assistance.operit.data.mcp.plugins` | `ProjectStructure.kt` | class ProjectStructure(val type: ProjectType, val hasRequirementsTxt: Boolean, val hasPyprojectToml: Boolean, val hasSetupPy: Boolean, val hasPackageJson: Boolean, val hasTsConfig: … | 项目结构信息数据类 | 14 |
| `ProjectType` | `ProjectType` | `com.ai.assistance.operit.data.mcp.plugins` | `ProjectStructure.kt` | class ProjectType | 项目类型枚举 | 6 |
| `ProviderApiConfig` | `ProviderApiConfig` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | class ProviderApiConfig(val providerType: ApiProviderType, val defaultModelName: String, val defaultApiEndpoint: String, val endpointOptions: List<ProviderEndpointOption>, val requir… |  | 11 |
| `ProviderEndpointOption` | `ProviderEndpointOption` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | class ProviderEndpointOption(val endpoint: String, val label: String) |  | 6 |
| `RankedSources` | `RankedSources` | `com.ai.assistance.operit.data.updates` | `UpdateDownloadSource.kt` | class RankedSources(val usable: List<SourceCandidate>, val rejected: List<SourceCandidate>) | Probe outcome split into the sources the updater may download from and the ones it must s… | 29 |
| `RawSnapshotBackupManager` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | object RawSnapshotBackupManager |  | 37 |
| `RawSnapshotBackupManager.ExportProgress` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | class ExportProgress |  | 69 |
| `RawSnapshotBackupManager.ExportProgressInfo` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | class ExportProgressInfo(val stage: ExportProgress, val percent: Int?, val scannedFiles: Int?) |  | 80 |
| `RawSnapshotBackupManager.Manifest` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | class Manifest(val formatVersion: Int, val packageName: String, val createdAt: Long, val includes: List<String>, val includeTerminalData: Boolean) |  | 57 |
| `RawSnapshotBackupManager.RestoreProgress` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | class RestoreProgress |  | 86 |
| `RawSnapshotBackupManager.SnapshotOptions` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | class SnapshotOptions(val includeTerminalData: Boolean) |  | 65 |
| `RawSnapshotBackupManagerTest` | `RawSnapshotBackupManagerTest` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManagerTest.kt` | class RawSnapshotBackupManagerTest |  | 7 |
| `RemoteAnnouncementDisplay` | `RemoteAnnouncementDisplay` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | class RemoteAnnouncementDisplay(val id: String, val version: Int, val title: String, val body: String, val acknowledgeText: String, val countdownSec: Int) |  | 76 |
| `RemoteAnnouncementPayload` | `RemoteAnnouncementPayload` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | class RemoteAnnouncementPayload(val schemaVersion: Int, val id: String, val version: Int, val enabled: Boolean, val type: String, val priority: String, val countdownSec: Int, val target: Ann… |  | 29 |
| `RemoteAnnouncementRepository` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | class RemoteAnnouncementRepository(private val pointerUrl: String) |  | 85 |
| `RemoteMcpImportedServer` | `RemoteMcpImportedServer` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | class RemoteMcpImportedServer(override val id: String, val endpoint: String, val connectionType: String, val headers: Map<String, String>, override val disabled: Boolean) : McpImportedServer |  | 27 |
| `RemoteMcpRuntimeSession` | `RemoteMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` | class RemoteMcpRuntimeSession(private val pluginId: String, private val descriptor: McpRuntimeDescriptor.Remote) : McpRuntimeSession | Remote MCP runtime backed directly by the Kotlin SDK and Ktor. | 29 |
| `ReportDataError` | `ReportDataError` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class ReportDataError(val message: String) | 原生返回给页面的错误体，页面原样展示 message。 | 176 |
| `ReportWindow` | `ReportWindow` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class ReportWindow(val start: String, val end: String, val timeZone: String) |  | 12 |
| `RoomDatabaseBackupManager` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | object RoomDatabaseBackupManager |  | 20 |
| `RoomDatabaseBackupManager.BackupResult` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | class BackupResult(val performed: Boolean, val backupFile: File?, val skippedReason: String?) |  | 27 |
| `RoomDatabaseBackupPreferences` | `RoomDatabaseBackupPreferences` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupPreferences.kt` | class RoomDatabaseBackupPreferences(private val context: Context) |  | 19 |
| `RoomDatabaseBackupScheduler` | `RoomDatabaseBackupScheduler` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupScheduler.kt` | object RoomDatabaseBackupScheduler |  | 15 |
| `RoomDatabaseBackupWorker` | `RoomDatabaseBackupWorker` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupWorker.kt` | class RoomDatabaseBackupWorker(appContext: Context, workerParams: WorkerParameters) : CoroutineWorker |  | 8 |
| `RoomDatabaseHealthManager` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | object RoomDatabaseHealthManager | User-triggered Room diagnostics and narrowly scoped repair operations. | 28 |
| `RoomDatabaseHealthManager.CheckItem` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | class CheckItem(val title: String, val detail: String, val status: ItemStatus) |  | 58 |
| `RoomDatabaseHealthManager.ItemStatus` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | class ItemStatus |  | 41 |
| `RoomDatabaseHealthManager.MainProcessState` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | class MainProcessState |  | 52 |
| `RoomDatabaseHealthManager.PreservingCorruptionHandler` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | class PreservingCorruptionHandler : DatabaseErrorHandler |  | 677 |
| `RoomDatabaseHealthManager.RepairAction` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | class RepairAction |  | 47 |
| `RoomDatabaseHealthManager.RepairFailedException` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | class RepairFailedException(val sourceArchive: File, cause: Throwable) : IllegalStateException |  | 81 |
| `RoomDatabaseHealthManager.RepairResult` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | class RepairResult(val sourceArchive: File, val completedActions: List<RepairAction>, val report: Report) |  | 75 |
| `RoomDatabaseHealthManager.Report` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | class Report(val status: Status, val summary: String, val databasePath: String, val checks: List<CheckItem>, val repairActions: List<RepairAction>) |  | 64 |
| `RoomDatabaseHealthManager.Status` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | class Status |  | 35 |
| `RoomDatabaseHealthManagerTest` | `RoomDatabaseHealthManagerTest` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManagerTest.kt` | class RoomDatabaseHealthManagerTest |  | 7 |
| `RoomDatabaseRestoreManager` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | object RoomDatabaseRestoreManager |  | 21 |
| `ScrapedModelPricingRowsCollect` | `ScrapedModelPricingRowsCollect` | `com.ai.assistance.operit.data.collects` | `ScrapedModelPricingRowsCollect.kt` | object ScrapedModelPricingRowsCollect |  | 3 |
| `SenderCountRow` | `SenderCountRow` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | class SenderCountRow(val sender: String, val count: Long) | 年度报告的只读聚合查询。所有统计都在 SQL 里完成，不把消息正文读进内存； 只有工具调用需要解析正文，这里只筛出候选消息的定位信息，正文交给 ChatContentDao 分段… | 11 |
| `ServiceInfo` | `ServiceInfo` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | class ServiceInfo(val name: String, val active: Boolean, val ready: Boolean, val toolCount: Int, val toolNames: List<String>) | Data class to hold service information | 660 |
| `SkillRepository` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | class SkillRepository(private val context: Context) |  | 24 |
| `SkillRepository.GitHubSkillTarget` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | class GitHubSkillTarget(val owner: String, val repo: String, val ref: String?, val subDir: String?) |  | 48 |
| `SkillRepository.SkillRepoImportResult` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | class SkillRepoImportResult(val message: String, val installedDir: File?) |  | 84 |
| `SourceCandidate` | `SourceCandidate` | `com.ai.assistance.operit.data.updates` | `UpdateDownloadSource.kt` | class SourceCandidate(val key: String, val url: String, val speedBytesPerSec: Long?, val latencyMs: Long?, val probeError: String?) | One download source probed for an update artifact, plus the reason it cannot be used when… | 15 |
| `StdioMcpImportedServer` | `StdioMcpImportedServer` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | class StdioMcpImportedServer(override val id: String, val command: String, val args: List<String>, val env: Map<String, String>, val autoApprove: List<String>, override val disabled: Bool… : McpImportedServer |  | 17 |
| `StreakRange` | `StreakRange` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class StreakRange(val days: Int, val start: String, val end: String) |  | 93 |
| `TextExporter` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | object TextExporter | 纯文本格式导出器 | 14 |
| `TokenUsageActivityDayRow` | `TokenUsageActivityDayRow` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | class TokenUsageActivityDayRow(val localDate: String, val tokens: Long) |  | 30 |
| `TokenUsageDao` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | class TokenUsageDao |  | 36 |
| `TokenUsageModelAggregateRow` | `TokenUsageModelAggregateRow` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | class TokenUsageModelAggregateRow(val provider: String, val model: String, val configId: String, val requests: Long, val uncachedInputTokens: Long, val uncachedInputKnown: Long, val cachedInpu… |  | 10 |
| `ToolUsage` | `ToolUsage` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class ToolUsage(val name: String, val count: Long) |  | 147 |
| `UnifiedToolInfo` | `UnifiedToolInfo` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | class UnifiedToolInfo(val name: String, val description: String, val inputSchema: String) | 统一的工具信息数据类 | 1363 |
| `UpdateReleaseRequest` | `UpdateReleaseRequest` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | class UpdateReleaseRequest(val tag_name: String?, val name: String?, val body: String?, val draft: Boolean?, val prerelease: Boolean?) |  | 84 |
| `UpdateSourceDownloader` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | object UpdateSourceDownloader | Fetches one update artifact, walking the ranked source list until a source delivers a fil… | 35 |
| `UpdateSourceDownloader.SourceFailure` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | class SourceFailure(val sourceKey: String, val reason: String) | One source rejected during this artifact download, with the reason. | 45 |
| `UpdateSourceDownloader.SourceFailure.Progress` | `SourceFailure` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | class Progress(val sourceKey: String, val readBytes: Long, val totalBytes: Long?, val speedBytesPerSec: Long) |  | 52 |
| `UpdateSourceDownloader.SourceFailure.Success` | `SourceFailure` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | class Success(val file: File, val sourceKey: String) : Outcome |  | 48 |
| `UpdateSourceDownloaderTest` | `UpdateSourceDownloaderTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloaderTest.kt` | class UpdateSourceDownloaderTest | Covers the failure switch that issue #1177 asks for: a source that returns 403/404, times… | 23 |
| `UpdateSourceRanking` | `UpdateSourceRanking` | `com.ai.assistance.operit.data.updates` | `UpdateDownloadSource.kt` | object UpdateSourceRanking | Turns probe results into the ordered source list both update paths walk. Ranking lives he… | 63 |
| `UpdateSourceRankingTest` | `UpdateSourceRankingTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceRankingTest.kt` | class UpdateSourceRankingTest | Ranking decides which source the downloader tries first and which ones it refuses to touc… | 14 |
| `UpdateStatus` | `UpdateStatus` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | class UpdateStatus | 更新状态 - 移除下载相关状态 | 16 |
| `UpdateStatus.Initial` | `UpdateStatus` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | object Initial : UpdateStatus |  | 17 |
| `UpdateStatus.UpdateManager` | `UpdateStatus` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | class UpdateManager(private val context: Context) | UpdateManager - 处理应用更新的核心类 负责检查更新 | 43 |
| `UpdateStatus.UpdateManager.ParsedVersion` | `UpdateManager` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | class ParsedVersion(val major: Int, val minor: Int, val patch: Int, val patchIndex: Int) : String | 比较两个版本号 | 70 |
| `UpdateStatus.UpToDate` | `UpdateStatus` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | object UpToDate : UpdateStatus |  | 38 |
| `UserActivity` | `UserActivity` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserActivity(val days: List<DailyActivity>, val activeDays: Int, val longestStreak: StreakRange?, val busiestDay: BusiestDay?) |  | 106 |
| `UserAiWork` | `UserAiWork` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserAiWork(val durationMs: Long, val longestReplyTokens: Long, val coverageStart: String?) |  | 140 |
| `UserCost` | `UserCost` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserCost(val currency: String, val known: Double, val unpricedRequests: Long) |  | 50 |
| `UserCreations` | `UserCreations` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserCreations(val memories: Long, val characterCards: Long, val workflows: Long) |  | 159 |
| `UserHours` | `UserHours` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserHours(val byHour: List<Long>, val latestNight: String?) |  | 114 |
| `UserInstall` | `UserInstall` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserInstall(val firstInstallAt: String) |  | 39 |
| `UserMessages` | `UserMessages` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserMessages(val user: Long, val ai: Long, val chatsCreated: Long, val regenerations: Long, val favorites: Long) |  | 77 |
| `UserReport` | `UserReport` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserReport(val schemaVersion: Int, val year: Int, val generatedAt: String, val window: ReportWindow, val install: UserInstall, val github: GitHubIdentity?, val tokens: U… |  | 19 |
| `UserTokens` | `UserTokens` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserTokens(val coverageStart: String?, val total: Long, val input: Long, val output: Long, val cachedInput: Long, val requests: Long, val cost: UserCost, val byMonth: Li… |  | 64 |
| `UserTools` | `UserTools` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | class UserTools(val total: Long, val top: List<ToolUsage>) |  | 153 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `RemoteAnnouncementRepository.fetchDisplayableAnnouncement` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | locale: Locale? | RemoteAnnouncementDisplay? |  | 96 |
| `RemoteAnnouncementRepository.fetchPointer` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` |  | AnnouncementPointer |  | 110 |
| `RemoteAnnouncementRepository.fetchPayload` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | latestFile: String | RemoteAnnouncementPayload |  | 115 |
| `RemoteAnnouncementRepository.fetchText` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | url: String | String |  | 121 |
| `RemoteAnnouncementRepository.toDisplay` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | payload: RemoteAnnouncementPayload<br>locale: Locale | RemoteAnnouncementDisplay? |  | 136 |
| `RemoteAnnouncementRepository.isVersionInRange` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | target: AnnouncementTarget | Boolean |  | 157 |
| `RemoteAnnouncementRepository.isChannelMatched` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | channels: List<String> | Boolean |  | 164 |
| `RemoteAnnouncementRepository.currentChannelAliases` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` |  | Set<String> |  | 170 |
| `RemoteAnnouncementRepository.isLocaleMatched` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | targetLocale: String<br>locale: Locale | Boolean |  | 185 |
| `RemoteAnnouncementRepository.isWithinSchedule` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | schedule: AnnouncementSchedule | Boolean |  | 194 |
| `RemoteAnnouncementRepository.pickLocalizedContent` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | content: AnnouncementContent<br>locale: Locale | AnnouncementLocaleContent? |  | 204 |
| `RemoteAnnouncementRepository.parseInstant` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | value: String? | Instant? |  | 218 |
| `RemoteAnnouncementRepository.resolveAnnouncementUrl` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | latestFile: String | String |  | 226 |
| `RemoteAnnouncementRepository.addCacheBust` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` | url: String | String |  | 248 |
| `RemoteAnnouncementRepository.normalizeLocaleKey` | `RemoteAnnouncementRepository` | `com.ai.assistance.operit.data.announcement` | `RemoteAnnouncementRepository.kt` |  | String |  | 253 |
| `AnnualReportCollector.collect` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | year: Int | UserReport |  | 50 |
| `AnnualReportCollector.collectPersonalMarket` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` |  | PersonalMarket | 登录 GitHub 的用户在插件市场的作品。需要联网，只在页面请求时调用。 | 79 |
| `AnnualReportCollector.windowOf` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | year: Int | Window |  | 97 |
| `AnnualReportCollector.iso` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | time: ZonedDateTime | String |  | 108 |
| `AnnualReportCollector.isoOf` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | epochMs: Long<br>zone: ZoneId | String |  | 111 |
| `AnnualReportCollector.installTime` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | zone: ZoneId | ZonedDateTime |  | 113 |
| `AnnualReportCollector.githubIdentity` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` |  | GitHubIdentity? |  | 119 |
| `AnnualReportCollector.tokenSummary` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | window: Window | TokenStatsAnnualSummary | 与 Token 统计页使用同一份货币与汇率设置。 | 125 |
| `AnnualReportCollector.tokens` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | window: Window<br>summary: TokenStatsAnnualSummary | UserTokens |  | 140 |
| `AnnualReportCollector.messages` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | window: Window | UserMessages |  | 163 |
| `AnnualReportCollector.activity` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | window: Window<br>tokenDays: Map<LocalDate, Long> | UserActivity |  | 175 |
| `AnnualReportCollector.hours` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | window: Window | UserHours |  | 189 |
| `AnnualReportCollector.firstMessage` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | window: Window | FirstMessage? |  | 198 |
| `AnnualReportCollector.aiWork` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | window: Window | UserAiWork |  | 206 |
| `AnnualReportCollector.tools` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | window: Window | UserTools | 统计采用的回复和重新生成的版本里所有工具标签；正文逐条分段读取，只在内存里保留计数。 | 218 |
| `AnnualReportCollector.creations` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | window: Window | UserCreations |  | 244 |
| `AnnualReportCollector.longestStreak` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | sortedDates: List<LocalDate> | StreakRange? | 连续有用户消息的最长天数；一天都没有时为 null。 | 266 |
| `AnnualReportCollector.cleanUserText` | `AnnualReportCollector` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportCollector.kt` | raw: String | String |  | 300 |
| `AnnualReportDao.countChatsCreated` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | Long |  | 57 |
| `AnnualReportDao.countMessagesBySender` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | List<SenderCountRow> |  | 67 |
| `AnnualReportDao.countUserMessagesByDay` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | List<DayCountRow> |  | 79 |
| `AnnualReportDao.countUserMessagesByHour` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | List<HourCountRow> |  | 90 |
| `AnnualReportDao.findLatestNightMessage` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | Long? |  | 103 |
| `AnnualReportDao.findFirstUserMessage` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | FirstMessageRow? |  | 116 |
| `AnnualReportDao.findLongestChat` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | ChatHighlightRow? |  | 129 |
| `AnnualReportDao.findTopCharacter` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | CharacterHighlightRow? |  | 144 |
| `AnnualReportDao.countVariants` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | Long | messages 表保存原始回复，重新生成的版本单独存在 message_variants，所以变体行数就是重新生成次数。 | 148 |
| `AnnualReportDao.countFavorites` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | Long |  | 151 |
| `AnnualReportDao.aiWorkInMessages` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | AiWorkRow |  | 162 |
| `AnnualReportDao.aiWorkInVariants` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | AiWorkRow |  | 173 |
| `AnnualReportDao.findToolMessages` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | List<MessageLocatorRow> |  | 184 |
| `AnnualReportDao.findToolVariantMessages` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | List<MessageLocatorRow> |  | 194 |
| `AnnualReportDao.earliestTokenRecord` | `AnnualReportDao` | `com.ai.assistance.operit.data.annualreport` | `AnnualReportDao.kt` | startMs: Long<br>endMs: Long | Long? |  | 197 |
| `CodexAuthManager.saveLoginTokens` | `CodexAuthManager` | `com.ai.assistance.operit.data.api` | `CodexAuthManager.kt` | tokens: CodexOAuthTokenResponse | CodexAuthState |  | 32 |
| `CodexAuthManager.getValidAccessToken` | `CodexAuthManager` | `com.ai.assistance.operit.data.api` | `CodexAuthManager.kt` |  | String |  | 57 |
| `CodexAuthManager.refreshAccessToken` | `CodexAuthManager` | `com.ai.assistance.operit.data.api` | `CodexAuthManager.kt` | current: CodexAuthState | CodexAuthState |  | 75 |
| `CodexAuthManager.logout` | `CodexAuthManager` | `com.ai.assistance.operit.data.api` | `CodexAuthManager.kt` |  | Unit |  | 98 |
| `CodexAuthManager.currentAccountId` | `CodexAuthManager` | `com.ai.assistance.operit.data.api` | `CodexAuthManager.kt` |  | String? |  | 111 |
| `CodexAuthManager.currentResidency` | `CodexAuthManager` | `com.ai.assistance.operit.data.api` | `CodexAuthManager.kt` |  | String? |  | 113 |
| `CodexAuthManager.fetchUsage` | `CodexAuthManager` | `com.ai.assistance.operit.data.api` | `CodexAuthManager.kt` |  | Result<CodexUsageSnapshot> |  | 115 |
| `CodexAuthManager.getInstance` | `CodexAuthManager` | `com.ai.assistance.operit.data.api` | `CodexAuthManager.kt` | context: Context | CodexAuthManager |  | 142 |
| `CodexOAuthTokenResponse.requireComplete` | `CodexOAuthTokenResponse` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` |  | CodexOAuthTokenResponse |  | 36 |
| `CodexOAuthProtocol.generatePkce` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | random: SecureRandom? | CodexPkceCodes |  | 54 |
| `CodexOAuthProtocol.generateState` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | random: SecureRandom? | String |  | 64 |
| `CodexOAuthProtocol.buildAuthorizationUrl` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | redirectUri: String<br>pkce: CodexPkceCodes<br>state: String | String |  | 70 |
| `CodexOAuthProtocol.parseJwtClaims` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | token: String | CodexJwtClaims? |  | 93 |
| `CodexOAuthProtocol.firstOrganizationId` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | organizations: JSONArray? | String |  | 136 |
| `CodexOAuthProtocol.firstNonBlank` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | values: String | String? |  | 140 |
| `CodexOAuthProtocol.encodeBase64Url` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | bytes: ByteArray | String |  | 144 |
| `CodexOAuthClient.exchangeAuthorizationCode` | `CodexOAuthClient` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | code: String<br>redirectUri: String<br>verifier: String | CodexOAuthTokenResponse |  | 156 |
| `CodexOAuthClient.refreshAccessToken` | `CodexOAuthClient` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | refreshToken: String | CodexOAuthTokenResponse |  | 177 |
| `CodexOAuthClient.revokeToken` | `CodexOAuthClient` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | token: String<br>tokenTypeHint: String | Unit |  | 192 |
| `CodexOAuthClient.executeTokenRequest` | `CodexOAuthClient` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | request: Request | CodexOAuthTokenResponse |  | 207 |
| `CodexOAuthClient.executeRequest` | `CodexOAuthClient` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | request: Request | String |  | 218 |
| `CodexOAuthClient.endpoint` | `CodexOAuthClient` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | path: String | String |  | 231 |
| `CodexOAuthClient.oauthErrorMessage` | `CodexOAuthClient` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | body: String | String |  | 233 |
| `CodexUsageClient.fetch` | `CodexUsageClient` | `com.ai.assistance.operit.data.api` | `CodexUsageClient.kt` | accessToken: String<br>accountId: String<br>residency: String? | Result<CodexUsageSnapshot> |  | 33 |
| `CodexUsageClient.parseUsage` | `CodexUsageClient` | `com.ai.assistance.operit.data.api` | `CodexUsageClient.kt` | responseBody: String | CodexUsageSnapshot |  | 70 |
| `CodexUsageClient.parseWindow` | `CodexUsageClient` | `com.ai.assistance.operit.data.api` | `CodexUsageClient.kt` | window: JSONObject? | CodexUsageWindow? |  | 88 |
| `GitHubApiService.getCurrentUser` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` |  | Result<GitHubUser> | 获取当前用户信息 | 160 |
| `GitHubApiService.getUser` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | username: String | Result<GitHubUser> | 根据用户名获取GitHub用户信息 | 191 |
| `GitHubApiService.searchRepositories` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | query: String<br>sort: String?<br>order: String?<br>page: Int?<br>perPage: Int? | Result<List<GitHubRepository>> | 搜索仓库 | 222 |
| `GitHubApiService.getUserRepositories` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | username: String??<br>type: String?<br>sort: String?<br>page: Int?<br>perPage: Int? | Result<List<GitHubRepository>> | 获取用户仓库 | 275 |
| `GitHubApiService.getRepository` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String | Result<GitHubRepository> | 获取仓库信息 | 338 |
| `GitHubApiService.getRepositoryReleases` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>page: Int?<br>perPage: Int? | Result<List<GitHubRelease>> | 获取仓库的Releases | 372 |
| `GitHubApiService.createRepository` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | name: String<br>description: String??<br>homepage: String??<br>isPrivate: Boolean?<br>autoInit: Boolean? | Result<GitHubRepository> |  | 416 |
| `GitHubApiService.createTextFile` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>path: String<br>message: String<br>textContent: String<br>branch: String?? | Result<Unit> |  | 462 |
| `GitHubApiService.getRepositoryContentFile` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>path: String | Result<GitHubRepositoryContentFile?> |  | 518 |
| `GitHubApiService.getReleaseByTag` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>tag: String | Result<GitHubRelease> |  | 553 |
| `GitHubApiService.findReleaseByTag` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>tag: String | Result<GitHubRelease?> |  | 581 |
| `GitHubApiService.createRelease` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>tagName: String<br>name: String??<br>body: String??<br>draft: Boolean?<br>prerelease: Boolean? | Result<GitHubRelease> |  | 598 |
| `GitHubApiService.updateRelease` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>releaseId: Long<br>tagName: String??<br>name: String??<br>body: String??<br>draft: Boolean??<br>prerelease: Boolean?? | Result<GitHubRelease> |  | 646 |
| `GitHubApiService.downloadReleaseAsset` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | downloadUrl: String | Result<ByteArray> |  | 695 |
| `GitHubApiService.deleteRelease` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>releaseId: Long | Result<Unit> |  | 715 |
| `GitHubApiService.deleteReleaseAsset` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>assetId: Long | Result<Unit> |  | 745 |
| `GitHubApiService.uploadReleaseAsset` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | owner: String<br>repo: String<br>releaseId: Long<br>assetName: String<br>contentType: String<br>content: ByteArray | Result<GitHubReleaseAsset> |  | 775 |
| `GitHubApiService.buildHttpException` | `GitHubApiService` | `com.ai.assistance.operit.data.api` | `GitHubApiService.kt` | code: Int<br>message: String<br>responseBody: String? | Exception |  | 821 |
| `GitHubOAuthBrokerService.startLogin` | `GitHubOAuthBrokerService` | `com.ai.assistance.operit.data.api` | `GitHubOAuthBrokerService.kt` | completionRedirectUri: String | Result<GitHubOAuthBrokerStartResponse> |  | 60 |
| `GitHubOAuthBrokerService.claimLogin` | `GitHubOAuthBrokerService` | `com.ai.assistance.operit.data.api` | `GitHubOAuthBrokerService.kt` | transactionId: String<br>deliveryCredential: String | Result<GitHubOAuthBrokerClaimResult> |  | 84 |
| `GitHubOAuthBrokerService.httpErrorMessage` | `GitHubOAuthBrokerService` | `com.ai.assistance.operit.data.api` | `GitHubOAuthBrokerService.kt` | code: Int<br>message: String<br>body: String? | String |  | 130 |
| `GitHubOAuthBrokerService.requireValue` | `GitHubOAuthBrokerService` | `com.ai.assistance.operit.data.api` | `GitHubOAuthBrokerService.kt` | value: T?<br>name: String | T |  | 138 |
| `MarketStatsApiService.getManifest` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | Result<MarketV2ManifestResponse> |  | 521 |
| `MarketStatsApiService.getStats` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | type: String | Result<MarketTypeStatsResponse> |  | 533 |
| `MarketStatsApiService.getRankPage` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | type: String<br>metric: String<br>page: Int | Result<MarketRankPageResponse> |  | 558 |
| `MarketStatsApiService.getAllRankPage` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | metric: String<br>page: Int | Result<MarketRankPageResponse> |  | 586 |
| `MarketStatsApiService.getTypeRankPage` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | type: String<br>metric: String<br>page: Int | Result<MarketRankPageResponse> |  | 597 |
| `MarketStatsApiService.getCategoryRankPage` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | categoryId: String<br>metric: String<br>page: Int | Result<MarketRankPageResponse> |  | 609 |
| `MarketStatsApiService.getTypedCategoryRankPage` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | type: String<br>categoryId: String<br>metric: String<br>page: Int | Result<MarketRankPageResponse> |  | 621 |
| `MarketStatsApiService.getArtifactRankPage` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | type: String<br>metric: String<br>page: Int | Result<ArtifactProjectRankPageResponse> |  | 634 |
| `MarketStatsApiService.getListRankPage` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | pathSegments: List<String><br>label: String<br>type: String<br>metric: String | Result<MarketRankPageResponse> |  | 665 |
| `MarketStatsApiService.getArtifactProject` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | projectId: String | Result<ArtifactProjectDetailResponse> |  | 693 |
| `MarketStatsApiService.artifactProjectFromEntry` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entry: MarketV2Entry | ArtifactProjectDetailResponse |  | 704 |
| `MarketStatsApiService.trackDownload` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | assetId: String | Result<Unit> |  | 757 |
| `MarketStatsApiService.downloadUrlForAsset` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | assetId: String | String |  | 773 |
| `MarketStatsApiService.getEntry` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String | Result<MarketV2Entry?> |  | 781 |
| `MarketStatsApiService.getComments` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String<br>page: Int? | Result<List<MarketV2Comment>> |  | 794 |
| `MarketStatsApiService.postComment` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String<br>body: String<br>parentId: String?? | Result<MarketV2Comment> |  | 807 |
| `MarketStatsApiService.addReaction` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String | Result<MarketV2Reaction> |  | 824 |
| `MarketStatsApiService.getUserPublishedEntries` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | type: String?? | Result<List<MarketV2PublisherEntrySummary>> |  | 837 |
| `MarketStatsApiService.getMyEntryDetail` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String | Result<MarketV2Entry> | Loads the authenticated publisher's full entry data, including an unpublished latest vers… | 859 |
| `MarketStatsApiService.findPublisherEntries` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | authorId: String | Result<List<MarketV2PublisherEntrySummary>> | 年度报告用：查询某个作者在市场发布过的条目。 发布者分片只收录发布过条目的作者，分片文件或分片里没有这个作者，都表示他还没有发布过任何条目， 这是数据本身的含义，所以返回空列表；… | 879 |
| `MarketStatsApiService.getPublisherEntries` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | authorId: String | Result<List<MarketV2PublisherEntrySummary>> |  | 896 |
| `MarketStatsApiService.getNotifications` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | limit: Int?<br>offset: Int? | Result<List<MarketV2Notification>> |  | 910 |
| `MarketStatsApiService.editComment` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | commentId: String<br>body: String | Result<Unit> |  | 924 |
| `MarketStatsApiService.deleteComment` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | commentId: String | Result<Unit> |  | 938 |
| `MarketStatsApiService.publish` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | request: MarketV2PublishRequest | Result<MarketV2Entry> |  | 949 |
| `MarketStatsApiService.updateEntry` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String<br>request: MarketV2EntryUpdateRequest | Result<MarketV2Entry> |  | 985 |
| `MarketStatsApiService.publishNewVersion` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String<br>request: MarketV2PublishRequest<br>entryPatch: MarketV2NewVersionEntryPatch?? | Result<MarketV2NewVersionResponse> |  | 1003 |
| `MarketStatsApiService.withdrawEntry` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String | Result<MarketV2Entry> |  | 1030 |
| `MarketStatsApiService.requestStaticJson` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | pathSegments: List<String><br>label: String<br>notFoundValue: T??<br>decode: (String) -> T | T |  | 1044 |
| `MarketStatsApiService.requestDynamic` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | method: String<br>pathSegments: List<String><br>label: String<br>body: String??<br>queryParameters: Map<String, String>?<br>includeMarketSession: Boolean?<br>followRedirects: Boolean?<br>decode: (String, Response) -> T | T |  | 1079 |
| `MarketStatsApiService.ensureMarketSession` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | String |  | 1128 |
| `MarketStatsApiService.requestMarketSession` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | githubToken: String | String |  | 1148 |
| `MarketStatsApiService.buildHttpErrorMessage` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | response: Response<br>body: String | String |  | 1174 |
| `MarketStatsApiService.resolveResponseSource` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | response: Response | String |  | 1190 |
| `MarketStatsApiService.toV2Sort` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | String |  | 1198 |
| `MarketStatsApiService.allListPathSegments` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | sort: String<br>page: Int | List<String> |  | 1206 |
| `MarketStatsApiService.typeListPathSegments` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | type: String<br>sort: String<br>page: Int | List<String> |  | 1210 |
| `MarketStatsApiService.categoryListPathSegments` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | categoryId: String<br>sort: String<br>page: Int | List<String> |  | 1214 |
| `MarketStatsApiService.typedCategoryListPathSegments` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | type: String<br>categoryId: String<br>sort: String<br>page: Int | List<String> |  | 1218 |
| `MarketStatsApiService.toRankEntry` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | MarketRankEntryResponse |  | 1227 |
| `MarketStatsApiService.toArtifactProjectRankEntry` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | ArtifactProjectRankEntryResponse |  | 1250 |
| `MarketStatsApiService.toPendingEntry` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String | MarketV2Entry |  | 1284 |
| `MarketStatsApiService.toPendingEntry` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | entryId: String | MarketV2Entry |  | 1298 |
| `MarketStatsApiService.publisherUser` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | GitHubUser |  | 1310 |
| `MarketStatsApiService.toPublisherUser` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | GitHubUser |  | 1320 |
| `MarketStatsApiService.publisherLogin` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | String |  | 1327 |
| `MarketStatsApiService.publisherAvatarUrl` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | String |  | 1333 |
| `MarketStatsApiService.downloadCountValue` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | Int |  | 1337 |
| `MarketStatsApiService.likesCount` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | Int |  | 1341 |
| `MarketStatsApiService.toPublicationState` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | String |  | 1348 |
| `MarketStatsApiService.marketShard` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` |  | String |  | 1352 |
| `MarketStatsApiService.stableLongId` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | value: String | Long |  | 1356 |
| `MarketStatsApiService.sha256Hex` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | bytes: ByteArray | String |  | 1365 |
| `MarketStatsApiService.fnv1a32Hex` | `MarketStatsApiService` | `com.ai.assistance.operit.data.api` | `MarketStatsApiService.kt` | value: String | String |  | 1369 |
| `OperitBackupDirs.operitRootDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` |  | File |  | 8 |
| `OperitBackupDirs.backupRootDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` |  | File |  | 12 |
| `OperitBackupDirs.rawSnapshotDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` |  | File |  | 16 |
| `OperitBackupDirs.roomDbDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` |  | File |  | 20 |
| `OperitBackupDirs.preferencesDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` |  | File |  | 24 |
| `OperitBackupDirs.chatDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` |  | File |  | 28 |
| `OperitBackupDirs.memoryDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` |  | File |  | 32 |
| `OperitBackupDirs.modelConfigDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` |  | File |  | 36 |
| `OperitBackupDirs.characterCardsDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` |  | File |  | 40 |
| `OperitBackupDirs.ensureDir` | `OperitBackupDirs` | `com.ai.assistance.operit.data.backup` | `OperitBackupDirs.kt` | dir: File | File |  | 44 |
| `isSupportedSnapshotPackageName` | — | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | packageName: String | Boolean |  | 34 |
| `RawSnapshotBackupManager.exportToBackupDir` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | context: Context<br>options: SnapshotOptions?<br>onProgress: ((ExportProgressInfo) -> Unit)?? | File |  | 105 |
| `RawSnapshotBackupManager.restoreFromBackupUri` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | context: Context<br>uri: Uri<br>onProgress: ((RestoreProgress) -> Unit)?? | Unit |  | 263 |
| `RawSnapshotBackupManager.extractZipToWorkDir` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | zipFile: File<br>workDir: File | Manifest |  | 348 |
| `RawSnapshotBackupManager.addDirToZip` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | zos: ZipOutputStream<br>dir: File<br>entryPrefix: String<br>excludedTopLevelDirNames: Set<String>?<br>totalFiles: Int?<br>onPercentChanged: ((Int) -> Unit)?? | Unit |  | 419 |
| `RawSnapshotBackupManager.shouldPruneDirForZip` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | currentDir: File<br>baseDir: File<br>entryPrefix: String<br>excludedTopLevelDirNames: Set<String> | Boolean |  | 478 |
| `RawSnapshotBackupManager.shouldSkipForZip` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | canonical: File<br>baseCanonical: File<br>entryPrefix: String<br>excludedTopLevelDirNames: Set<String> | Boolean |  | 498 |
| `totalFilesForZip` | — | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | dir: File<br>entryPrefix: String<br>excludedTopLevelDirNames: Set<String><br>onScannedCountChanged: ((Int) -> Unit)?? | Int |  | 543 |
| `replaceDirContents` | — | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | fromDir: File<br>toDir: File<br>preservedTopLevelDirNames: Set<String>? | Unit |  | 575 |
| `copyDir` | — | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | fromDir: File<br>toDir: File<br>preservedTopLevelDirNames: Set<String> | Unit |  | 598 |
| `readBytesSafely` | — | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | maxBytes: Int | ByteArray |  | 642 |
| `RoomDatabaseBackupManager.pruneExcessBackups` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | context: Context | Unit |  | 33 |
| `RoomDatabaseBackupManager.backupIfNeeded` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | context: Context<br>force: Boolean | BackupResult |  | 41 |
| `RoomDatabaseBackupManager.createOrReplaceAutoBackup` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | context: Context<br>day: String | File |  | 69 |
| `RoomDatabaseBackupManager.createManualBackup` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | context: Context | File |  | 111 |
| `RoomDatabaseBackupManager.enforceMaxBackupCount` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | context: Context<br>keepLatest: Int | Unit |  | 155 |
| `RoomDatabaseBackupManager.isRoomDatabaseBackupFileName` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | name: String | Boolean |  | 183 |
| `RoomDatabaseBackupManager.writeZip` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | outputFile: File<br>entries: Map<String, File> | Unit |  | 188 |
| `RoomDatabaseBackupManager.parseBackupDay` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | fileName: String | LocalDate |  | 207 |
| `RoomDatabaseBackupPreferences.getInstance` | `RoomDatabaseBackupPreferences` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupPreferences.kt` | context: Context | RoomDatabaseBackupPreferences |  | 24 |
| `RoomDatabaseBackupPreferences.isDailyBackupEnabled` | `RoomDatabaseBackupPreferences` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupPreferences.kt` |  | Boolean |  | 57 |
| `RoomDatabaseBackupPreferences.setDailyBackupEnabled` | `RoomDatabaseBackupPreferences` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupPreferences.kt` | enabled: Boolean | Unit |  | 59 |
| `RoomDatabaseBackupPreferences.markSuccess` | `RoomDatabaseBackupPreferences` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupPreferences.kt` | day: String<br>timestamp: Long | Unit |  | 63 |
| `RoomDatabaseBackupPreferences.markFailure` | `RoomDatabaseBackupPreferences` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupPreferences.kt` | error: String | Unit |  | 71 |
| `RoomDatabaseBackupPreferences.getMaxBackupCount` | `RoomDatabaseBackupPreferences` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupPreferences.kt` |  | Int |  | 75 |
| `RoomDatabaseBackupPreferences.setMaxBackupCount` | `RoomDatabaseBackupPreferences` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupPreferences.kt` | count: Int | Unit |  | 77 |
| `RoomDatabaseBackupScheduler.ensureScheduled` | `RoomDatabaseBackupScheduler` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupScheduler.kt` | context: Context | Unit |  | 20 |
| `RoomDatabaseBackupScheduler.cancelScheduled` | `RoomDatabaseBackupScheduler` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupScheduler.kt` | context: Context | Unit |  | 40 |
| `RoomDatabaseBackupScheduler.enqueueManualBackup` | `RoomDatabaseBackupScheduler` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupScheduler.kt` | context: Context<br>force: Boolean | Unit |  | 45 |
| `RoomDatabaseBackupScheduler.calculateInitialDelayToHour` | `RoomDatabaseBackupScheduler` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupScheduler.kt` | targetHour: Int | Long |  | 63 |
| `RoomDatabaseBackupWorker.doWork` | `RoomDatabaseBackupWorker` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupWorker.kt` |  | Result |  | 18 |
| `RoomDatabaseRestoreManager.listRecentAutoBackups` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | context: Context<br>limit: Int? | List<File> |  | 29 |
| `RoomDatabaseRestoreManager.listRecentBackups` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | context: Context<br>limit: Int? | List<File> |  | 45 |
| `RoomDatabaseRestoreManager.isRoomDatabaseBackupFile` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | name: String | Boolean |  | 63 |
| `RoomDatabaseRestoreManager.restoreFromBackupUri` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | context: Context<br>uri: Uri | Unit |  | 68 |
| `RoomDatabaseRestoreManager.restoreFromBackupFile` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | context: Context<br>zipFile: File | Unit |  | 87 |
| `RoomDatabaseRestoreManager.restoreFromBackupFileInternal` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | context: Context<br>zipFile: File | Unit |  | 95 |
| `RoomDatabaseRestoreManager.writeStreamToFile` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | input: ZipInputStream<br>target: File | Unit |  | 176 |
| `RoomDatabaseRestoreManager.atomicallyReplace` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | from: File<br>to: File | Unit |  | 187 |
| `ApiProviderConfigs.get` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | providerType: ApiProviderType | ProviderApiConfig |  | 301 |
| `ApiProviderConfigs.getDefaultModelName` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | providerType: ApiProviderType | String |  | 305 |
| `ApiProviderConfigs.getDefaultApiEndpoint` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | providerType: ApiProviderType | String |  | 309 |
| `ApiProviderConfigs.getEndpointOptions` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | providerType: ApiProviderType | List<ProviderEndpointOption>? |  | 313 |
| `ApiProviderConfigs.requiresApiKey` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | providerType: ApiProviderType<br>apiEndpoint: String? | Boolean |  | 317 |
| `ApiProviderConfigs.requiresApiKey` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | providerTypeId: String<br>apiEndpoint: String? | Boolean |  | 325 |
| `ApiProviderConfigs.isDefaultModelName` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | modelName: String | Boolean |  | 330 |
| `ApiProviderConfigs.isDefaultApiEndpoint` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | endpoint: String | Boolean |  | 334 |
| `ApiProviderConfigs.isLoopbackEndpoint` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | apiEndpoint: String | Boolean |  | 338 |
| `ApiProviderConfigs.isLoopbackHost` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | host: String | Boolean |  | 356 |
| `isLoopbackEndpointText` | — | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | apiEndpoint: String | Boolean |  | 367 |
| `DefaultModelPricingCollect.defaultPricePerRequest` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | currency: PricingCurrency | Double |  | 42 |
| `DefaultModelPricingCollect.zeroPricing` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | currency: PricingCurrency | ModelPricingDefaults |  | 49 |
| `DefaultModelPricingCollect.tokenPricing` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | inputPricePerMillion: Double<br>outputPricePerMillion: Double<br>cachedInputPricePerMillion: Double?<br>currency: PricingCurrency<br>pricePerRequest: Double? | ModelPricingDefaults |  | 60 |
| `DefaultModelPricingCollect.countPricing` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | pricePerRequest: Double<br>currency: PricingCurrency | ModelPricingDefaults |  | 77 |
| `DefaultModelPricingCollect.splitProviderModel` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | providerModel: String | Pair<String, String> |  | 193 |
| `DefaultModelPricingCollect.isDomesticProvider` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | provider: String | Boolean |  | 203 |
| `DefaultModelPricingCollect.getDefaultPricing` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | providerModel: String | ModelPricingDefaults |  | 207 |
| `DefaultModelPricingCollect.getCurrency` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | providerModel: String | PricingCurrency |  | 238 |
| `ModelThinkingConfigDefaults.forProvider` | `ModelThinkingConfigDefaults` | `com.ai.assistance.operit.data.collects` | `ModelThinkingConfigDefaultsCollect.kt` | providerTypeId: String | String |  | 400 |
| `ChatBoxConverter.convert` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | content: String | List<ChatHistory> |  | 44 |
| `ChatBoxConverter.getSupportedFormat` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` |  | ChatFormat |  | 58 |
| `ChatBoxConverter.parseObjectFormat` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | obj: JsonObject | List<ChatHistory> | 解析对象格式 | 63 |
| `ChatBoxConverter.parseSession` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | sessionObj: JsonObject<br>fallbackId: String??<br>fallbackTitle: String?? | ChatHistory? | 解析单个 session | 80 |
| `ChatBoxConverter.parseMessage` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | msgObj: JsonObject<br>baseTimestamp: Long<br>index: Int<br>fallbackModelName: String? | ChatMessage? | 解析单条消息 | 150 |
| `ChatBoxConverter.parseRootElement` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | content: String | JsonElement |  | 190 |
| `ChatBoxConverter.normalizeInput` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | content: String | String |  | 206 |
| `ChatBoxConverter.extractJsonIfStringWrapper` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | element: JsonElement | JsonElement |  | 212 |
| `ChatBoxConverter.repairEscapedJson` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | content: String | String |  | 220 |
| `ChatBoxConverter.isKvExportFormat` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | obj: JsonObject | Boolean |  | 233 |
| `ChatBoxConverter.parseKvExportFormat` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | obj: JsonObject | List<ChatHistory> |  | 238 |
| `ChatBoxConverter.buildMessageContent` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | msgObj: JsonObject | String? |  | 258 |
| `ChatBoxConverter.extractMessageText` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | msgObj: JsonObject | String? |  | 279 |
| `ChatBoxConverter.extractErrorText` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | msgObj: JsonObject | String? |  | 294 |
| `ChatBoxConverter.normalizeTimestamp` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | raw: Long | Long |  | 308 |
| `ChatBoxConverter.normalizeRole` | `ChatBoxConverter` | `com.ai.assistance.operit.data.converter` | `ChatBoxConverter.kt` | role: String | String | 规范化角色名称 | 319 |
| `ChatFormatConverter.convert` | `ChatFormatConverter` | `com.ai.assistance.operit.data.converter` | `ChatFormatConverter.kt` | content: String | List<ChatHistory> | 将字符串内容转换为 ChatHistory 列表 | 15 |
| `ChatFormatConverter.getSupportedFormat` | `ChatFormatConverter` | `com.ai.assistance.operit.data.converter` | `ChatFormatConverter.kt` |  | ChatFormat | 获取转换器支持的格式 | 20 |
| `ChatFormatDetector.detectFormat` | `ChatFormatDetector` | `com.ai.assistance.operit.data.converter` | `ChatFormatDetector.kt` | content: String | ChatFormat | 检测文件内容的格式 | 16 |
| `ChatFormatDetector.detectJsonFormat` | `ChatFormatDetector` | `com.ai.assistance.operit.data.converter` | `ChatFormatDetector.kt` | content: String | ChatFormat | 检测 JSON 的具体格式 | 45 |
| `ChatFormatDetector.detectJsonObjectFormat` | `ChatFormatDetector` | `com.ai.assistance.operit.data.converter` | `ChatFormatDetector.kt` | obj: JsonObject | ChatFormat | 检测 JSON 对象的具体格式 | 78 |
| `ChatFormatDetector.isMarkdownFormat` | `ChatFormatDetector` | `com.ai.assistance.operit.data.converter` | `ChatFormatDetector.kt` | content: String | Boolean | 检测是否为 Markdown 格式 | 120 |
| `ChatFormatDetector.isCsvFormat` | `ChatFormatDetector` | `com.ai.assistance.operit.data.converter` | `ChatFormatDetector.kt` | content: String | Boolean | 检测是否为 CSV 格式 | 151 |
| `ChatFormatDetector.detectFormatByExtension` | `ChatFormatDetector` | `com.ai.assistance.operit.data.converter` | `ChatFormatDetector.kt` | fileName: String | ChatFormat? | 根据文件扩展名推测格式 | 171 |
| `ChatGPTConverter.convert` | `ChatGPTConverter` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | content: String | List<ChatHistory> |  | 23 |
| `ChatGPTConverter.getSupportedFormat` | `ChatGPTConverter` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` |  | ChatFormat |  | 32 |
| `ChatGPTConverter.convertConversation` | `ChatGPTConverter` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | conv: ChatGPTConversation | ChatHistory? |  | 34 |
| `ChatGPTConverter.extractMessagesFromMapping` | `ChatGPTConverter` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | mapping: Map<String, ChatGPTNode><br>currentNodeId: String? | List<ChatMessage> | 从 ChatGPT 的 mapping 结构中提取消息链 | 76 |
| `ChatGPTConverter.shouldIncludeMessage` | `ChatGPTConverter` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | message: ChatGPTMessage | Boolean | 判断是否应该包含该消息 | 109 |
| `ChatGPTConverter.convertMessage` | `ChatGPTConverter` | `com.ai.assistance.operit.data.converter` | `ChatGPTConverter.kt` | message: ChatGPTMessage | ChatMessage? | 转换单条消息 | 132 |
| `ChatHistoryCsv.writeHeader` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | writer: Writer | Unit |  | 75 |
| `ChatHistoryCsv.writeChat` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | writer: Writer<br>history: OperitArchivedChat | Unit |  | 79 |
| `ChatHistoryCsv.writeMessage` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | writer: Writer<br>chatId: String<br>orderIndex: Int<br>message: ChatMessage | Unit |  | 102 |
| `ChatHistoryCsv.writeVariant` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | writer: Writer<br>chatId: String<br>messageTimestamp: Long<br>variant: OperitArchivedMessageVariant | Unit |  | 133 |
| `ChatHistoryCsv.writeRow` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | writer: Writer<br>values: List<String?> | Unit |  | 159 |
| `ChatHistoryCsv.emptyRow` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` |  | MutableList<String?> |  | 169 |
| `ChatHistoryCsv.put` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | row: MutableList<String?><br>name: String<br>value: String? | Unit |  | 171 |
| `ChatHistoryCsv.writeField` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | writer: Writer<br>value: String | Unit |  | 175 |
| `GenericJsonConverter.convert` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` | content: String | List<ChatHistory> |  | 23 |
| `GenericJsonConverter.getSupportedFormat` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` |  | ChatFormat |  | 37 |
| `GenericJsonConverter.parseArrayFormat` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` | array: JsonArray | List<ChatHistory> | 解析数组格式 可能是对话数组或消息数组 | 43 |
| `GenericJsonConverter.parseObjectFormat` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` | obj: JsonObject | List<ChatHistory> | 解析对象格式 | 86 |
| `GenericJsonConverter.isConversationObject` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` | obj: JsonObject | Boolean | 判断是否为对话对象 | 103 |
| `GenericJsonConverter.isMessageObject` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` | obj: JsonObject | Boolean | 判断是否为消息对象 | 112 |
| `GenericJsonConverter.parseConversationObject` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` | obj: JsonObject | ChatHistory? | 解析对话对象 | 119 |
| `GenericJsonConverter.parseMessageObject` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` | obj: JsonObject<br>baseTimestamp: Long<br>index: Int | ChatMessage? | 解析消息对象 | 168 |
| `GenericJsonConverter.normalizeRole` | `GenericJsonConverter` | `com.ai.assistance.operit.data.converter` | `GenericJsonConverter.kt` | role: String | String | 规范化角色名称 | 201 |
| `MarkdownConverter.convert` | `MarkdownConverter` | `com.ai.assistance.operit.data.converter` | `MarkdownConverter.kt` | content: String | List<ChatHistory> |  | 26 |
| `MarkdownConverter.getSupportedFormat` | `MarkdownConverter` | `com.ai.assistance.operit.data.converter` | `MarkdownConverter.kt` |  | ChatFormat |  | 36 |
| `MarkdownConverter.splitConversations` | `MarkdownConverter` | `com.ai.assistance.operit.data.converter` | `MarkdownConverter.kt` | content: String | List<String> | 分割多个对话（如果存在） | 41 |
| `MarkdownConverter.parseConversation` | `MarkdownConverter` | `com.ai.assistance.operit.data.converter` | `MarkdownConverter.kt` | content: String | ChatHistory? | 解析单个对话 | 49 |
| `MarkdownConverter.parseSimpleProperties` | `MarkdownConverter` | `com.ai.assistance.operit.data.converter` | `MarkdownConverter.kt` | comment: String<br>prefix: String | Map<String, String> | 解析简单的属性字符串 格式: key=value, key2=value2, simpleFlag | 211 |
| `MarkdownConverter.parseRole` | `MarkdownConverter` | `com.ai.assistance.operit.data.converter` | `MarkdownConverter.kt` | roleText: String | String? | 解析角色标记 只支持明确的角色名称，避免误判 | 243 |
| `MarkdownConverter.createMessage` | `MarkdownConverter` | `com.ai.assistance.operit.data.converter` | `MarkdownConverter.kt` | role: String<br>content: String<br>timestamp: Long<br>model: String | ChatMessage | 创建消息对象 | 267 |
| `MarkdownConverter.parseDate` | `MarkdownConverter` | `com.ai.assistance.operit.data.converter` | `MarkdownConverter.kt` | dateStr: String | LocalDateTime? | 尝试解析日期字符串 | 280 |
| `ChatContentDao.queryMessagesForChat` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String | List<MessageContentRow> |  | 92 |
| `ChatContentDao.queryMessagesForChatFromTimestampAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>startTimestampInclusive: Long | List<MessageContentRow> |  | 98 |
| `ChatContentDao.queryMessagesForChatWindowAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>startTimestampInclusive: Long<br>endTimestampInclusive: Long | List<MessageContentRow> |  | 108 |
| `ChatContentDao.queryMessagesForChatAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>limit: Int | List<MessageContentRow> |  | 115 |
| `ChatContentDao.queryMessagesForChatDesc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>limit: Int | List<MessageContentRow> |  | 121 |
| `ChatContentDao.queryMessagesForChatAscRange` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>offset: Int<br>limit: Int | List<MessageContentRow> |  | 130 |
| `ChatContentDao.queryMessagesForChatDescRange` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>offset: Int<br>limit: Int | List<MessageContentRow> |  | 140 |
| `ChatContentDao.queryMessagesForChatAfterTimestampExclusiveAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>afterTimestampExclusive: Long<br>limit: Int | List<MessageContentRow> |  | 151 |
| `ChatContentDao.queryMessagesForChatInRangeAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>afterTimestampExclusive: Long?<br>beforeTimestampExclusive: Long?<br>upToTimestampInclusive: Long? | List<MessageContentRow> |  | 165 |
| `ChatContentDao.queryMessagesForChatBeforeTimestampDesc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>maxTimestamp: Long<br>limit: Int | List<MessageContentRow> |  | 177 |
| `ChatContentDao.queryMessagesForChatBeforeTimestampExclusiveDesc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>beforeTimestampExclusive: Long<br>limit: Int | List<MessageContentRow> |  | 188 |
| `ChatContentDao.queryMessageByTimestamp` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>timestamp: Long | MessageContentRow? |  | 198 |
| `ChatContentDao.queryMessageContentChunk` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | messageId: Long<br>startByte: Long<br>byteCount: Int | ByteArray? |  | 207 |
| `ChatContentDao.queryVariantsForChat` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String | List<MessageVariantContentRow> |  | 217 |
| `ChatContentDao.queryVariantsForMessageRange` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>minTimestamp: Long<br>maxTimestamp: Long | List<MessageVariantContentRow> |  | 226 |
| `ChatContentDao.queryVariantsForMessage` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>messageTimestamp: Long | List<MessageVariantContentRow> |  | 237 |
| `ChatContentDao.queryVariantForMessage` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>messageTimestamp: Long<br>variantIndex: Int | MessageVariantContentRow? |  | 247 |
| `ChatContentDao.queryMessageVariantContentChunk` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | variantId: Long<br>startByte: Long<br>byteCount: Int | ByteArray? |  | 257 |
| `ChatContentDao.getSelectedContentCharacterCountsByChat` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` |  | List<ChatContentCharacterCount> |  | 286 |
| `ChatContentDao.getMessagesForChat` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String | List<MessageEntity> |  | 289 |
| `ChatContentDao.getMessagesForChatFromTimestampAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>startTimestampInclusive: Long | List<MessageEntity> |  | 293 |
| `ChatContentDao.getMessagesForChatWindowAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>startTimestampInclusive: Long<br>endTimestampInclusive: Long | List<MessageEntity> |  | 300 |
| `ChatContentDao.getMessagesForChatAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>limit: Int | List<MessageEntity> |  | 310 |
| `ChatContentDao.getMessagesForChatDesc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>limit: Int | List<MessageEntity> |  | 314 |
| `ChatContentDao.getMessagesForChatAscRange` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>offset: Int<br>limit: Int | List<MessageEntity> |  | 318 |
| `ChatContentDao.getMessagesForChatDescRange` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>offset: Int<br>limit: Int | List<MessageEntity> |  | 325 |
| `ChatContentDao.getMessagesForChatAfterTimestampExclusiveAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>afterTimestampExclusive: Long<br>limit: Int | List<MessageEntity> |  | 332 |
| `ChatContentDao.getMessagesForChatInRangeAsc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>afterTimestampExclusive: Long?<br>beforeTimestampExclusive: Long?<br>upToTimestampInclusive: Long? | List<MessageEntity> |  | 342 |
| `ChatContentDao.getMessagesForChatBeforeTimestampDesc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>maxTimestamp: Long<br>limit: Int | List<MessageEntity> |  | 358 |
| `ChatContentDao.getMessagesForChatBeforeTimestampExclusiveDesc` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>beforeTimestampExclusive: Long<br>limit: Int | List<MessageEntity> |  | 366 |
| `ChatContentDao.getMessageByTimestamp` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>timestamp: Long | MessageEntity? |  | 376 |
| `ChatContentDao.getVariantsForChat` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String | List<MessageVariantEntity> |  | 380 |
| `ChatContentDao.getVariantsForMessages` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>messageTimestamps: List<Long> | List<MessageVariantEntity> |  | 384 |
| `ChatContentDao.getVariantsForMessage` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>messageTimestamp: Long | List<MessageVariantEntity> |  | 407 |
| `ChatContentDao.getVariantForMessage` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | chatId: String<br>messageTimestamp: Long<br>variantIndex: Int | MessageVariantEntity? |  | 414 |
| `ChatContentDao.materializeMessages` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | rows: List<MessageContentRow> | List<MessageEntity> |  | 423 |
| `ChatContentDao.materializeMessage` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | row: MessageContentRow | MessageEntity |  | 426 |
| `ChatContentDao.materializeVariants` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | rows: List<MessageVariantContentRow> | List<MessageVariantEntity> |  | 452 |
| `ChatContentDao.materializeVariant` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | row: MessageVariantContentRow | MessageVariantEntity |  | 456 |
| `ChatContentDao.readContentBytes` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | contentByteCount: Long<br>firstChunk: ByteArray<br>fetchChunk: suspend (startByte: Long, byteCount…<br>missingRowMessage: String<br>emptyChunkMessage: String<br>byteCountMismatchMessage: String | ByteArray |  | 482 |
| `ChatContentDao.decodeUtf8` | `ChatContentDao` | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | bytes: ByteArray | String |  | 518 |
| `ChatDao.getAllChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` |  | Flow<List<ChatEntity>> | 获取所有聊天，按显示顺序排列 | 18 |
| `ChatDao.getTotalChatCount` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` |  | Int | 获取聊天总数 | 22 |
| `ChatDao.getAllChatsDirectly` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` |  | List<ChatEntity> | 获取所有聊天（挂起函数版本） | 26 |
| `ChatDao.getChatById` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String | ChatEntity? | 根据ID获取单个聊天 | 30 |
| `ChatDao.updateChatMetadata` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>title: String<br>timestamp: Long<br>inputTokens: Long<br>outputTokens: Long<br>currentWindowSize: Long | Unit |  | 42 |
| `ChatDao.updateChatTitle` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>title: String<br>timestamp: Long? | Unit | 更新聊天标题 | 53 |
| `ChatDao.updateChatWorkspace` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>workspace: String?<br>workspaceEnv: String?<br>timestamp: Long? | Unit | 更新聊天工作区 | 57 |
| `ChatDao.updateChatTitleAndWorkspace` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>title: String<br>workspace: String?<br>workspaceEnv: String?<br>timestamp: Long? | Unit |  | 63 |
| `ChatDao.updateChatGroup` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>group: String?<br>timestamp: Long? | Unit | 更新聊天分组 | 73 |
| `ChatDao.updateChatCharacterCardName` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>characterCardName: String?<br>timestamp: Long? | Unit | 更新聊天绑定的角色卡名称 | 77 |
| `ChatDao.updateChatCharacterGroupId` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>characterGroupId: String?<br>timestamp: Long? | Unit | 更新聊天绑定的群组角色卡ID | 81 |
| `ChatDao.updateChatCharacterBinding` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>characterCardName: String?<br>characterGroupId: String?<br>timestamp: Long? | Unit |  | 87 |
| `ChatDao.updateChatLocked` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>locked: Boolean<br>timestamp: Long? | Unit | 更新聊天锁定状态 | 96 |
| `ChatDao.updateChatPinned` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>pinned: Boolean<br>timestamp: Long? | Unit | 更新聊天置顶状态 | 100 |
| `ChatDao.updateChatOrderAndGroup` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatId: String<br>displayOrder: Long<br>group: String?<br>timestamp: Long? | Unit | 更新单个聊天的顺序和分组 | 104 |
| `ChatDao.updateChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chats: List<ChatEntity> | Unit | 批量更新聊天的顺序和分组 | 108 |
| `ChatDao.updateGroupName` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | oldName: String<br>newName: String | Unit | 重命名分组 | 112 |
| `ChatDao.updateGroupNameForCharacter` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | oldName: String<br>newName: String<br>characterCardName: String | Unit | 重命名指定角色卡下的分组 | 116 |
| `ChatDao.deleteChatsInGroup` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | groupName: String | Unit | 删除分组下的所有聊天 | 120 |
| `ChatDao.deleteChatsInGroupForCharacter` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | groupName: String<br>characterCardName: String | Unit | 删除指定角色卡下分组的所有聊天 | 124 |
| `ChatDao.removeGroupFromChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | groupName: String<br>timestamp: Long? | Unit | 将分组下的所有聊天移动到"未分组" | 128 |
| `ChatDao.removeGroupFromLockedChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | groupName: String<br>timestamp: Long? | Unit | 将分组下的所有【锁定】聊天移动到"未分组"（用于删除分组但保留锁定聊天） | 132 |
| `ChatDao.removeGroupFromChatsForCharacter` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | groupName: String<br>characterCardName: String<br>timestamp: Long? | Unit | 将指定角色卡下分组的所有聊天移动到"未分组" | 136 |
| `ChatDao.removeGroupFromLockedChatsForCharacter` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | groupName: String<br>characterCardName: String<br>timestamp: Long? | Unit | 将指定角色卡下分组的所有【锁定】聊天移动到"未分组"（用于删除分组但保留锁定聊天） | 140 |
| `ChatDao.getBranchesByParentId` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | parentChatId: String | List<ChatEntity> | 根据parentChatId获取所有分支对话 | 144 |
| `ChatDao.getBranchesByParentIdFlow` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | parentChatId: String | Flow<List<ChatEntity>> | 根据parentChatId获取所有分支对话（Flow版本） | 148 |
| `ChatDao.getMainChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` |  | List<ChatEntity> | 获取所有没有父对话的对话（即主对话） | 152 |
| `ChatDao.getMainChatsFlow` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` |  | Flow<List<ChatEntity>> | 获取所有没有父对话的对话（Flow版本） | 156 |
| `ChatDao.getChatsByCharacterCard` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | characterCardName: String | Flow<List<ChatEntity>> | 根据角色卡名称过滤聊天（非默认角色卡：只显示该角色卡名称的对话） | 160 |
| `ChatDao.getChatsByCharacterGroupId` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | characterGroupId: String | Flow<List<ChatEntity>> | 根据群组ID过滤聊天 | 164 |
| `ChatDao.getChatsByCharacterCardOrNull` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | characterCardName: String | Flow<List<ChatEntity>> | 根据角色卡名称过滤聊天（默认角色卡：显示该角色卡名称的对话 + 所有characterCardName为null的对话） | 168 |
| `ChatDao.clearCharacterCardBinding` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | characterCardName: String<br>timestamp: Long? | Unit | 批量清理绑定特定角色卡名称的对话（将characterCardName设为null） | 172 |
| `ChatDao.deleteUnlockedChatsByCharacterCardName` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | characterCardName: String | Int | 批量删除绑定特定角色卡名称的未锁定对话 | 176 |
| `ChatDao.deleteUnlockedUnboundChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` |  | Int | 批量删除未绑定角色卡的未锁定对话 | 180 |
| `ChatDao.renameCharacterCardBinding` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | oldName: String<br>newName: String<br>timestamp: Long? | Int | 批量重命名角色卡绑定 | 184 |
| `ChatDao.renameCharacterGroupBinding` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | sourceGroupId: String<br>targetGroupId: String<br>timestamp: Long? | Int | 批量重命名角色群组绑定 | 192 |
| `ChatDao.assignCharacterCardToUnbound` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | newName: String<br>timestamp: Long? | Int | 将所有未绑定角色卡的聊天归类到指定角色卡 | 200 |
| `ChatDao.assignCharacterGroupToUnbound` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | targetGroupId: String<br>timestamp: Long? | Int | 将所有未绑定角色群组的聊天归类到指定角色群组 | 207 |
| `ChatDao.updateCharacterCardForChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatIds: List<String><br>newName: String?<br>timestamp: Long? | Int | 批量为指定聊天更新角色卡绑定 | 214 |
| `ChatDao.updateCharacterGroupForChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatIds: List<String><br>characterGroupId: String?<br>timestamp: Long? | Int | 批量为指定聊天更新角色群组绑定 | 222 |
| `ChatDao.clearCharacterGroupForChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatIds: List<String><br>timestamp: Long? | Int | 批量为指定聊天移除角色群组绑定 | 230 |
| `ChatDao.clearCharacterGroupBinding` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | sourceGroupId: String<br>timestamp: Long? | Int | 批量清理绑定特定角色群组ID的对话（将characterGroupId设为null） | 237 |
| `ChatDao.updateGroupForChats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` | chatIds: List<String><br>groupName: String?<br>timestamp: Long? | Int | 批量为指定聊天更新分组 | 244 |
| `ChatDao.getCharacterCardChatStats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` |  | Flow<List<CharacterCardChatStats>> |  | 267 |
| `ChatDao.getCharacterGroupChatStats` | `ChatDao` | `com.ai.assistance.operit.data.dao` | `ChatDao.kt` |  | Flow<List<CharacterGroupChatStats>> |  | 286 |
| `MessageDao.getTotalMessageCount` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` |  | Int | 获取消息总数 | 16 |
| `MessageDao.countMessagesForChatUpToTimestamp` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>upToTimestampInclusive: Long? | Int |  | 21 |
| `MessageDao.getLocatorPreviewsForChat` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>previewCharCount: Int | List<ChatMessageLocatorPreview> |  | 52 |
| `MessageDao.searchLocatorPreviewsForChat` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>query: String<br>previewCharCount: Int | List<ChatMessageLocatorPreview> |  | 83 |
| `MessageDao.existsMessagesBeforeTimestamp` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>beforeTimestampExclusive: Long | Boolean |  | 92 |
| `MessageDao.existsMessagesAfterTimestamp` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>afterTimestampExclusive: Long | Boolean |  | 100 |
| `MessageDao.getLatestSummaryTimestamp` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String | Long? |  | 108 |
| `MessageDao.getLatestSummaryTimestampBefore` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>beforeTimestampExclusive: Long | Long? |  | 113 |
| `MessageDao.getLatestSummaryTimestampUpTo` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>upToTimestampInclusive: Long | Long? |  | 121 |
| `MessageDao.existsUserMessage` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String | Boolean |  | 129 |
| `MessageDao.existsAnyMessage` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String | Boolean |  | 132 |
| `MessageDao.getMessageCountsByChatId` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` |  | List<ChatMessageCount> |  | 135 |
| `MessageDao.insertMessage` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | message: MessageEntity | Long | 插入单条消息并返回消息ID | 139 |
| `MessageDao.insertMessages` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | messages: List<MessageEntity> | Unit | 批量插入消息 | 143 |
| `MessageDao.copyMessagesToChat` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | sourceChatId: String<br>targetChatId: String<br>upToTimestampInclusive: Long? | Unit |  | 191 |
| `MessageDao.updateMessageContent` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | messageId: Long<br>content: String | Unit | 更新消息内容 | 199 |
| `MessageDao.updateMessage` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | message: MessageEntity | Unit | 更新整条消息 | 203 |
| `MessageDao.getMaxOrderIndex` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String | Int? | 获取指定聊天中最大的序号 | 207 |
| `MessageDao.deleteAllMessagesForChat` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String | Unit | 删除指定聊天的所有消息 | 211 |
| `MessageDao.deleteMessagesFrom` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>timestamp: Long | Unit | 删除指定聊天中从某个时间戳开始的所有消息 | 215 |
| `MessageDao.deleteMessageByTimestamp` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>timestamp: Long | Unit |  | 218 |
| `MessageDao.updateSelectedVariantIndex` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>timestamp: Long<br>selectedVariantIndex: Int | Unit |  | 223 |
| `MessageDao.updateMessageFavorite` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | chatId: String<br>timestamp: Long<br>isFavorite: Boolean | Unit |  | 232 |
| `MessageDao.searchChatIdsByContent` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | query: String | List<String> | 查找包含特定关键词的聊天ID列表（不重复） | 240 |
| `MessageDao.renameRoleName` | `MessageDao` | `com.ai.assistance.operit.data.dao` | `MessageDao.kt` | oldName: String<br>newName: String | Int | 批量重命名消息中的角色名 | 244 |
| `MessageVariantDao.insertVariant` | `MessageVariantDao` | `com.ai.assistance.operit.data.dao` | `MessageVariantDao.kt` | variant: MessageVariantEntity | Long |  | 13 |
| `MessageVariantDao.insertVariants` | `MessageVariantDao` | `com.ai.assistance.operit.data.dao` | `MessageVariantDao.kt` | variants: List<MessageVariantEntity> | Unit |  | 16 |
| `MessageVariantDao.copyVariantsToChat` | `MessageVariantDao` | `com.ai.assistance.operit.data.dao` | `MessageVariantDao.kt` | sourceChatId: String<br>targetChatId: String<br>upToTimestampInclusive: Long? | Unit |  | 56 |
| `MessageVariantDao.updateVariant` | `MessageVariantDao` | `com.ai.assistance.operit.data.dao` | `MessageVariantDao.kt` | variant: MessageVariantEntity | Unit |  | 63 |
| `MessageVariantDao.deleteVariant` | `MessageVariantDao` | `com.ai.assistance.operit.data.dao` | `MessageVariantDao.kt` | chatId: String<br>messageTimestamp: Long<br>variantIndex: Int | Unit |  | 68 |
| `MessageVariantDao.deleteVariantsForMessage` | `MessageVariantDao` | `com.ai.assistance.operit.data.dao` | `MessageVariantDao.kt` | chatId: String<br>messageTimestamp: Long | Unit |  | 75 |
| `MessageVariantDao.deleteVariantsFrom` | `MessageVariantDao` | `com.ai.assistance.operit.data.dao` | `MessageVariantDao.kt` | chatId: String<br>messageTimestamp: Long | Unit |  | 78 |
| `MessageVariantDao.deleteAllVariantsForChat` | `MessageVariantDao` | `com.ai.assistance.operit.data.dao` | `MessageVariantDao.kt` | chatId: String | Unit |  | 81 |
| `TokenUsageDao.insertRecord` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | record: TokenUsageRecordEntity | Long |  | 39 |
| `TokenUsageDao.insertRecords` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | records: List<TokenUsageRecordEntity> | Unit |  | 42 |
| `TokenUsageDao.upsertStatsModel` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | model: TokenStatsModelEntity | Unit |  | 45 |
| `TokenUsageDao.getStatsModel` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | configId: String<br>provider: String<br>model: String | TokenStatsModelEntity? |  | 53 |
| `TokenUsageDao.getAllStatsModels` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` |  | List<TokenStatsModelEntity> |  | 60 |
| `TokenUsageDao.clearPricing` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | configId: String<br>provider: String<br>model: String | Int |  | 75 |
| `TokenUsageDao.deleteEmptyStatsModels` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` |  | Int |  | 89 |
| `TokenUsageDao.aggregateModelsForLifetime` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | providerModels: List<String><br>allModels: Boolean | List<TokenUsageModelAggregateRow> |  | 114 |
| `TokenUsageDao.getEarliestOccurredAtMs` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | providerModels: List<String><br>allModels: Boolean | Long? |  | 127 |
| `TokenUsageDao.aggregateModelsInRange` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | startMs: Long<br>endMs: Long<br>providerModels: List<String><br>allModels: Boolean | List<TokenUsageModelAggregateRow> |  | 156 |
| `TokenUsageDao.getActivityDaysInRange` | `TokenUsageDao` | `com.ai.assistance.operit.data.dao` | `TokenUsageDao.kt` | startMs: Long<br>endMs: Long<br>providerModels: List<String><br>allModels: Boolean | List<TokenUsageActivityDayRow> |  | 186 |
| `AppDatabase.chatDao` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` |  | ChatDao | 获取聊天DAO | 41 |
| `AppDatabase.messageDao` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` |  | MessageDao | 获取消息DAO | 44 |
| `AppDatabase.messageVariantDao` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` |  | MessageVariantDao |  | 45 |
| `AppDatabase.chatContentDao` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` |  | ChatContentDao |  | 46 |
| `AppDatabase.tokenUsageDao` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` |  | TokenUsageDao |  | 47 |
| `AppDatabase.annualReportDao` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` |  | AnnualReportDao | 年度报告的只读聚合查询，只新增 DAO，不改表结构。 | 50 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 61 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 101 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 114 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 126 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 156 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 163 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 199 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 208 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 217 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 226 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 238 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 246 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | connection: androidx.sqlite.SQLiteConnection | Unit |  | 250 |
| `AppDatabase.runSql` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | exec: (String) -> Unit | Unit |  | 261 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 361 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 370 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 382 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 391 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 404 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 413 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 424 |
| `AppDatabase.migrate` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | db: SupportSQLiteDatabase | Unit |  | 435 |
| `AppDatabase.getDatabase` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | context: Context | AppDatabase | 获取数据库实例，单例模式 | 446 |
| `AppDatabase.validateRecoveryCopy` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | context: Context<br>sourceDatabase: File | Boolean | Opens a private copy through Room so the recovery UI can validate the complete schema and… | 459 |
| `AppDatabase.buildDatabase` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | context: Context<br>databaseName: String | AppDatabase |  | 514 |
| `AppDatabase.databaseFiles` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | databaseFile: File | List<File> |  | 544 |
| `AppDatabase.closeDatabase` | `AppDatabase` | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` |  | Unit |  | 552 |
| `ObjectBoxManager.get` | `ObjectBoxManager` | `com.ai.assistance.operit.data.db` | `ObjectBox.kt` | context: Context<br>profileId: String | BoxStore |  | 13 |
| `ObjectBoxManager.buildStore` | `ObjectBoxManager` | `com.ai.assistance.operit.data.db` | `ObjectBox.kt` | context: Context<br>profileId: String | BoxStore |  | 22 |
| `ObjectBoxManager.close` | `ObjectBoxManager` | `com.ai.assistance.operit.data.db` | `ObjectBox.kt` | profileId: String | Unit |  | 33 |
| `ObjectBoxManager.delete` | `ObjectBoxManager` | `com.ai.assistance.operit.data.db` | `ObjectBox.kt` | context: Context<br>profileId: String | Unit | 物理删除指定profileId的数据库（包括关闭store和删除文件夹）。 | 43 |
| `ObjectBoxManager.closeAll` | `ObjectBoxManager` | `com.ai.assistance.operit.data.db` | `ObjectBox.kt` |  | Unit |  | 54 |
| `HtmlExporter.exportSingle` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | context: Context<br>chatHistory: ChatHistory | String | 导出单个对话为 HTML | 23 |
| `HtmlExporter.exportMultiple` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | context: Context<br>chatHistories: List<ChatHistory> | String | 导出多个对话为 HTML | 32 |
| `HtmlExporter.writeMultipleHeader` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | context: Context<br>chatHistories: List<ChatHistory><br>totalMessageCount: Int<br>writer: Writer | Unit | 写入多个对话的 HTML 头部。 | 51 |
| `HtmlExporter.writeConversationSeparator` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | writer: Writer<br>index: Int | Unit | 写入对话之间的 HTML 分隔线。 | 71 |
| `HtmlExporter.writeSingleToWriter` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | context: Context<br>chatHistory: ChatHistory<br>writer: Writer<br>onContentCharactersWritten: (Long) -> Unit? | Unit | 写入单个对话。 | 80 |
| `HtmlExporter.writeConversationToWriter` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | context: Context<br>writer: Writer<br>chatHistory: ChatHistory<br>onContentCharactersWritten: (Long) -> Unit? | Unit | 写入单个对话内容，不包含 HTML 文档头尾。 | 94 |
| `HtmlExporter.writeMultipleFooter` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | context: Context<br>writer: Writer | Unit | 写入多个对话的 HTML 尾部。 | 106 |
| `HtmlExporter.appendHtmlHeader` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | writer: Writer<br>title: String | Unit | 添加 HTML 头部 | 113 |
| `HtmlExporter.appendChatContent` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | context: Context<br>writer: Writer<br>chatHistory: ChatHistory<br>onContentCharactersWritten: (Long) -> Unit | Unit | 添加对话内容 | 131 |
| `HtmlExporter.appendMessageHtml` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | context: Context<br>writer: Writer<br>message: ChatMessage<br>onContentCharactersWritten: (Long) -> Unit | Unit | 添加单条消息 | 162 |
| `HtmlExporter.appendHtmlFooter` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | context: Context<br>writer: Writer | Unit | 添加 HTML 尾部 | 194 |
| `HtmlExporter.getCss` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` |  | String | 获取 CSS 样式 | 206 |
| `HtmlExporter.escapeHtml` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | text: String | String | 转义 HTML 特殊字符 | 334 |
| `HtmlExporter.writeFormattedContent` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | writer: Writer<br>content: String<br>onContentCharactersWritten: (Long) -> Unit | Unit | 逐段格式化内容（保留换行，转义HTML）。 | 346 |
| `HtmlExporter.writeEscapedRange` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | writer: Writer<br>content: String<br>start: Int<br>end: Int<br>onContentCharactersWritten: (Long) -> Unit | Unit |  | 395 |
| `HtmlExporter.findNextHtmlEscapeCharacter` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | content: String<br>start: Int<br>end: Int | Int |  | 446 |
| `HtmlExporter.isHtmlEscapeCharacter` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | character: Char | Boolean |  | 458 |
| `HtmlExporter.reportCharacters` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | characterCount: Int<br>onContentCharactersWritten: (Long) -> Unit | Unit |  | 465 |
| `HtmlExporter.startsWithCodeFence` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | content: String<br>start: Int<br>end: Int | Boolean |  | 477 |
| `HtmlExporter.findLineBreakStart` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | content: String<br>start: Int | Int? |  | 485 |
| `MarkdownExporter.exportSingle` | `MarkdownExporter` | `com.ai.assistance.operit.data.exporter` | `MarkdownExporter.kt` | context: Context<br>chatHistory: ChatHistory | String | 导出单个对话为 Markdown | 19 |
| `MarkdownExporter.exportMultiple` | `MarkdownExporter` | `com.ai.assistance.operit.data.exporter` | `MarkdownExporter.kt` | context: Context<br>chatHistories: List<ChatHistory> | String | 导出多个对话为 Markdown | 71 |
| `MarkdownExporter.appendMessage` | `MarkdownExporter` | `com.ai.assistance.operit.data.exporter` | `MarkdownExporter.kt` | sb: StringBuilder<br>message: ChatMessage | Unit | 添加单条消息 | 99 |
| `TextExporter.exportSingle` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | context: Context<br>chatHistory: ChatHistory | String | 导出单个对话为纯文本 | 22 |
| `TextExporter.exportMultiple` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | context: Context<br>chatHistories: List<ChatHistory> | String | 导出多个对话为纯文本 | 31 |
| `TextExporter.writeMultipleHeader` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | context: Context<br>chatHistories: List<ChatHistory><br>totalMessageCount: Int<br>writer: Writer | Unit | 写入多个对话的纯文本头部。 长文本导出使用 Writer，避免把所有结果拼接成一个大字符串。 | 52 |
| `TextExporter.writeConversationSeparator` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | writer: Writer<br>index: Int | Unit | 写入对话之间的分隔内容。 | 80 |
| `TextExporter.writeSingleToWriter` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | context: Context<br>chatHistory: ChatHistory<br>writer: Writer<br>onContentCharactersWritten: (Long) -> Unit? | Unit | 写入单个对话。 长文本按固定大小写入，避免 Writer 调用方再次创建整段正文副本。 | 92 |
| `TextExporter.writeMultipleFooter` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | context: Context<br>writer: Writer | Unit | 写入多个对话的纯文本尾部。 | 138 |
| `TextExporter.writeMessage` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | context: Context<br>writer: Writer<br>message: ChatMessage<br>onContentCharactersWritten: (Long) -> Unit | Unit | 添加单条消息 | 147 |
| `TextExporter.writeContent` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | writer: Writer<br>content: String<br>onContentCharactersWritten: (Long) -> Unit | Unit |  | 173 |
| `TextExporter.center` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | width: Int | String | 字符串居中扩展函数 | 194 |
| `McpConfigImportParser.parse` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | jsonConfig: String | McpConfigImport |  | 43 |
| `McpConfigImportParser.parseServer` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | serverId: String<br>configElement: JsonElement | McpImportedServer |  | 61 |
| `McpConfigImportParser.parseStdioServer` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | serverId: String<br>config: JsonObject<br>declaredType: String? | StdioMcpImportedServer |  | 74 |
| `McpConfigImportParser.parseRemoteServer` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | serverId: String<br>config: JsonObject<br>declaredType: String? | RemoteMcpImportedServer |  | 94 |
| `McpConfigImportParser.requiredObject` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | field: String | JsonObject |  | 118 |
| `McpConfigImportParser.requiredNonBlankString` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | field: String<br>serverId: String | String |  | 125 |
| `McpConfigImportParser.optionalString` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | field: String | String? |  | 132 |
| `McpConfigImportParser.optionalNonBlankString` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | field: String<br>serverId: String | String? |  | 138 |
| `McpConfigImportParser.optionalBoolean` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | field: String<br>serverId: String | Boolean |  | 145 |
| `McpConfigImportParser.optionalStringList` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | field: String<br>serverId: String | List<String> |  | 153 |
| `McpConfigImportParser.optionalStringMap` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | field: String<br>serverId: String | Map<String, String> |  | 164 |
| `MCPLocalServer.getInstance` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | context: Context | MCPLocalServer |  | 59 |
| `MCPLocalServer.reloadConfigurations` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | Unit | 重新加载配置文件（用于用户手动编辑配置后刷新） | 230 |
| `MCPLocalServer.loadAllConfigurations` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | Unit | 加载所有配置文件 | 240 |
| `MCPLocalServer.autoFillMissingMetadata` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | config: MCPConfig | MCPConfig | 自动为缺失的服务器创建默认元数据 | 295 |
| `MCPLocalServer.displayNameForServerId` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | String |  | 334 |
| `MCPLocalServer.createRemoteMetadata` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | server: RemoteMcpImportedServer<br>existingMetadata: PluginMetadata? | PluginMetadata |  | 342 |
| `MCPLocalServer.sanitizeServerConfig` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String<br>serverConfig: MCPConfig.ServerConfig<br>source: String | MCPConfig.ServerConfig? |  | 374 |
| `MCPLocalServer.resetRuntimeState` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | Unit |  | 403 |
| `MCPLocalServer.hasLocalRuntimeConfigurationChanged` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | existing: MCPConfig.ServerConfig<br>replacement: MCPConfig.ServerConfig | Boolean |  | 412 |
| `MCPLocalServer.hasRemoteRuntimeConfigurationChanged` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | existing: PluginMetadata<br>replacement: PluginMetadata | Boolean |  | 424 |
| `MCPLocalServer.sanitizeMCPConfig` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | config: MCPConfig<br>source: String | SanitizedConfigResult |  | 435 |
| `MCPLocalServer.initializeMissingServerStatus` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | Unit | 为新配置的服务器初始化状态 | 481 |
| `MCPLocalServer.saveMCPConfig` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | Unit | 保存MCP配置 | 510 |
| `MCPLocalServer.saveServerStatus` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | Unit | 保存服务器状态 | 523 |
| `MCPLocalServer.addOrUpdateMCPServer` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String<br>command: String<br>args: List<String>??<br>env: Map<String, String>??<br>disabled: Boolean?<br>autoApprove: List<String>??<br>cwd: String?? | Unit | 添加或更新MCP服务器配置 | 538 |
| `MCPLocalServer.removeMCPServer` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | Unit | 删除MCP服务器配置 | 590 |
| `MCPLocalServer.mergeConfigFromJson` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | jsonConfig: String | Result<Int> | 合并JSON配置到现有配置 | 608 |
| `MCPLocalServer.getConfigFilePath` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | String | 获取配置文件路径 | 704 |
| `MCPLocalServer.getMCPServer` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | MCPConfig.ServerConfig? | 获取MCP服务器配置 | 709 |
| `MCPLocalServer.getAllMCPServers` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | Map<String, MCPConfig.ServerConfig> | 获取所有MCP服务器配置 | 716 |
| `MCPLocalServer.addOrUpdatePluginMetadata` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | metadata: PluginMetadata | Unit | 添加或更新插件元数据 | 725 |
| `MCPLocalServer.removePluginMetadata` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | pluginId: String | Unit | 删除插件元数据 | 751 |
| `MCPLocalServer.getPluginMetadata` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | pluginId: String | PluginMetadata? | 获取插件元数据 | 764 |
| `MCPLocalServer.getAllPluginMetadata` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | Map<String, PluginMetadata> | 获取所有插件元数据 | 771 |
| `MCPLocalServer.updateServerStatus` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String<br>errorMessage: String??<br>cachedTools: List<CachedToolInfo>??<br>lastStartTime: Long??<br>lastStopTime: Long?? | Unit | 更新服务器状态 注意：启用/禁用状态请使用 setServerEnabled() 方法 | 781 |
| `MCPLocalServer.cacheServerTools` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String<br>tools: List<CachedToolInfo> | Unit | 缓存服务器的工具列表 | 808 |
| `MCPLocalServer.getCachedTools` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | List<CachedToolInfo>? | 获取缓存的工具列表 | 816 |
| `MCPLocalServer.hasValidToolCache` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | Boolean | 检查工具缓存是否有效 (有效期1天) | 823 |
| `MCPLocalServer.removeServerStatus` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | Unit | 删除服务器状态 | 841 |
| `MCPLocalServer.getServerStatus` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | ServerStatus? | 获取服务器状态 | 852 |
| `MCPLocalServer.getAllServerStatus` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | Map<String, ServerStatus> | 获取所有服务器状态 | 859 |
| `MCPLocalServer.isServerLikelyRunning` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | Boolean | 基于时间戳推断服务是否处于运行态（近似状态，不是实时状态） | 866 |
| `MCPLocalServer.isServerEnabled` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String | Boolean | 检查服务器是否启用 本地插件从 mcpServers.disabled 读取；远程插件从 pluginMetadata.disabled 读取 | 875 |
| `MCPLocalServer.setServerEnabled` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | serverId: String<br>enabled: Boolean | Unit | 设置服务器启用状态 本地插件写入 mcpServers.disabled；远程插件写入 pluginMetadata.disabled | 893 |
| `MCPLocalServer.getPluginRuntimeDirectory` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | pluginId: String | String |  | 943 |
| `MCPLocalServer.pluginRuntimeUsesAppManagedDirectory` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | pluginId: String | Boolean | True when the service is launched from the app-managed ~/mcp_plugins/<id> directory. | 959 |
| `MCPLocalServer.pluginRuntimeAllowsEmptyDirectory` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | pluginId: String | Boolean | npx/uvx/uv 由包管理器下载自身载荷，因此运行目录允许为空。 | 969 |
| `MCPLocalServer.isPluginRuntimeReady` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | pluginId: String | Boolean | 检查插件运行目录是否已就绪。 配置了绝对命令、绝对入口脚本或显式 cwd 的 stdio 服务不依赖 Operit 复制插件目录， 因此直接视为就绪；否则按既有规则检查 ~/mc… | 983 |
| `MCPLocalServer.getPluginConfig` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | pluginId: String | String | 获取插件配置（兼容旧接口） | 1063 |
| `MCPLocalServer.savePluginConfig` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | pluginId: String<br>config: String | Boolean | 保存插件配置（兼容旧接口） | 1082 |
| `MCPLocalServer.exportConfigAsJson` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | String | 导出配置为JSON字符串 | 1114 |
| `MCPLocalServer.importConfigFromJson` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` | json: String | Boolean | 从JSON字符串导入配置 | 1127 |
| `MCPLocalServer.getConfigDirectory` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | String | 获取配置目录路径 | 1159 |
| `MCPLocalServer.cleanupInvalidConfigurations` | `MCPLocalServer` | `com.ai.assistance.operit.data.mcp` | `MCPLocalServer.kt` |  | Unit | 清理无效配置 | 1164 |
| `MCPRepository.refreshInstalledPlugins` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` |  | Unit |  | 109 |
| `MCPRepository.loadPluginsFromMCPLocalServer` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` |  | Unit | 从MCPLocalServer加载插件信息（主要数据源） | 118 |
| `MCPRepository.scanPhysicallyInstalledPlugins` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` |  | Set<String> | 扫描文件系统中实际安装的插件（辅助验证） | 186 |
| `MCPRepository.needsPhysicalInstallation` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | serverId: String | Boolean | 判断插件是否需要物理安装（npx/uvx/uv 以及自包含路径配置不需要） | 206 |
| `MCPRepository.checkConfigNeedsPhysicalInstallation` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | jsonConfig: String | Boolean | 检查标准 MCP 配置中的 stdio 服务器是否需要物理安装。 远程 HTTP/SSE 服务器只写入远程元数据，不需要仓库目录。 | 220 |
| `MCPRepository.isPluginPhysicallyInstalled` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | serverId: String | Boolean | 检查插件是否在文件系统中物理存在 | 236 |
| `MCPRepository.isPluginInstalled` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | serverId: String | Boolean | 检查插件是否已安装（优先从MCPLocalServer检查） | 252 |
| `MCPRepository.getInstalledPluginPath` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | serverId: String | String? | 获取已安装插件的路径 | 269 |
| `MCPRepository.installMCPServer` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginId: String<br>progressCallback: (InstallProgress) -> Unit? | InstallResult | 安装MCP插件 | 292 |
| `MCPRepository.installMCPServerWithObject` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | server: MCPLocalServer.PluginMetadata<br>progressCallback: (InstallProgress) -> Unit? | InstallResult | 安装MCP插件 - 使用服务器对象 | 319 |
| `MCPRepository.installMCPServerFromZip` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | serverId: String<br>zipUri: Uri<br>name: String<br>description: String<br>author: String<br>progressCallback: (InstallProgress) -> Unit? | InstallResult | 从本地ZIP文件安装MCP插件 | 342 |
| `MCPRepository.uninstallMCPServer` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginId: String | Boolean | 卸载MCP插件 | 392 |
| `MCPRepository.installPluginInternal` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | server: MCPLocalServer.PluginMetadata<br>progressCallback: (InstallProgress) -> Unit | InstallResult | 内部安装插件实现 | 425 |
| `MCPRepository.installPluginFromZipInternal` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | server: MCPLocalServer.PluginMetadata<br>zipUri: Uri<br>progressCallback: (InstallProgress) -> Unit | InstallResult | 从ZIP文件安装插件的内部实现 | 486 |
| `MCPRepository.downloadRepositoryZip` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | owner: String<br>repoName: String<br>serverId: String<br>progressCallback: (InstallProgress) -> Unit | File? | 下载仓库ZIP文件 | 548 |
| `MCPRepository.getGithubDefaultBranch` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | owner: String<br>repoName: String | String? | 使用 GitHub API 获取仓库的默认分支 | 577 |
| `MCPRepository.downloadFromUrl` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | zipUrl: String<br>serverId: String<br>progressCallback: (InstallProgress) -> Unit | File? | 从URL下载文件 | 614 |
| `MCPRepository.extractZipFile` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | zipFile: File<br>targetDir: File<br>progressCallback: (InstallProgress) -> Unit | Boolean | 解压ZIP文件 | 681 |
| `MCPRepository.countZipEntries` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | zipFile: File | Int | 计算ZIP文件中的条目数量 | 758 |
| `MCPRepository.extractOwnerAndRepo` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | repoUrl: String | Pair<String, String>? | 从GitHub仓库URL中提取所有者和仓库名 | 781 |
| `MCPRepository.checkForRequiredFiles` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginDir: File | Boolean | 检查插件目录中是否包含必要的关键文件 | 800 |
| `MCPRepository.hasPluginRequiredFiles` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | dir: File | Boolean | 检查目录是否包含插件所需的必要文件 | 813 |
| `MCPRepository.savePluginMetadata` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | server: MCPLocalServer.PluginMetadata<br>pluginPath: String | Unit | 保存插件元数据到MCPLocalServer | 838 |
| `MCPRepository.addRemoteServer` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | server: MCPLocalServer.PluginMetadata | Unit | 添加远程服务器 | 852 |
| `MCPRepository.updateRemoteServer` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | server: MCPLocalServer.PluginMetadata | Unit | 更新远程服务器 | 875 |
| `MCPRepository.removeRemoteServer` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | serverId: String | Boolean | 删除远程服务器 | 903 |
| `MCPRepository.syncBridgeStatus` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` |  | Unit | Synchronizes local stdio plugin status from the bridge. | 921 |
| `MCPRepository.syncInstalledStatus` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` |  | Unit | 同步已安装状态 | 997 |
| `MCPRepository.initialize` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` |  | Unit | 初始化仓库 | 1011 |
| `MCPRepository.getInstalledPluginInfo` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginId: String | MCPLocalServer.PluginMetadata? | 获取已安装插件的信息 | 1021 |
| `MCPRepository.generatePluginDescription` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginId: String<br>pluginName: String | Result<String> |  | 1025 |
| `MCPRepository.collectToolDescriptionsForDescriptionGeneration` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | metadata: MCPLocalServer.PluginMetadata | List<String> |  | 1066 |
| `MCPRepository.getRemoteToolNames` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginId: String | List<String> | Returns the names exposed by a remote MCP service for list presentation, and registers th… | 1101 |
| `MCPRepository.discoverRemoteToolNames` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginId: String<br>metadata: MCPLocalServer.PluginMetadata | List<String> |  | 1119 |
| `MCPRepository.refreshPluginList` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` |  | Unit | 手动刷新插件列表 会重新加载配置文件，自动识别新添加的 mcpServers 配置 | 1163 |
| `MCPRepository.registerToolsForLoadedPlugins` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | successfulPluginIds: List<String> | Unit | 为加载成功的插件注册工具 优先使用本地缓存的工具信息，避免重复连接服务 | 1179 |
| `MCPRepository.registerToolsForPlugin` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginId: String | Unit | 把单个插件接入 AI 运行时：在 MCPManager 中注册服务器（这是 AI 能看到该包的前提）， 并把它的工具注册到 AIToolHandler。 注册由多个生命周期节点触… | 1197 |
| `MCPRepository.unregisterToolsForPlugins` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginIds: List<String> | Unit | 反注册插件对应的运行时服务器与工具，避免禁用后仍出现在系统提示词。 | 1263 |
| `MCPRepository.getToolsForPlugin` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | pluginId: String | List<UnifiedToolInfo> |  | 1289 |
| `MCPRepository.createRuntimeDescriptor` | `MCPRepository` | `com.ai.assistance.operit.data.mcp` | `MCPRepository.kt` | metadata: MCPLocalServer.PluginMetadata | McpRuntimeDescriptor |  | 1336 |
| `McpStdioConfigResolver.commandName` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | command: String | String |  | 19 |
| `McpStdioConfigResolver.isTerminalPath` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | value: String | Boolean | True when the value points at a concrete path in the terminal environment. | 23 |
| `McpStdioConfigResolver.normalizeHomePath` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | value: String | String |  | 31 |
| `McpStdioConfigResolver.isAppManagedRuntimePath` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | value: String | Boolean | True when the path belongs to the directory Operit populates by copying a plugin. | 43 |
| `McpStdioConfigResolver.isExternalTerminalPath` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | value: String | Boolean | A path outside `~/mcp_plugins` already exists in the terminal and needs no app copy. | 50 |
| `McpStdioConfigResolver.firstPositionalArgument` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | args: List<String> | String? | First argument that is not a flag or the value of an inline evaluation flag. | 54 |
| `McpStdioConfigResolver.usesAppManagedRuntimeDirectory` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | command: String<br>args: List<String><br>cwd: String? | Boolean | True when the service runs from `~/mcp_plugins/<id>` instead of a directory the user conf… | 72 |
| `McpStdioConfigResolver.requiresAppManagedInstallation` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | command: String<br>args: List<String><br>cwd: String? | Boolean | True when Operit must copy an Android-side plugin directory into the Linux runtime before… | 93 |
| `McpStdioConfigResolver.resolveWorkingDirectory` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | configuredCwd: String?<br>pluginId: String<br>command: String<br>args: List<String> | String | Working directory used when launching the service. An explicit `cwd` always wins. For a s… | 107 |
| `BridgeMcpRuntimeSession.connect` | `BridgeMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `BridgeMcpRuntimeSession.kt` |  | Boolean |  | 17 |
| `BridgeMcpRuntimeSession.isConnected` | `BridgeMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `BridgeMcpRuntimeSession.kt` |  | Boolean |  | 19 |
| `BridgeMcpRuntimeSession.isActive` | `BridgeMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `BridgeMcpRuntimeSession.kt` |  | Boolean |  | 21 |
| `BridgeMcpRuntimeSession.listTools` | `BridgeMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `BridgeMcpRuntimeSession.kt` |  | List<McpRuntimeTool> |  | 23 |
| `BridgeMcpRuntimeSession.callTool` | `BridgeMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `BridgeMcpRuntimeSession.kt` | name: String<br>arguments: Map<String, Any?> | McpRuntimeCallResult |  | 34 |
| `BridgeMcpRuntimeSession.getLastFailureDetail` | `BridgeMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `BridgeMcpRuntimeSession.kt` |  | String? |  | 51 |
| `BridgeMcpRuntimeSession.close` | `BridgeMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `BridgeMcpRuntimeSession.kt` |  | Unit |  | 53 |
| `MCPBridge.getInstance` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | context: Context | MCPBridge |  | 98 |
| `MCPBridge.detectPort` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` |  | Int | 智能检测可用端口 优先尝试 8752（本地直连），失败后尝试 8751（SSH转发） | 111 |
| `MCPBridge.isPortAvailable` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | host: String<br>port: Int | Boolean | 检查端口是否可用（快速检测，无日志污染） | 143 |
| `MCPBridge.closeCommandConnectionLocked` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` |  | Unit |  | 161 |
| `MCPBridge.isCommandSocketReusable` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | host: String<br>port: Int<br>nowMs: Long | Boolean |  | 175 |
| `MCPBridge.scheduleCommandConnectionCloseLocked` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` |  | Unit |  | 189 |
| `MCPBridge.deployBridge` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | context: Context<br>sessionId: String?? | Boolean | 部署桥接器到终端 | 205 |
| `MCPBridge.startBridge` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | context: Context??<br>port: Int?<br>mcpCommand: String??<br>mcpArgs: List<String>??<br>sessionId: String?? | Boolean | 在终端中启动桥接器 | 298 |
| `MCPBridge.reset` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | context: Context?? | JSONObject? | 重置桥接器（静态方法） | 427 |
| `MCPBridge.redactForLog` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | value: Any? | Any? | Copies a JSON payload for logging with secret-bearing values masked. `env` maps carry API… | 459 |
| `MCPBridge.redactSensitiveParams` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | params: JSONObject? | String |  | 484 |
| `MCPBridge.sendCommandThroughStream` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | command: JSONObject<br>writer: PrintWriter<br>reader: BufferedReader<br>cmdId: String<br>cmdType: String<br>serviceName: String?<br>emptyResponseMessage: String | JSONObject? |  | 489 |
| `MCPBridge.sendCommand` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | command: JSONObject<br>host: String?<br>port: Int?? | JSONObject? |  | 520 |
| `MCPBridge.sendCommand` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | context: Context<br>command: JSONObject<br>host: String?<br>port: Int?? | JSONObject? | 发送命令到桥接器 | 534 |
| `MCPBridge.registerMcpService` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | name: String<br>command: String<br>args: List<String>?<br>description: String??<br>env: Map<String, String>?<br>cwd: String?? | JSONObject? | 注册新的MCP服务 | 654 |
| `MCPBridge.unregisterMcpService` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | name: String | JSONObject? | 取消注册MCP服务 | 675 |
| `MCPBridge.listMcpServices` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | serviceName: String?? | JSONObject? | 列出所有注册的MCP服务或查询单个服务 | 680 |
| `MCPBridge.spawnMcpService` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | name: String??<br>command: String??<br>args: List<String>??<br>env: Map<String, String>??<br>cwd: String??<br>timeoutMs: Long?? | JSONObject? | 启动MCP服务 | 685 |
| `MCPBridge.unspawnMcpService` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | name: String | JSONObject? | 停止MCP服务（不注销） | 706 |
| `MCPBridge.listTools` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | serviceName: String?? | JSONObject? | 获取工具列表 | 711 |
| `MCPBridge.callTool` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | method: String<br>params: JSONObject | JSONObject? | 调用工具 | 717 |
| `MCPBridge.toolcall` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | method: String<br>params: Map<String, Any> | JSONObject? | 简化调用工具的方法 | 722 |
| `MCPBridge.getServiceStatus` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | serviceName: String | JSONObject? | 查询特定MCP服务的状态 | 734 |
| `MCPBridge.getServiceLogs` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` | serviceName: String | JSONObject? |  | 745 |
| `MCPBridge.resetBridge` | `MCPBridge` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridge.kt` |  | JSONObject? | 重置桥接器 - 关闭所有服务、清空注册表和池子 | 754 |
| `MCPBridgeClient.buildRegisterLocalCommand` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | name: String<br>command: String<br>args: List<String>?<br>description: String??<br>env: Map<String, String>?<br>cwd: String?? | JSONObject |  | 19 |
| `MCPBridgeClient.buildUnregisterCommand` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | name: String | JSONObject |  | 54 |
| `MCPBridgeClient.buildListServicesCommand` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | serviceName: String?? | JSONObject |  | 62 |
| `MCPBridgeClient.buildSpawnCommand` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | name: String??<br>command: String??<br>args: List<String>??<br>env: Map<String, String>??<br>cwd: String??<br>timeoutMs: Long?? | JSONObject |  | 72 |
| `MCPBridgeClient.buildUnspawnCommand` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | name: String | JSONObject |  | 109 |
| `MCPBridgeClient.buildListToolsCommand` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | serviceName: String?? | JSONObject |  | 117 |
| `MCPBridgeClient.buildToolCallCommand` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | name: String??<br>method: String<br>params: JSONObject | JSONObject |  | 132 |
| `MCPBridgeClient.buildLogsCommand` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | name: String | JSONObject |  | 153 |
| `MCPBridgeClient.buildResetCommand` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | JSONObject |  | 161 |
| `MCPBridgeClient.getLastConnectionFailureDetail` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | String? |  | 174 |
| `MCPBridgeClient.setLastConnectionFailureDetail` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | detail: String? | Unit |  | 176 |
| `MCPBridgeClient.buildSpawnFailureDetail` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | spawnResp: JSONObject?<br>fallbackMessage: String | String |  | 180 |
| `MCPBridgeClient.connect` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | Boolean | Connect to the MCP service. If the service is registered but not active, this will attemp… | 212 |
| `MCPBridgeClient.isConnected` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | Boolean | Check if connected | 277 |
| `MCPBridgeClient.ping` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | Boolean | Ping the service | 280 |
| `MCPBridgeClient.pingSync` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | Boolean | Synchronous ping method | 311 |
| `MCPBridgeClient.spawnBlocking` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | timeoutMs: Long? | JSONObject? | Spawn the MCP service if it's not already active | 314 |
| `MCPBridgeClient.unspawn` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | Boolean | Unspawn the MCP service (stops the process, but keeps it registered) | 349 |
| `MCPBridgeClient.isActive` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | Boolean | Check if the service is currently active on the bridge | 372 |
| `MCPBridgeClient.callTool` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | method: String<br>params: JSONObject | JSONObject? | Call a tool on the MCP service - 返回完整的响应（包括 success, result, error） | 377 |
| `MCPBridgeClient.callToolSync` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | method: String<br>params: JSONObject | JSONObject? | Synchronous tool call | 472 |
| `MCPBridgeClient.callToolSync` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | method: String<br>params: Map<String, Any> | JSONObject? | Synchronous tool call with Map | 477 |
| `MCPBridgeClient.convertToJsonType` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` | value: Any? | Any? | 将 Kotlin 类型转换为 JSON 类型 - List -> JSONArray - Map -> JSONObject - 其他 -> 保持原样 | 493 |
| `MCPBridgeClient.getTools` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | List<JSONObject> | Get all tools provided by the service | 518 |
| `MCPBridgeClient.getServiceInfo` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | ServiceInfo? | Get service info including tools count and running status | 580 |
| `MCPBridgeClient.getToolDescriptions` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | List<String> | Get tool descriptions provided by the service as a list of strings | 630 |
| `MCPBridgeClient.disconnect` | `MCPBridgeClient` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPBridgeClient.kt` |  | Unit | Disconnect from the service | 654 |
| `MCPCommandGenerator.generateDeployCommands` | `MCPCommandGenerator` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPCommandGenerator.kt` | projectStructure: ProjectStructure<br>readmeContent: String? | List<String> | 生成部署命令 | 24 |
| `MCPCommandGenerator.findSpecificPipInstallCommand` | `MCPCommandGenerator` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPCommandGenerator.kt` | readmeContent: String | String? | 从README内容中查找特定的pip安装命令 | 168 |
| `MCPCommandGenerator.extractPackageNameFromDirectory` | `MCPCommandGenerator` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPCommandGenerator.kt` | projectStructure: ProjectStructure | String? | 从目录名提取可能的包名 | 196 |
| `MCPCommandGenerator.convertNpmScriptToDirectCommand` | `MCPCommandGenerator` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPCommandGenerator.kt` | scriptContent: String | String | 将npm脚本转换为直接命令 | 221 |
| `MCPCommandGenerator.processIndividualCommand` | `MCPCommandGenerator` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPCommandGenerator.kt` | command: String | String | 处理单个命令 | 235 |
| `MCPConfigGenerator.generateMcpConfig` | `MCPConfigGenerator` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPConfigGenerator.kt` | pluginId: String<br>projectStructure: ProjectStructure<br>environmentVariables: Map<String, String>?<br>pluginDirPath: String?? | String | 生成MCP配置 | 29 |
| `saveMcpConfig` | — | `com.ai.assistance.operit.data.mcp.plugins` | `MCPConfigGenerator.kt` | pluginId: String<br>config: String<br>serverPath: String | Boolean | 保存MCP配置到文件 | 261 |
| `extractServerNameFromConfig` | — | `com.ai.assistance.operit.data.mcp.plugins` | `MCPConfigGenerator.kt` | configJson: String | String? | 从配置文件中提取服务器名称 | 285 |
| `extractEnvironmentVariables` | — | `com.ai.assistance.operit.data.mcp.plugins` | `MCPConfigGenerator.kt` | configJson: String | Map<String, String> | 提取配置中的环境变量 | 304 |
| `MCPDeployer.getOrCreateSharedSession` | `MCPDeployer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` |  | String? | Get or create shared session | 35 |
| `MCPDeployer.DeploymentStatus.emitCommandOutput` | `DeploymentStatus` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` | output: String<br>statusCallback: (DeploymentStatus) -> Unit | Unit |  | 47 |
| `MCPDeployer.executeCommandWithStreaming` | `MCPDeployer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` | terminal: Terminal<br>sessionId: String<br>command: String<br>statusCallback: (DeploymentStatus) -> Unit | String? |  | 61 |
| `MCPDeployer.deployPluginWithCommands` | `MCPDeployer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` | pluginId: String<br>pluginPath: String<br>customCommands: List<String><br>environmentVariables: Map<String, String>?<br>statusCallback: (DeploymentStatus) -> Unit | Boolean | 部署MCP插件（使用自定义命令） | 94 |
| `MCPDeployer.getDeployCommands` | `MCPDeployer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` | pluginId: String<br>pluginPath: String | List<String> | 获取部署命令 - 在部署前调用，用于分析和生成命令 | 242 |
| `MCPDeployer.executeDeployCommands` | `MCPDeployer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` | pluginId: String<br>pluginPath: String<br>deployCommands: List<String><br>statusCallback: (DeploymentStatus) -> Unit<br>serverName: String? | Boolean | 执行部署命令（提取的公共方法） | 280 |
| `MCPDeployer.saveMCPConfigToLocalServer` | `MCPDeployer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPDeployer.kt` | mcpLocalServer: MCPLocalServer<br>pluginId: String<br>mcpConfigJson: String | Boolean | 将生成的MCP配置正确保存到MCPLocalServer | 455 |
| `MCPProjectAnalyzer.analyzeProjectStructure` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | pluginDir: File<br>readmeContent: String | ProjectStructure | 分析项目结构 | 31 |
| `MCPProjectAnalyzer.parseTsConfig` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | pluginDir: File | Triple<String?, String?, String?> | 解析tsconfig.json并提取outDir和rootDir配置 | 166 |
| `MCPProjectAnalyzer.parsePyprojectToml` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | pluginDir: File | String? | 解析 pyproject.toml 并提取 Python 包名 | 205 |
| `MCPProjectAnalyzer.findMainPythonModule` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | pluginDir: File<br>pythonFiles: Array<File>? | String? | 查找主Python模块 | 266 |
| `MCPProjectAnalyzer.findMainJsFile` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | pluginDir: File<br>jsFiles: Array<File>? | String? | 查找主JS文件 | 314 |
| `MCPProjectAnalyzer.findMainTsFile` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | pluginDir: File<br>tsFiles: Array<File>? | String? | 查找主TS文件 | 341 |
| `MCPProjectAnalyzer.extractConfigExample` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | readmeContent: String | String? | 从README中提取配置示例 | 428 |
| `MCPProjectAnalyzer.validateConfigExample` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | configExample: String?<br>projectType: ProjectType | String? | 验证配置示例是否可信 | 451 |
| `MCPProjectAnalyzer.findReadmeFile` | `MCPProjectAnalyzer` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPProjectAnalyzer.kt` | pluginDir: File | File? | 查找README文件 | 476 |
| `MCPSharedSession.getOrCreateSharedSession` | `MCPSharedSession` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPSharedSession.kt` | context: Context | String? | 获取或创建共享的终端会话 | 30 |
| `MCPSharedSession.getCurrentSessionId` | `MCPSharedSession` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPSharedSession.kt` |  | String? | 获取当前共享会话ID（如果存在） | 63 |
| `MCPSharedSession.clearSession` | `MCPSharedSession` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPSharedSession.kt` |  | Unit | 清除共享会话引用 注意：这不会实际关闭会话，只是清除引用 | 69 |
| `MCPSharedSession.hasActiveSession` | `MCPSharedSession` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPSharedSession.kt` |  | Boolean | 检查共享会话是否存在 | 79 |
| `MCPStarter.PluginStartProgressListener.onPluginStarting` | `PluginStartProgressListener` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginId: String<br>index: Int<br>total: Int | Unit |  | 52 |
| `MCPStarter.PluginStartProgressListener.onPluginRegistered` | `PluginStartProgressListener` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginId: String<br>serviceName: String<br>success: Boolean | Unit |  | 53 |
| `MCPStarter.PluginStartProgressListener.onPluginStarted` | `PluginStartProgressListener` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginId: String<br>success: Boolean<br>index: Int<br>total: Int<br>failureDetail: String?? | Unit |  | 58 |
| `MCPStarter.PluginStartProgressListener.onPluginLog` | `PluginStartProgressListener` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginId: String<br>message: String | Unit |  | 65 |
| `MCPStarter.PluginStartProgressListener.onAllPluginsStarted` | `PluginStartProgressListener` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | successCount: Int<br>totalCount: Int<br>status: PluginInitStatus? | Unit |  | 66 |
| `MCPStarter.PluginStartProgressListener.onAllPluginsVerified` | `PluginStartProgressListener` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | verificationResults: List<VerificationResult> | Unit |  | 73 |
| `MCPStarter.getOrCreateSharedSession` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` |  | String? | Get or create shared session | 77 |
| `MCPStarter.isPnpmInstalled` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` |  | Boolean | Check if pnpm is installed in terminal | 82 |
| `MCPStarter.isTerminalServiceConnected` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` |  | Boolean | Check if terminal service is connected and initialized | 104 |
| `MCPStarter.requiresPnpmForPlugins` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginIds: List<String> | Boolean | True when bringing these local plugins up needs pnpm. Only two cases need it: `npx` servi… | 117 |
| `MCPStarter.bridgeFailureStatus` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginIds: List<String> | PluginInitStatus | Maps a failed bridge initialization to the status the loading UI reports. | 133 |
| `MCPStarter.initBridge` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | requirePnpm: Boolean | Boolean | Initialize and start the bridge | 144 |
| `MCPStarter.startPlugin` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginId: String<br>statusCallback: (StartStatus) -> Unit | Boolean | Start a plugin using the bridge | 195 |
| `MCPStarter.summarizeEnvKeys` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | env: Map<String, String>? | String |  | 199 |
| `MCPStarter.startPluginInternal` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginId: String<br>statusCallback: (StartStatus) -> Unit<br>initBridgeFirst: Boolean | Boolean | Internal plugin start logic | 208 |
| `MCPStarter.startAllDeployedPlugins` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | progressListener: PluginStartProgressListener? | Unit | Start all deployed plugins | 443 |
| `MCPStarter.processPlugin` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginId: String<br>serviceName: String<br>mcpRepository: MCPRepository<br>progressListener: PluginStartProgressListener | VerificationResult |  | 593 |
| `MCPStarter.registerPlugin` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginId: String<br>progressListener: PluginStartProgressListener?? | PluginRegistration |  | 651 |
| `MCPStarter.verifyPlugins` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | progressListener: PluginStartProgressListener | Unit | Verify plugin statuses | 808 |
| `MCPStarter.cacheToolsFromService` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | pluginId: String | Unit | 从服务缓存工具列表 | 831 |
| `MCPStarter.registerToolsForVerifiedPlugins` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | results: List<VerificationResult> | Unit | 为验证成功的插件注册工具 这确保只有真正就绪并响应的插件才会注册其工具 | 867 |
| `MCPStarter.generateMissingDescriptions` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | results: List<VerificationResult> | Unit | 为没有描述的工具包自动生成描述 | 892 |
| `MCPStarter.verifyAllMcpPlugins` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` |  | List<VerificationResult> | Verify all MCP plugins | 949 |
| `MCPStarter.extractServerNameFromConfig` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | configJson: String | String? | Extract server name from config | 1012 |
| `MCPStarter.parseConfigJson` | `MCPStarter` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPStarter.kt` | configJson: String | MCPLocalServer.MCPConfig? | Parse config JSON to MCPConfig | 1026 |
| `RemoteMcpRuntimeSession.connect` | `RemoteMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` |  | Boolean |  | 55 |
| `RemoteMcpRuntimeSession.isConnected` | `RemoteMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` |  | Boolean |  | 95 |
| `RemoteMcpRuntimeSession.getLastFailureDetail` | `RemoteMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` |  | String? |  | 97 |
| `RemoteMcpRuntimeSession.isActive` | `RemoteMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` |  | Boolean |  | 99 |
| `RemoteMcpRuntimeSession.listTools` | `RemoteMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` |  | List<McpRuntimeTool> |  | 101 |
| `RemoteMcpRuntimeSession.callTool` | `RemoteMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` | name: String<br>arguments: Map<String, Any?> | McpRuntimeCallResult |  | 117 |
| `RemoteMcpRuntimeSession.close` | `RemoteMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` |  | Unit |  | 136 |
| `RemoteMcpRuntimeSession.requireClient` | `RemoteMcpRuntimeSession` | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` |  | Client |  | 150 |
| `toRuntimeTool` | — | `com.ai.assistance.operit.data.mcp.plugins` | `RemoteMcpRuntimeSession.kt` |  | McpRuntimeTool |  | 165 |
| `DownloadState.MnnModelDownloadManager.getInstance` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | context: Context | MnnModelDownloadManager |  | 102 |
| `DownloadState.MnnModelDownloadManager.loadPersistentStates` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` |  | Unit |  | 144 |
| `DownloadState.MnnModelDownloadManager.savePersistentStates` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` |  | Unit |  | 198 |
| `DownloadState.MnnModelDownloadManager.addPersistentState` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | state: PersistentDownloadState | Unit |  | 219 |
| `DownloadState.MnnModelDownloadManager.removePersistentState` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String | Unit |  | 224 |
| `DownloadState.MnnModelDownloadManager.getDownloadState` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String | StateFlow<DownloadState> |  | 231 |
| `DownloadState.MnnModelDownloadManager.fetchModelList` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` |  | Result<List<MnnModel>> |  | 242 |
| `DownloadState.MnnModelDownloadManager.saveToCache` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | jsonString: String | Unit |  | 262 |
| `DownloadState.MnnModelDownloadManager.loadFromCache` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` |  | Result<List<MnnModel>> |  | 270 |
| `DownloadState.MnnModelDownloadManager.fetchRepoFiles` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelScopeId: String | Result<List<MsFileInfo>> | 获取 ModelScope 仓库的文件列表 参考: MsApiService.java:11-15 | 289 |
| `DownloadState.MnnModelDownloadManager.downloadModel` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String<br>url: String | Unit |  | 342 |
| `DownloadState.MnnModelDownloadManager.pauseDownload` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String | Unit |  | 563 |
| `DownloadState.MnnModelDownloadManager.cancelDownload` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String | Unit |  | 567 |
| `DownloadState.MnnModelDownloadManager.deleteModel` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String | Boolean |  | 573 |
| `DownloadState.MnnModelDownloadManager.getDownloadedModels` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` |  | List<File> |  | 598 |
| `DownloadState.MnnModelDownloadManager.isModelDownloaded` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String | Boolean |  | 605 |
| `DownloadState.MnnModelDownloadManager.updateDownloadState` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String<br>state: DownloadState | Unit |  | 612 |
| `DownloadState.MnnModelDownloadManager.getFileName` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String | String |  | 617 |
| `DownloadState.MnnModelDownloadManager.formatSpeed` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | bytesPerSecond: Double | String |  | 621 |
| `DownloadState.MnnModelDownloadManager.formatFileSize` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | bytes: Long | String |  | 629 |
| `DownloadState.MnnModelDownloadManager.getLastFileName` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | path: String | String |  | 638 |
| `DownloadState.MnnModelDownloadManager.downloadAllFiles` | `MnnModelDownloadManager` | `com.ai.assistance.operit.data.mnn` | `MnnModelDownloadManager.kt` | modelName: String<br>repositoryPath: String<br>files: List<MsFileInfo><br>modelFolder: File | Result<File> | 下载仓库中的所有文件到模型文件夹 参考 MsModelDownloader.kt:162-219 | 648 |
| `PreferencesHealthManager.CopyValidation.inspect` | `CopyValidation` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context | Report |  | 104 |
| `PreferencesHealthManager.repair` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context | RepairResult |  | 111 |
| `PreferencesHealthManager.inspectLocked` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context | Report |  | 158 |
| `PreferencesHealthManager.report` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context<br>checks: List<CheckItem><br>repairableFileNames: List<String><br>hasBlockingFailure: Boolean<br>hasRepairableIssue: Boolean | Report |  | 296 |
| `PreferencesHealthManager.summaryFor` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context<br>status: Status | String |  | 318 |
| `PreferencesHealthManager.validateCopy` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context<br>source: File | CopyValidation |  | 326 |
| `PreferencesHealthManager.inspectDomainIssues` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | source: File<br>preferences: Preferences | List<DomainIssue> |  | 354 |
| `PreferencesHealthManager.shouldInspectStructuredJsonValue` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | value: String | Boolean |  | 374 |
| `PreferencesHealthManager.resolveRepairSources` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context<br>fileNames: List<String> | List<File> |  | 379 |
| `PreferencesHealthManager.preserveConfigurationFiles` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | sources: List<File> | File |  | 399 |
| `PreferencesHealthManager.preferencesDirectory` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context | File |  | 430 |
| `PreferencesHealthManager.hasExpectedPath` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | file: File<br>directory: File | Boolean |  | 433 |
| `PreferencesHealthManager.mainProcessState` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context | MainProcessState |  | 439 |
| `PreferencesHealthManager.requireMainProcessStopped` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | context: Context | Unit |  | 455 |
| `RoomDatabaseHealthManager.inspect` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context | Report |  | 86 |
| `RoomDatabaseHealthManager.repair` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context | RepairResult |  | 93 |
| `RoomDatabaseHealthManager.inspectLocked` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context | Report |  | 127 |
| `RoomDatabaseHealthManager.failureReport` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context<br>databaseFile: File<br>checks: List<CheckItem> | Report |  | 502 |
| `RoomDatabaseHealthManager.summaryFor` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context<br>status: Status | String |  | 515 |
| `RoomDatabaseHealthManager.readQuickCheck` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | database: SQLiteDatabase | List<String> |  | 524 |
| `RoomDatabaseHealthManager.readUserVersion` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | database: SQLiteDatabase | Int |  | 534 |
| `RoomDatabaseHealthManager.countForeignKeyViolations` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | database: SQLiteDatabase | Int |  | 541 |
| `RoomDatabaseHealthManager.isIndexOnlyQuickCheckFailure` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | messages: List<String> | Boolean |  | 551 |
| `RoomDatabaseHealthManager.rebuildIndexes` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context | Unit |  | 564 |
| `RoomDatabaseHealthManager.runRoomMigrations` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context | Unit |  | 581 |
| `RoomDatabaseHealthManager.preserveDatabaseFiles` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context | File |  | 590 |
| `RoomDatabaseHealthManager.databaseFiles` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | databaseFile: File | List<File> |  | 633 |
| `RoomDatabaseHealthManager.hasExpectedDatabasePath` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | file: File<br>expectedName: String | Boolean |  | 641 |
| `RoomDatabaseHealthManager.mainProcessState` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context | MainProcessState |  | 647 |
| `RoomDatabaseHealthManager.requireMainProcessStopped` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | context: Context | Unit |  | 663 |
| `RoomDatabaseHealthManager.PreservingCorruptionHandler.onCorruption` | `PreservingCorruptionHandler` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | database: SQLiteDatabase | Unit |  | 681 |
| `PluginDenylistRepository.refreshFromRemote` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` |  | Boolean |  | 59 |
| `PluginDenylistRepository.findDeniedImport` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | file: File | PluginDenylistEntry? |  | 76 |
| `PluginDenylistRepository.cacheSignature` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` |  | String |  | 88 |
| `PluginDenylistRepository.readCachedPayload` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` |  | PluginDenylistPayload? |  | 103 |
| `PluginDenylistRepository.writeCachedPayload` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | bytes: ByteArray | Unit |  | 117 |
| `PluginDenylistRepository.validatePointer` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | pointer: PluginDenylistPointer | Unit |  | 135 |
| `PluginDenylistRepository.validatePayload` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | pointer: PluginDenylistPointer?<br>payload: PluginDenylistPayload | Unit |  | 141 |
| `PluginDenylistRepository.fetchText` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | url: String | String |  | 158 |
| `PluginDenylistRepository.resolveUrl` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | latestFile: String | String |  | 173 |
| `PluginDenylistRepository.addCacheBust` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | url: String | String |  | 180 |
| `PluginDenylistRepository.cacheFile` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` |  | File |  | 185 |
| `PluginDenylistRepository.atomicBackupFile` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | file: File | File |  | 187 |
| `PluginDenylistRepository.sha256Hex` | `PluginDenylistRepository` | `com.ai.assistance.operit.data.security` | `PluginDenylistRepository.kt` | file: File | String |  | 189 |
| `SkillRepository.getInstance` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | context: Context | SkillRepository |  | 35 |
| `SkillRepository.getSkillsDirectoryPath` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` |  | String |  | 55 |
| `SkillRepository.getAvailableSkillPackages` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` |  | Map<String, SkillPackage> |  | 57 |
| `SkillRepository.getAvailableSkillPackagesSnapshot` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` |  | Pair<Map<String, SkillPackage>, Map<String, String>> |  | 59 |
| `SkillRepository.getSkillLoadErrors` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` |  | Map<String, String> |  | 62 |
| `SkillRepository.getAiVisibleSkillPackages` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` |  | Map<String, SkillPackage> |  | 64 |
| `SkillRepository.readSkillContent` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | skillName: String | String? |  | 70 |
| `SkillRepository.deleteSkill` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | skillName: String | Boolean |  | 72 |
| `SkillRepository.importSkillFromZip` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | zipFile: File | String |  | 74 |
| `SkillRepository.importSkillFromGitHubRepo` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | repoUrl: String | String |  | 80 |
| `SkillRepository.importSkillFromGitHubRepoDetailed` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | repoUrl: String | SkillRepoImportResult |  | 89 |
| `SkillRepository.importSkillFromDirectInput` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | skillId: String<br>description: String<br>content: String<br>attachmentUris: List<Uri>? | String |  | 144 |
| `SkillRepository.buildDirectSkillMarkdown` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | skillId: String<br>description: String<br>content: String | String |  | 237 |
| `SkillRepository.escapeFrontMatterValue` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | value: String | String |  | 251 |
| `SkillRepository.resolveAttachmentDisplayName` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | uri: Uri | String? |  | 259 |
| `SkillRepository.sanitizeAttachmentName` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | rawName: String | String |  | 278 |
| `SkillRepository.isValidSkillId` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | skillId: String | Boolean |  | 283 |
| `SkillRepository.ensureUniqueFileName` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | baseName: String<br>usedNames: MutableSet<String> | String |  | 287 |
| `SkillRepository.parseGitHubSkillTarget` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | inputUrlRaw: String | GitHubSkillTarget? |  | 301 |
| `SkillRepository.cleanRepoName` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | repoRaw: String | String |  | 323 |
| `SkillRepository.encodePathSegment` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | value: String | String |  | 373 |
| `SkillRepository.downloadFromUrl` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | zipUrl: String<br>outFile: File | Boolean |  | 381 |
| `SkillRepository.getGithubDefaultBranch` | `SkillRepository` | `com.ai.assistance.operit.data.skill` | `SkillRepository.kt` | owner: String<br>repoName: String | String? |  | 414 |
| `FullUpdateInstaller.downloadAndPrepareUpdate` | `FullUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | context: Context<br>apkUrl: String<br>sourceKeys: List<String><br>downloadMessage: String<br>readyMessage: String<br>expectedSha256: String??<br>expectedSize: Long??<br>onEvent: (ProgressEvent) -> Unit | File |  | 55 |
| `FullUpdateInstaller.resolveSources` | `FullUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | apkUrl: String<br>sourceKeys: List<String> | List<SourceCandidate> | Map the ordered source keys onto concrete URLs. Keys come from [GithubReleaseUtil.getDown… | 121 |
| `FullUpdateInstaller.prepareCleanWorkDir` | `FullUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `FullUpdateInstaller.kt` | context: Context | File |  | 126 |
| `PatchUpdateInstaller.installApk` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | context: Context<br>apkFile: File | Unit |  | 112 |
| `PatchUpdateInstaller.downloadAndPreparePatchUpdate` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | context: Context<br>patchUrl: String<br>metaUrl: String<br>sourceKeys: List<String><br>metaSha256: String??<br>patchSha256: String??<br>onEvent: (ProgressEvent) -> Unit | File | Download and apply a patch chain. [sourceKeys] is the ordered candidate list produced by … | 146 |
| `PatchUpdateInstaller.resolvePatchChain` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | context: Context<br>patchUrl: String<br>metaUrl: String<br>currentBaseSha: String<br>targetMeta: JSONObject<br>targetMetaSha256: String?<br>targetPatchSha256: String?<br>onEvent: (ProgressEvent) -> Unit | List<PatchStep> |  | 337 |
| `PatchUpdateInstaller.parsePatchStep` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | meta: JSONObject<br>patchUrl: String<br>metaUrl: String<br>tag: String<br>metaAssetSha256: String?<br>patchAssetSha256: String? | PatchStep? |  | 473 |
| `PatchUpdateInstaller.parseRepoFromReleaseAssetUrl` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | url: String | Pair<String, String>? |  | 509 |
| `PatchUpdateInstaller.parseReleaseBodyAsPatchMeta` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | body: String? | JSONObject? |  | 514 |
| `PatchUpdateInstaller.cleanupPatchWorkDir` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | workDir: File<br>keepFile: File | Unit |  | 527 |
| `PatchUpdateInstaller.prepareCleanWorkDir` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | context: Context | File |  | 546 |
| `PatchUpdateInstaller.resolveSources` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | originalUrl: String<br>sourceKeys: List<String> | List<SourceCandidate> | Map ordered source keys onto concrete URLs for [originalUrl]. Keys come from [GithubRelea… | 562 |
| `PatchUpdateInstaller.downloadWithFailover` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | sources: List<SourceCandidate><br>out: File<br>label: String<br>expectedSha256: String??<br>multiThread: Boolean<br>onEvent: (ProgressEvent) -> Unit | Unit | Fetch one artifact through the ordered source list, verifying it. A source is dropped for… | 573 |
| `PatchUpdateInstaller.applyApkrawPatch` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | baseApk: File<br>patchZip: File<br>meta: JSONObject<br>outApk: File | Unit |  | 620 |
| `PatchUpdateInstaller.readCentralDirectory` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | raf: RandomAccessFile | Map<String, CdEntry> |  | 671 |
| `PatchUpdateInstaller.copyLocalRecord` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | raf: RandomAccessFile<br>cd: CdEntry<br>out: java.io.OutputStream | Unit |  | 730 |
| `PatchUpdateInstaller.copyBytes` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | raf: RandomAccessFile<br>out: java.io.OutputStream<br>count: Long | Unit |  | 769 |
| `PatchUpdateInstaller.sha256Hex` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | file: File | String |  | 781 |
| `PatchUpdateInstaller.readUShortLE` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | buf: ByteArray<br>off: Int | Int |  | 794 |
| `PatchUpdateInstaller.readUIntLE` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | buf: ByteArray<br>off: Int | Long |  | 798 |
| `RankedSources.remaining` | `RankedSources` | `com.ai.assistance.operit.data.updates` | `UpdateDownloadSource.kt` | failedKeys: Set<String> | List<SourceCandidate> | Sources still worth trying, in order, minus the ones that already failed during this upda… | 39 |
| `RankedSources.prioritized` | `RankedSources` | `com.ai.assistance.operit.data.updates` | `UpdateDownloadSource.kt` | preferredKey: String<br>failedKeys: Set<String> | List<SourceCandidate> | Same list with [preferredKey] moved to the front, used when the user picks a source by ha… | 49 |
| `UpdateSourceRanking.rank` | `UpdateSourceRanking` | `com.ai.assistance.operit.data.updates` | `UpdateDownloadSource.kt` | candidates: Collection<SourceCandidate> | RankedSources |  | 70 |
| `UpdateSourceRanking.failureLines` | `UpdateSourceRanking` | `com.ai.assistance.operit.data.updates` | `UpdateDownloadSource.kt` | rejected: List<SourceCandidate><br>downloadFailures: Map<String, String> | List<String> | Per-source failure lines for the "could not download" message: probe rejections first, th… | 82 |
| `UpdateStatus.UpdateManager.getInstance` | `UpdateManager` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | context: Context | UpdateManager |  | 57 |
| `UpdateStatus.UpdateManager.parseVersion` | `UpdateManager` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | v: String | ParsedVersion |  | 78 |
| `UpdateStatus.UpdateManager.compareVersions` | `UpdateManager` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | v1: String<br>v2: String | Int |  | 93 |
| `UpdateStatus.UpdateManager.checkForUpdates` | `UpdateManager` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | context: Context<br>currentVersion: String | UpdateStatus | 检查更新，返回更新状态 用于从MainActivity直接检查更新 | 104 |
| `UpdateStatus.UpdateManager.checkForUpdatesSilently` | `UpdateManager` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | currentVersion: String | Unit |  | 110 |
| `UpdateStatus.UpdateManager.checkForUpdates` | `UpdateManager` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | currentVersion: String | Unit | 开始更新检查流程 | 124 |
| `UpdateStatus.UpdateManager.checkForUpdatesInternal` | `UpdateManager` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | currentVersion: String | UpdateStatus | 检查更新的内部实现 | 139 |
| `UpdateStatus.UpdateManager.tryFetchLatestPatchUpdate` | `UpdateManager` | `com.ai.assistance.operit.data.updates` | `UpdateManager.kt` | currentVersion: String | UpdateStatus? |  | 231 |
| `UpdateSourceDownloader.SourceFailure.download` | `SourceFailure` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | sources: List<SourceCandidate><br>out: File<br>expectedSha256: String??<br>expectedSize: Long??<br>multiThread: Boolean?<br>onAttempt: (attempt: Int, total: Int, source: …?<br>onSourceFailed: (attempt: Int, total: Int, source: …?<br>onProg… | Outcome | Download [sources] in order into [out], verifying the result. | 71 |
| `UpdateSourceDownloader.describeFailure` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | e: Throwable | String |  | 120 |
| `UpdateSourceDownloader.verifyArtifact` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | file: File<br>sourceKey: String<br>expectedSha256: String?<br>expectedSize: Long? | Unit |  | 125 |
| `UpdateSourceDownloader.sha256Hex` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | file: File | String |  | 150 |
| `UpdateSourceDownloader.transfer` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | source: SourceCandidate<br>out: File<br>multiThread: Boolean<br>onProgress: (Progress) -> Unit | Unit |  | 163 |
| `UpdateSourceDownloader.transferSequential` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | source: SourceCandidate<br>out: File<br>onProgress: (Progress) -> Unit | Unit |  | 181 |
| `UpdateSourceDownloader.transferRanged` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | source: SourceCandidate<br>out: File<br>onProgress: (Progress) -> Unit | Unit |  | 240 |
| `UpdateSourceDownloader.fetchContentLength` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | url: String | Long |  | 300 |
| `UpdateSourceDownloader.verifyRangeSupported` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | url: String | Unit |  | 315 |
| `UpdateSourceDownloader.splitRanges` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | totalBytes: Long<br>threadCount: Int | List<Pair<Long, Long>> |  | 327 |
| `UpdateSourceDownloader.downloadRange` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | url: String<br>out: File<br>start: Long<br>end: Long<br>downloadedBytes: AtomicLong | Unit |  | 343 |
| `CodexOAuthTokenResponseTest.completeTokenResponseIsAccepted` | `CodexOAuthTokenResponseTest` | `com.ai.assistance.operit.data.api` | `CodexOAuthTokenResponseTest.kt` |  | Unit |  | 8 ⚑ |
| `CodexOAuthTokenResponseTest.missingRefreshTokenIsRejected` | `CodexOAuthTokenResponseTest` | `com.ai.assistance.operit.data.api` | `CodexOAuthTokenResponseTest.kt` |  | Unit |  | 20 ⚑ |
| `CodexUsageClientTest.parsesPlanAndRollingWindows` | `CodexUsageClientTest` | `com.ai.assistance.operit.data.api` | `CodexUsageClientTest.kt` |  | Unit |  | 17 ⚑ |
| `CodexUsageClientTest.classifiesSevenDayWindowFromPrimarySlot` | `CodexUsageClientTest` | `com.ai.assistance.operit.data.api` | `CodexUsageClientTest.kt` |  | Unit |  | 46 ⚑ |
| `CodexUsageClientTest.persistedSnapshotRoundTripsWithoutTokenData` | `CodexUsageClientTest` | `com.ai.assistance.operit.data.api` | `CodexUsageClientTest.kt` |  | Unit |  | 68 ⚑ |
| `RawSnapshotBackupManagerTest.snapshotPackageName_acceptsOperitPackagePrefix` | `RawSnapshotBackupManagerTest` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManagerTest.kt` |  | Unit |  | 10 ⚑ |
| `RawSnapshotBackupManagerTest.snapshotPackageName_rejectsDifferentPackagePrefix` | `RawSnapshotBackupManagerTest` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManagerTest.kt` |  | Unit |  | 17 ⚑ |
| `ChatContentDaoNulContentTest.setUp` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 38 ⚑ |
| `ChatContentDaoNulContentTest.tearDown` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 59 ⚑ |
| `ChatContentDaoNulContentTest.shortMessageWithNulIsRestoredCompletely` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 65 ⚑ |
| `ChatContentDaoNulContentTest.emptyContentIsRestoredAsEmptyString` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 77 ⚑ |
| `ChatContentDaoNulContentTest.messageWithLeadingAndMultipleNulCharactersIsRestoredCompletely` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 84 ⚑ |
| `ChatContentDaoNulContentTest.longMessageWithNulAndMultibyteCharacterAcrossChunkBoundaryIsRestoredCompletely` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 95 ⚑ |
| `ChatContentDaoNulContentTest.alternativesReadPathsAlsoRestoreNulContent` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 118 ⚑ |
| `ChatContentDaoNulContentTest.longMessageWithoutNulStillUsesChunkedRead` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 136 ⚑ |
| `ChatContentDaoNulContentTest.shortVariantWithNulIsRestoredCompletely` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 147 ⚑ |
| `ChatContentDaoNulContentTest.longVariantWithNulAcrossChunkBoundariesIsRestoredCompletely` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 174 ⚑ |
| `ChatContentDaoNulContentTest.selectedVariantContentIsRestoredCompletelyForHistoryHydration` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` |  | Unit |  | 204 ⚑ |
| `ChatContentDaoNulContentTest.insertMessage` | `ChatContentDaoNulContentTest` | `com.ai.assistance.operit.data.dao` | `ChatContentDaoNulContentTest.kt` | timestamp: Long<br>orderIndex: Int<br>content: String<br>selectedVariantIndex: Int? | Unit |  | 224 ⚑ |
| `AppDatabaseMigrationTest.migration20To21CreatesMessageIndexesExpectedByRoom` | `AppDatabaseMigrationTest` | `com.ai.assistance.operit.data.db` | `AppDatabaseMigrationTest.kt` |  | Unit |  | 11 ⚑ |
| `AppDatabaseMigrationTest.recordingDatabase` | `AppDatabaseMigrationTest` | `com.ai.assistance.operit.data.db` | `AppDatabaseMigrationTest.kt` | executedSql: MutableList<String> | SupportSQLiteDatabase |  | 27 ⚑ |
| `AppDatabaseMigrationTest.assertSqlWasExecuted` | `AppDatabaseMigrationTest` | `com.ai.assistance.operit.data.db` | `AppDatabaseMigrationTest.kt` | normalizedSql: List<String><br>expectedSql: String | Unit |  | 52 ⚑ |
| `JdbcSQLiteDriver.open` | `JdbcSQLiteDriver` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | fileName: String | SQLiteConnection |  | 35 ⚑ |
| `JdbcSQLiteConnection.prepare` | `JdbcSQLiteConnection` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | sql: String | SQLiteStatement |  | 48 ⚑ |
| `JdbcSQLiteConnection.inTransaction` | `JdbcSQLiteConnection` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Boolean |  | 68 ⚑ |
| `JdbcSQLiteConnection.close` | `JdbcSQLiteConnection` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Unit |  | 70 ⚑ |
| `JdbcSQLiteConnection.executeRawSql` | `JdbcSQLiteConnection` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | sql: String | Unit |  | 74 ⚑ |
| `JdbcSQLiteConnection.beginJdbcTransaction` | `JdbcSQLiteConnection` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Unit |  | 82 ⚑ |
| `JdbcSQLiteConnection.endJdbcTransaction` | `JdbcSQLiteConnection` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | commit: Boolean | Unit |  | 88 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.bindBlob` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int<br>value: ByteArray | Unit |  | 95 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.bindDouble` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int<br>value: Double | Unit |  | 96 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.bindLong` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int<br>value: Long | Unit |  | 97 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.bindText` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int<br>value: String | Unit |  | 98 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.bindNull` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Unit |  | 99 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.getBlob` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | ByteArray |  | 100 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.getDouble` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Double |  | 101 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.getLong` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Long |  | 102 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.getText` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | String |  | 103 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.isNull` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Boolean |  | 104 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.getColumnCount` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Int |  | 105 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.getColumnName` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | String |  | 106 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.getColumnType` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Int |  | 107 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.step` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Boolean |  | 108 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.reset` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Unit |  | 112 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.clearBindings` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Unit |  | 113 ⚑ |
| `JdbcSQLiteConnection.TransactionStatement.close` | `TransactionStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Unit |  | 114 ⚑ |
| `JdbcSQLiteStatement.bindBlob` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int<br>value: ByteArray | Unit |  | 125 ⚑ |
| `JdbcSQLiteStatement.bindDouble` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int<br>value: Double | Unit |  | 127 ⚑ |
| `JdbcSQLiteStatement.bindLong` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int<br>value: Long | Unit |  | 129 ⚑ |
| `JdbcSQLiteStatement.bindText` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int<br>value: String | Unit |  | 131 ⚑ |
| `JdbcSQLiteStatement.bindNull` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Unit |  | 133 ⚑ |
| `JdbcSQLiteStatement.getBlob` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | ByteArray |  | 135 ⚑ |
| `JdbcSQLiteStatement.getDouble` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Double |  | 137 ⚑ |
| `JdbcSQLiteStatement.getLong` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Long |  | 139 ⚑ |
| `JdbcSQLiteStatement.getText` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | String |  | 141 ⚑ |
| `JdbcSQLiteStatement.isNull` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Boolean |  | 143 ⚑ |
| `JdbcSQLiteStatement.getColumnCount` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Int |  | 145 ⚑ |
| `JdbcSQLiteStatement.getColumnName` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | String |  | 147 ⚑ |
| `JdbcSQLiteStatement.getColumnType` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` | index: Int | Int |  | 150 ⚑ |
| `JdbcSQLiteStatement.step` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Boolean |  | 166 ⚑ |
| `JdbcSQLiteStatement.ensureExecuted` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Unit | 尽早执行查询：Room 生成的代码在 step() 之前先取列元数据 （getColumnIndexOrThrow），而 sqlite-jdbc 的 PreparedStatem… | 177 ⚑ |
| `JdbcSQLiteStatement.reset` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Unit |  | 195 ⚑ |
| `JdbcSQLiteStatement.clearBindings` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Unit |  | 201 ⚑ |
| `JdbcSQLiteStatement.close` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | Unit |  | 205 ⚑ |
| `JdbcSQLiteStatement.resultSetOrThrow` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | ResultSet |  | 210 ⚑ |
| `JdbcSQLiteStatement.metadataOrNull` | `JdbcSQLiteStatement` | `com.ai.assistance.operit.data.db` | `JdbcSQLiteDriver.kt` |  | ResultSetMetaData? | 列元数据：已执行时直接用结果集元数据，未执行时先执行查询再取。 | 214 ⚑ |
| `McpConfigImportParserTest.parse_classifiesStdioAndRemoteTransports` | `McpConfigImportParserTest` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParserTest.kt` |  | Unit |  | 11 ⚑ |
| `McpConfigImportParserTest.parse_rejectsMissingTransportDeclaration` | `McpConfigImportParserTest` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParserTest.kt` |  | Unit |  | 55 ⚑ |
| `McpConfigImportParserTest.parse_rejectsAmbiguousStdioAndRemoteConfiguration` | `McpConfigImportParserTest` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParserTest.kt` |  | Unit |  | 69 ⚑ |
| `McpConfigImportParserTest.parse_readsStdioWorkingDirectory` | `McpConfigImportParserTest` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParserTest.kt` |  | Unit |  | 87 ⚑ |
| `McpConfigImportParserTest.parse_rejectsBlankStdioWorkingDirectory` | `McpConfigImportParserTest` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParserTest.kt` |  | Unit |  | 110 ⚑ |
| `McpConfigImportParserTest.assertParseFails` | `McpConfigImportParserTest` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParserTest.kt` | config: String | Unit |  | 127 ⚑ |
| `McpStdioConfigResolverTest.commandName_ignoresDirectoryAndCase` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 11 ⚑ |
| `McpStdioConfigResolverTest.isTerminalPath_acceptsLinuxFormsOnly` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 18 ⚑ |
| `McpStdioConfigResolverTest.appManagedRuntimePath_coversCopiedDirectory` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 28 ⚑ |
| `McpStdioConfigResolverTest.requiresAppManagedInstallation_skipsPackageRunners` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 35 ⚑ |
| `McpStdioConfigResolverTest.requiresAppManagedInstallation_relativeEntryNeedsDeployment` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 53 ⚑ |
| `McpStdioConfigResolverTest.requiresAppManagedInstallation_absoluteEntryIsSelfContained` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 64 ⚑ |
| `McpStdioConfigResolverTest.requiresAppManagedInstallation_explicitCwdIsSelfContained` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 75 ⚑ |
| `McpStdioConfigResolverTest.requiresAppManagedInstallation_cwdInsideAppManagedDirectoryStillDeploys` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 86 ⚑ |
| `McpStdioConfigResolverTest.requiresAppManagedInstallation_absoluteCommandWithoutRelativeEntryIsSelfContained` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 99 ⚑ |
| `McpStdioConfigResolverTest.requiresAppManagedInstallation_absoluteCommandWithRelativeEntryStillDeploys` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 111 ⚑ |
| `McpStdioConfigResolverTest.requiresAppManagedInstallation_appManagedAbsoluteArgsStillDeploy` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 124 ⚑ |
| `McpStdioConfigResolverTest.requiresAppManagedInstallation_inlineScriptKeepsDeployment` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 137 ⚑ |
| `McpStdioConfigResolverTest.resolveWorkingDirectory_prefersConfiguredCwd` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 150 ⚑ |
| `McpStdioConfigResolverTest.resolveWorkingDirectory_usesAbsoluteEntryParent` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 163 ⚑ |
| `McpStdioConfigResolverTest.resolveWorkingDirectory_usesAppManagedDirectoryForRelativeEntry` | `McpStdioConfigResolverTest` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolverTest.kt` |  | Unit |  | 176 ⚑ |
| `RoomDatabaseHealthManagerTest.indexEntryFailuresAreRepairable` | `RoomDatabaseHealthManagerTest` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManagerTest.kt` |  | Unit |  | 9 ⚑ |
| `RoomDatabaseHealthManagerTest.pageDamageIsNotClassifiedAsIndexOnly` | `RoomDatabaseHealthManagerTest` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManagerTest.kt` |  | Unit |  | 21 ⚑ |
| `RoomDatabaseHealthManagerTest.unrelatedFailureContainingIndexWordsIsNotRepairable` | `RoomDatabaseHealthManagerTest` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManagerTest.kt` |  | Unit |  | 30 ⚑ |
| `RoomDatabaseHealthManagerTest.successfulQuickCheckDoesNotRequestIndexRepair` | `RoomDatabaseHealthManagerTest` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManagerTest.kt` |  | Unit |  | 39 ⚑ |
| `UpdateSourceDownloaderTest.setUp` | `UpdateSourceDownloaderTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloaderTest.kt` |  | Unit |  | 29 ⚑ |
| `UpdateSourceDownloaderTest.tearDown` | `UpdateSourceDownloaderTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloaderTest.kt` |  | Unit |  | 38 ⚑ |
| `UpdateSourceDownloaderTest.source` | `UpdateSourceDownloaderTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloaderTest.kt` | key: String<br>path: String | Unit |  | 43 ⚑ |
| `UpdateSourceDownloaderTest.outFile` | `UpdateSourceDownloaderTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloaderTest.kt` | name: String? | Unit |  | 46 ⚑ |
| `UpdateSourceDownloaderTest.dispatch` | `UpdateSourceDownloaderTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloaderTest.kt` | request: RecordedRequest | MockResponse |  | 178 ⚑ |
| `UpdateSourceDownloaderTest.rangedDispatcher` | `UpdateSourceDownloaderTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloaderTest.kt` | payload: ByteArray | Unit | Serves whole bodies for plain GETs and byte slices for ranged requests. | 194 ⚑ |
| `UpdateSourceDownloaderTest.dispatch` | `UpdateSourceDownloaderTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloaderTest.kt` | request: RecordedRequest | MockResponse |  | 195 ⚑ |
| `UpdateSourceRankingTest.candidate` | `UpdateSourceRankingTest` | `com.ai.assistance.operit.data.updates` | `UpdateSourceRankingTest.kt` | key: String<br>speed: Long??<br>latency: Long??<br>error: String?? | Unit |  | 16 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ANNUAL_REPORT_SCHEMA_VERSION` | — | `com.ai.assistance.operit.data.annualreport` | `AnnualReportModels.kt` | inferred | 年度报告用户数据契约，与 annual-report/src/data/types.ts 一一对应，增删字段必须两侧同步。 口径见 docs/TODO/ann… | 9 |
| `ApiProviderConfigs.configs` | `ApiProviderConfigs` | `com.ai.assistance.operit.data.collects` | `ApiProviderConfigCollect.kt` | Map<ApiProviderType, ProviderApiConfig> |  | 20 |
| `APP_DATABASE_VERSION` | — | `com.ai.assistance.operit.data.db` | `AppDatabase.kt` | inferred |  | 25 |
| `ChatHistoryCsv.columnIndex` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | inferred |  | 73 |
| `ChatHistoryCsv.dateFormatter` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | inferred |  | 20 |
| `ChatHistoryCsv.FORMAT_VERSION` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | inferred |  | 15 |
| `ChatHistoryCsv.HEADER` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | List<String> |  | 22 |
| `ChatHistoryCsv.RECORD_CHAT` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | inferred |  | 16 |
| `ChatHistoryCsv.RECORD_MESSAGE` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | inferred |  | 17 |
| `ChatHistoryCsv.RECORD_VARIANT` | `ChatHistoryCsv` | `com.ai.assistance.operit.data.converter` | `ChatHistoryCsv.kt` | inferred |  | 18 |
| `CodexOAuthProtocol.CALLBACK_PATH` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | inferred |  | 51 |
| `CodexOAuthProtocol.CLIENT_ID` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | inferred |  | 45 |
| `CodexOAuthProtocol.CODEX_RESPONSES_ENDPOINT` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | inferred |  | 47 |
| `CodexOAuthProtocol.CODEX_USAGE_ENDPOINT` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | inferred |  | 48 |
| `CodexOAuthProtocol.ISSUER` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | inferred |  | 46 |
| `CodexOAuthProtocol.MODEL_CATALOG_ENDPOINT` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | inferred |  | 49 |
| `CodexOAuthProtocol.OAUTH_TIMEOUT_MILLIS` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | inferred |  | 52 |
| `CodexOAuthProtocol.PRIMARY_CALLBACK_PORT` | `CodexOAuthProtocol` | `com.ai.assistance.operit.data.api` | `CodexOAuthClient.kt` | inferred |  | 50 |
| `CONTENT_CHUNK_BYTE_COUNT` | — | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | inferred | SQLite 的 LENGTH/SUBSTR 把 TEXT 当字符处理，遇到第一个 U+0000 就截断；PDF 提取文本里的 NUL 会让消息被误判为只有前… | 13 |
| `DefaultModelPricingCollect.domesticProviders` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | inferred |  | 23 |
| `DefaultModelPricingCollect.providerFallbacks` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | inferred |  | 156 |
| `DefaultModelPricingCollect.scrapedModelDefaults` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | Map<String, ModelPricingDefaults> by lazy { |  | 145 |
| `DefaultModelPricingCollect.scrapedModelNameFallbacks` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | Map<String, List<ModelPricingDefaults>> by lazy { |  | 149 |
| `DefaultModelPricingCollect.scrapedPricingRows` | `DefaultModelPricingCollect` | `com.ai.assistance.operit.data.collects` | `ModelPricingDefaultsCollect.kt` | List<ScrapedPricingRow> by lazy { |  | 97 |
| `gson` | — | `com.ai.assistance.operit.data.mcp.plugins` | `MCPConfigGenerator.kt` | inferred | 使用格式化的JSON输出 | 249 |
| `HtmlExporter.CONTENT_PROGRESS_CHARACTER_COUNT` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | inferred |  | 17 |
| `HtmlExporter.dateFormatter` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | inferred |  | 18 |
| `HtmlExporter.HTML_CONTENT_WRITE_CHUNK_CHARACTER_COUNT` | `HtmlExporter` | `com.ai.assistance.operit.data.exporter` | `HtmlExporter.kt` | inferred |  | 16 |
| `MarkdownExporter.dateFormatter` | `MarkdownExporter` | `com.ai.assistance.operit.data.exporter` | `MarkdownExporter.kt` | inferred |  | 14 |
| `McpConfigImportParser.SSE_TYPE` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | inferred |  | 40 |
| `McpConfigImportParser.STDIO_TYPE` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | inferred |  | 41 |
| `McpConfigImportParser.STREAMABLE_HTTP_TYPE` | `McpConfigImportParser` | `com.ai.assistance.operit.data.mcp` | `McpConfigImportParser.kt` | inferred |  | 39 |
| `MCPSharedSession.mutex` | `MCPSharedSession` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPSharedSession.kt` | inferred |  | 22 |
| `MCPSharedSession.SESSION_NAME` | `MCPSharedSession` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPSharedSession.kt` | inferred |  | 18 |
| `MCPSharedSession.sharedSessionId` | `MCPSharedSession` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPSharedSession.kt` | String? |  | 21 |
| `MCPSharedSession.TAG` | `MCPSharedSession` | `com.ai.assistance.operit.data.mcp.plugins` | `MCPSharedSession.kt` | inferred |  | 17 |
| `McpStdioConfigResolver.APP_MANAGED_PREFIX` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | inferred |  | 17 |
| `McpStdioConfigResolver.EVAL_FLAGS` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | inferred |  | 16 |
| `McpStdioConfigResolver.PACKAGE_RUNNER_COMMANDS` | `McpStdioConfigResolver` | `com.ai.assistance.operit.data.mcp` | `McpStdioConfigResolver.kt` | inferred |  | 15 |
| `MESSAGE_CONTENT_ROW_QUERY` | — | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | inferred |  | 15 |
| `MESSAGE_VARIANT_CONTENT_ROW_QUERY` | — | `com.ai.assistance.operit.data.dao` | `ChatContentDao.kt` | inferred |  | 45 |
| `ModelThinkingConfigDefaults.DEFAULT_JSON` | `ModelThinkingConfigDefaults` | `com.ai.assistance.operit.data.collects` | `ModelThinkingConfigDefaultsCollect.kt` | String |  | 8 |
| `ObjectBoxManager.storeLock` | `ObjectBoxManager` | `com.ai.assistance.operit.data.db` | `ObjectBox.kt` | inferred |  | 11 |
| `ObjectBoxManager.stores` | `ObjectBoxManager` | `com.ai.assistance.operit.data.db` | `ObjectBox.kt` | inferred |  | 10 |
| `PatchUpdateInstaller.MAX_CHAIN_STEPS` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | inferred |  | 29 |
| `PatchUpdateInstaller.TAG` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | inferred |  | 28 |
| `PatchUpdateInstaller.WORK_DIR_NAME` | `PatchUpdateInstaller` | `com.ai.assistance.operit.data.updates` | `PatchUpdateInstaller.kt` | inferred |  | 84 |
| `PreferencesHealthManager.domainJson` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | inferred |  | 39 |
| `PreferencesHealthManager.operationMutex` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | inferred |  | 38 |
| `PreferencesHealthManager.PREFERENCES_SUFFIX` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | inferred |  | 37 |
| `PreferencesHealthManager.TAG` | `PreferencesHealthManager` | `com.ai.assistance.operit.data.recovery` | `PreferencesHealthManager.kt` | inferred |  | 36 |
| `RawSnapshotBackupManager.ENTRY_DATABASES` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 50 |
| `RawSnapshotBackupManager.ENTRY_DATASTORE` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 49 |
| `RawSnapshotBackupManager.ENTRY_EXTERNAL_FILES` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 47 |
| `RawSnapshotBackupManager.ENTRY_FILES` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 46 |
| `RawSnapshotBackupManager.ENTRY_MANIFEST` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 43 |
| `RawSnapshotBackupManager.ENTRY_PAYLOAD_PREFIX` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 44 |
| `RawSnapshotBackupManager.ENTRY_SHARED_PREFS` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 48 |
| `RawSnapshotBackupManager.FORMAT_VERSION` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 40 |
| `RawSnapshotBackupManager.json` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 98 |
| `RawSnapshotBackupManager.mainHandler` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 54 |
| `RawSnapshotBackupManager.TAG` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 39 |
| `RawSnapshotBackupManager.terminalTopLevelDirNames` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 52 |
| `RawSnapshotBackupManager.ZIP_PREFIX` | `RawSnapshotBackupManager` | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 41 |
| `RoomDatabaseBackupManager.AUTO_BACKUP_FILE_PREFIX` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | inferred |  | 24 |
| `RoomDatabaseBackupManager.DB_NAME` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | inferred |  | 23 |
| `RoomDatabaseBackupManager.MANUAL_BACKUP_FILE_PREFIX` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | inferred |  | 25 |
| `RoomDatabaseBackupManager.TAG` | `RoomDatabaseBackupManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupManager.kt` | inferred |  | 22 |
| `RoomDatabaseBackupScheduler.UNIQUE_ONE_TIME_WORK_NAME` | `RoomDatabaseBackupScheduler` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupScheduler.kt` | inferred |  | 18 |
| `RoomDatabaseBackupScheduler.UNIQUE_PERIODIC_WORK_NAME` | `RoomDatabaseBackupScheduler` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseBackupScheduler.kt` | inferred |  | 17 |
| `RoomDatabaseHealthManager.DATABASE_NAME` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | inferred |  | 30 |
| `RoomDatabaseHealthManager.missingIndexEntryPattern` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | inferred |  | 31 |
| `RoomDatabaseHealthManager.operationMutex` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | inferred |  | 33 |
| `RoomDatabaseHealthManager.TAG` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | inferred |  | 29 |
| `RoomDatabaseHealthManager.wrongIndexEntryCountPattern` | `RoomDatabaseHealthManager` | `com.ai.assistance.operit.data.recovery` | `RoomDatabaseHealthManager.kt` | inferred |  | 32 |
| `RoomDatabaseRestoreManager.AUTO_BACKUP_FILE_PREFIX` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | inferred |  | 26 |
| `RoomDatabaseRestoreManager.DB_NAME` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | inferred |  | 24 |
| `RoomDatabaseRestoreManager.MANUAL_BACKUP_FILE_PREFIX` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | inferred |  | 27 |
| `RoomDatabaseRestoreManager.TAG` | `RoomDatabaseRestoreManager` | `com.ai.assistance.operit.data.backup` | `RoomDatabaseRestoreManager.kt` | inferred |  | 23 |
| `ScrapedModelPricingRowsCollect.rows` | `ScrapedModelPricingRowsCollect` | `com.ai.assistance.operit.data.collects` | `ScrapedModelPricingRowsCollect.kt` | String |  | 4 |
| `SNAPSHOT_PACKAGE_NAME_PREFIX` | — | `com.ai.assistance.operit.data.backup` | `RawSnapshotBackupManager.kt` | inferred |  | 32 |
| `TextExporter.CONTENT_WRITE_CHUNK_CHARACTER_COUNT` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | inferred |  | 16 |
| `TextExporter.dateFormatter` | `TextExporter` | `com.ai.assistance.operit.data.exporter` | `TextExporter.kt` | inferred |  | 17 |
| `UpdateSourceDownloader.httpClient` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | inferred |  | 38 |
| `UpdateSourceDownloader.RANGED_THREAD_COUNT` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | inferred |  | 298 |
| `UpdateSourceDownloader.TAG` | `UpdateSourceDownloader` | `com.ai.assistance.operit.data.updates` | `UpdateSourceDownloader.kt` | inferred |  | 36 |
| `UpdateSourceRanking.fastestFirst` | `UpdateSourceRanking` | `com.ai.assistance.operit.data.updates` | `UpdateDownloadSource.kt` | inferred |  | 65 |
