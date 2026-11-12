# operit.core.tools

> 函数 191 · 类型 156 · 顶层常量 74 · 共 421 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ADBResultData` | `ADBResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ADBResultData(val command: String, val output: String, val exitCode: Int) : ToolResultData | ADB命令执行结果数据 | 249 |
| `AgentStatusResultData` | `AgentStatusResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class AgentStatusResultData(val chatId: String, val state: String, val message: String?, val isIdle: Boolean, val isProcessing: Boolean) : ToolResultData | 对话输入状态结果数据 | 2071 |
| `AIToolHandler` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | class AIToolHandler(private val context: Context) | Handles the extraction and execution of AI tools from responses Supports real-time stream… | 29 |
| `AIToolHookDecision` | `AIToolHookDecision` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | class AIToolHookDecision | Decision returned by a tool hook before execution begins. | 7 |
| `AIToolHookDecision.AIToolHook` | `AIToolHookDecision` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | interface AIToolHook | Hook for observing tool call lifecycle events. Hooks can block a tool call by returning [… | 16 |
| `AIToolHookDecision.Allow` | `AIToolHookDecision` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | object Allow : AIToolHookDecision |  | 8 |
| `AppListData` | `AppListData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class AppListData(val includesSystemApps: Boolean, val packages: List<String>) : ToolResultData | 应用列表数据 | 691 |
| `AppOperationData` | `AppOperationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class AppOperationData(val operationType: String, val packageName: String, val success: Boolean, val details: String) : ToolResultData | 应用操作结果数据 | 672 |
| `AppUsageTimeEntry` | `AppUsageTimeEntry` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class AppUsageTimeEntry(val packageName: String, val appName: String, val totalForegroundTimeMs: Long, val lastTimeUsed: Long, val isSystemApp: Boolean) | 单个应用的使用时长统计 | 701 |
| `AppUsageTimeResultData` | `AppUsageTimeResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class AppUsageTimeResultData(val startTime: Long, val endTime: Long, val sinceHours: Int, val requestedPackageName: String?, val includesSystemApps: Boolean, val totalEntries: Int, val en… : ToolResultData | 应用使用时长数据 | 711 |
| `AutomationConfigSearchResult` | `AutomationConfigSearchResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class AutomationConfigSearchResult(val searchPackageName: String?, val searchAppName: String?, val foundConfigs: List<ConfigInfo>, val totalFound: Int) : ToolResultData | 自动化配置搜索结果数据 | 1432 |
| `AutomationConfigSearchResult.ConfigInfo` | `AutomationConfigSearchResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ConfigInfo(val appName: String, val packageName: String, val description: String, val isBuiltIn: Boolean, val fileName: String, val matchType: String) |  | 1440 |
| `AutomationExecutionResult` | `AutomationExecutionResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class AutomationExecutionResult(val functionName: String, val providedParameters: Map<String, String>, val agentId: String?, val displayId: Int?, val executionSuccess: Boolean, val execution… : ToolResultData | 自动化执行结果数据 | 1526 |
| `AutomationExecutionResult.UIStateInfo` | `AutomationExecutionResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class UIStateInfo(val nodeId: String, val packageName: String, val activityName: String) |  | 1539 |
| `AutomationFunctionListResult` | `AutomationFunctionListResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class AutomationFunctionListResult(val packageName: String?, val functions: List<FunctionInfo>, val totalCount: Int) : ToolResultData | 自动化功能列表结果数据 | 1578 |
| `AutomationFunctionListResult.FunctionInfo` | `AutomationFunctionListResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FunctionInfo(val name: String, val description: String, val targetNodeName: String) |  | 1585 |
| `AutomationPlanParametersResult` | `AutomationPlanParametersResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class AutomationPlanParametersResult(val functionName: String, val targetPackageName: String?, val requiredParameters: List<ParameterInfo>, val planSteps: Int, val planDescription: String) : ToolResultData | 自动化计划参数结果数据 | 1481 |
| `AutomationPlanParametersResult.ParameterInfo` | `AutomationPlanParametersResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ParameterInfo(val key: String, val description: String, val type: String, val isRequired: Boolean, val defaultValue: String?) |  | 1490 |
| `BinaryFileContentData` | `BinaryFileContentData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BinaryFileContentData(val path: String, val contentBase64: String, val size: Long, val env: String) : ToolResultData | Represents a binary file content result (Base64 encoded) | 464 |
| `BinaryResultData` | `BinaryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BinaryResultData(val value: ByteArray) : ToolResultData |  | 211 |
| `BluetoothBleCharacteristicData` | `BluetoothBleCharacteristicData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothBleCharacteristicData(val uuid: String, val properties: List<String>) |  | 878 |
| `BluetoothBleNotificationData` | `BluetoothBleNotificationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothBleNotificationData(val sessionId: String, val notifications: List<BluetoothBleNotification…) : ToolResultData |  | 884 |
| `BluetoothBleNotificationEntry` | `BluetoothBleNotificationEntry` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothBleNotificationEntry(val characteristicUuid: String, val bytesRead: Int, val text: String?, val dataBase64: String?, val timestamp: Long) |  | 897 |
| `BluetoothBleServiceData` | `BluetoothBleServiceData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothBleServiceData(val uuid: String, val characteristics: List<BluetoothBleCharacterist…) |  | 872 |
| `BluetoothBleServicesData` | `BluetoothBleServicesData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothBleServicesData(val sessionId: String, val services: List<BluetoothBleServiceData>) : ToolResultData |  | 856 |
| `BluetoothBondedDevicesData` | `BluetoothBondedDevicesData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothBondedDevicesData(val devices: List<BluetoothDeviceData>) : ToolResultData | Bluetooth bonded device list. | 773 |
| `BluetoothDeviceData` | `BluetoothDeviceData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothDeviceData(val name: String?, val address: String, val type: String, val bondState: String) |  | 788 |
| `BluetoothReadData` | `BluetoothReadData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothReadData(val sessionId: String, val bytesRead: Int, val text: String?, val dataBase64: String?) : ToolResultData | Bluetooth read result. | 844 |
| `BluetoothScannedDeviceData` | `BluetoothScannedDeviceData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothScannedDeviceData(val name: String?, val address: String, val type: String, val bondState: String, val source: String, val rssi: Int?) |  | 814 |
| `BluetoothScanResultData` | `BluetoothScanResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothScanResultData(val devices: List<BluetoothScannedDeviceDa…, val durationMs: Long, val includesBle: Boolean) : ToolResultData | Bluetooth scan result. | 797 |
| `BluetoothSessionData` | `BluetoothSessionData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothSessionData(val sessionId: String, val address: String, val mode: String) : ToolResultData | Bluetooth connection/session result. | 825 |
| `BluetoothStateData` | `BluetoothStateData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothStateData(val supported: Boolean, val enabled: Boolean, val state: String) : ToolResultData | Bluetooth adapter state. | 758 |
| `BluetoothTransferData` | `BluetoothTransferData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BluetoothTransferData(val sessionId: String, val bytesWritten: Int) : ToolResultData | Bluetooth write result. | 835 |
| `BooleanResultData` | `BooleanResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class BooleanResultData(val value: Boolean) : ToolResultData | Basic result data types (moved from AITool.kt) | 32 |
| `CalculationResultData` | `CalculationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CalculationResultData(val expression: String, val result: Double, val formattedResult: String, val variables: Map<String, Double>) : ToolResultData | 计算结果结构化数据 | 371 |
| `CharacterCardActivationResultData` | `CharacterCardActivationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardActivationResultData(val activeCharacterCardId: String?) : ToolResultData | 角色卡活跃状态更新结果 | 2493 |
| `CharacterCardCreateResultData` | `CharacterCardCreateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardCreateResultData(val created: Boolean, val card: CharacterCardResultItem, val activeCharacterCardId: String?, val changedFields: List<String>) : ToolResultData | 角色卡创建结果 | 2455 |
| `CharacterCardDeleteResultData` | `CharacterCardDeleteResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardDeleteResultData(val deleted: Boolean, val characterCardId: String, val activeCharacterCardId: String?) : ToolResultData | 角色卡删除结果 | 2481 |
| `CharacterCardExportResultData` | `CharacterCardExportResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardExportResultData(val characterCardId: String, val tavernJson: String) : ToolResultData | 角色卡 Tavern JSON 导出结果 | 2515 |
| `CharacterCardImportResultData` | `CharacterCardImportResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardImportResultData(val imported: Boolean, val card: CharacterCardResultItem, val activeCharacterCardId: String?) : ToolResultData | 角色卡 Tavern JSON 导入结果 | 2503 |
| `CharacterCardListResultData` | `CharacterCardListResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardListResultData(val totalCount: Int, val cards: List<CharacterCardInfo>) : ToolResultData | 角色卡列表结果数据 | 2177 |
| `CharacterCardListResultData.CharacterCardInfo` | `CharacterCardListResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardInfo(val id: String, val name: String, val description: String, val isDefault: Boolean, val createdAt: Long, val updatedAt: Long) |  | 2183 |
| `CharacterCardResultData` | `CharacterCardResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardResultData(val card: CharacterCardResultItem, val activeCharacterCardId: String?) : ToolResultData | 单张角色卡查询结果 | 2444 |
| `CharacterCardResultItem` | `CharacterCardResultItem` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardResultItem(val id: String, val name: String, val description: String, val characterSetting: String, val openingStatement: String, val otherContentChat: String, val other… | 角色卡配置条目 | 2408 |
| `CharacterCardsResultData` | `CharacterCardsResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardsResultData(val totalCount: Int, val activeCharacterCardId: String?, val cards: List<CharacterCardResultItem>) : ToolResultData | 角色卡列表结果 | 2432 |
| `CharacterCardToolAccessConfigResultItem` | `CharacterCardToolAccessConfigResultItem` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardToolAccessConfigResultItem(val enabled: Boolean, val allowedBuiltinTools: List<String>, val allowedPackages: List<String>, val allowedSkills: List<String>, val allowedMcpServers: List<S… | 角色卡工具访问配置条目 | 2398 |
| `CharacterCardUpdateResultData` | `CharacterCardUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CharacterCardUpdateResultData(val updated: Boolean, val card: CharacterCardResultItem, val activeCharacterCardId: String?, val changedFields: List<String>) : ToolResultData | 角色卡更新结果 | 2468 |
| `ChatCallResultData` | `ChatCallResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatCallResultData(val text: String, val turns: List<ChatCallTurnInfo>, val finishReason: String, val metadata: Map<String, JsonElement>, val receivedAt: Long) : ToolResultData | 功能模型调用结果数据 | 2159 |
| `ChatCallTurnInfo` | `ChatCallTurnInfo` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatCallTurnInfo(val kind: String, val content: String, val toolName: String?, val metadata: Map<String, JsonElement>) |  | 2150 |
| `ChatCreationResultData` | `ChatCreationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatCreationResultData(val chatId: String, val createdAt: Long) : ToolResultData | 新建对话结果数据 | 1986 |
| `ChatDeleteResultData` | `ChatDeleteResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatDeleteResultData(val chatId: String, val deletedAt: Long) : ToolResultData | 删除对话结果数据 | 2114 |
| `ChatFindResultData` | `ChatFindResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatFindResultData(val matchedCount: Int, val chat: ChatListResultData.ChatInfo?) : ToolResultData | 查找对话结果数据 | 2056 |
| `ChatListResultData` | `ChatListResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatListResultData(val totalCount: Int, val currentChatId: String?, val chats: List<ChatInfo>) : ToolResultData | 对话列表结果数据 | 1997 |
| `ChatListResultData.ChatInfo` | `ChatListResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatInfo(val id: String, val title: String, val messageCount: Int, val createdAt: String, val updatedAt: String, val isCurrent: Boolean, val inputTokens: Long, val out… |  | 2004 |
| `ChatMessagesResultData` | `ChatMessagesResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatMessagesResultData(val chatId: String, val order: String, val limit: Int, val messages: List<ChatMessageInfo>, val start: Int?, val end: Int?) : ToolResultData |  | 2124 |
| `ChatMessagesResultData.ChatMessageInfo` | `ChatMessagesResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatMessageInfo(val sender: String, val content: String, val timestamp: Long, val roleName: String, val provider: String, val modelName: String) |  | 2134 |
| `ChatServiceStartResultData` | `ChatServiceStartResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatServiceStartResultData(val isConnected: Boolean, val connectionTime: Long) : ToolResultData | 对话服务启动结果数据 | 1971 |
| `ChatSwitchResultData` | `ChatSwitchResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatSwitchResultData(val chatId: String, val chatTitle: String, val switchedAt: Long) : ToolResultData | 切换对话结果数据 | 2086 |
| `ChatTitleUpdateResultData` | `ChatTitleUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ChatTitleUpdateResultData(val chatId: String, val title: String, val updatedAt: Long) : ToolResultData | 更新对话标题结果数据 | 2102 |
| `CombinedOperationResultData` | `CombinedOperationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class CombinedOperationResultData(val operationSummary: String, val waitTime: Int, val pageInfo: UIPageResultData) : ToolResultData | Represents a combined operation result data | 996 |
| `ComputerDesktopActionResultData` | `ComputerDesktopActionResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ComputerDesktopActionResultData(val action: String, val target: String?, val resultSummary: String, val tabs: List<ComputerTabInfo>?, val pageContent: ComputerPageInfoNode?) : ToolResultData | Represents the result of a computer desktop action | 1339 |
| `ComputerDesktopActionResultData.ComputerTabInfo` | `ComputerDesktopActionResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ComputerTabInfo(val id: String, val title: String, val url: String, val isActive: Boolean) |  | 1347 |
| `ComputerPageInfoNode` | `ComputerPageInfoNode` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ComputerPageInfoNode(val interactionId: Int?, val type: String, val description: String, val children: List<ComputerPageInfoNode>) | Represents a simplified HTML node for computer desktop actions, focusing on interactabili… | 1316 |
| `ConnectionResultData` | `ConnectionResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ConnectionResultData(val connectionId: String, val isActive: Boolean, val timestamp: Long) : ToolResultData | Connection result data | 402 |
| `DateResultData` | `DateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class DateResultData(val date: String, val format: String, val formattedDate: String) : ToolResultData | 日期结果结构化数据 | 393 |
| `DeviceInfoResultData` | `DeviceInfoResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class DeviceInfoResultData(val deviceId: String, val model: String, val manufacturer: String, val androidVersion: String, val sdkVersion: Int, val screenResolution: String, val screenDe… : ToolResultData | Device information result data | 1008 |
| `DirectoryListingData` | `DirectoryListingData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class DirectoryListingData(val path: String, val entries: List<FileEntry>, val env: String) : ToolResultData | Represents a directory listing result | 415 |
| `DirectoryListingData.FileEntry` | `DirectoryListingData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FileEntry(val name: String, val isDirectory: Boolean, val size: Long, val permissions: String, val lastModified: String) |  | 422 |
| `EnvironmentVariableReadResultData` | `EnvironmentVariableReadResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class EnvironmentVariableReadResultData(val key: String, val value: String?, val exists: Boolean) : ToolResultData |  | 76 |
| `EnvironmentVariableWriteResultData` | `EnvironmentVariableWriteResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class EnvironmentVariableWriteResultData(val key: String, val requestedValue: String, val value: String?, val exists: Boolean, val cleared: Boolean) : ToolResultData |  | 91 |
| `EnvVar` | `EnvVar` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | class EnvVar(val name: String, val description: LocalizedText, val required: Boolean, val defaultValue: String?) | Represents an environment variable declaration for a package | 204 |
| `EnvVarSerializer` | `EnvVarSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | object EnvVarSerializer : KSerializer<EnvVar> | Custom serializer for EnvVar that handles both old format (string) and new format (object… | 216 |
| `FFmpegResultData` | `FFmpegResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FFmpegResultData(val command: String, val returnCode: Int, val output: String, val duration: Long, val outputFile: String?, val mediaInfo: MediaInfo?) : ToolResultData | FFmpeg处理结果数据 | 1174 |
| `FFmpegResultData.MediaInfo` | `FFmpegResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class MediaInfo(val format: String, val duration: String, val bitrate: String, val videoStreams: List<StreamInfo>, val audioStreams: List<StreamInfo>) |  | 1183 |
| `FFmpegResultData.StreamInfo` | `FFmpegResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class StreamInfo(val index: Int, val codecType: String, val codecName: String, val resolution: String?, val frameRate: String?, val sampleRate: String?, val channels: Int?) |  | 1192 |
| `FileApplyResultData` | `FileApplyResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FileApplyResultData(val operation: FileOperationData, val aiDiffInstructions: String, val diffContent: String?) : ToolResultData | Represents the result of an 'apply_file' operation, including the AI-generated diff | 548 |
| `FileContentData` | `FileContentData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FileContentData(val path: String, val content: String, val size: Long, val env: String) : ToolResultData | Represents a file content result | 448 |
| `FileExistsData` | `FileExistsData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FileExistsData(val path: String, val exists: Boolean, val isDirectory: Boolean, val size: Long, val env: String) : ToolResultData | Represents file existence check result | 479 |
| `FileInfoData` | `FileInfoData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FileInfoData(val path: String, val exists: Boolean, val fileType: String, val size: Long, val permissions: String, val owner: String, val group: String, val lastModified: … : ToolResultData | Represents detailed file information | 500 |
| `FileOperationData` | `FileOperationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FileOperationData(val operation: String, val env: String, val path: String, val successful: Boolean, val details: String) : ToolResultData | Represents a file operation result | 533 |
| `FilePartContentData` | `FilePartContentData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FilePartContentData(val path: String, val content: String, val partIndex: Int, val totalParts: Int, val startLine: Int, val endLine: Int, val totalLines: Int, val env: String) : ToolResultData | 文件分段读取结果数据 | 229 |
| `FindFilesResultData` | `FindFilesResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FindFilesResultData(val path: String, val pattern: String, val files: List<String>, val env: String) : ToolResultData | 文件查找结果数据 | 1145 |
| `FunctionModelBindingResultData` | `FunctionModelBindingResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FunctionModelBindingResultData(val functionType: String, val configId: String, val configName: String, val requestedModelIndex: Int, val actualModelIndex: Int, val selectedModel: String) : ToolResultData | 设置功能模型绑定结果 | 2676 |
| `FunctionModelConfigResultData` | `FunctionModelConfigResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FunctionModelConfigResultData(val defaultConfigId: String, val functionType: String, val configId: String, val configName: String, val modelIndex: Int, val actualModelIndex: Int, val selec… : ToolResultData | 查询单个功能模型绑定结果 | 2659 |
| `FunctionModelConfigsResultData` | `FunctionModelConfigsResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FunctionModelConfigsResultData(val defaultConfigId: String, val mappings: List<FunctionModelMappingResu…) : ToolResultData | 列出功能模型绑定结果 | 2648 |
| `FunctionModelMappingResultItem` | `FunctionModelMappingResultItem` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FunctionModelMappingResultItem(val functionType: String, val configId: String, val configName: String?, val modelIndex: Int, val actualModelIndex: Int?, val selectedModel: String?) | 功能模型绑定条目 | 2586 |
| `GrepResultData` | `GrepResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class GrepResultData(val searchPath: String, val pattern: String, val matches: List<FileMatch>, val totalMatches: Int, val filesSearched: Int, val env: String) : ToolResultData | Grep代码搜索结果数据 | 1661 |
| `GrepResultData.FileMatch` | `GrepResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class FileMatch(val filePath: String, val lineMatches: List<LineMatch>) |  | 1672 |
| `GrepResultData.LineMatch` | `GrepResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class LineMatch(val lineNumber: Int, val lineContent: String, val matchContext: String?) |  | 1678 |
| `GrepResultDataTest` | `GrepResultDataTest` | `com.ai.assistance.operit.core.tools` | `GrepResultDataTest.kt` | class GrepResultDataTest | Regression tests for issue #1346: grep context rendering must show the real source line n… | 15 |
| `HiddenTerminalCommandResultData` | `HiddenTerminalCommandResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class HiddenTerminalCommandResultData(val command: String, val output: String, val exitCode: Int, val executorKey: String, val timedOut: Boolean) : ToolResultData | 隐藏终端命令执行结果数据 | 309 |
| `HttpResponseData` | `HttpResponseData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class HttpResponseData(val url: String, val statusCode: Int, val statusMessage: String, val headers: Map<String, String>, val contentType: String, val content: String, val contentBa… : ToolResultData | HTTP响应结果结构化数据 | 602 |
| `HttpStreamEventData` | `HttpStreamEventData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class HttpStreamEventData(val type: String, val url: String, val statusCode: Int?, val statusMessage: String?, val headers: Map<String, String>, val contentType: String?, val chunk: St… : ToolResultData |  | 640 |
| `IntentResultData` | `IntentResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class IntentResultData(val action: String, val uri: String, val package_name: String, val component: String, val flags: Int, val extras_count: Int, val result: String) : ToolResultData | Intent execution result data | 1119 |
| `IntResultData` | `IntResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class IntResultData(val value: Int) : ToolResultData |  | 206 |
| `LocalizedText` | `LocalizedText` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | class LocalizedText(val values: Map<String, String>) | Represents a package of tools that can be imported by the AI | 40 |
| `LocalizedTextSerializer` | `LocalizedTextSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | object LocalizedTextSerializer : KSerializer<LocalizedText> |  | 129 |
| `LocationData` | `LocationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class LocationData(val latitude: Double, val longitude: Double, val accuracy: Float, val provider: String, val timestamp: Long, val rawData: String, val address: String, val cit… : ToolResultData | 位置数据结构 | 1274 |
| `McpRestartLogPluginResultItem` | `McpRestartLogPluginResultItem` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class McpRestartLogPluginResultItem(val id: String, val displayName: String, val shortName: String, val status: String, val message: String, val serviceName: String, val log: String) |  | 152 |
| `McpRestartWithLogsResultData` | `McpRestartWithLogsResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class McpRestartWithLogsResultData(val timeoutMs: Long, val elapsedMs: Long, val timedOut: Boolean, val progress: Double, val message: String, val pluginsTotal: Int, val pluginsStarted: Int, va… : ToolResultData |  | 163 |
| `MemoryLinkQueryResultData` | `MemoryLinkQueryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class MemoryLinkQueryResultData(val totalCount: Int, val links: List<LinkInfo>) : ToolResultData | 记忆链接查询结果数据 | 2279 |
| `MemoryLinkQueryResultData.LinkInfo` | `MemoryLinkQueryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class LinkInfo(val linkId: Long, val sourceTitle: String, val targetTitle: String, val linkType: String, val weight: Float, val description: String) |  | 2284 |
| `MemoryLinkResultData` | `MemoryLinkResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class MemoryLinkResultData(val sourceTitle: String, val targetTitle: String, val linkType: String, val weight: Float, val description: String) : ToolResultData | 记忆链接结果数据 | 2265 |
| `MemoryQueryResultData` | `MemoryQueryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class MemoryQueryResultData(val memories: List<MemoryInfo>, val snapshotId: String?, val snapshotCreated: Boolean, val excludedBySnapshotCount: Int) : ToolResultData | Represents the result of a memory query | 1375 |
| `MemoryQueryResultData.MemoryInfo` | `MemoryQueryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class MemoryInfo(val title: String, val content: String, val source: String, val tags: List<String>, val createdAt: String, val chunkInfo: String?, val chunkIndices: List<Int>… |  | 1383 |
| `MessageSendResultData` | `MessageSendResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class MessageSendResultData(val chatId: String, val message: String, val aiResponse: String?, val receivedAt: Long?, val sentAt: Long) : ToolResultData | 发送消息结果数据 | 2216 |
| `MessageSendStreamEventData` | `MessageSendStreamEventData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class MessageSendStreamEventData(val type: String, val chatId: String, val message: String, val waifu: Boolean, val chunk: String?, val chunkIndex: Int?, val receivedChars: Int?) : ToolResultData | 发送消息流式事件数据 | 2245 |
| `ModelConfigConnectionTestItemResultData` | `ModelConfigConnectionTestItemResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ModelConfigConnectionTestItemResultData(val type: String, val success: Boolean, val outcome: String, val error: String?) | 模型配置连接测试单项 | 2691 |
| `ModelConfigConnectionTestResultData` | `ModelConfigConnectionTestResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ModelConfigConnectionTestResultData(val configId: String, val configName: String, val providerType: String, val requestedModelIndex: Int, val actualModelIndex: Int, val testedModelName: String, … : ToolResultData | 模型配置连接测试结果 | 2700 |
| `ModelConfigCreateResultData` | `ModelConfigCreateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ModelConfigCreateResultData(val created: Boolean, val config: ModelConfigResultItem, val changedFields: List<String>) : ToolResultData | 创建模型配置结果 | 2610 |
| `ModelConfigDeleteResultData` | `ModelConfigDeleteResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ModelConfigDeleteResultData(val deleted: Boolean, val configId: String, val affectedFunctions: List<String>, val fallbackConfigId: String) : ToolResultData | 删除模型配置结果 | 2635 |
| `ModelConfigResultItem` | `ModelConfigResultItem` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ModelConfigResultItem : Int, | 模型配置条目 | 2526 |
| `ModelConfigsResultData` | `ModelConfigsResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ModelConfigsResultData(val totalConfigCount: Int, val defaultConfigId: String, val configs: List<ModelConfigResultItem>, val functionMappings: List<FunctionModelMappingResu…) : ToolResultData | 列出模型配置结果 | 2597 |
| `ModelConfigUpdateResultData` | `ModelConfigUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ModelConfigUpdateResultData(val updated: Boolean, val config: ModelConfigResultItem, val changedFields: List<String>, val affectedFunctions: List<String>) : ToolResultData | 更新模型配置结果 | 2622 |
| `MusicPlaybackResultData` | `MusicPlaybackResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class MusicPlaybackResultData(val state: String, val source: String?, val sourceType: String?, val title: String?, val artist: String?, val durationMs: Long?, val positionMs: Long, val buf… : ToolResultData | 音乐播放结果数据 | 333 |
| `NotificationData` | `NotificationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class NotificationData(val notifications: List<Notification>, val timestamp: Long) : ToolResultData | 通知数据结构 | 1249 |
| `NotificationData.Notification` | `NotificationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class Notification(val packageName: String, val text: String, val timestamp: Long) : String |  | 1252 |
| `PackageTool` | `PackageTool` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | class PackageTool(val name: String, val description: LocalizedText, val parameters: List<PackageToolParameter>, val script: String, val advice: Boolean) | Represents a tool within a package | 354 |
| `PackageToolExecutor` | `PackageToolExecutor` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | class PackageToolExecutor(private val toolPackage: ToolPackage, private val context: Context, private val packageManager: PackageManager) : ToolExecutor | Executor for package tools | 376 |
| `PackageToolParameter` | `PackageToolParameter` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | class PackageToolParameter(val name: String, val description: LocalizedText, val type: String, val required: Boolean) | Represents a parameter for a tool in a package | 366 |
| `ParsedProxyInvocation` | `ParsedProxyInvocation` | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | class ParsedProxyInvocation(val targetToolName: String, val forwardedParameters: MutableList<ToolParameter>) |  | 86 |
| `SandboxPackageResultItem` | `SandboxPackageResultItem` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SandboxPackageResultItem(val packageName: String, val displayName: String, val description: String, val isBuiltIn: Boolean, val enabledByDefault: Boolean, val enabled: Boolean, val im… |  | 108 |
| `SandboxPackagesResultData` | `SandboxPackagesResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SandboxPackagesResultData(val externalPackagesPath: String, val scriptDevGuide: String, val totalCount: Int, val builtInCount: Int, val externalCount: Int, val enabledCount: Int, val d… : ToolResultData |  | 122 |
| `SandboxPackageUpdateResultData` | `SandboxPackageUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SandboxPackageUpdateResultData(val packageName: String, val requestedEnabled: Boolean, val previousEnabled: Boolean, val currentEnabled: Boolean, val message: String) : ToolResultData |  | 139 |
| `SandboxScriptExecutionResultData` | `SandboxScriptExecutionResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SandboxScriptExecutionResultData(val success: Boolean, val scriptPath: String, val functionName: String, val params: JsonElement?, val envFilePath: String?, val startedAtMs: Long, val finishe… : ToolResultData |  | 50 |
| `ScriptExecutionTraceData` | `ScriptExecutionTraceData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ScriptExecutionTraceData(val kind: String, val level: String?, val message: String, val callId: String?, val timestampMs: Long) : ToolResultData |  | 182 |
| `SimplifiedUINode` | `SimplifiedUINode` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SimplifiedUINode(val className: String?, val text: String?, val contentDesc: String?, val resourceId: String?, val bounds: String?, val isClickable: Boolean, val children: Lis… | Represents UI node structure for hierarchical display | 907 |
| `SleepResultData` | `SleepResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SleepResultData(val requestedMs: Int, val sleptMs: Int) : ToolResultData |  | 42 |
| `SpeechServicesConfigResultData` | `SpeechServicesConfigResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SpeechServicesConfigResultData(val ttsServiceType: String, val ttsHttpConfig: SpeechTtsHttpConfigResultItem, val ttsVitsPackageConfig: SpeechTtsVitsPackageConfigRes…, val ttsCleanerRegexs: … : ToolResultData | 获取语音服务配置结果 | 2344 |
| `SpeechServicesTtsPlaybackTestResultData` | `SpeechServicesTtsPlaybackTestResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SpeechServicesTtsPlaybackTestResultData(val ttsServiceType: String, val providerClass: String, val initialized: Boolean, val playbackTriggered: Boolean, val interrupt: Boolean, val textLength: Int, … : ToolResultD… | TTS 单次播放测试结果 | 2376 |
| `SpeechServicesUpdateResultData` | `SpeechServicesUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SpeechServicesUpdateResultData(val updated: Boolean, val changedFields: List<String>, val ttsServiceType: String, val sttServiceType: String, val ttsApiKeySet: Boolean, val sttApiKeySet: Bo… : ToolResultData | 更新语音服务配置结果 | 2361 |
| `SpeechSttHttpConfigResultItem` | `SpeechSttHttpConfigResultItem` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SpeechSttHttpConfigResultItem(val endpointUrl: String, val apiKeySet: Boolean, val apiKeyPreview: String, val modelName: String) | 语音服务 STT HTTP 配置条目 | 2335 |
| `SpeechTtsHttpConfigResultItem` | `SpeechTtsHttpConfigResultItem` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SpeechTtsHttpConfigResultItem(val urlTemplate: String, val apiKeySet: Boolean, val apiKeyPreview: String, val headers: Map<String, String>, val httpMethod: String, val requestBody: String,… | 语音服务 TTS HTTP 配置条目 | 2311 |
| `SpeechTtsVitsPackageConfigResultItem` | `SpeechTtsVitsPackageConfigResultItem` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SpeechTtsVitsPackageConfigResultItem(val packagePath: String, val speakerId: String, val options: Map<String, String>) | 语音服务 TTS VITS/Piper 包配置条目 | 2327 |
| `StringOrStringListSerializer` | `StringOrStringListSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | object StringOrStringListSerializer : KSerializer<List<String>> |  | 171 |
| `StringResultData` | `StringResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class StringResultData(val value: String) : ToolResultData |  | 37 |
| `SystemSettingData` | `SystemSettingData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class SystemSettingData(val namespace: String, val setting: String, val value: String) : ToolResultData | 系统设置数据 | 663 |
| `TerminalCommandResultData` | `TerminalCommandResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class TerminalCommandResultData(val command: String, val output: String, val exitCode: Int, val sessionId: String, val timedOut: Boolean, val sessionAlive: Boolean) : ToolResultData | 终端命令执行结果数据 | 264 |
| `TerminalSessionCloseResultData` | `TerminalSessionCloseResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class TerminalSessionCloseResultData(val sessionId: String, val success: Boolean, val message: String) : ToolResultData | 终端会话关闭结果数据 | 1631 |
| `TerminalSessionCreationResultData` | `TerminalSessionCreationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class TerminalSessionCreationResultData(val sessionId: String, val sessionName: String, val isNewSession: Boolean) : ToolResultData | 终端会话创建结果数据 | 1615 |
| `TerminalSessionScreenResultData` | `TerminalSessionScreenResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class TerminalSessionScreenResultData(val sessionId: String, val rows: Int, val cols: Int, val content: String) : ToolResultData | 终端会话当前屏幕内容结果数据（仅当前屏，不含历史滚动缓冲） | 1641 |
| `TerminalStreamEventData` | `TerminalStreamEventData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class TerminalStreamEventData(val type: String, val command: String, val sessionId: String, val chunk: String?, val chunkIndex: Int?, val receivedChars: Int?) : ToolResultData | 终端命令流式事件数据 | 290 |
| `ToolExecutionLimits` | `ToolExecutionLimits` | `com.ai.assistance.operit.core.tools` | `ToolExecutionLimits.kt` | object ToolExecutionLimits |  | 3 |
| `ToolExecutor` | `ToolExecutor` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | interface ToolExecutor | Interface for tool executors | 479 |
| `ToolPackage` | `ToolPackage` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | class ToolPackage(val name: String, val description: LocalizedText, val tools: List<PackageTool>, val states: List<ToolPackageState>, /** * Optional list of environment variabl… |  | 303 |
| `ToolPackageState` | `ToolPackageState` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | class ToolPackageState(val id: String, val condition: String, val inheritTools: Boolean, val excludeTools: List<String>, val tools: List<PackageTool>) |  | 342 |
| `ToolProgressBus` | `ToolProgressBus` | `com.ai.assistance.operit.core.tools` | `ToolProgressBus.kt` | object ToolProgressBus |  | 15 |
| `ToolProgressEvent` | `ToolProgressEvent` | `com.ai.assistance.operit.core.tools` | `ToolProgressBus.kt` | class ToolProgressEvent(val toolName: String, val progress: Float, val message: String, val priority: Int, val level: Int) |  | 7 |
| `ToolResultData` | `ToolResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class ToolResultData | This file contains all implementations of ToolResultData Centralized for easier maintenan… | 17 |
| `UIActionResultData` | `UIActionResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class UIActionResultData(val actionType: String, val actionDescription: String, val coordinates: Pair<Int, Int>?, val elementId: String?) : ToolResultData | Represents a UI action result data | 983 |
| `UIPageResultData` | `UIPageResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class UIPageResultData(val packageName: String, val activityName: String, val uiElements: SimplifiedUINode) : ToolResultData | Represents UI page information result data | 965 |
| `VisitWebResultData` | `VisitWebResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class VisitWebResultData(val url: String, val title: String, val content: String, val metadata: Map<String, String>, val links: List<LinkData>, val imageLinks: List<String>, val visit… : ToolResultData | Web page visit result data | 1050 |
| `VisitWebResultData.LinkData` | `VisitWebResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class LinkData(val url: String, val text: String) : String |  | 1068 |
| `WorkflowDetailResultData` | `WorkflowDetailResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class WorkflowDetailResultData(val id: String, val name: String, val description: String, val nodes: List<com.ai.assistance.operit…, val connections: List<com.ai.assistance.operit…, val ena… : ToolResultData | 工作流详细信息结果数据（包含完整的节点和连接信息） | 1854 |
| `WorkflowListResultData` | `WorkflowListResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class WorkflowListResultData(val workflows: List<WorkflowResultData>, val totalCount: Int) : ToolResultData | 工作流列表结果数据 | 1817 |
| `WorkflowResultData` | `WorkflowResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | class WorkflowResultData(val id: String, val name: String, val description: String, val nodeCount: Int, val connectionCount: Int, val enabled: Boolean, val createdAt: Long, val update… : ToolResultData | 工作流基本信息结果数据 | 1781 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `AIToolHandler.getInstance` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | context: Context | AIToolHandler |  | 36 |
| `AIToolHandler.getToolPermissionSystem` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` |  | ToolPermissionSystem | Get the tool permission system for UI use | 55 |
| `AIToolHandler.unregisterTool` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | toolName: String | Unit |  | 59 |
| `AIToolHandler.addToolHook` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | hook: AIToolHook | Unit | Registers a hook for tool call lifecycle events and pre-execution interception. Hook call… | 67 |
| `AIToolHandler.removeToolHook` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | hook: AIToolHook | Unit | Removes a previously registered tool hook. | 74 |
| `AIToolHandler.clearToolHooks` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` |  | Unit | Clears all registered tool hooks. | 79 |
| `AIToolHandler.notifyHooks` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | eventName: String<br>action: (AIToolHook) -> Unit | Unit | Dispatches lifecycle hook callbacks safely. | 84 |
| `AIToolHandler.notifyToolCallRequested` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | Unit | Notify that a tool call request is received. | 95 |
| `AIToolHandler.checkToolInterception` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | AIToolHookDecision | Ask hooks whether the tool call should continue. | 100 |
| `AIToolHandler.buildToolInterceptionResult` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | toolName: String<br>decision: AIToolHookDecision.Block | ToolResult | Build the standard result returned when a hook blocks a tool call. | 120 |
| `AIToolHandler.notifyToolPermissionChecked` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool<br>granted: Boolean<br>reason: String?? | Unit | Notify that permission check finished for a tool call. | 133 |
| `AIToolHandler.notifyToolExecutionStarted` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | Unit | Notify that actual tool execution starts. | 138 |
| `AIToolHandler.notifyToolExecutionResult` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool<br>result: ToolResult | Unit | Notify that a tool execution result is produced. | 143 |
| `AIToolHandler.notifyToolExecutionError` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool<br>throwable: Throwable | Unit | Notify that tool execution throws an exception. | 148 |
| `AIToolHandler.notifyToolExecutionFinished` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | Unit | Notify that a tool request lifecycle is finished. | 153 |
| `AIToolHandler.getAllToolNames` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` |  | List<String> | Get all registered tool names | 160 |
| `AIToolHandler.getToolDescription` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | toolName: String | String | Get human-readable description for a tool by name. Used by the tool selector UI to help u… | 167 |
| `AIToolHandler.refreshPermissionState` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` |  | Boolean | Force refresh permission request state Can be called if permission dialog is not showing | 174 |
| `AIToolHandler.registerTool` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | name: String<br>descriptionGenerator: ((AITool) -> String)??<br>executor: ToolExecutor | Unit | 工具注册的唯一方法 - 提供完整信息的注册 | 179 |
| `AIToolHandler.registerTool` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | name: String<br>descriptionGenerator: ((AITool) -> String)??<br>executor: (AITool) -> ToolResult | Unit | 添加重载方法接受函数式接口作为executor的便捷写法 | 193 |
| `AIToolHandler.invoke` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | ToolResult |  | 203 |
| `AIToolHandler.registerDefaultTools` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` |  | Unit | Register all default tools | 211 |
| `AIToolHandler.getOrCreatePackageManager` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` |  | PackageManager | Gets or creates the package manager instance | 224 |
| `AIToolHandler.replaceToolInvocation` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | response: String<br>invocation: ToolInvocation<br>result: String | String | Replace a tool invocation in the response with its result | 233 |
| `AIToolHandler.unescapeXml` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | input: String | String | Unescapes XML special characters | 249 |
| `AIToolHandler.reset` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` |  | Unit | Reset the tool execution state | 274 |
| `AIToolHandler.getToolExecutor` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | toolName: String | ToolExecutor? | Get a registered tool executor by name | 287 |
| `AIToolHandler.isMcpServiceActive` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | packageName: String | Boolean |  | 291 |
| `AIToolHandler.getToolExecutorOrActivate` | `AIToolHandler` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | toolName: String | ToolExecutor? | Returns a tool executor if available. If missing, it will: - Ensure default tools are reg… | 303 |
| `executeTool` | — | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | ToolResult | Executes a tool directly | 363 |
| `executeToolAndStream` | — | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | Flow<ToolResult> | Executes a tool and preserves intermediate streaming results when supported by the execut… | 419 |
| `ToolExecutor.invoke` | `ToolExecutor` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | ToolResult |  | 480 |
| `ToolExecutor.invokeAndStream` | `ToolExecutor` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | Flow<ToolResult> |  | 482 |
| `ToolExecutor.validateParameters` | `ToolExecutor` | `com.ai.assistance.operit.core.tools` | `AIToolHandler.kt` | tool: AITool | ToolValidationResult | Validates the parameters of a tool before execution Default implementation always returns… | 488 |
| `AIToolHookDecision.AIToolHook.onToolCallRequested` | `AIToolHook` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | tool: AITool | Unit | Called when a tool call request is received. | 18 |
| `AIToolHookDecision.AIToolHook.onToolCallIntercept` | `AIToolHook` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | tool: AITool | AIToolHookDecision | Called before permission checks and executor activation. | 21 |
| `AIToolHookDecision.AIToolHook.onToolPermissionChecked` | `AIToolHook` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | tool: AITool<br>granted: Boolean<br>reason: String?? | Unit | Called after permission check is completed (if applicable). | 24 |
| `AIToolHookDecision.AIToolHook.onToolExecutionStarted` | `AIToolHook` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | tool: AITool | Unit | Called when actual tool execution is about to start. | 27 |
| `AIToolHookDecision.AIToolHook.onToolExecutionResult` | `AIToolHook` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | tool: AITool<br>result: ToolResult | Unit | Called when a tool execution result is produced. | 30 |
| `AIToolHookDecision.AIToolHook.onToolExecutionError` | `AIToolHook` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | tool: AITool<br>throwable: Throwable | Unit | Called when execution throws an exception. | 33 |
| `AIToolHookDecision.AIToolHook.onToolExecutionFinished` | `AIToolHook` | `com.ai.assistance.operit.core.tools` | `AIToolHook.kt` | tool: AITool | Unit | Called when the tool request lifecycle is finished. | 36 |
| `LocalizedText.resolve` | `LocalizedText` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | context: Context | String |  | 44 |
| `LocalizedText.resolve` | `LocalizedText` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | preferredLanguage: String | String |  | 90 |
| `LocalizedText.of` | `LocalizedText` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | value: String | LocalizedText |  | 123 |
| `LocalizedTextSerializer.deserialize` | `LocalizedTextSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | decoder: Decoder | LocalizedText |  | 136 |
| `LocalizedTextSerializer.serialize` | `LocalizedTextSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | encoder: Encoder<br>value: LocalizedText | Unit |  | 158 |
| `StringOrStringListSerializer.deserialize` | `StringOrStringListSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | decoder: Decoder | List<String> |  | 176 |
| `StringOrStringListSerializer.serialize` | `StringOrStringListSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | encoder: Encoder<br>value: List<String> | Unit |  | 190 |
| `EnvVarSerializer.deserialize` | `EnvVarSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | decoder: Decoder | EnvVar |  | 221 |
| `EnvVarSerializer.serialize` | `EnvVarSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | encoder: Encoder<br>value: EnvVar | Unit |  | 285 |
| `PackageToolExecutor.invoke` | `PackageToolExecutor` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | tool: AITool | ToolResult |  | 384 |
| `PackageToolExecutor.invokeAndStream` | `PackageToolExecutor` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | tool: AITool | Flow<ToolResult> |  | 425 |
| `PackageToolExecutor.validateParameters` | `PackageToolExecutor` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | tool: AITool | ToolValidationResult |  | 433 |
| `PackageToolExecutor.describePackage` | `PackageToolExecutor` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` |  | String | Returns information about the tools available in this package | 480 |
| `ToolProgressBus.priorityForTool` | `ToolProgressBus` | `com.ai.assistance.operit.core.tools` | `ToolProgressBus.kt` | toolName: String | Int |  | 21 |
| `ToolProgressBus.update` | `ToolProgressBus` | `com.ai.assistance.operit.core.tools` | `ToolProgressBus.kt` | toolName: String<br>progress: Float<br>message: String? | Unit |  | 31 |
| `ToolProgressBus.update` | `ToolProgressBus` | `com.ai.assistance.operit.core.tools` | `ToolProgressBus.kt` | toolName: String<br>progress: Float<br>message: String?<br>priority: Int<br>level: Int? | Unit |  | 35 |
| `ToolProgressBus.clear` | `ToolProgressBus` | `com.ai.assistance.operit.core.tools` | `ToolProgressBus.kt` |  | Unit |  | 57 |
| `registerAllTools` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | handler: AIToolHandler<br>context: Context | Unit | Register all available tools with the AIToolHandler | 36 |
| `executeUiToolWithVisibility` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool<br>showStatusIndicator: Boolean?<br>delayMs: Long?<br>action: suspend (AITool) -> ToolResult | ToolResult | Helper function to wrap UI tool execution with visibility changes | 39 |
| `s` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | resId: Int<br>args: Any | String |  | 61 |
| `formatEnvInfo` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | environment: String? | String |  | 63 |
| `formatEnvArrowInfo` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | sourceEnv: String<br>destEnv: String | String |  | 71 |
| `isEnglishLanguage` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` |  | Boolean |  | 91 |
| `buildToolErrorResult` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool<br>error: String | ToolResult |  | 95 |
| `parseProxyInvocation` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool<br>requireQualifiedTarget: Boolean | Pair<ParsedProxyInvocation?, ToolResult?> |  | 104 |
| `resolveCurrentRoleCardToolAccess` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` |  | ResolvedCharacterCardToolAccess |  | 186 |
| `isProxyTargetAllowedForRoleCard` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | targetToolName: String<br>forwardedParameters: List<ToolParameter><br>roleCardToolAccess: ResolvedCharacterCardToolAccess | Boolean |  | 198 |
| `executeProxyTargetWithPermissionCheck` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | targetToolName: String<br>forwardedParameters: List<ToolParameter><br>useEnglish: Boolean | ToolResult |  | 222 |
| `invoke` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool | ToolResult |  | 340 |
| `invokeAndStream` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool | kotlinx.coroutines.flow.Flow<ToolResult> |  | 345 |
| `invoke` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool | ToolResult |  | 1716 |
| `invokeAndStream` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool | kotlinx.coroutines.flow.Flow<ToolResult> |  | 1720 |
| `invoke` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool | ToolResult |  | 1976 |
| `invokeAndStream` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool | kotlinx.coroutines.flow.Flow<ToolResult> |  | 1980 |
| `invoke` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool | ToolResult |  | 2133 |
| `invokeAndStream` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | tool: AITool | kotlinx.coroutines.flow.Flow<ToolResult> |  | 2137 |
| `ToolResultData.toString` | `ToolResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String | Converts the structured data to a string representation | 19 |
| `ToolResultData.toJson` | `ToolResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 20 |
| `BooleanResultData.toString` | `BooleanResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 33 |
| `StringResultData.toString` | `StringResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 38 |
| `SleepResultData.toString` | `SleepResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 46 |
| `SandboxScriptExecutionResultData.toString` | `SandboxScriptExecutionResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 66 |
| `EnvironmentVariableReadResultData.toString` | `EnvironmentVariableReadResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 81 |
| `EnvironmentVariableWriteResultData.toString` | `EnvironmentVariableWriteResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 98 |
| `SandboxPackagesResultData.toString` | `SandboxPackagesResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 133 |
| `SandboxPackageUpdateResultData.toString` | `SandboxPackageUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 146 |
| `McpRestartWithLogsResultData.toString` | `McpRestartWithLogsResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 176 |
| `ScriptExecutionTraceData.toString` | `ScriptExecutionTraceData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 189 |
| `IntResultData.toString` | `IntResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 207 |
| `BinaryResultData.toString` | `BinaryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 212 |
| `BinaryResultData.equals` | `BinaryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | other: Any? | Boolean |  | 214 |
| `BinaryResultData.hashCode` | `BinaryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | Int |  | 221 |
| `FilePartContentData.toString` | `FilePartContentData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 240 |
| `ADBResultData.toString` | `ADBResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 251 |
| `TerminalCommandResultData.toString` | `TerminalCommandResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 272 |
| `TerminalStreamEventData.toString` | `TerminalStreamEventData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 298 |
| `HiddenTerminalCommandResultData.toString` | `HiddenTerminalCommandResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 316 |
| `MusicPlaybackResultData.toString` | `MusicPlaybackResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 348 |
| `CalculationResultData.toString` | `CalculationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 377 |
| `DateResultData.toString` | `DateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 395 |
| `ConnectionResultData.toString` | `ConnectionResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 407 |
| `DirectoryListingData.toString` | `DirectoryListingData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 430 |
| `FileContentData.toString` | `FileContentData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 456 |
| `BinaryFileContentData.toString` | `BinaryFileContentData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 471 |
| `FileExistsData.toString` | `FileExistsData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 487 |
| `FileInfoData.toString` | `FileInfoData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 513 |
| `FileOperationData.toString` | `FileOperationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 541 |
| `FileApplyResultData.buildRequestContent` | `FileApplyResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 553 |
| `FileApplyResultData.extractDiffSummaryLine` | `FileApplyResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String? |  | 562 |
| `FileApplyResultData.toString` | `FileApplyResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 575 |
| `HttpResponseData.toString` | `HttpResponseData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 613 |
| `HttpStreamEventData.toString` | `HttpStreamEventData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 651 |
| `SystemSettingData.toString` | `SystemSettingData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 665 |
| `AppOperationData.toString` | `AppOperationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 678 |
| `AppListData.toString` | `AppListData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 693 |
| `AppUsageTimeResultData.toString` | `AppUsageTimeResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 720 |
| `AppUsageTimeResultData.formatDuration` | `AppUsageTimeResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | durationMs: Long | String |  | 742 |
| `BluetoothStateData.toString` | `BluetoothStateData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 763 |
| `BluetoothBondedDevicesData.toString` | `BluetoothBondedDevicesData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 776 |
| `BluetoothScanResultData.toString` | `BluetoothScanResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 802 |
| `BluetoothSessionData.toString` | `BluetoothSessionData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 830 |
| `BluetoothTransferData.toString` | `BluetoothTransferData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 839 |
| `BluetoothReadData.toString` | `BluetoothReadData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 850 |
| `BluetoothBleServicesData.toString` | `BluetoothBleServicesData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 860 |
| `BluetoothBleNotificationData.toString` | `BluetoothBleNotificationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 888 |
| `SimplifiedUINode.toTreeString` | `SimplifiedUINode` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | indent: String? | String |  | 916 |
| `SimplifiedUINode.shouldKeepNode` | `SimplifiedUINode` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | Boolean |  | 951 |
| `UIPageResultData.toString` | `UIPageResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 970 |
| `UIActionResultData.toString` | `UIActionResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 989 |
| `CombinedOperationResultData.toString` | `CombinedOperationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1001 |
| `DeviceInfoResultData.toString` | `DeviceInfoResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1026 |
| `IntentResultData.toString` | `IntentResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1128 |
| `FindFilesResultData.toString` | `FindFilesResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1153 |
| `FFmpegResultData.toString` | `FFmpegResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1202 |
| `LocationData.toString` | `LocationData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1286 |
| `ComputerPageInfoNode.toTreeString` | `ComputerPageInfoNode` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | level: Int? | String |  | 1322 |
| `ComputerDesktopActionResultData.toString` | `ComputerDesktopActionResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1354 |
| `MemoryQueryResultData.toString` | `MemoryQueryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1393 |
| `AutomationConfigSearchResult.toString` | `AutomationConfigSearchResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1449 |
| `AutomationPlanParametersResult.toString` | `AutomationPlanParametersResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1498 |
| `AutomationExecutionResult.toString` | `AutomationExecutionResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1545 |
| `AutomationFunctionListResult.toString` | `AutomationFunctionListResult` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1591 |
| `TerminalSessionCreationResultData.toString` | `TerminalSessionCreationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1620 |
| `TerminalSessionCloseResultData.toString` | `TerminalSessionCloseResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1636 |
| `TerminalSessionScreenResultData.toString` | `TerminalSessionScreenResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1647 |
| `GrepResultData.parsePreNumberedLineNumber` | `GrepResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | line: String | Int? |  | 1684 |
| `GrepResultData.markPreNumberedContextLine` | `GrepResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | line: String | String |  | 1691 |
| `GrepResultData.toString` | `GrepResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1702 |
| `WorkflowResultData.toString` | `WorkflowResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1796 |
| `WorkflowListResultData.toString` | `WorkflowListResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1821 |
| `WorkflowListResultData.empty` | `WorkflowListResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | Unit | 创建一个空的WorkflowListResultData，用于错误情况 | 1845 |
| `WorkflowDetailResultData.toString` | `WorkflowDetailResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1869 |
| `WorkflowDetailResultData.empty` | `WorkflowDetailResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | Unit | 创建一个空的WorkflowDetailResultData，用于错误情况 | 1951 |
| `ChatServiceStartResultData.toString` | `ChatServiceStartResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1975 |
| `ChatCreationResultData.toString` | `ChatCreationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 1990 |
| `ChatListResultData.toString` | `ChatListResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2018 |
| `ChatFindResultData.toString` | `ChatFindResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2060 |
| `AgentStatusResultData.toString` | `AgentStatusResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2078 |
| `ChatSwitchResultData.toString` | `ChatSwitchResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2091 |
| `ChatTitleUpdateResultData.toString` | `ChatTitleUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2107 |
| `ChatDeleteResultData.toString` | `ChatDeleteResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2118 |
| `ChatMessagesResultData.toString` | `ChatMessagesResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2143 |
| `ChatCallResultData.toString` | `ChatCallResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2166 |
| `CharacterCardListResultData.toString` | `CharacterCardListResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2192 |
| `MessageSendResultData.toString` | `MessageSendResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2223 |
| `MessageSendStreamEventData.toString` | `MessageSendStreamEventData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2254 |
| `MemoryLinkResultData.toString` | `MemoryLinkResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2272 |
| `MemoryLinkQueryResultData.toString` | `MemoryLinkQueryResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2293 |
| `SpeechServicesConfigResultData.toString` | `SpeechServicesConfigResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2354 |
| `SpeechServicesUpdateResultData.toString` | `SpeechServicesUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2369 |
| `SpeechServicesTtsPlaybackTestResultData.toString` | `SpeechServicesTtsPlaybackTestResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2391 |
| `CharacterCardsResultData.toString` | `CharacterCardsResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2437 |
| `CharacterCardResultData.toString` | `CharacterCardResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2448 |
| `CharacterCardCreateResultData.toString` | `CharacterCardCreateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2461 |
| `CharacterCardUpdateResultData.toString` | `CharacterCardUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2474 |
| `CharacterCardDeleteResultData.toString` | `CharacterCardDeleteResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2486 |
| `CharacterCardActivationResultData.toString` | `CharacterCardActivationResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2496 |
| `CharacterCardImportResultData.toString` | `CharacterCardImportResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2508 |
| `CharacterCardExportResultData.toString` | `CharacterCardExportResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2519 |
| `ModelConfigsResultData.toString` | `ModelConfigsResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2603 |
| `ModelConfigCreateResultData.toString` | `ModelConfigCreateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2615 |
| `ModelConfigUpdateResultData.toString` | `ModelConfigUpdateResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2628 |
| `ModelConfigDeleteResultData.toString` | `ModelConfigDeleteResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2641 |
| `FunctionModelConfigsResultData.toString` | `FunctionModelConfigsResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2652 |
| `FunctionModelConfigResultData.toString` | `FunctionModelConfigResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2669 |
| `FunctionModelBindingResultData.toString` | `FunctionModelBindingResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2684 |
| `ModelConfigConnectionTestResultData.toString` | `ModelConfigConnectionTestResultData` | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` |  | String |  | 2715 |
| `GrepResultDataTest.grepResult` | `GrepResultDataTest` | `com.ai.assistance.operit.core.tools` | `GrepResultDataTest.kt` | lineNumber: Int<br>lineContent: String<br>matchContext: String? | GrepResultData |  | 17 ⚑ |
| `GrepResultDataTest.renderedNumberedLines` | `GrepResultDataTest` | `com.ai.assistance.operit.core.tools` | `GrepResultDataTest.kt` | output: String | List<Triple<Int, Boolean, String>> | Extracts (lineNumber, isMarked, text) for every rendered "N\|" output line. | 45 ⚑ |
| `GrepResultDataTest.assertNoInvalidLineNumbers` | `GrepResultDataTest` | `com.ai.assistance.operit.core.tools` | `GrepResultDataTest.kt` | output: String | Unit |  | 59 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `apiEndpoint` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | String, |  | 2531 |
| `apiKeyPoolCount` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int |  | 2581 |
| `apiKeyPreview` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | String, |  | 2535 |
| `apiKeySet` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2534 |
| `apiProviderType` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | String, |  | 2529 |
| `apiProviderTypeId` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | String, |  | 2530 |
| `chatManagerTool` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | inferred | 对话管理工具 | 1609 |
| `contextLength` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Float, |  | 2554 |
| `customHeaders` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | String, |  | 2553 |
| `customParameters` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | String, |  | 2551 |
| `enableClaude1hPromptCache` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2576 |
| `enableDirectAudioProcessing` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2573 |
| `enableDirectImageProcessing` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2572 |
| `enableDirectVideoProcessing` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2574 |
| `enableGoogleSearch` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2575 |
| `enableMaxContextMode` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2556 |
| `enableSummary` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2558 |
| `enableSummaryByMessageCount` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2559 |
| `enableToolCall` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2577 |
| `EnvVarSerializer.delegateSerializer` | `EnvVarSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | inferred |  | 217 |
| `EnvVarSerializer.descriptor` | `EnvVarSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | SerialDescriptor |  | 219 |
| `fileSystemTools` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | inferred | 文件系统工具 | 1772 |
| `frequencyPenalty` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Float, |  | 2547 |
| `frequencyPenaltyEnabled` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2546 |
| `hasCustomHeaders` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2552 |
| `hasCustomParameters` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2550 |
| `httpTools` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | inferred | HTTP请求工具 | 1964 |
| `id` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | String, |  | 2527 |
| `llamaBatchSize` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2565 |
| `llamaContextSize` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2564 |
| `llamaFlashAttention` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2569 |
| `llamaGpuLayers` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2567 |
| `llamaKvUnified` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2570 |
| `llamaOffloadKqv` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2571 |
| `llamaThreadCount` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2563 |
| `llamaUBatchSize` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2566 |
| `llamaUseMmap` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2568 |
| `LocalizedTextSerializer.descriptor` | `LocalizedTextSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | SerialDescriptor |  | 131 |
| `maxConcurrentRequests` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2579 |
| `maxContextLength` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Float, |  | 2555 |
| `maxTokens` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2537 |
| `maxTokensEnabled` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2536 |
| `mnnForwardType` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2561 |
| `mnnThreadCount` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2562 |
| `modelList` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | List<String>, |  | 2533 |
| `modelName` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | String, |  | 2532 |
| `musicPlaybackTools` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | inferred | 音乐播放工具 | 406 |
| `name` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | String, |  | 2528 |
| `presencePenalty` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Float, |  | 2545 |
| `presencePenaltyEnabled` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2544 |
| `repetitionPenalty` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Float, |  | 2549 |
| `repetitionPenaltyEnabled` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2548 |
| `requestLimitPerMinute` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2578 |
| `StringOrStringListSerializer.delegateSerializer` | `StringOrStringListSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | inferred |  | 172 |
| `StringOrStringListSerializer.descriptor` | `StringOrStringListSerializer` | `com.ai.assistance.operit.core.tools` | `ToolPackage.kt` | SerialDescriptor |  | 174 |
| `summaryMessageCountThreshold` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2560 |
| `summaryTokenThreshold` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Float, |  | 2557 |
| `systemOperationTools` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | inferred | 系统操作工具 | 2273 |
| `temperature` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Float, |  | 2539 |
| `temperatureEnabled` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2538 |
| `ToolExecutionLimits.DEFAULT_FILE_READ_PART_LINES` | `ToolExecutionLimits` | `com.ai.assistance.operit.core.tools` | `ToolExecutionLimits.kt` | inferred |  | 5 |
| `ToolExecutionLimits.MAX_FILE_READ_BYTES` | `ToolExecutionLimits` | `com.ai.assistance.operit.core.tools` | `ToolExecutionLimits.kt` | inferred |  | 4 |
| `ToolExecutionLimits.MAX_SINGLE_TOOL_RESULT_MESSAGE_CHARS` | `ToolExecutionLimits` | `com.ai.assistance.operit.core.tools` | `ToolExecutionLimits.kt` | inferred | Maximum serialized size of one tool result sent back to the model. | 8 |
| `ToolExecutionLimits.MAX_TEXT_RESULT_LENGTH` | `ToolExecutionLimits` | `com.ai.assistance.operit.core.tools` | `ToolExecutionLimits.kt` | inferred |  | 6 |
| `ToolProgressBus._progress` | `ToolProgressBus` | `com.ai.assistance.operit.core.tools` | `ToolProgressBus.kt` | inferred |  | 18 |
| `ToolProgressBus.progress` | `ToolProgressBus` | `com.ai.assistance.operit.core.tools` | `ToolProgressBus.kt` | StateFlow<ToolProgressEvent?> |  | 19 |
| `ToolProgressBus.SUMMARY_PROGRESS_TOOL_NAME` | `ToolProgressBus` | `com.ai.assistance.operit.core.tools` | `ToolProgressBus.kt` | String |  | 16 |
| `topK` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Int, |  | 2543 |
| `topKEnabled` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2542 |
| `topP` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Float, |  | 2541 |
| `topPEnabled` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2540 |
| `uiTools` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | inferred | UI自动化工具 | 1901 |
| `useMultipleApiKeys` | — | `com.ai.assistance.operit.core.tools` | `ToolResultDataClasses.kt` | Boolean, |  | 2580 |
| `workflowTools` | — | `com.ai.assistance.operit.core.tools` | `ToolRegistration.kt` | inferred | 工作流工具 | 1514 |
