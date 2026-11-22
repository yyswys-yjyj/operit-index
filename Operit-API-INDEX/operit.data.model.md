# operit.data.model

> 函数 63 · 类型 143 · 顶层常量 84 · 共 290 条
> 每日定时任务自动生成。

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ActivePrompt` | `ActivePrompt` | `com.ai.assistance.operit.data.model` | `ActivePrompt.kt` | interface ActivePrompt |  | 3 |
| `ActivePrompt.CharacterCard` | `ActivePrompt` | `com.ai.assistance.operit.data.model` | `ActivePrompt.kt` | class CharacterCard(val id: String) : ActivePrompt data class CharacterGroup |  | 4 |
| `AiReference` | `AiReference` | `com.ai.assistance.operit.data.model` | `AiReference.kt` | class AiReference(val text: String, val url: String) | Represents a reference in the AI response This is a public model class that can be used b… | 10 |
| `AITool` | `AITool` | `com.ai.assistance.operit.data.model` | `AITool.kt` | class AITool(val name: String, val parameters: List<ToolParameter>, val description: String) | Represents a tool that can be used by the AI | 12 |
| `AIToolTest` | `AIToolTest` | `com.ai.assistance.operit.data.model` | `AIToolTest.kt` | class AIToolTest |  | 10 |
| `ApiKeyAvailabilityStatus` | `ApiKeyAvailabilityStatus` | `com.ai.assistance.operit.data.model` | `ApiKeyInfo.kt` | class ApiKeyAvailabilityStatus | API Key详细信息 | 16 |
| `ApiKeyFormatValidator` | `ApiKeyFormatValidator` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidator.kt` | object ApiKeyFormatValidator |  | 3 |
| `ApiKeyFormatValidatorTest` | `ApiKeyFormatValidatorTest` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidatorTest.kt` | class ApiKeyFormatValidatorTest |  | 7 |
| `ApiKeyInfo` | `ApiKeyInfo` | `com.ai.assistance.operit.data.model` | `ApiKeyInfo.kt` | class ApiKeyInfo(val id: String, val key: String, val name: String, val isEnabled: Boolean, val availabilityStatus: ApiKeyAvailabilityStatus, val usageCount: Long, val lastUse… | API Key详细信息 | 33 |
| `ApiKeyInfoTest` | `ApiKeyInfoTest` | `com.ai.assistance.operit.data.model` | `ApiKeyInfoTest.kt` | class ApiKeyInfoTest |  | 8 |
| `ApiProviderType` | `ApiProviderType` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | class ApiProviderType | API提供商类型枚举 | 7 |
| `AttachmentInfo` | `AttachmentInfo` | `com.ai.assistance.operit.data.model` | `AttachmentInfo.kt` | class AttachmentInfo(val filePath: String, val fileName: String, val mimeType: String, val fileSize: Long, val content: String) | Data class to store information about an attachment This represents a file or content tha… | 7 |
| `AttachmentInfoTest` | `AttachmentInfoTest` | `com.ai.assistance.operit.data.model` | `AttachmentInfoTest.kt` | class AttachmentInfoTest |  | 6 |
| `BillingMode` | `BillingMode` | `com.ai.assistance.operit.data.model` | `BillingMode.kt` | class BillingMode | 计费方式枚举 用于定义AI模型的计费模式 | 7 |
| `CharacterCard` | `CharacterCard` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class CharacterCard(val id: String, val name: String, val description: String, val characterSetting: String, val openingStatement: String, val otherContentChat: String, val other… | 角色卡数据模型 | 42 |
| `CharacterCardChatModelBindingMode` | `CharacterCardChatModelBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | object CharacterCardChatModelBindingMode |  | 65 |
| `CharacterCardChatStats` | `CharacterCardChatStats` | `com.ai.assistance.operit.data.model` | `CharacterCardChatStats.kt` | class CharacterCardChatStats(val characterCardName: String?, val chatCount: Int, val messageCount: Int) | 角色卡聊天统计结果 | 6 |
| `CharacterCardMemoryProfileBindingMode` | `CharacterCardMemoryProfileBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | object CharacterCardMemoryProfileBindingMode |  | 74 |
| `CharacterCardToolAccessConfig` | `CharacterCardToolAccessConfig` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class CharacterCardToolAccessConfig(val enabled: Boolean, val allowedBuiltinTools: List<String>, val allowedPackages: List<String>, val allowedSkills: List<String>, val allowedMcpServers: List<S… |  | 8 |
| `CharacterGroupCard` | `CharacterGroupCard` | `com.ai.assistance.operit.data.model` | `CharacterGroupCard.kt` | class CharacterGroupCard(val id: String, val name: String, val description: String, val members: List<GroupMemberConfig>, val createdAt: Long, val updatedAt: Long) | 群组角色卡 | 14 |
| `CharacterGroupChatStats` | `CharacterGroupChatStats` | `com.ai.assistance.operit.data.model` | `CharacterGroupChatStats.kt` | class CharacterGroupChatStats(val characterGroupId: String?, val chatCount: Int, val messageCount: Int) | 角色群组聊天统计结果 | 6 |
| `ChatEntity` | `ChatEntity` | `com.ai.assistance.operit.data.model` | `ChatEntity.kt` | class ChatEntity(val id: String, val title: String, val createdAt: Long, val updatedAt: Long, val inputTokens: Long, val outputTokens: Long, val currentWindowSize: Long, val g… | 聊天实体类，用于Room数据库存储聊天元数据 | 11 |
| `ChatEntityTest` | `ChatEntityTest` | `com.ai.assistance.operit.data.model` | `ChatEntityTest.kt` | class ChatEntityTest |  | 11 |
| `ChatHistory` | `ChatHistory` | `com.ai.assistance.operit.data.model` | `ChatHistory.kt` | class ChatHistory(val id: String, val title: String, val messages: List<ChatMessage>, val createdAt: LocalDateTime, val updatedAt: LocalDateTime, val inputTokens: Long, val out… |  | 9 |
| `ChatHistoryTest` | `ChatHistoryTest` | `com.ai.assistance.operit.data.model` | `ChatHistoryTest.kt` | class ChatHistoryTest |  | 11 |
| `ChatMessage` | `ChatMessage` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | class ChatMessage(val sender: String, var content: String, val timestamp: Long, val roleName: String, val selectedVariantIndex: Int, val variantCount: Int, val provider: String… : Parcelable |  | 10 |
| `ChatMessage.CREATOR` | `ChatMessage` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | object CREATOR : Parcelable.Creator<ChatMessage> |  | 85 |
| `ChatMessageDisplayMode` | `ChatMessageDisplayMode` | `com.ai.assistance.operit.data.model` | `ChatMessageDisplayMode.kt` | class ChatMessageDisplayMode |  | 6 |
| `ChatMessageDisplayModeTest` | `ChatMessageDisplayModeTest` | `com.ai.assistance.operit.data.model` | `ChatMessageDisplayModeTest.kt` | class ChatMessageDisplayModeTest |  | 7 |
| `ChatMessageLocatorPreview` | `ChatMessageLocatorPreview` | `com.ai.assistance.operit.data.model` | `ChatMessageLocatorPreview.kt` | class ChatMessageLocatorPreview(val messageIndex: Int?, val timestamp: Long, val sender: String, val previewContent: String, val contentLength: Int, val displayMode: String, val isFavorite: … |  | 3 |
| `ChatMessageTest` | `ChatMessageTest` | `com.ai.assistance.operit.data.model` | `ChatMessageTest.kt` | class ChatMessageTest |  | 10 |
| `ChatMessageTimestampAllocator` | `ChatMessageTimestampAllocator` | `com.ai.assistance.operit.data.model` | `ChatMessageTimestampAllocator.kt` | object ChatMessageTimestampAllocator | 为聊天消息分配单调递增的时间戳。 项目里大量逻辑仍然把 timestamp 当作消息唯一标识使用， 因此这里需要保证同一进程内新建消息不会拿到重复值。 | 11 |
| `ChatMessageTimestampAllocatorTest` | `ChatMessageTimestampAllocatorTest` | `com.ai.assistance.operit.data.model` | `ChatMessageTimestampAllocatorTest.kt` | class ChatMessageTimestampAllocatorTest |  | 7 |
| `ChatTurnOptions` | `ChatTurnOptions` | `com.ai.assistance.operit.data.model` | `ChatTurnOptions.kt` | class ChatTurnOptions(val persistTurn: Boolean, val notifyReply: Boolean?, val hideUserMessage: Boolean, val disableWarning: Boolean) |  | 3 |
| `CloudEmbeddingConfig` | `CloudEmbeddingConfig` | `com.ai.assistance.operit.data.model` | `CloudEmbeddingConfig.kt` | class CloudEmbeddingConfig(val enabled: Boolean, val endpoint: String, val apiKey: String, val model: String) |  | 3 |
| `ConditionNode` | `ConditionNode` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class ConditionNode(override val id: String, override val type: String, override var name: String, override var description: String, override var position: NodePosition, var left… : WorkflowNode |  | 96 |
| `ConditionOperator` | `ConditionOperator` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class ConditionOperator |  | 82 |
| `ConversationSummaryConfig` | `ConversationSummaryConfig` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | class ConversationSummaryConfig(val globalRules: String?, val sectionOverrides: List<SummarySectionOverride>, val dialogueReviewEnabled: Boolean, val dialogueReviewTitle: String) |  | 86 |
| `CustomEmoji` | `CustomEmoji` | `com.ai.assistance.operit.data.model` | `CustomEmoji.kt` | class CustomEmoji(val id: String, val emotionCategory: String, val fileName: String, val isBuiltInCategory: Boolean, val createdAt: Long) | 自定义表情数据模型 | 18 |
| `CustomParameterData` | `CustomParameterData` | `com.ai.assistance.operit.data.model` | `ModelParameter.kt` | class CustomParameterData(val id: String, val name: String, val apiName: String, val description: String, val defaultValue: String, val currentValue: String, val isEnabled: Boolean, va… | 自定义参数数据，用于JSON序列化 | 40 |
| `DateSerializer` | `DateSerializer` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | object DateSerializer : KSerializer<Date> | Date 类型的序列化器 将 Date 序列化为时间戳（Long） | 16 |
| `DimensionCount` | `DimensionCount` | `com.ai.assistance.operit.data.model` | `EmbeddingDimensionUsage.kt` | class DimensionCount(val dimension: Int, val count: Int) |  | 3 |
| `DocumentChunk` | `DocumentChunk` | `com.ai.assistance.operit.data.model` | `DocumentChunk.kt` | class DocumentChunk(var id: Long, var content: String, var chunkIndex: Int, var embedding: Embedding?) | 表示外部文档中的一个内容区块（例如，一个段落）。 每个区块都有自己的内容和向量嵌入，以便进行独立的语义搜索。 | 14 |
| `DragonBonesConfig` | `DragonBonesConfig` | `com.ai.assistance.operit.data.model` | `DragonBones.kt` | class DragonBonesConfig(val modelId: String, val scale: Float, val translateX: Float, val translateY: Float) | Represents the configuration for the DragonBones view. | 42 |
| `DragonBonesModel` | `DragonBonesModel` | `com.ai.assistance.operit.data.model` | `DragonBones.kt` | class DragonBonesModel(val id: String, val name: String, val folderPath: String, val skeletonFile: String, val textureJsonFile: String, val textureImageFile: String, val isBuiltIn: … | Represents a single DragonBones model's metadata. | 24 |
| `Embedding` | `Embedding` | `com.ai.assistance.operit.data.model` | `Embedding.kt` | class Embedding(val vector: FloatArray) | A wrapper class for a FloatArray to be used as an ObjectBox entity property. This helps t… | 9 |
| `EmbeddingConverter` | `EmbeddingConverter` | `com.ai.assistance.operit.data.model` | `EmbeddingConverter.kt` | class EmbeddingConverter | ObjectBox-compatible converter for Embedding <-> ByteArray. | 9 |
| `EmbeddingDimensionUsage` | `EmbeddingDimensionUsage` | `com.ai.assistance.operit.data.model` | `EmbeddingDimensionUsage.kt` | class EmbeddingDimensionUsage(val memoryTotal: Int, val memoryMissing: Int, val memoryDimensions: List<DimensionCount>, val chunkTotal: Int, val chunkMissing: Int, val chunkDimensions: Lis… |  | 8 |
| `EmbeddingRebuildProgress` | `EmbeddingRebuildProgress` | `com.ai.assistance.operit.data.model` | `EmbeddingDimensionUsage.kt` | class EmbeddingRebuildProgress(val total: Int, val processed: Int, val failed: Int, val currentStage: String) |  | 17 |
| `ExecuteNode` | `ExecuteNode` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class ExecuteNode(override val id: String, override val type: String, override var name: String, override var description: String, override var position: NodePosition, var acti… : WorkflowNode | 执行节点 定义工作流的执行动作 | 70 |
| `ExecutionStatus` | `ExecutionStatus` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class ExecutionStatus | 执行状态枚举 | 32 |
| `ExtractMode` | `ExtractMode` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class ExtractMode |  | 124 |
| `ExtractNode` | `ExtractNode` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class ExtractNode(override val id: String, override val type: String, override var name: String, override var description: String, override var position: NodePosition, var sour… : WorkflowNode |  | 134 |
| `FunctionType` | `FunctionType` | `com.ai.assistance.operit.data.model` | `FunctionType.kt` | class FunctionType | 表示不同功能类型，用于指定不同功能使用的AI配置 | 4 |
| `FunctionTypeTest` | `FunctionTypeTest` | `com.ai.assistance.operit.data.model` | `FunctionTypeTest.kt` | class FunctionTypeTest |  | 7 |
| `GroupMemberConfig` | `GroupMemberConfig` | `com.ai.assistance.operit.data.model` | `CharacterGroupCard.kt` | class GroupMemberConfig(val characterCardId: String, val orderIndex: Int) | 群组角色卡成员配置 | 6 |
| `ImportStrategy` | `ImportStrategy` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | class ImportStrategy | 导入策略枚举 定义遇到重复记忆时的处理方式 | 80 |
| `InputProcessingState` | `InputProcessingState` | `com.ai.assistance.operit.data.model` | `InputProcessingState.kt` | class InputProcessingState | UI状态，用于显示AI服务在做什么 | 4 |
| `InputProcessingState.Completed` | `InputProcessingState` | `com.ai.assistance.operit.data.model` | `InputProcessingState.kt` | object Completed : InputProcessingState |  | 36 |
| `InputProcessingState.Connecting` | `InputProcessingState` | `com.ai.assistance.operit.data.model` | `InputProcessingState.kt` | class Connecting(val message: String) : InputProcessingState | 正在连接到AI服务 | 12 |
| `InputProcessingState.ExecutingPlan` | `InputProcessingState` | `com.ai.assistance.operit.data.model` | `InputProcessingState.kt` | class ExecutingPlan(val message: String) : InputProcessingState | 新增：正在执行计划 | 33 |
| `InputProcessingState.ExecutingTool` | `InputProcessingState` | `com.ai.assistance.operit.data.model` | `InputProcessingState.kt` | class ExecutingTool(val toolName: String) : InputProcessingState | 新增：正在执行工具 | 18 |
| `InputProcessingState.Idle` | `InputProcessingState` | `com.ai.assistance.operit.data.model` | `InputProcessingState.kt` | object Idle : InputProcessingState | 空闲状态 | 6 |
| `InputProcessingState.ProcessingToolResult` | `InputProcessingState` | `com.ai.assistance.operit.data.model` | `InputProcessingState.kt` | class ProcessingToolResult(val toolName: String) : InputProcessingState | 新增：正在处理工具结果 | 27 |
| `LegacyUserProfile` | `LegacyUserProfile` | `com.ai.assistance.operit.data.model` | `LegacyUserProfile.kt` | class LegacyUserProfile(val id: String, val name: String, val birthDate: Long, val gender: String, val personality: String, val identity: String, val occupation: String, val aiStyle:… | Released structured profile payload, retained only so later migrations can preserve data. | 7 |
| `LogicNode` | `LogicNode` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class LogicNode(override val id: String, override val type: String, override var name: String, override var description: String, override var position: NodePosition, var oper… : WorkflowNode |  | 114 |
| `LogicOperator` | `LogicOperator` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class LogicOperator |  | 108 |
| `Memory` | `Memory` | `com.ai.assistance.operit.data.model` | `Memory.kt` | class Memory(var id: Long, var uuid: String, var title: String, var content: String, var contentType: String, var source: String, var credibility: Float, var importance: F… | 核心记忆单元 (Memory Unit) 代表一个独立的知识片段、事件、概念或任何AI需要记住的东西。 | 18 |
| `MemoryAutoSaveCandidate` | `MemoryAutoSaveCandidate` | `com.ai.assistance.operit.data.model` | `MemoryAutoSaveCandidate.kt` | class MemoryAutoSaveCandidate(var id: Long, var chatId: String, var triggerMessageTimestamp: Long, var createdAt: Date, var updatedAt: Date, var status: String, var attemptCount: Int, var … |  | 9 |
| `MemoryAutoSaveCandidateTest` | `MemoryAutoSaveCandidateTest` | `com.ai.assistance.operit.data.model` | `MemoryAutoSaveCandidateTest.kt` | class MemoryAutoSaveCandidateTest |  | 10 |
| `MemoryExportData` | `MemoryExportData` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | class MemoryExportData(val memories: List<SerializableMemory>, val links: List<SerializableLink>, val exportDate: Date, val version: String) | 记忆导出数据容器 包含完整的记忆库数据 | 68 |
| `MemoryImportResult` | `MemoryImportResult` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | class MemoryImportResult(val newMemories: Int, val updatedMemories: Int, val skippedMemories: Int, val newLinks: Int) | 记忆导入结果 记录导入操作的统计信息 | 101 |
| `MemoryLink` | `MemoryLink` | `com.ai.assistance.operit.data.model` | `Memory.kt` | class MemoryLink(var id: Long, var type: String, var weight: Float, var description: String) | 记忆关联 (Memory Link) 定义记忆之间的关系。 | 93 |
| `MemoryProperty` | `MemoryProperty` | `com.ai.assistance.operit.data.model` | `Memory.kt` | class MemoryProperty(var id: Long, var key: String, var value: String) | 记忆属性 (Memory Property) 灵活的键值对存储，用于扩展记忆的元数据。 | 109 |
| `MemoryScoreMode` | `MemoryScoreMode` | `com.ai.assistance.operit.data.model` | `MemorySearchConfig.kt` | class MemoryScoreMode |  | 3 |
| `MemorySearchConfig` | `MemorySearchConfig` | `com.ai.assistance.operit.data.model` | `MemorySearchConfig.kt` | class MemorySearchConfig(val scoreMode: MemoryScoreMode, val keywordWeight: Float, val tagWeight: Float, val vectorWeight: Float, val edgeWeight: Float) |  | 9 |
| `MemorySearchDebugCandidate` | `MemorySearchDebugCandidate` | `com.ai.assistance.operit.data.model` | `MemorySearchDebugInfo.kt` | class MemorySearchDebugCandidate(val memoryId: Long, val title: String, val folderPath: String?, val matchedKeywordTokenCount: Int, val keywordScore: Double, val tagScore: Double, val reverse… |  | 26 |
| `MemorySearchDebugInfo` | `MemorySearchDebugInfo` | `com.ai.assistance.operit.data.model` | `MemorySearchDebugInfo.kt` | class MemorySearchDebugInfo(val query: String, val keywords: List<String>, val lexicalTokens: List<String>, val scoreMode: MemoryScoreMode, val relevanceThreshold: Double, val effectiveK… |  | 3 |
| `MemorySpace` | `MemorySpace` | `com.ai.assistance.operit.data.model` | `MemorySpace.kt` | class MemorySpace(val id: String, val name: String, val profileAutoUpdateEnabled: Boolean, val profileAutoUpdateLocked: Boolean) | Metadata for an isolated long-term memory database. The identifier intentionally remains … | 12 |
| `MemoryTag` | `MemoryTag` | `com.ai.assistance.operit.data.model` | `Memory.kt` | class MemoryTag(var id: Long, var name: String) | 记忆标签 (Memory Tag) 用于对记忆进行分类和组织，支持层级结构。 | 76 |
| `MessageEntity` | `MessageEntity` | `com.ai.assistance.operit.data.model` | `MessageEntity.kt` | class MessageEntity(val messageId: Long, val chatId: String, val sender: String, val content: String, val timestamp: Long, val orderIndex: Int, val roleName: String, val selected… |  | 21 |
| `MessageEntityTest` | `MessageEntityTest` | `com.ai.assistance.operit.data.model` | `MessageEntityTest.kt` | class MessageEntityTest |  | 10 |
| `MessageVariantEntity` | `MessageVariantEntity` | `com.ai.assistance.operit.data.model` | `MessageVariantEntity.kt` | class MessageVariantEntity(val variantId: Long, val chatId: String, val messageTimestamp: Long, val variantIndex: Int, val content: String, val roleName: String, val provider: String, v… |  | 23 |
| `MessageVariantEntityTest` | `MessageVariantEntityTest` | `com.ai.assistance.operit.data.model` | `MessageVariantEntityTest.kt` | class MessageVariantEntityTest |  | 7 |
| `MiscModelTest` | `MiscModelTest` | `com.ai.assistance.operit.data.model` | `MiscModelTest.kt` | class MiscModelTest |  | 8 |
| `ModelConfigData` | `ModelConfigData` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | class ModelConfigData | 表示完整的模型配置，包括API设置和模型参数 | 95 |
| `ModelConfigDefaults` | `ModelConfigDefaults` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | object ModelConfigDefaults |  | 60 |
| `ModelConfigSummary` | `ModelConfigSummary` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | class ModelConfigSummary(val id: String, val name: String, val modelName: String, val apiEndpoint: String, val apiProviderType: ApiProviderType, val apiProviderTypeId: String, val thi… | 简化版的模型配置数据，用于列表显示 | 206 |
| `ModelOption` | `ModelOption` | `com.ai.assistance.operit.data.model` | `OpenAIModels.kt` | class ModelOption(val id: String, val name: String) | 提供给UI列表显示的模型信息 | 9 |
| `ModelParameter` | `ModelParameter` | `com.ai.assistance.operit.data.model` | `ModelParameter.kt` | class ModelParameter(val id: String, val name: String, val apiName: String, val description: String, val defaultValue: T, val currentValue: T, val isEnabled: Boolean, val valueTyp… | 模型参数类，支持泛型以表示不同类型的参数 | 6 |
| `ModelParameterTest` | `ModelParameterTest` | `com.ai.assistance.operit.data.model` | `ModelParameterTest.kt` | class ModelParameterTest |  | 9 |
| `ModelType` | `ModelType` | `com.ai.assistance.operit.data.model` | `DragonBones.kt` | class ModelType | The type of animation logic to apply to a model. | 8 |
| `OperitArchivedChat` | `OperitArchivedChat` | `com.ai.assistance.operit.data.model` | `OperitChatArchive.kt` | class OperitArchivedChat(val id: String, val title: String, val messages: List<OperitArchivedMessage>, val createdAt: LocalDateTime, val updatedAt: LocalDateTime, val inputTokens: Lon… |  | 21 |
| `OperitArchivedMessage` | `OperitArchivedMessage` | `com.ai.assistance.operit.data.model` | `OperitChatArchive.kt` | class OperitArchivedMessage(val baseMessage: ChatMessage, val variants: List<OperitArchivedMessageVar…) |  | 93 |
| `OperitArchivedMessageVariant` | `OperitArchivedMessageVariant` | `com.ai.assistance.operit.data.model` | `OperitChatArchive.kt` | class OperitArchivedMessageVariant(val variantIndex: Int, val content: String, val roleName: String, val provider: String, val modelName: String, val inputTokens: Long, val outputTokens: Long, … |  | 99 |
| `OperitAttachedTagPayload` | `OperitAttachedTagPayload` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class OperitAttachedTagPayload(val id: String, val name: String, val description: String, val promptContent: String, val tagType: String) |  | 142 |
| `OperitCharacterCardPayload` | `OperitCharacterCardPayload` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class OperitCharacterCardPayload(val name: String, val description: String, val characterSetting: String, val openingStatement: String, val otherContent: String, val otherContentChat: String,… |  | 122 |
| `OperitChatArchive` | `OperitChatArchive` | `com.ai.assistance.operit.data.model` | `OperitChatArchive.kt` | class OperitChatArchive(val archiveType: String, val formatVersion: Int, val exportedAt: Long, val chats: List<OperitArchivedChat>) |  | 8 |
| `OperitNodeInfo` | `OperitNodeInfo` | `com.ai.assistance.operit.data.model` | `OperitNodeInfo.kt` | class OperitNodeInfo(val children: List<OperitNodeInfo>, val className: String?, val packageName: String?, val text: String?, val contentDescription: String?, val viewIdResourceNa… : Serializable | 一个可序列化的数据类，用于替代AccessibilityNodeInfo，以便在进程间传递。 它包含了节点的大部分关键信息，并且可以方便地通过Gson进行序列化和反序列化。 | 10 |
| `OperitTavernExtension` | `OperitTavernExtension` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class OperitTavernExtension(val schema: String, val character_card: OperitCharacterCardPayload) |  | 117 |
| `PackageToolPromptCategory` | `PackageToolPromptCategory` | `com.ai.assistance.operit.data.model` | `ToolPrompt.kt` | class PackageToolPromptCategory(val packageName: String, val packageDescription: String, val tools: List<ToolPrompt>) | 包工具提示词分类数据类 表示来自包（Package）的工具集合，用于动态生成包工具的提示词 | 119 |
| `ParameterCategory` | `ParameterCategory` | `com.ai.assistance.operit.data.model` | `ModelParameter.kt` | class ParameterCategory | 参数分类枚举 | 31 |
| `ParameterDefinition` | `ParameterDefinition` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | class ParameterDefinition(val id: String, val name: String, : StringRes val nameResId: Int, val apiName: String, val description: String, : StringRes val descriptionResI…, val defaultV… : Any> | A data class to hold the static definition of a model parameter. This serves as a single … | 23 |
| `ParameterValue` | `ParameterValue` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class ParameterValue | 参数值类型 支持静态值或引用其他节点的输出 | 161 |
| `ParameterValue.NodePosition` | `ParameterValue` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class NodePosition(var x: Float, var y: Float) | 节点位置信息（用于将来的可视化编辑器） | 173 |
| `ParameterValue.StaticValue` | `ParameterValue` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class StaticValue(val value: String) : ParameterValue |  | 163 |
| `ParameterValue.WorkflowNodeConnection` | `ParameterValue` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class WorkflowNodeConnection(val id: String, val sourceNodeId: String, val targetNodeId: String, var condition: String?) | 工作流节点连接 定义节点之间的连接关系 | 183 |
| `ParameterValueType` | `ParameterValueType` | `com.ai.assistance.operit.data.model` | `ModelParameter.kt` | class ParameterValueType | 参数值类型枚举 | 22 |
| `PromptFunctionType` | `PromptFunctionType` | `com.ai.assistance.operit.data.model` | `PromptFunctionType.kt` | class PromptFunctionType | Prompt function type, used to distinguish message context | 6 |
| `PromptTag` | `PromptTag` | `com.ai.assistance.operit.data.model` | `PromptTag.kt` | class PromptTag(val id: String, val name: String, val description: String, val promptContent: String, val tagType: TagType, val createdAt: Long, val updatedAt: Long) | 提示词标签数据模型 | 10 |
| `PromptTagTest` | `PromptTagTest` | `com.ai.assistance.operit.data.model` | `PromptTagTest.kt` | class PromptTagTest |  | 7 |
| `ProviderIdentityUtilsTest` | `ProviderIdentityUtilsTest` | `com.ai.assistance.operit.data.model` | `ProviderIdentityUtilsTest.kt` | class ProviderIdentityUtilsTest |  | 6 |
| `SerializableColorScheme` | `SerializableColorScheme` | `com.ai.assistance.operit.data.model` | `SerializableColorScheme.kt` | class SerializableColorScheme(val primary: Long, val onPrimary: Long, val primaryContainer: Long, val onPrimaryContainer: Long, val inversePrimary: Long, val secondary: Long, val onSeconda… : Parcelable |  | 9 |
| `SerializableLink` | `SerializableLink` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | class SerializableLink(val sourceUuid: String, val targetUuid: String, val type: String, val weight: Float, val description: String) | 可序列化的链接关系 使用 UUID 来引用记忆 | 55 |
| `SerializableMemory` | `SerializableMemory` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | class SerializableMemory(val uuid: String, val title: String, val content: String, val contentType: String, val source: String, val credibility: Float, val importance: Float, val fold… | 可序列化的记忆数据 用于导出导入时的数据传输 | 34 |
| `SerializableTextStyle` | `SerializableTextStyle` | `com.ai.assistance.operit.data.model` | `SerializableTypography.kt` | class SerializableTextStyle(val fontSize: Float, val lineHeight: Float, val letterSpacing: Float, val fontWeight: Int) : Parcelable |  | 31 |
| `SerializableTypography` | `SerializableTypography` | `com.ai.assistance.operit.data.model` | `SerializableTypography.kt` | class SerializableTypography(val displayLarge: SerializableTextStyle, val displayMedium: SerializableTextStyle, val displaySmall: SerializableTextStyle, val headlineLarge: SerializableTex… : Parcelable |  | 12 |
| `StandardModelParameters` | `StandardModelParameters` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | object StandardModelParameters | A central repository for the definitions of all standard model parameters. | 40 |
| `SummarySectionConfig` | `SummarySectionConfig` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | class SummarySectionConfig(val id: String, val enabled: Boolean, val title: String, val instruction: String) |  | 71 |
| `SummarySectionOverride` | `SummarySectionOverride` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | class SummarySectionOverride(val id: String, val enabled: Boolean?, val title: String?, val instruction: String?) |  | 79 |
| `SystemToolPromptCategory` | `SystemToolPromptCategory` | `com.ai.assistance.operit.data.model` | `ToolPrompt.kt` | class SystemToolPromptCategory(val categoryName: String, val categoryHeader: String, val tools: List<ToolPrompt>, val categoryFooter: String) | 工具分类数据类 表示一组相关工具的集合 | 74 |
| `TagType` | `TagType` | `com.ai.assistance.operit.data.model` | `PromptTag.kt` | class TagType | 标签类型枚举 | 24 |
| `TavernBookEntry` | `TavernBookEntry` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class TavernBookEntry(val name: String, val keys: List<String>, val secondary_keys: List<String>, val content: String, val enabled: Boolean, val insertion_order: Int, val case_sens… |  | 177 |
| `TavernCharacterBook` | `TavernCharacterBook` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class TavernCharacterBook(val name: String, val description: String, val scan_depth: Int, val token_budget: Int, val recursive_scanning: Boolean, val extensions: Map<String, Any>, val … |  | 167 |
| `TavernCharacterCard` | `TavernCharacterCard` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class TavernCharacterCard(val spec: String, val spec_version: String, val data: TavernCharacterData) | 酒馆角色卡格式数据模型 | 86 |
| `TavernCharacterData` | `TavernCharacterData` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class TavernCharacterData(val name: String, val description: String, val personality: String, val first_mes: String, val avatar: String, val mes_example: String, val scenario: String, … |  | 92 |
| `TavernChubExtension` | `TavernChubExtension` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class TavernChubExtension(val id: Long, val preset: String?, val full_path: String, val extensions: List<String>, val expressions: String?, val alt_expressions: Map<String, String>, va… |  | 150 |
| `TavernDepthPrompt` | `TavernDepthPrompt` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class TavernDepthPrompt(val role: String, val depth: Int, val prompt: String) |  | 161 |
| `TavernExtensions` | `TavernExtensions` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | class TavernExtensions(val chub: TavernChubExtension?, val depth_prompt: TavernDepthPrompt?, val operit: OperitTavernExtension?) |  | 111 |
| `TokenStatsModelEntity` | `TokenStatsModelEntity` | `com.ai.assistance.operit.data.model` | `TokenStatsModelEntity.kt` | class TokenStatsModelEntity(/** Empty means provider/model-wide pricing and the configuration-unscoped identity. */ val configId: String, val provider: String, val model: String, val bil… |  | 9 |
| `TokenUsageRecordEntity` | `TokenUsageRecordEntity` | `com.ai.assistance.operit.data.model` | `TokenUsageRecordEntity.kt` | class TokenUsageRecordEntity(val id: Long, val importKey: String?, val occurredAtMs: Long?, val configId: String, val provider: String, val model: String, val requestCount: Long, val unca… |  | 16 |
| `ToolInvocation` | `ToolInvocation` | `com.ai.assistance.operit.data.model` | `AITool.kt` | class ToolInvocation(val tool: AITool, val rawText: String, val responseLocation: IntRange) | Represents an invocation of a tool in the AI's response | 20 |
| `ToolParameterSchema` | `ToolParameterSchema` | `com.ai.assistance.operit.data.model` | `ToolPrompt.kt` | class ToolParameterSchema(val name: String, val type: String, val description: String, val required: Boolean, val default: String?) | 工具参数模式定义（用于定义工具的参数结构） | 6 |
| `ToolPrompt` | `ToolPrompt` | `com.ai.assistance.operit.data.model` | `ToolPrompt.kt` | class ToolPrompt(val name: String, val description: String, val parameters: String, val parametersStructured: List<ToolParameterSchema>?, val details: String, val notes: Strin… | 工具提示词数据类 表示单个工具的完整提示词信息 | 18 |
| `ToolResult` | `ToolResult` | `com.ai.assistance.operit.data.model` | `AITool.kt` | class ToolResult(val toolName: String, val success: Boolean, val result: ToolResultData, val error: String?) | Represents the result of a tool execution | 29 |
| `TriggerNode` | `TriggerNode` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class TriggerNode(override val id: String, override val type: String, override var name: String, override var description: String, override var position: NodePosition, var trig… : WorkflowNode | 触发节点 定义工作流的触发条件（暂时为占位符） | 55 |
| `Workflow` | `Workflow` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class Workflow(val id: String, var name: String, var description: String, var nodes: List<WorkflowNode>, var connections: List<WorkflowNodeConnection>, val createdAt: Long, … | 工作流模型 代表一个完整的自动化工作流程 | 11 |
| `WorkflowExecutionFailureStage` | `WorkflowExecutionFailureStage` | `com.ai.assistance.operit.data.model` | `WorkflowExecutionLog.kt` | class WorkflowExecutionFailureStage |  | 14 |
| `WorkflowExecutionLogEntry` | `WorkflowExecutionLogEntry` | `com.ai.assistance.operit.data.model` | `WorkflowExecutionLog.kt` | class WorkflowExecutionLogEntry(val timestamp: Long, val level: WorkflowLogLevel, val message: String, val nodeId: String?, val nodeName: String?) |  | 22 |
| `WorkflowExecutionRecord` | `WorkflowExecutionRecord` | `com.ai.assistance.operit.data.model` | `WorkflowExecutionLog.kt` | class WorkflowExecutionRecord(val runId: String, val workflowId: String, val workflowName: String, val triggerNodeId: String?, val startedAt: Long, val finishedAt: Long, val success: Boole… |  | 31 |
| `WorkflowLogLevel` | `WorkflowLogLevel` | `com.ai.assistance.operit.data.model` | `WorkflowExecutionLog.kt` | class WorkflowLogLevel |  | 7 |
| `WorkflowNode` | `WorkflowNode` | `com.ai.assistance.operit.data.model` | `Workflow.kt` | class WorkflowNode | 工作流节点基类 | 42 |
| `WorkspaceRenameResult` | `WorkspaceRenameResult` | `com.ai.assistance.operit.data.model` | `WorkspaceRenameResult.kt` | class WorkspaceRenameResult(val workspacePath: String, val workspaceEnv: String?, val workspaceName: String) |  | 3 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `ApiKeyFormatValidator.normalize` | `ApiKeyFormatValidator` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidator.kt` | value: String | String |  | 4 |
| `ApiKeyFormatValidator.isValid` | `ApiKeyFormatValidator` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidator.kt` | value: String | Boolean |  | 6 |
| `ApiKeyFormatValidator.hasUsableKey` | `ApiKeyFormatValidator` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidator.kt` | config: ModelConfigData | Boolean |  | 13 |
| `BillingMode.fromString` | `BillingMode` | `com.ai.assistance.operit.data.model` | `BillingMode.kt` | value: String? | BillingMode | 从字符串解析计费方式 | 26 |
| `CharacterCardToolAccessConfig.normalized` | `CharacterCardToolAccessConfig` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` |  | CharacterCardToolAccessConfig |  | 15 |
| `CharacterCardToolAccessConfig.hasExternalSelections` | `CharacterCardToolAccessConfig` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` |  | Boolean |  | 24 |
| `CharacterCardToolAccessConfig.normalizeEntries` | `CharacterCardToolAccessConfig` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | values: List<String> | List<String> |  | 30 |
| `CharacterCardChatModelBindingMode.normalize` | `CharacterCardChatModelBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | mode: String? | String |  | 69 |
| `CharacterCardMemoryProfileBindingMode.normalize` | `CharacterCardMemoryProfileBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | mode: String? | String |  | 78 |
| `ChatEntity.toChatHistory` | `ChatEntity` | `com.ai.assistance.operit.data.model` | `ChatEntity.kt` | messages: List<ChatMessage> | ChatHistory | 转换为ChatHistory对象（供UI层使用） | 30 |
| `ChatEntity.fromChatHistory` | `ChatEntity` | `com.ai.assistance.operit.data.model` | `ChatEntity.kt` | chatHistory: ChatHistory | ChatEntity | 从ChatHistory创建ChatEntity | 62 |
| `ChatMessage.writeToParcel` | `ChatMessage` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | parcel: Parcel<br>flags: Int | Unit |  | 60 |
| `ChatMessage.describeContents` | `ChatMessage` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` |  | Int |  | 81 |
| `ChatMessage.CREATOR.readDisplayModeFromParcel` | `CREATOR` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | parcel: Parcel | ChatMessageDisplayMode |  | 86 |
| `ChatMessage.CREATOR.readBooleanFromParcel` | `CREATOR` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | parcel: Parcel | Boolean |  | 97 |
| `ChatMessage.CREATOR.createFromParcel` | `CREATOR` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | parcel: Parcel | ChatMessage |  | 101 |
| `ChatMessage.CREATOR.newArray` | `CREATOR` | `com.ai.assistance.operit.data.model` | `ChatMessage.kt` | size: Int | Array<ChatMessage?> |  | 105 |
| `ChatMessageTimestampAllocator.next` | `ChatMessageTimestampAllocator` | `com.ai.assistance.operit.data.model` | `ChatMessageTimestampAllocator.kt` | baseTimestamp: Long? | Long |  | 14 |
| `ChatMessageTimestampAllocator.observe` | `ChatMessageTimestampAllocator` | `com.ai.assistance.operit.data.model` | `ChatMessageTimestampAllocator.kt` | timestamp: Long | Unit |  | 24 |
| `CloudEmbeddingConfig.normalized` | `CloudEmbeddingConfig` | `com.ai.assistance.operit.data.model` | `CloudEmbeddingConfig.kt` |  | CloudEmbeddingConfig |  | 9 |
| `CloudEmbeddingConfig.isReady` | `CloudEmbeddingConfig` | `com.ai.assistance.operit.data.model` | `CloudEmbeddingConfig.kt` |  | Boolean |  | 17 |
| `Embedding.equals` | `Embedding` | `com.ai.assistance.operit.data.model` | `Embedding.kt` | other: Any? | Boolean | Custom equals/hashCode to properly compare float arrays | 11 |
| `Embedding.hashCode` | `Embedding` | `com.ai.assistance.operit.data.model` | `Embedding.kt` |  | Int |  | 18 |
| `EmbeddingConverter.convertToEntityProperty` | `EmbeddingConverter` | `com.ai.assistance.operit.data.model` | `EmbeddingConverter.kt` | databaseValue: ByteArray? | Embedding? |  | 10 |
| `EmbeddingConverter.convertToDatabaseValue` | `EmbeddingConverter` | `com.ai.assistance.operit.data.model` | `EmbeddingConverter.kt` | entityProperty: Embedding? | ByteArray? |  | 21 |
| `MemoryAutoSaveCandidate.isSelectedUserMessageSource` | `MemoryAutoSaveCandidate` | `com.ai.assistance.operit.data.model` | `MemoryAutoSaveCandidate.kt` | sourceType: String | Boolean |  | 28 |
| `DateSerializer.serialize` | `DateSerializer` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | encoder: Encoder<br>value: Date | Unit |  | 20 |
| `DateSerializer.deserialize` | `DateSerializer` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | decoder: Decoder | Date |  | 24 |
| `MemorySearchConfig.normalized` | `MemorySearchConfig` | `com.ai.assistance.operit.data.model` | `MemorySearchConfig.kt` |  | MemorySearchConfig |  | 16 |
| `MessageEntity.toChatMessage` | `MessageEntity` | `com.ai.assistance.operit.data.model` | `MessageEntity.kt` |  | ChatMessage | 转换为ChatMessage对象（供UI层使用） | 43 |
| `MessageEntity.fromChatMessage` | `MessageEntity` | `com.ai.assistance.operit.data.model` | `MessageEntity.kt` | chatId: String<br>message: ChatMessage<br>orderIndex: Int<br>messageId: Long? | MessageEntity | 从ChatMessage创建MessageEntity | 68 |
| `MessageVariantEntity.applyTo` | `MessageVariantEntity` | `com.ai.assistance.operit.data.model` | `MessageVariantEntity.kt` | baseMessage: ChatMessage<br>variantCount: Int | ChatMessage |  | 40 |
| `MessageVariantEntity.fromChatMessage` | `MessageVariantEntity` | `com.ai.assistance.operit.data.model` | `MessageVariantEntity.kt` | chatId: String<br>messageTimestamp: Long<br>variantIndex: Int<br>message: ChatMessage<br>variantId: Long? | MessageVariantEntity |  | 59 |
| `ApiProviderType.fromProviderTypeId` | `ApiProviderType` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | providerTypeId: String | ApiProviderType? |  | 48 |
| `getModelByIndex` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | modelName: String<br>index: Int | String | 从逗号分隔的模型名称字符串中根据索引获取具体模型 | 219 |
| `getModelList` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | modelName: String | List<String> | 获取模型列表 | 226 |
| `getValidModelIndex` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | modelName: String<br>requestedIndex: Int | Int | 计算有效的模型索引（处理越界情况） 如果索引超出范围，自动返回0（第一个模型） | 238 |
| `OperitArchivedChat.toChatHistory` | `OperitArchivedChat` | `com.ai.assistance.operit.data.model` | `OperitChatArchive.kt` |  | ChatHistory |  | 42 |
| `OperitArchivedChat.fromChatHistory` | `OperitArchivedChat` | `com.ai.assistance.operit.data.model` | `OperitChatArchive.kt` | history: ChatHistory<br>messages: List<OperitArchivedMessage> | OperitArchivedChat |  | 65 |
| `OperitArchivedMessageVariant.toEntity` | `OperitArchivedMessageVariant` | `com.ai.assistance.operit.data.model` | `OperitChatArchive.kt` | chatId: String<br>messageTimestamp: Long | MessageVariantEntity |  | 113 |
| `OperitArchivedMessageVariant.fromEntity` | `OperitArchivedMessageVariant` | `com.ai.assistance.operit.data.model` | `OperitChatArchive.kt` | entity: MessageVariantEntity | OperitArchivedMessageVariant |  | 133 |
| `OperitNodeInfo.getBounds` | `OperitNodeInfo` | `com.ai.assistance.operit.data.model` | `OperitNodeInfo.kt` |  | android.graphics.Rect? | 为了方便，可以添加一些辅助函数来解析bounds | 47 |
| `normalizeProviderTypeId` | — | `com.ai.assistance.operit.data.model` | `ProviderIdentityUtils.kt` | providerTypeId: String | String | Keeps legacy display-oriented provider values usable without rewriting stored history. | 4 |
| `normalizeProviderModel` | — | `com.ai.assistance.operit.data.model` | `ProviderIdentityUtils.kt` | providerModel: String | String | Normalizes only the provider part of a `provider:model` identity. | 15 |
| `hasIndependentCacheWriteBilling` | — | `com.ai.assistance.operit.data.model` | `ProviderIdentityUtils.kt` | providerTypeId: String | Boolean | Returns whether missing cache-write usage must remain an unknown billed component. | 23 |
| `toSerializable` | — | `com.ai.assistance.operit.data.model` | `SerializableColorScheme.kt` |  | SerializableColorScheme |  | 41 |
| `toComposeColorScheme` | — | `com.ai.assistance.operit.data.model` | `SerializableColorScheme.kt` |  | ColorScheme |  | 75 |
| `toSerializable` | — | `com.ai.assistance.operit.data.model` | `SerializableTypography.kt` |  | SerializableTypography |  | 38 |
| `toSerializable` | — | `com.ai.assistance.operit.data.model` | `SerializableTypography.kt` |  | SerializableTextStyle |  | 58 |
| `toComposeTypography` | — | `com.ai.assistance.operit.data.model` | `SerializableTypography.kt` |  | Typography |  | 67 |
| `toComposeTextStyle` | — | `com.ai.assistance.operit.data.model` | `SerializableTypography.kt` |  | TextStyle |  | 87 |
| `ToolPrompt.toString` | `ToolPrompt` | `com.ai.assistance.operit.data.model` | `ToolPrompt.kt` |  | String | 将工具提示词转换为原始系统提示词格式 | 29 |
| `SystemToolPromptCategory.toString` | `SystemToolPromptCategory` | `com.ai.assistance.operit.data.model` | `ToolPrompt.kt` |  | String | 将整个分类转换为原始系统提示词格式 | 83 |
| `PackageToolPromptCategory.toString` | `PackageToolPromptCategory` | `com.ai.assistance.operit.data.model` | `ToolPrompt.kt` |  | String | 将包工具分类转换为系统提示词格式 | 127 |
| `ApiKeyFormatValidatorTest.outerWhitespace_isNormalized` | `ApiKeyFormatValidatorTest` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidatorTest.kt` |  | Unit |  | 9 ⚑ |
| `ApiKeyFormatValidatorTest.nonAsciiCharacters_areRejected` | `ApiKeyFormatValidatorTest` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidatorTest.kt` |  | Unit |  | 14 ⚑ |
| `ApiKeyFormatValidatorTest.whitespaceAndControlCharacters_areRejected` | `ApiKeyFormatValidatorTest` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidatorTest.kt` |  | Unit |  | 21 ⚑ |
| `ApiKeyFormatValidatorTest.availableKeyPool_isAcceptedWithoutSingleKey` | `ApiKeyFormatValidatorTest` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidatorTest.kt` |  | Unit |  | 29 ⚑ |
| `ApiKeyFormatValidatorTest.invalidEnabledPoolEntry_rejectsWholePool` | `ApiKeyFormatValidatorTest` | `com.ai.assistance.operit.data.model` | `ApiKeyFormatValidatorTest.kt` |  | Unit |  | 49 ⚑ |
| `ChatHistoryTest.createHistory` | `ChatHistoryTest` | `com.ai.assistance.operit.data.model` | `ChatHistoryTest.kt` | id: String?<br>title: String?<br>messages: List<ChatMessage>?<br>displayOrder: Long? | Unit |  | 13 ⚑ |
| `ChatMessageTest.tearDown` | `ChatMessageTest` | `com.ai.assistance.operit.data.model` | `ChatMessageTest.kt` |  | Unit |  | 13 ⚑ |
| `MessageEntityTest.tearDown` | `MessageEntityTest` | `com.ai.assistance.operit.data.model` | `MessageEntityTest.kt` |  | Unit |  | 13 ⚑ |
| `MessageVariantEntityTest.tearDown` | `MessageVariantEntityTest` | `com.ai.assistance.operit.data.model` | `MessageVariantEntityTest.kt` |  | Unit |  | 10 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `apiEndpoint` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String |  | 101 |
| `apiKey` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String | API设置 | 100 |
| `apiKeyPool` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | List<ApiKeyInfo> |  | 108 |
| `apiProviderType` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | ApiProviderType |  | 103 |
| `apiProviderTypeId` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String |  | 104 |
| `CharacterCardChatModelBindingMode.FIXED_CONFIG` | `CharacterCardChatModelBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | inferred |  | 67 |
| `CharacterCardChatModelBindingMode.FOLLOW_GLOBAL` | `CharacterCardChatModelBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | inferred |  | 66 |
| `CharacterCardMemoryProfileBindingMode.FIXED_PROFILE` | `CharacterCardMemoryProfileBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | inferred |  | 76 |
| `CharacterCardMemoryProfileBindingMode.FOLLOW_GLOBAL` | `CharacterCardMemoryProfileBindingMode` | `com.ai.assistance.operit.data.model` | `CharacterCard.kt` | inferred |  | 75 |
| `ChatMessageTimestampAllocator.lastIssuedTimestamp` | `ChatMessageTimestampAllocator` | `com.ai.assistance.operit.data.model` | `ChatMessageTimestampAllocator.kt` | inferred |  | 12 |
| `contextLength` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Float | 上下文/总结配置 | 146 |
| `currentKeyIndex` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int |  | 109 |
| `customHeaders` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String | 自定义请求头JSON字符串 | 143 |
| `customParameters` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String | 自定义参数JSON字符串 | 134 |
| `DateSerializer.descriptor` | `DateSerializer` | `com.ai.assistance.operit.data.model` | `MemoryExportModel.kt` | SerialDescriptor |  | 17 |
| `enableClaude1hPromptCache` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | Claude特定配置 | 194 |
| `enableCodexWebSearch` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | Codex特定配置 | 191 |
| `enableDeepSeekWebSearch` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | DeepSeek特定配置 | 188 |
| `enableDirectAudioProcessing` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | 音频/视频处理配置 | 181 |
| `enableDirectImageProcessing` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | 图片处理配置 | 178 |
| `enableDirectVideoProcessing` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 182 |
| `enableGoogleSearch` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | Gemini特定配置 | 185 |
| `enableMaxContextMode` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 148 |
| `enableSummary` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 150 |
| `enableSummaryByMessageCount` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 151 |
| `enableSummaryDialogueReview` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 158 |
| `enableToolCall` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | Tool Call配置 | 197 |
| `frequencyPenalty` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Float |  | 130 |
| `frequencyPenaltyEnabled` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 121 |
| `hasCustomParameters` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | 是否包含自定义参数 | 113 |
| `id` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String, |  | 96 |
| `keyRotationMode` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String |  | 110 |
| `llamaBatchSize` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int |  | 169 |
| `llamaContextSize` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int |  | 168 |
| `llamaFlashAttention` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 173 |
| `llamaGpuLayers` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int |  | 171 |
| `llamaKvUnified` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 174 |
| `llamaOffloadKqv` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 175 |
| `llamaThreadCount` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int | llama.cpp 特定配置 | 167 |
| `llamaUBatchSize` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int |  | 170 |
| `llamaUseMmap` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 172 |
| `maxConcurrentRequests` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int |  | 201 |
| `maxContextLength` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Float |  | 147 |
| `maxTokens` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int | 模型参数值 | 125 |
| `maxTokensEnabled` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | 模型参数的enabled状态 | 116 |
| `mnnForwardType` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int | MNN特定配置 注意：MNN模型路径会根据modelName自动构建，不需要单独存储 | 163 |
| `mnnThreadCount` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int |  | 164 |
| `ModelConfigDefaults.DEFAULT_CONTEXT_LENGTH` | `ModelConfigDefaults` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | inferred |  | 61 |
| `ModelConfigDefaults.DEFAULT_ENABLE_MAX_CONTEXT_MODE` | `ModelConfigDefaults` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | inferred |  | 63 |
| `ModelConfigDefaults.DEFAULT_ENABLE_SUMMARY` | `ModelConfigDefaults` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | inferred |  | 66 |
| `ModelConfigDefaults.DEFAULT_ENABLE_SUMMARY_BY_MESSAGE_COUNT` | `ModelConfigDefaults` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | inferred |  | 67 |
| `ModelConfigDefaults.DEFAULT_ENABLE_TOOL_CALL` | `ModelConfigDefaults` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | inferred |  | 64 |
| `ModelConfigDefaults.DEFAULT_MAX_CONTEXT_LENGTH` | `ModelConfigDefaults` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | inferred |  | 62 |
| `ModelConfigDefaults.DEFAULT_SUMMARY_MESSAGE_COUNT_THRESHOLD` | `ModelConfigDefaults` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | inferred |  | 68 |
| `ModelConfigDefaults.DEFAULT_SUMMARY_TOKEN_THRESHOLD` | `ModelConfigDefaults` | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | inferred |  | 65 |
| `modelName` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String |  | 102 |
| `name` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String, |  | 97 |
| `presencePenalty` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Float |  | 129 |
| `presencePenaltyEnabled` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 120 |
| `repetitionPenalty` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Float |  | 131 |
| `repetitionPenaltyEnabled` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 122 |
| `requestLimitPerMinute` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int | 请求频率限制配置 | 200 |
| `StandardModelParameters.DEFAULT_FREQUENCY_PENALTY` | `StandardModelParameters` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | inferred |  | 47 |
| `StandardModelParameters.DEFAULT_MAX_TOKENS` | `StandardModelParameters` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | inferred | Default values for standard model parameters | 42 |
| `StandardModelParameters.DEFAULT_PRESENCE_PENALTY` | `StandardModelParameters` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | inferred |  | 46 |
| `StandardModelParameters.DEFAULT_REPETITION_PENALTY` | `StandardModelParameters` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | inferred |  | 48 |
| `StandardModelParameters.DEFAULT_TEMPERATURE` | `StandardModelParameters` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | inferred |  | 43 |
| `StandardModelParameters.DEFAULT_TOP_K` | `StandardModelParameters` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | inferred |  | 45 |
| `StandardModelParameters.DEFAULT_TOP_P` | `StandardModelParameters` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | inferred |  | 44 |
| `StandardModelParameters.DEFINITIONS` | `StandardModelParameters` | `com.ai.assistance.operit.data.model` | `StandardModelParameters.kt` | List<ParameterDefinition<*>> |  | 50 |
| `summaryCustomRules` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String | 自定义总结规则 | 156 |
| `summaryDialogueReviewTitle` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String |  | 159 |
| `summaryMessageCountThreshold` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int |  | 153 |
| `summarySectionOverrides` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | List<SummarySectionOverride> |  | 157 |
| `summaryTokenThreshold` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Float |  | 149 |
| `temperature` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Float |  | 126 |
| `temperatureEnabled` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 117 |
| `thinkingConfigurations` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String | 当前模型配置的思考规则；内置适配规则由data.collects集中维护并在配置创建或供应商切换时写入 | 137 |
| `thinkingOptionId` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | String | 当前模型配置选中的思考档位 | 140 |
| `topK` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Int |  | 128 |
| `topKEnabled` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 119 |
| `topP` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Float |  | 127 |
| `topPEnabled` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean |  | 118 |
| `useMultipleApiKeys` | — | `com.ai.assistance.operit.data.model` | `ModelConfigData.kt` | Boolean | 多API Key支持 | 107 |
