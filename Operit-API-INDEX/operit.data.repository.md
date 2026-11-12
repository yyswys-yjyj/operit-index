# operit.data.repository

> 函数 346 · 类型 34 · 顶层常量 34 · 共 414 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `AddedMessageVariant` | `AddedMessageVariant` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | class AddedMessageVariant(val selectedVariantIndex: Int, val message: ChatMessage) |  | 87 |
| `AvatarConfig` | `AvatarConfig` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class AvatarConfig(val id: String, val name: String, val type: AvatarType, val isBuiltIn: Boolean, /** Type-specific data: , e.g.: , file paths: , settings. */ val data: Map<Str… | Data class representing the persisted configuration of a single avatar. This is what gets… | 33 |
| `AvatarConfigDecodeResult` | `AvatarConfigDecodeResult` | `com.ai.assistance.operit.data.repository` | `AvatarConfigPersistence.kt` | class AvatarConfigDecodeResult(val configs: List<AvatarConfig>, val invalidEntryIndexes: List<Int>) |  | 8 |
| `AvatarConfigPersistenceTest` | `AvatarConfigPersistenceTest` | `com.ai.assistance.operit.data.repository` | `AvatarConfigPersistenceTest.kt` | class AvatarConfigPersistenceTest |  | 8 |
| `AvatarInstanceSettings` | `AvatarInstanceSettings` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class AvatarInstanceSettings(val scale: Float, val translateX: Float, val translateY: Float, val customSettings: Map<String, Float>) | Data class for avatar instance settings like scale and position. | 179 |
| `AvatarPersistenceDelegate` | `AvatarPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | interface AvatarPersistenceDelegate | Defines a contract for type-specific avatar persistence logic. Each supported AvatarType … | 198 |
| `AvatarRepository` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class AvatarRepository(private val context: Context, private val modelFactory: AvatarModelFactory) | A generic repository for managing all types of virtual avatars. It handles loading, savin… | 497 |
| `AvatarRepository.AvatarImportKind` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class AvatarImportKind |  | 821 |
| `AvatarSettings` | `AvatarSettings` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class AvatarSettings(val currentAvatarId: String?, val isVoiceCallAvatarEnabled: Boolean) | Data class for global avatar settings. | 189 |
| `ChatExportProgress` | `ChatExportProgress` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | class ChatExportProgress(val isLongText: Boolean, val progress: Float, val processedCharacters: Long, val totalCharacters: Long) |  | 75 |
| `ChatExportResult` | `ChatExportResult` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | class ChatExportResult(val filePath: String, val chatCount: Int) |  | 82 |
| `ChatHistoryManager` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | class ChatHistoryManager(private val context: Context) |  | 92 |
| `ChatHistoryManager.ImportCounters` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | class ImportCounters(var newCount: Int, var updatedCount: Int, var skippedCount: Int) |  | 127 |
| `ChatHistoryManager.PreferencesKeys` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | object PreferencesKeys | DataStore键 | 454 |
| `ChatHistoryManager.StreamImportedChat` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | interface StreamImportedChat |  | 133 |
| `ChatHistoryManager.StreamImportedChat.Archive` | `StreamImportedChat` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | class Archive(val chat: OperitArchivedChat) : StreamImportedChat data class Legacy |  | 134 |
| `ChatImportResult` | `ChatImportResult` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | class ChatImportResult(val new: Int, val updated: Int, val skipped: Int) |  | 2888 |
| `CustomEmojiRepository` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | class CustomEmojiRepository(private val context: Context) | 自定义表情 Repository 管理按角色卡/角色组隔离的表情文件和数据持久化。 - 文件存储在 filesDir/custom_emoji/<target_scope>/{c… | 28 |
| `DragonBonesPersistenceDelegate` | `DragonBonesPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class DragonBonesPersistenceDelegate : AvatarPersistenceDelegate | Persistence delegate for DragonBones models. | 214 |
| `FbxPersistenceDelegate` | `FbxPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class FbxPersistenceDelegate(private val inspectModel: (String) -> FbxModelInfo?) : AvatarPersistenceDelegate |  | 431 |
| `GltfPersistenceDelegate` | `GltfPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class GltfPersistenceDelegate : AvatarPersistenceDelegate |  | 391 |
| `MemoryAutoSaveCandidateRepository` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` | class MemoryAutoSaveCandidateRepository(context: Context, profileId: String) |  | 11 |
| `MemoryRepository` | `MemoryRepository` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | class MemoryRepository(private val context: Context, profileId: String) | Repository for handling Memory data operations. It abstracts the data source (ObjectBox) … | 55 |
| `MmdPersistenceDelegate` | `MmdPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class MmdPersistenceDelegate : AvatarPersistenceDelegate |  | 347 |
| `Mp4PersistenceDelegate` | `Mp4PersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class Mp4PersistenceDelegate : AvatarPersistenceDelegate |  | 310 |
| `PersistedAvatarConfig` | `PersistedAvatarConfig` | `com.ai.assistance.operit.data.repository` | `AvatarConfigPersistence.kt` | class PersistedAvatarConfig(val id: String?, val name: String?, val type: AvatarType?, val isBuiltIn: Boolean?, val data: Map<String, Any>?) |  | 13 |
| `ResolvedSearchWeights` | `ResolvedSearchWeights` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | class ResolvedSearchWeights(val scoreMode: MemoryScoreMode, val effectiveKeywordWeight: Double, val effectiveTagWeight: Double, val effectiveSemanticWeight: Float, val effectiveEdgeWeigh… |  | 180 |
| `SearchComputationResult` | `SearchComputationResult` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | class SearchComputationResult(val memories: List<Memory>, val debug: MemorySearchDebugInfo) |  | 175 |
| `SearchScoreParts` | `SearchScoreParts` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | class SearchScoreParts(var matchedKeywordTokenCount: Int, var keywordScore: Double, var tagScore: Double, var reverseContainmentScore: Double, var semanticScore: Double, var edgeSco… |  | 166 |
| `TitleMatchCandidate` | `TitleMatchCandidate` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | class TitleMatchCandidate(val memory: Memory, val matchedTokenCount: Int) |  | 161 |
| `UIHierarchyManager` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | object UIHierarchyManager | UI层次结构管理器 负责与独立的无障碍服务提供者App进行通信，获取UI层次结构。 | 40 |
| `WebPPersistenceDelegate` | `WebPPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | class WebPPersistenceDelegate : AvatarPersistenceDelegate | Persistence delegate for WebP models. | 273 |
| `WorkflowRepository` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | class WorkflowRepository(private val context: Context) | 工作流仓库 负责工作流的持久化存储和管理 | 48 |
| `WorkflowRepository.WorkflowStorageException` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | class WorkflowStorageException(message: String, cause: Throwable?) : IOException |  | 130 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `decodePersistedAvatarConfigs` | — | `com.ai.assistance.operit.data.repository` | `AvatarConfigPersistence.kt` | json: String<br>gson: Gson | AvatarConfigDecodeResult |  | 21 |
| `AvatarConfig.getBasePath` | `AvatarConfig` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | String? |  | 41 |
| `getEmotionAnimationMapping` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | Map<AvatarEmotion, String> |  | 50 |
| `getMoodAnimationMapping` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | Map<String, String> |  | 70 |
| `getCustomMoodDefinitions` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | List<AvatarCustomMoodDefinition> |  | 83 |
| `withEmotionAnimationMapping` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | mapping: Map<AvatarEmotion, String> | AvatarConfig |  | 98 |
| `withMoodAnimationMapping` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | mapping: Map<String, String> | AvatarConfig |  | 114 |
| `withCustomMoodDefinitions` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | definitions: List<AvatarCustomMoodDefinition> | AvatarConfig |  | 134 |
| `normalizeAvatarPath` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | path: String | String |  | 154 |
| `buildAvatarConfigId` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | type: AvatarType<br>directory: File<br>isBuiltIn: Boolean | String |  | 161 |
| `avatarSourceKey` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | config: AvatarConfig | String? |  | 171 |
| `AvatarPersistenceDelegate.scanDirectory` | `AvatarPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | directory: File<br>isBuiltIn: Boolean | List<AvatarConfig> | Scans a directory to find and parse model configurations for this delegate's avatar type. | 208 |
| `DragonBonesPersistenceDelegate.scanDirectory` | `DragonBonesPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | directory: File<br>isBuiltIn: Boolean | List<AvatarConfig> |  | 217 |
| `WebPPersistenceDelegate.scanDirectory` | `WebPPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | directory: File<br>isBuiltIn: Boolean | List<AvatarConfig> |  | 276 |
| `Mp4PersistenceDelegate.scanDirectory` | `Mp4PersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | directory: File<br>isBuiltIn: Boolean | List<AvatarConfig> |  | 313 |
| `MmdPersistenceDelegate.scanDirectory` | `MmdPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | directory: File<br>isBuiltIn: Boolean | List<AvatarConfig> |  | 350 |
| `GltfPersistenceDelegate.scanDirectory` | `GltfPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | directory: File<br>isBuiltIn: Boolean | List<AvatarConfig> |  | 394 |
| `FbxPersistenceDelegate.scanDirectory` | `FbxPersistenceDelegate` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | directory: File<br>isBuiltIn: Boolean | List<AvatarConfig> |  | 436 |
| `AvatarRepository.getInstance` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | context: Context<br>modelFactory: AvatarModelFactory | AvatarRepository |  | 518 |
| `AvatarRepository.synchronizeAssets` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | Unit |  | 559 |
| `AvatarRepository.loadAvatars` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | Unit |  | 586 |
| `AvatarRepository.scanUserAvatarDirectory` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | List<AvatarConfig> |  | 632 |
| `AvatarRepository.isPathFromAssets` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | path: String | Boolean |  | 642 |
| `AvatarRepository.refreshAvatars` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | Unit |  | 648 |
| `AvatarRepository.switchAvatar` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String | Unit |  | 652 |
| `AvatarRepository.updateVoiceCallAvatarEnabled` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | enabled: Boolean | Unit |  | 660 |
| `AvatarRepository.updateCurrentAvatar` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | targetId: String? | Unit |  | 669 |
| `AvatarRepository.deleteAvatar` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String | Boolean |  | 690 |
| `AvatarRepository.renameAvatar` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String<br>newName: String | Boolean |  | 727 |
| `AvatarRepository.updateAvatarSettings` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String<br>newSettings: AvatarInstanceSettings | Unit |  | 756 |
| `AvatarRepository.updateAvatarEmotionAnimationMapping` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String<br>mapping: Map<AvatarEmotion, String> | Unit |  | 763 |
| `AvatarRepository.updateAvatarMoodAnimationMapping` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String<br>mapping: Map<String, String> | Unit |  | 772 |
| `AvatarRepository.updateAvatarCustomMoodDefinitions` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String<br>definitions: List<AvatarCustomMoodDefinition> | Unit |  | 781 |
| `AvatarRepository.updateAvatarMoodConfig` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String<br>definitions: List<AvatarCustomMoodDefinition><br>moodAnimationMapping: Map<String, String> | Unit |  | 790 |
| `AvatarRepository.getAvatarSettings` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String | AvatarInstanceSettings |  | 801 |
| `AvatarRepository.updateAvatarConfig` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | avatarId: String<br>transform: (AvatarConfig) -> AvatarConfig | Unit |  | 805 |
| `AvatarRepository.importAvatarFromUri` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | uri: Uri | Boolean |  | 827 |
| `AvatarRepository.detectImportKind` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | uri: Uri | AvatarImportKind |  | 838 |
| `AvatarRepository.resolveImportDisplayName` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | uri: Uri | String? |  | 867 |
| `AvatarRepository.sanitizeImportFileName` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | rawName: String | String |  | 890 |
| `AvatarRepository.sanitizeImportDirectoryName` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | rawName: String | String |  | 901 |
| `AvatarRepository.createUniqueImportDirectory` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | baseName: String | File |  | 911 |
| `AvatarRepository.importAvatarFromModelFile` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | uri: Uri | Boolean |  | 925 |
| `AvatarRepository.importAvatarFromZip` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | uri: Uri | Boolean |  | 995 |
| `AvatarRepository.loadConfigsFromPrefs` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | List<AvatarConfig> |  | 1149 |
| `AvatarRepository.saveConfigsToPrefs` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | configs: List<AvatarConfig> | Unit |  | 1167 |
| `AvatarRepository.loadInstanceSettingsFromPrefs` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | Map<String, AvatarInstanceSettings> |  | 1172 |
| `AvatarRepository.saveInstanceSettingsToPrefs` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | settings: Map<String, AvatarInstanceSettings> | Unit |  | 1183 |
| `AvatarRepository.loadSettingsFromPrefs` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` |  | AvatarSettings |  | 1188 |
| `AvatarRepository.saveSettingsToPrefs` | `AvatarRepository` | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | settings: AvatarSettings | Unit |  | 1201 |
| `ChatHistoryManager.getInstance` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | context: Context | ChatHistoryManager |  | 103 |
| `ChatHistoryManager.StreamImportedChat.hydrateMessages` | `StreamImportedChat` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | messageEntities: List<MessageEntity><br>variants: List<MessageVariantEntity> | List<ChatMessage> |  | 139 |
| `ChatHistoryManager.hydrateMessages` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>messageEntities: List<MessageEntity> | List<ChatMessage> |  | 161 |
| `ChatHistoryManager.loadDisplayHistory` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatHistory: ChatHistory | ChatHistory |  | 173 |
| `ChatHistoryManager.loadDisplayHistories` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatHistories: List<ChatHistory> | List<ChatHistory> |  | 178 |
| `ChatHistoryManager.buildOperitArchivedChat` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatHistory: ChatHistory | OperitArchivedChat |  | 186 |
| `ChatHistoryManager.exportOperitArchiveJsonStream` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | file: File<br>chatHistories: List<ChatHistory> | Unit |  | 204 |
| `ChatHistoryManager.exportOperitArchiveCsvStream` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | file: File<br>chatHistories: List<ChatHistory> | Unit |  | 246 |
| `ChatHistoryManager.decodeStreamElement` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | reader: JsonReader<br>decode: (String) -> T | T |  | 286 |
| `ChatHistoryManager.consumeImportedChat` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | imported: StreamImportedChat<br>existingIds: MutableSet<String><br>counters: ImportCounters<br>importedIndex: Int | Unit |  | 294 |
| `ChatHistoryManager.importOperitChatHistoriesStream` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | inputStream: InputStream<br>existingIds: MutableSet<String> | ChatImportResult |  | 355 |
| `ChatHistoryManager.chatMutex` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | Mutex |  | 449 |
| `ChatHistoryManager.toChatHistory` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` |  | ChatHistory | 辅助函数：将ChatEntity转换为ChatHistory | 459 |
| `ChatHistoryManager.getChatHistorySnapshot` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | ChatHistory? | Reads persisted metadata for a specific chat without subscribing to the UI cache. | 510 |
| `ChatHistoryManager.getTotalChatCount` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` |  | Int |  | 515 |
| `ChatHistoryManager.getTotalMessageCount` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` |  | Int |  | 519 |
| `ChatHistoryManager.getMessageCountsByChatId` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` |  | Map<String, Int> |  | 523 |
| `ChatHistoryManager.getChatHistoriesByCharacterCard` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | characterCardName: String<br>isDefault: Boolean | Flow<List<ChatHistory>> | 根据角色卡过滤聊天历史 | 546 |
| `ChatHistoryManager.validateArchivedMessageVariants` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | message: ChatMessage<br>variants: List<OperitArchivedMessageVariant> | Unit |  | 585 |
| `ChatHistoryManager.saveChatHistoryInternal` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | history: ChatHistory<br>variantsByTimestamp: Map<Long, List<OperitArchivedMessag…? | Unit |  | 615 |
| `ChatHistoryManager.saveChatHistory` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | history: ChatHistory | Unit | 保存聊天历史 | 675 |
| `ChatHistoryManager.saveArchivedChat` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | history: OperitArchivedChat | Unit |  | 679 |
| `ChatHistoryManager.updateChatLocked` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>locked: Boolean | Unit | 更新聊天锁定状态 | 688 |
| `ChatHistoryManager.updateChatPinned` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>pinned: Boolean | Unit | 更新聊天置顶状态 | 700 |
| `ChatHistoryManager.persistMessageLocked` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>messageToPersist: ChatMessage | ChatMessage |  | 711 |
| `ChatHistoryManager.resolveAnchoredMessageLocked` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>message: ChatMessage<br>beforeTimestamp: Long?<br>afterTimestamp: Long? | ChatMessage? |  | 735 |
| `ChatHistoryManager.addSummaryMessageBetweenSliceNeighbors` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>message: ChatMessage<br>beforeTimestamp: Long?<br>afterTimestamp: Long? | ChatMessage? |  | 836 |
| `ChatHistoryManager.addMessage` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>message: ChatMessage | ChatMessage | 添加单条消息，并返回最终持久化的消息 | 893 |
| `ChatHistoryManager.updateChatOrderAndGroup` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | updatedHistories: List<ChatHistory> | Unit | 批量更新聊天记录的顺序和分组 | 908 |
| `ChatHistoryManager.updateGroupName` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | oldName: String<br>newName: String<br>characterCardName: String? | Unit | 重命名分组 | 935 |
| `ChatHistoryManager.deleteGroup` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | groupName: String<br>deleteChats: Boolean<br>characterCardName: String? | Unit | 删除分组 | 962 |
| `ChatHistoryManager.deleteMessage` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>timestamp: Long | Unit | 删除单条消息. | 1000 |
| `ChatHistoryManager.deleteMessageVariant` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>messageTimestamp: Long<br>variantIndex: Int | Unit |  | 1026 |
| `ChatHistoryManager.updateMessage` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>message: ChatMessage | Unit | 更新现有消息 | 1137 |
| `ChatHistoryManager.setMessageFavorite` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>timestamp: Long<br>isFavorite: Boolean | Unit |  | 1235 |
| `ChatHistoryManager.addMessageVariant` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>messageTimestamp: Long<br>message: ChatMessage | AddedMessageVariant |  | 1255 |
| `ChatHistoryManager.selectMessageVariant` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>messageTimestamp: Long<br>selectedVariantIndex: Int | Unit |  | 1296 |
| `ChatHistoryManager.deleteMessagesFrom` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>timestamp: Long | Unit | 从数据库中删除指定时间戳之后的所有消息。 这需要您在MessageDao中添加相应的@Query。 示例: ``` | 1323 |
| `ChatHistoryManager.clearChatMessages` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | Unit | 清除一个聊天中的所有消息，但保留聊天本身。 这需要您在MessageDao中添加相应的@Query。 ``` | 1357 |
| `ChatHistoryManager.updateChatTitle` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>title: String | Unit | 更新聊天标题 | 1381 |
| `ChatHistoryManager.updateChatCharacterCardName` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>characterCardName: String? | Unit | 更新聊天绑定的角色卡 | 1393 |
| `ChatHistoryManager.updateChatTokenCounts` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>inputTokens: Long<br>outputTokens: Long<br>currentWindowSize: Long | Unit | 更新聊天的token计数 | 1405 |
| `ChatHistoryManager.setCurrentChatId` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | Unit | 设置当前聊天ID | 1431 |
| `ChatHistoryManager.clearCurrentChatId` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` |  | Unit | 清除当前聊天ID | 1438 |
| `ChatHistoryManager.chatExists` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | Boolean | 检查聊天是否存在 | 1445 |
| `ChatHistoryManager.canDeleteChatHistory` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | Boolean |  | 1456 |
| `ChatHistoryManager.deleteChatHistory` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | Boolean | 删除聊天历史 | 1469 |
| `ChatHistoryManager.createNewChat` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | group: String??<br>inheritGroupFromChatId: String??<br>characterCardName: String??<br>characterGroupId: String??<br>setAsCurrentChat: Boolean? | ChatHistory | 创建新对话 | 1498 |
| `ChatHistoryManager.updateChatWorkspace` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>workspace: String?<br>workspaceEnv: String? | Unit | 更新聊天工作区 | 1549 |
| `ChatHistoryManager.renameManagedWorkspace` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>newWorkspaceName: String | WorkspaceRenameResult |  | 1560 |
| `ChatHistoryManager.updateChatGroup` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>group: String? | Unit | 更新聊天分组 | 1627 |
| `ChatHistoryManager.getChatTitle` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | String? |  | 1638 |
| `ChatHistoryManager.loadChatMessages` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | List<ChatMessage> | 直接加载聊天消息 | 1650 |
| `ChatHistoryManager.loadChatMessages` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>order: String??<br>limit: Int?? | List<ChatMessage> |  | 1664 |
| `ChatHistoryManager.loadChatMessagesRange` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>order: String??<br>start: Int<br>end: Int | List<ChatMessage> |  | 1700 |
| `ChatHistoryManager.searchChatIdsByContent` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | query: String | Set<String> | 搜索包含特定关键词的聊天ID列表 | 1725 |
| `ChatHistoryManager.createBranch` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | parentChatId: String<br>upToMessageTimestamp: Long?? | ChatHistory | 创建对话分支 | 1753 |
| `ChatHistoryManager.getBranches` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | parentChatId: String | List<ChatHistory> | 获取指定对话的所有分支 | 1818 |
| `ChatHistoryManager.getBranchesFlow` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | parentChatId: String | Flow<List<ChatHistory>> | 获取指定对话的所有分支（Flow版本） | 1861 |
| `ChatHistoryManager.exportChatHistoriesToDownloads` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | selectedChatIds: Set<String><br>format: ExportFormat<br>onProgress: ((ChatExportProgress) -> Unit)? | ChatExportResult? | 导出指定聊天记录到「下载/Operit」目录。 | 1900 |
| `ChatHistoryManager.exportLongTextHistories` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | file: File<br>format: ExportFormat<br>chatHistories: List<ChatHistory><br>totalMessageCount: Int<br>totalTextCharacters: Long<br>onProgress: ((ChatExportProgress) -> Unit)? | Unit |  | 2054 |
| `ChatHistoryManager.reportProgress` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | force: Boolean? | Unit |  | 2067 |
| `ChatHistoryManager.importChatHistoriesFromUri` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | uri: Uri<br>format: ChatFormat | ChatImportResult | 从指定URI导入聊天记录（指定格式） | 2170 |
| `ChatHistoryManager.parseLegacyOperitChatHistories` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | content: String | List<ChatHistory> |  | 2271 |
| `ChatHistoryManager.convertToOperitFormat` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | content: String<br>format: ChatFormat | List<ChatHistory> |  | 2284 |
| `ChatHistoryManager.clearCharacterCardBinding` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | characterCardName: String | Unit | 清理绑定已删除角色卡的对话（将characterCardName设为null） | 2332 |
| `ChatHistoryManager.reassignChatsToCharacterCard` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | sourceCharacterCardName: String?<br>targetCharacterCardName: String | Int | 将指定角色卡或未绑定的对话转移到新的角色卡 | 2347 |
| `ChatHistoryManager.getLatestSummaryTimestamp` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | Long? |  | 2374 |
| `ChatHistoryManager.loadMessagesAfterLatestSummaryInRange` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>beforeTimestampExclusive: Long??<br>upToTimestampInclusive: Long?? | List<ChatMessage> |  | 2385 |
| `ChatHistoryManager.hasUserMessage` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | Boolean |  | 2421 |
| `ChatHistoryManager.loadRuntimeChatMessages` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String | List<ChatMessage> |  | 2432 |
| `ChatHistoryManager.loadRuntimeChatMessagesUpTo` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>upToTimestampInclusive: Long | List<ChatMessage> |  | 2450 |
| `ChatHistoryManager.loadChatMessageLocatorPreviews` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>query: String? | List<ChatMessageLocatorPreview> |  | 2476 |
| `ChatHistoryManager.loadChatMessagesFromTimestamp` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>startTimestampInclusive: Long | List<ChatMessage> |  | 2499 |
| `ChatHistoryManager.loadChatMessagesWindow` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>startTimestampInclusive: Long<br>endTimestampInclusive: Long | List<ChatMessage> |  | 2515 |
| `ChatHistoryManager.loadChatMessagesAscAfter` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>afterTimestampExclusive: Long<br>limit: Int | List<ChatMessage> |  | 2536 |
| `ChatHistoryManager.loadOlderChatMessages` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>beforeTimestampExclusive: Long<br>limit: Int | List<ChatMessage> |  | 2557 |
| `ChatHistoryManager.hasMessagesBefore` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>beforeTimestampExclusive: Long | Boolean |  | 2579 |
| `ChatHistoryManager.hasMessagesAfter` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>afterTimestampExclusive: Long | Boolean |  | 2593 |
| `ChatHistoryManager.loadChatMessagesDesc` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>limit: Int<br>beforeTimestampExclusive: Long?? | List<ChatMessage> |  | 2607 |
| `ChatHistoryManager.loadChatMessagesDescUpTo` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>maxTimestampInclusive: Long<br>limit: Int | List<ChatMessage> |  | 2632 |
| `ChatHistoryManager.reassignChatsToCharacterGroup` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | sourceCharacterGroupId: String?<br>targetCharacterGroupId: String | Int | 将指定角色群组下的对话转移到新的角色群组 | 2657 |
| `ChatHistoryManager.updateChatCharacterGroupId` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>characterGroupId: String? | Unit | 更新聊天绑定的群组角色卡 | 2685 |
| `ChatHistoryManager.updateChatCharacterBinding` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatId: String<br>characterCardName: String?<br>characterGroupId: String? | Unit | 同时更新聊天绑定的角色卡与群组 | 2697 |
| `ChatHistoryManager.clearCharacterGroupBinding` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | characterGroupId: String | Int | 清理绑定已删除角色群组的对话（将characterGroupId设为null） | 2716 |
| `ChatHistoryManager.deleteChatsByCharacterCardBinding` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | sourceCharacterCardName: String? | Int | 批量删除绑定到缺失角色卡（或未绑定）的未锁定对话 | 2733 |
| `ChatHistoryManager.assignCharacterCardToChats` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatIds: List<String><br>targetCharacterCardName: String? | Int | 批量为特定聊天更新角色卡绑定 | 2778 |
| `ChatHistoryManager.assignCharacterGroupToChats` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatIds: List<String><br>targetCharacterGroupId: String? | Int | 批量为特定聊天更新角色群组绑定 | 2799 |
| `ChatHistoryManager.clearCharacterGroupBindingForChats` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatIds: List<String> | Int | 批量为特定聊天移除角色群组绑定 | 2820 |
| `ChatHistoryManager.assignGroupToChats` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | chatIds: List<String><br>groupName: String? | Int | 批量为特定聊天更新分组 | 2840 |
| `ChatHistoryManager.renameCharacterCardInChats` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | oldName: String<br>newName: String | Int | 批量重命名对话中绑定的角色卡名称 | 2861 |
| `ChatHistoryManager.renameRoleNameInMessages` | `ChatHistoryManager` | `com.ai.assistance.operit.data.repository` | `ChatHistoryManager.kt` | oldName: String<br>newName: String | Int | 批量重命名消息中的角色名称 | 2876 |
| `CustomEmojiRepository.getInstance` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | context: Context | CustomEmojiRepository |  | 34 |
| `CustomEmojiRepository.initializeBuiltinEmojis` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` |  | Unit |  | 52 |
| `CustomEmojiRepository.initializeBuiltinEmojis` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt | Unit |  | 56 |
| `CustomEmojiRepository.resetToDefault` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` |  | Unit |  | 67 |
| `CustomEmojiRepository.resetToDefault` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt | Unit | 重置指定目标的表情库为默认表情（重新从 assets 复制） | 74 |
| `CustomEmojiRepository.addCustomEmoji` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | category: String<br>sourceUri: Uri | Result<CustomEmoji> |  | 89 |
| `CustomEmojiRepository.addCustomEmoji` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt<br>category: String<br>sourceUri: Uri | Result<CustomEmoji> | 为指定目标添加自定义表情 | 96 |
| `CustomEmojiRepository.deleteCustomEmoji` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | emojiId: String | Result<Unit> |  | 146 |
| `CustomEmojiRepository.deleteCustomEmoji` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt<br>emojiId: String | Result<Unit> |  | 150 |
| `CustomEmojiRepository.deleteCategory` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | category: String | Result<Unit> |  | 174 |
| `CustomEmojiRepository.deleteCategory` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt<br>category: String | Result<Unit> |  | 178 |
| `CustomEmojiRepository.getEmojiFile` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt<br>emoji: CustomEmoji | File |  | 203 |
| `CustomEmojiRepository.getEmojiUri` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt<br>emoji: CustomEmoji | Uri |  | 207 |
| `CustomEmojiRepository.getEmojisForCategory` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt<br>category: String | Flow<List<CustomEmoji>> |  | 211 |
| `CustomEmojiRepository.getAllCategories` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt | Flow<List<String>> |  | 215 |
| `CustomEmojiRepository.getAllEmojis` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt | Flow<List<CustomEmoji>> |  | 219 |
| `CustomEmojiRepository.addCategory` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt<br>categoryName: String | Unit |  | 223 |
| `CustomEmojiRepository.categoryExists` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt<br>categoryName: String | Boolean |  | 228 |
| `CustomEmojiRepository.cloneEmojiSet` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | source: ActivePrompt<br>target: ActivePrompt | Unit |  | 233 |
| `CustomEmojiRepository.deleteTarget` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt | Unit |  | 265 |
| `CustomEmojiRepository.cloneEmojisBetweenCharacterCards` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | sourceCharacterCardId: String<br>targetCharacterCardId: String | Unit |  | 270 |
| `CustomEmojiRepository.deleteCharacterCardEmojis` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | characterCardId: String | Unit |  | 277 |
| `CustomEmojiRepository.cloneEmojisBetweenCharacterGroups` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | sourceGroupId: String<br>targetGroupId: String | Unit |  | 281 |
| `CustomEmojiRepository.deleteCharacterGroupEmojis` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | characterGroupId: String | Unit |  | 288 |
| `CustomEmojiRepository.isValidCategoryName` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | categoryName: String | Boolean |  | 292 |
| `CustomEmojiRepository.copyBuiltinEmojisFromAssets` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt | Unit |  | 296 |
| `CustomEmojiRepository.getTargetScopeDirName` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt | String |  | 344 |
| `CustomEmojiRepository.purgeLegacyGlobalStorage` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` |  | Unit |  | 351 |
| `CustomEmojiRepository.getTargetBaseDir` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt | File |  | 368 |
| `CustomEmojiRepository.getCategoryDir` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | target: ActivePrompt<br>category: String | File |  | 372 |
| `CustomEmojiRepository.getFileExtension` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | uri: Uri | String? |  | 376 |
| `CustomEmojiRepository.getFileNameFromUri` | `CustomEmojiRepository` | `com.ai.assistance.operit.data.repository` | `CustomEmojiRepository.kt` | uri: Uri | String? |  | 403 |
| `MemoryAutoSaveCandidateRepository.enqueue` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` | chatId: String<br>triggerMessageTimestamp: Long<br>sourceType: String? | Long |  | 18 |
| `MemoryAutoSaveCandidateRepository.enqueueSelectedUserMessages` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` | chatId: String<br>triggerMessageTimestamps: List<Long> | Unit |  | 36 |
| `MemoryAutoSaveCandidateRepository.getPendingAndFailedCandidates` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` |  | List<MemoryAutoSaveCandidate> |  | 55 |
| `MemoryAutoSaveCandidateRepository.countPendingAndFailedChats` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` |  | Int |  | 71 |
| `MemoryAutoSaveCandidateRepository.countPendingAndFailedCandidates` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` |  | Int |  | 79 |
| `MemoryAutoSaveCandidateRepository.markProcessing` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` | candidateIds: List<Long> | Unit |  | 83 |
| `MemoryAutoSaveCandidateRepository.markPending` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` | candidateIds: List<Long> | Unit |  | 95 |
| `MemoryAutoSaveCandidateRepository.deleteCandidates` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` | candidateIds: List<Long> | Unit |  | 107 |
| `MemoryAutoSaveCandidateRepository.markFailed` | `MemoryAutoSaveCandidateRepository` | `com.ai.assistance.operit.data.repository` | `MemoryAutoSaveCandidateRepository.kt` | candidateIds: List<Long><br>errorMessage: String | Unit |  | 112 |
| `MemoryRepository.normalizeFolderPath` | `MemoryRepository` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | folderPath: String? | String? |  | 72 |
| `MemoryRepository.sanitizeIndexKey` | `MemoryRepository` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | raw: String | String |  | 84 |
| `MemoryRepository.generateEmbedding` | `MemoryRepository` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | text: String<br>config: CloudEmbeddingConfig | Embedding? |  | 102 |
| `MemoryRepository.cosineSimilarity` | `MemoryRepository` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | left: Embedding<br>right: Embedding | Float |  | 106 |
| `MemoryRepository.expandKeywordToken` | `MemoryRepository` | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | token: String | Set<String> | 对关键词做“切碎扩展”： - 保留原词 - 使用 Jieba 分词补充分片 目的：在未开启语义检索时，提高中文长句与标题之间的匹配召回。 | 140 |
| `splitSearchKeywords` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | query: String | List<String> |  | 189 |
| `buildLexicalQueryTokens` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | query: String<br>keywords: List<String> | List<String> |  | 197 |
| `isFolderPlaceholderMemory` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory | Boolean |  | 211 |
| `resolveSearchWeights` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | scoreMode: MemoryScoreMode<br>keywordWeight: Float<br>tagWeight: Float<br>semanticWeight: Float<br>edgeWeight: Float<br>keywordCount: Int | ResolvedSearchWeights |  | 217 |
| `computeRrfBaseScore` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | rank: Int | Double |  | 247 |
| `computeKeywordCoverageMultiplier` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | matchedTokenCount: Int<br>totalTokenCount: Int | Double |  | 251 |
| `computeSemanticWeightedScore` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | rank: Int<br>baseImportance: Float<br>similarity: Float<br>resolvedWeights: ResolvedSearchWeights | Double |  | 260 |
| `vectorIndexDir` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` |  | File |  | 273 |
| `currentProfileMemoryIndexFiles` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` |  | List<File> |  | 275 |
| `currentProfileDocumentIndexFiles` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` |  | List<File> |  | 284 |
| `memoryIndexFileForDimension` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | dimension: Int | File |  | 293 |
| `documentIndexFile` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long<br>dimension: Int | File |  | 297 |
| `parseMemoryIndexDimension` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | file: File | Int? |  | 301 |
| `deleteIndexFileIfExists` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | file: File? | Unit |  | 311 |
| `loadChunksForDocument` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory | List<DocumentChunk> |  | 317 |
| `countDocumentChunkIndexableItems` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory | Int |  | 322 |
| `createMemoryIndexItem` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory | IndexItem<Long, Long>? |  | 332 |
| `createChunkIndexItem` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | chunk: DocumentChunk | IndexItem<Long, Long>? |  | 343 |
| `rebuildMemoryVectorIndexForDimension` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | dimension: Int<br>excludedMemoryId: Long?? | Int | HNSW 的删除会保留 tombstone，直接增量 add 容易命中容量异常，因此按维度重建活跃记忆索引。 | 355 |
| `rebuildAffectedMemoryVectorIndices` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | dimensions: Collection<Int?><br>excludedMemoryId: Long?? | Unit |  | 388 |
| `addMemoryToIndexInternal` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory<br>previousDimension: Int?? | Unit |  | 404 |
| `removeMemoryFromIndexInternal` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory<br>memoryAlreadyRemoved: Boolean? | Unit |  | 413 |
| `rebuildAllMemoryVectorIndices` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | onItemIndexed: (() -> Unit)?? | Int |  | 428 |
| `resolveDocumentIndexDimension` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | chunks: List<DocumentChunk><br>forcedDimension: Int? | Int? |  | 461 |
| `rebuildDocumentChunkIndex` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory<br>forcedDimension: Int??<br>onItemIndexed: (() -> Unit)?? | Int |  | 477 |
| `rebuildAllDocumentChunkIndices` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | onItemIndexed: (() -> Unit)?? | Int |  | 544 |
| `ensureMemoryVectorIndex` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | dimension: Int | VectorIndexManager<IndexItem<Long, Long>, Long>? |  | 557 |
| `ensureDocumentChunkIndex` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory<br>dimension: Int | VectorIndexManager<IndexItem<Long, Long>, Long>? |  | 570 |
| `getSemanticMemoryCandidatesFromIndex` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | queryEmbedding: Embedding | List<Pair<Memory, Float>> |  | 583 |
| `getSemanticChunkCandidatesFromIndex` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory<br>queryEmbedding: Embedding | List<Pair<DocumentChunk, Float>> |  | 607 |
| `shouldKeepRawLexicalToken` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | token: String | Boolean |  | 634 |
| `isWildcardLexicalToken` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | token: String | Boolean |  | 645 |
| `shouldKeepPlainLexicalToken` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | token: String | Boolean |  | 649 |
| `shouldKeepWildcardLexicalToken` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | token: String | Boolean |  | 653 |
| `isSearchableLexicalBody` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | text: String | Boolean |  | 659 |
| `buildWildcardRegex` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | token: String | Regex? |  | 664 |
| `textMatchesLexicalToken` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | text: String<br>token: String | Boolean |  | 675 |
| `queryTitleCandidatesByFragments` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | fragments: List<String><br>scopedMemories: List<Memory> | List<TitleMatchCandidate> |  | 686 |
| `queryTagCandidatesByFragments` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | fragments: List<String><br>scopedMemories: List<Memory> | List<TitleMatchCandidate> |  | 732 |
| `createMemoryFromDocument` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | documentName: String<br>originalPath: String<br>text: String<br>folderPath: String? | Memory | 从外部文档创建记忆。 | 769 |
| `generateTextForEmbedding` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory | String | 生成带有元数据（可信度、重要性）的文本，用于embedding。 | 823 |
| `saveMemory` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory | Long | Creates or updates a memory, automatically generating its embedding. | 834 |
| `findMemoryById` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | id: Long | Memory? | Finds a memory by its ID. | 855 |
| `findMemoryByUuid` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | uuid: String | Memory? | Finds a memory by its UUID. | 864 |
| `findMemoryByTitle` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | title: String | Memory? | Finds a memory by its exact title. | 873 |
| `findMemoriesByTitle` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | title: String | List<Memory> | Finds all memories with the exact title (case-sensitive). | 882 |
| `deleteMemory` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long | Boolean | Deletes a memory and all its links. This is a critical operation and should be handled wi… | 892 |
| `collectLinkIdsForDeletion` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryIdsToDelete: Set<Long><br>includeDangling: Boolean? | Set<Long> | --- Link CRUD Operations --- | 921 |
| `cleanupDanglingLinksIfNeeded` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | force: Boolean? | Unit |  | 948 |
| `findLinkById` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | linkId: Long | MemoryLink? |  | 964 |
| `updateLink` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | linkId: Long<br>type: String<br>weight: Float<br>description: String | MemoryLink? |  | 968 |
| `deleteLink` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | linkId: Long | Boolean |  | 987 |
| `addTagToMemory` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory<br>tagName: String | MemoryTag | Adds a tag to a memory. | 1009 |
| `linkMemories` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | source: Memory<br>target: Memory<br>type: String<br>weight: Float?<br>description: String? | Unit | Creates a link between two memories. | 1038 |
| `getOutgoingLinks` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long | List<MemoryLink> | Gets all outgoing links from a memory. | 1069 |
| `getIncomingLinks` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long | List<MemoryLink> | Gets all incoming links to a memory. | 1076 |
| `queryMemoryLinks` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | linkId: Long??<br>sourceMemoryId: Long??<br>targetMemoryId: Long??<br>linkType: String??<br>limit: Int? | List<MemoryLink> | Query memory links with optional filters. If no filter is provided, returns recent links … | 1086 |
| `searchMemories` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | query: String<br>folderPath: String??<br>scoreMode: MemoryScoreMode?<br>keywordWeight: Float?<br>tagWeight: Float?<br>semanticWeight: Float?<br>edgeWeight: Float?<br>relevanceThreshold: Double?<br>createdAtStartMs: Long??<br>createdAtEndMs… | List<Memory> | Searches memories using semantic search if a query is provided, otherwise returns all mem… | 1131 |
| `searchMemoriesDebug` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | query: String<br>folderPath: String??<br>scoreMode: MemoryScoreMode?<br>keywordWeight: Float?<br>tagWeight: Float?<br>semanticWeight: Float?<br>edgeWeight: Float?<br>relevanceThreshold: Double?<br>createdAtStartMs: Long??<br>createdAtEndMs… | MemorySearchDebugInfo |  | 1157 |
| `runSearchMemoriesWithDebug` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | query: String<br>folderPath: String??<br>scoreMode: MemoryScoreMode?<br>keywordWeight: Float?<br>tagWeight: Float?<br>semanticWeight: Float?<br>edgeWeight: Float?<br>relevanceThreshold: Double?<br>createdAtStartMs: Long??<br>createdAtEndMs… | SearchComputationResult |  | 1183 |
| `buildDebug` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | debugKeywords: List<String>?<br>lexicalTokens: List<String>?<br>debugSemanticKeywordNormFactor: Double?<br>keywordMatchesCount: Int?<br>tagMatchesCount: Int?<br>reverseContainmentMatchesCount: Int?<br>semanticMatchesCount: Int?<br>graphEdg… | MemorySearchDebugInfo |  | 1235 |
| `getScoreParts` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long | SearchScoreParts |  | 1298 |
| `getChunksForMemory` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long | List<DocumentChunk> | 获取指定记忆的所有文档区块。 | 1603 |
| `getChunkByIndex` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long<br>chunkIndex: Int | DocumentChunk? | 根据索引获取单个文档区块。 | 1615 |
| `getChunksByRange` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long<br>startIndex: Int<br>endIndex: Int | List<DocumentChunk> | 获取指定范围内的文档区块。 | 1627 |
| `getTotalChunkCount` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long | Int | 获取文档的总区块数。 | 1637 |
| `searchChunksInDocument` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryId: Long<br>query: String<br>limit: Int? | List<DocumentChunk> | 在指定文档的区块内进行搜索。 | 1647 |
| `updateChunk` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | chunkId: Long<br>newContent: String | Unit | 更新单个文档区块的内容。 | 1797 |
| `addMemoryToIndex` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory | Unit |  | 1810 |
| `removeMemoryFromIndex` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory | Unit |  | 1814 |
| `loadCloudEmbeddingConfig` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` |  | CloudEmbeddingConfig |  | 1818 |
| `saveCloudEmbeddingConfig` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | config: CloudEmbeddingConfig | Unit |  | 1822 |
| `getEmbeddingDimensionUsage` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` |  | EmbeddingDimensionUsage |  | 1826 |
| `rebuildVectorIndices` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | onProgress: (EmbeddingRebuildProgress) -> Unit | EmbeddingRebuildProgress |  | 1856 |
| `report` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | stage: String | Unit |  | 1950 |
| `getGraphForMemories` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memories: List<Memory> | Graph | Builds a Graph object from a given list of memories. This is used to display a subset of … | 2039 |
| `getMemoryByUuid` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | uuid: String | Memory? | Retrieves a single memory by its UUID. | 2059 |
| `getAllFolderPaths` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` |  | List<String> | 获取所有唯一的文件夹路径。 | 2068 |
| `getMemoriesByFolderPath` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | folderPath: String | List<Memory> | 按文件夹路径获取记忆（包括所有子文件夹）。 | 2084 |
| `getGraphForFolder` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | folderPath: String | Graph | 获取指定文件夹的图谱（包括跨文件夹的边）。 | 2101 |
| `renameFolder` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | oldPath: String<br>newPath: String | Boolean | 重命名文件夹（更新该文件夹下所有记忆的 folderPath）。 | 2112 |
| `moveMemoriesToFolder` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memoryIds: List<Long><br>targetFolderPath: String | Boolean | 移动记忆到新文件夹。 | 2148 |
| `createFolder` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | folderPath: String | Boolean | 创建新文件夹（实际上是通过在该路径下创建一个占位记忆来实现）。 | 2170 |
| `createMemory` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | title: String<br>content: String<br>contentType: String?<br>source: String?<br>folderPath: String?<br>tags: List<String>?? | Memory? | 创建新记忆并自动生成embedding，保存到数据库并同步索引。 | 2199 |
| `updateMemory` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory<br>newTitle: String<br>newContent: String<br>newContentType: String?<br>newSource: String?<br>newCredibility: Float?<br>newImportance: Float?<br>newFolderPath: String??<br>newTags: List<String>?? | Memory? | 更新已有记忆内容（title/content等），自动更新embedding和索引。 | 2239 |
| `mergeMemories` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | sourceTitles: List<String><br>newTitle: String<br>newContent: String<br>newTags: List<String><br>folderPath: String | Memory? | Merges multiple source memories into a single new memory, redirecting all links. | 2313 |
| `deleteMemoriesByUuids` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | uuids: Set<String> | Boolean | 根据UUID批量删除记忆及其所有关联。 | 2413 |
| `getMemoryGraph` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` |  | Graph | Fetches all memories and their links, and converts them into a Graph data structure. | 2484 |
| `buildGraphFromMemories` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memories: List<Memory><br>currentFolderPath: String?? | Graph | Private helper to construct a graph from a specific list of memories. Ensures that edges … | 2495 |
| `deleteFolder` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | folderPath: String | Unit | 删除文件夹：将所有属于 folderPath 的记忆移动到"未分类" | 2569 |
| `exportMemoriesToJson` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` |  | String | 导出所有记忆（不包括文档节点）为 JSON 字符串 | 2589 |
| `importMemoriesFromJson` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | jsonString: String<br>strategy: ImportStrategy? | MemoryImportResult | 从 JSON 字符串导入记忆 | 2662 |
| `createMemoryFromSerializable` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | serializable: SerializableMemory<br>forceNewUuid: Boolean | Memory | 从可序列化的记忆数据创建 Memory 对象 | 2772 |
| `updateMemoryTags` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | memory: Memory<br>tagNames: List<String> | Unit | 更新记忆的标签 | 2802 |
| `UIHierarchyManager.onServiceConnected` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | name: ComponentName?<br>service: IBinder? | Unit |  | 65 |
| `UIHierarchyManager.onServiceDisconnected` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | name: ComponentName? | Unit |  | 73 |
| `UIHierarchyManager.extractProviderApkFromAssets` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | File? | 从应用内assets目录中提取无障碍服务提供者APK文件。 | 87 |
| `UIHierarchyManager.launchProviderInstall` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | Unit | 启动安装流程来安装提供者应用 | 107 |
| `UIHierarchyManager.isUpdateNeeded` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | Boolean | 检查无障碍服务提供者是否需要更新 | 158 |
| `UIHierarchyManager.ensureBound` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | Boolean | 确保服务已绑定，如果未绑定则尝试自动重新绑定。 | 166 |
| `UIHierarchyManager.isProviderAppInstalled` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | Boolean | 检查无障碍服务提供者应用是否已安装 | 183 |
| `UIHierarchyManager.bindToService` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | Boolean | 绑定到外部无障碍服务。 这是一个挂起函数，它会等待服务连接成功或失败。 | 197 |
| `UIHierarchyManager.unbindFromService` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | Unit | 解绑服务 | 291 |
| `UIHierarchyManager.getUIHierarchy` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | String | 从外部服务获取UI层次结构。 如果服务未绑定，会尝试自动重新绑定一次。 | 308 |
| `UIHierarchyManager.extractWindowInfo` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | xmlHierarchy: String | Pair<String?, String?> | 从UI层次结构的XML中解析出窗口信息（包名）。 活动名称现在通过 getCurrentActivityName() 函数单独获取。 | 328 |
| `UIHierarchyManager.performClick` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context<br>x: Int<br>y: Int | Boolean | 请求远程服务在指定坐标执行点击。 | 363 |
| `UIHierarchyManager.performLongPress` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context<br>x: Int<br>y: Int | Boolean |  | 376 |
| `UIHierarchyManager.performSwipe` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context<br>startX: Int<br>startY: Int<br>endX: Int<br>endY: Int<br>duration: Long | Boolean | 请求远程服务执行滑动。 | 392 |
| `UIHierarchyManager.performGlobalAction` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context<br>actionId: Int | Boolean | 请求远程服务执行全局操作。 | 408 |
| `UIHierarchyManager.findFocusedNodeId` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | String? | 请求远程服务查找有焦点的节点的ID。 | 424 |
| `UIHierarchyManager.setTextOnNode` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context<br>nodeId: String<br>text: String | Boolean | 请求远程服务在指定ID的节点上设置文本。 | 440 |
| `UIHierarchyManager.takeScreenshot` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context<br>path: String<br>format: String | Boolean | 请求远程服务截取屏幕截图。 | 459 |
| `UIHierarchyManager.isAccessibilityServiceEnabled` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | Boolean | 检查远程无障碍服务是否已在系统设置中启用。 | 475 |
| `UIHierarchyManager.getCurrentActivityName` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | context: Context | String? | 从远程服务获取当前Activity名称。 | 491 |
| `WorkflowRepository.notifyWorkflowsChanged` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` |  | Unit |  | 82 |
| `WorkflowRepository.publishRunningWorkflowIdsLocked` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` |  | Unit |  | 88 |
| `WorkflowRepository.registerRunningWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflowId: String<br>job: Job | Unit |  | 100 |
| `WorkflowRepository.unregisterRunningWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflowId: String<br>job: Job | Unit |  | 107 |
| `WorkflowRepository.getRunningWorkflowJobs` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflowId: String<br>targetJob: Job?? | List<Job> |  | 114 |
| `WorkflowRepository.getWorkflowDirectory` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` |  | File | 获取工作流存储目录 | 138 |
| `WorkflowRepository.getWorkflowFile` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflowId: String | File | 获取工作流文件 | 164 |
| `WorkflowRepository.getAtomicBackupFile` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | file: File | File |  | 168 |
| `WorkflowRepository.hasAtomicReadableFile` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | file: File | Boolean |  | 176 |
| `WorkflowRepository.listWorkflowFiles` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflowDir: File | List<File> |  | 180 |
| `WorkflowRepository.readWorkflowFile` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | file: File<br>workflowId: String? | Workflow |  | 203 |
| `WorkflowRepository.writeTextAtomically` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | file: File<br>content: String | Unit |  | 216 |
| `WorkflowRepository.withWorkflowStoreLock` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | block: suspend () -> T | T |  | 238 |
| `WorkflowRepository.getExecutionLogDirectory` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflowId: String<br>createIfMissing: Boolean? | File |  | 242 |
| `WorkflowRepository.saveExecutionRecord` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | record: WorkflowExecutionRecord | Unit |  | 250 |
| `WorkflowRepository.hasScheduleTrigger` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflow: Workflow | Boolean |  | 270 |
| `WorkflowRepository.getAllWorkflows` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` |  | Result<List<Workflow>> | 获取所有工作流 | 277 |
| `WorkflowRepository.getWorkflowById` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String | Result<Workflow?> | 根据ID获取工作流 | 316 |
| `WorkflowRepository.getLatestExecutionRecord` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflowId: String | Result<WorkflowExecutionRecord?> |  | 340 |
| `WorkflowRepository.createWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflow: Workflow | Result<Workflow> | 创建工作流 | 363 |
| `WorkflowRepository.updateWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflow: Workflow | Result<Workflow> | 更新工作流 | 391 |
| `WorkflowRepository.buildPreExecutionFailureRecord` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflow: Workflow<br>triggerNodeId: String?<br>failureStage: WorkflowExecutionFailureStage<br>failureReason: String<br>logLevel: WorkflowLogLevel | WorkflowExecutionRecord |  | 419 |
| `WorkflowRepository.persistPreExecutionFailure` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | workflow: Workflow<br>triggerNodeId: String?<br>failureStage: WorkflowExecutionFailureStage<br>failureReason: String<br>logLevel: WorkflowLogLevel | WorkflowExecutionRecord |  | 452 |
| `WorkflowRepository.setWorkflowEnabled` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String<br>enabled: Boolean | Result<Workflow> |  | 471 |
| `WorkflowRepository.deleteWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String | Result<Boolean> | 删除工作流 | 508 |
| `WorkflowRepository.triggerWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String<br>triggerNodeId: String??<br>triggerExtras: Map<String, String>? | Result<String> | 触发工作流执行 | 552 |
| `WorkflowRepository.triggerWorkflowWithCallback` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String<br>triggerNodeId: String??<br>triggerExtras: Map<String, String>?<br>onNodeStateChange: (nodeId: String, state: NodeExecuti… | Result<String> | 触发工作流执行（带状态回调） | 570 |
| `WorkflowRepository.cancelWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String<br>targetJob: Job?? | Result<Boolean> |  | 582 |
| `WorkflowRepository.triggerWorkflowInternal` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String<br>triggerNodeId: String??<br>triggerExtras: Map<String, String>?<br>onNodeStateChange: (nodeId: String, state: NodeExecuti… | Result<String> |  | 603 |
| `WorkflowRepository.updateExecutionStatus` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String<br>status: ExecutionStatus<br>executionTime: Long | Unit | 更新工作流执行状态（仅状态和时间） | 687 |
| `WorkflowRepository.updateExecutionStatistics` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String<br>status: ExecutionStatus<br>executionTime: Long | Unit | 更新工作流执行统计信息 | 718 |
| `WorkflowRepository.scheduleWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String | Boolean | Schedule a workflow | 761 |
| `WorkflowRepository.unscheduleWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String | Unit | Unschedule a workflow | 790 |
| `WorkflowRepository.rescheduleWorkflow` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String | Boolean | Reschedule a workflow (cancel + schedule) | 802 |
| `WorkflowRepository.isWorkflowScheduled` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String | Boolean | Check if workflow is scheduled | 810 |
| `WorkflowRepository.getNextExecutionTime` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | id: String | Long? | Get next execution time for a workflow | 822 |
| `WorkflowRepository.triggerWorkflowsByTaskerEvent` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | params: List<String>? | Unit | Finds and triggers workflows based on a Tasker event. It checks all enabled workflows for… | 840 |
| `WorkflowRepository.triggerWorkflowsByIntentEvent` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | intent: Intent | Unit | Finds and triggers workflows based on a received Intent. It checks all enabled workflows … | 873 |
| `WorkflowRepository.triggerWorkflowsByColdStartAppOpen` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | extras: Map<String, String>? | Unit |  | 909 |
| `WorkflowRepository.triggerWorkflowsBySpeechEvent` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | text: String<br>isFinal: Boolean | Unit |  | 937 |
| `WorkflowRepository.parseBoolean` | `WorkflowRepository` | `com.ai.assistance.operit.data.repository` | `WorkflowRepository.kt` | value: String?<br>defaultValue: Boolean | Boolean |  | 952 |
| `AvatarConfigPersistenceTest.decodePersistedAvatarConfigs_rejectsEntriesWithNullOrMissingData` | `AvatarConfigPersistenceTest` | `com.ai.assistance.operit.data.repository` | `AvatarConfigPersistenceTest.kt` |  | Unit |  | 13 ⚑ |
| `AvatarConfigPersistenceTest.decodePersistedAvatarConfigs_preservesValidSavedConfig` | `AvatarConfigPersistenceTest` | `com.ai.assistance.operit.data.repository` | `AvatarConfigPersistenceTest.kt` |  | Unit |  | 48 ⚑ |
| `AvatarConfigPersistenceTest.decodePersistedAvatarConfigs_rejectsMalformedEntryWithoutDiscardingValidSiblings` | `AvatarConfigPersistenceTest` | `com.ai.assistance.operit.data.repository` | `AvatarConfigPersistenceTest.kt` |  | Unit |  | 65 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `allMemoriesWithEmbedding` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred | 3. Semantic search (for conceptual matches) | 1416 |
| `basePropagationScore` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1474 |
| `candidateRows` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1544 |
| `cloudConfig` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1417 |
| `DATA_KEY_CUSTOM_MOOD_DEFINITIONS` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | inferred |  | 48 |
| `DATA_KEY_EMOTION_ANIMATION_MAPPING` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | inferred |  | 46 |
| `DATA_KEY_MOOD_ANIMATION_MAPPING` | — | `com.ai.assistance.operit.data.repository` | `AvatarRepository.kt` | inferred |  | 47 |
| `debugInfo` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1562 |
| `edgesTraversed` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1472 |
| `filteredScores` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred | 添加相关性阈值过滤，避免返回不相关的记忆 | 1530 |
| `graphPropagationWeight` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1473 |
| `keywordResults` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred | 1. Keyword-based search (DB title contains any fragment from the query) | 1340 |
| `memoriesToSearch` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred | --- PRE-FILTERING BY FOLDER --- If a folder path is provided, all subsequent se… | 1324 |
| `reverseContainmentResults` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred | 2. Reverse Containment Search (Query contains Memory Title) This is crucial for… | 1398 |
| `scopedMemoryIds` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1419 |
| `scoredMemoryMap` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1536 |
| `semanticMatchedIds` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1418 |
| `sortedMemories` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred | Fetch the sorted entities from the database | 1588 |
| `sortedMemoryIds` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1585 |
| `sortedScoresForLogging` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred | 只显示前3个结果的分数 | 1535 |
| `tagResults` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred |  | 1368 |
| `topMemoriesForExpansion` | — | `com.ai.assistance.operit.data.repository` | `MemoryRepository.kt` | inferred | 4. Graph-based expansion: Boost scores of connected memories based on edge weig… | 1466 |
| `UIHierarchyManager._isBound` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred |  | 56 |
| `UIHierarchyManager.accessibilityProvider` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | IAccessibilityProvider? |  | 54 |
| `UIHierarchyManager.BIND_SERVICE_TIMEOUT_MS` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred |  | 42 |
| `UIHierarchyManager.bindingMutex` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred |  | 59 |
| `UIHierarchyManager.connectionContinuation` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | ((Boolean) -> Unit)? |  | 62 |
| `UIHierarchyManager.isBound` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred |  | 57 |
| `UIHierarchyManager.PROVIDER_ACTION` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred | 用于绑定的自定义Action，必须与服务提供者应用中的声明一致 | 49 |
| `UIHierarchyManager.PROVIDER_APK_NAME` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred | 无障碍服务提供者APK的文件名 | 47 |
| `UIHierarchyManager.PROVIDER_MARKET_URL` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred | TODO: 如果你不在Google Play上发布，可以将其更改为直接下载的URL | 51 |
| `UIHierarchyManager.PROVIDER_PACKAGE_NAME` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred | 新的无障碍服务提供者应用的包名 | 45 |
| `UIHierarchyManager.serviceConnection` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred |  | 64 |
| `UIHierarchyManager.TAG` | `UIHierarchyManager` | `com.ai.assistance.operit.data.repository` | `UIHierarchyManager.kt` | inferred |  | 41 |
