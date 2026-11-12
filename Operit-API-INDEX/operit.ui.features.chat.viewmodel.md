# operit.ui.features.chat.viewmodel

> 函数 215 · 类型 10 · 顶层常量 1 · 共 226 条
> 每日定时任务自动生成。

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ChatHistoryDisplayMode` | `ChatHistoryDisplayMode` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | class ChatHistoryDisplayMode |  | 98 |
| `ChatToastEvent` | `ChatToastEvent` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` | class ChatToastEvent(val id: Long, val message: String) |  | 11 |
| `ChatViewModel` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | class ChatViewModel(private val context: Context) : ViewModel |  | 104 |
| `ChatViewModel.ActiveMentionTrigger` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | class ActiveMentionTrigger(val triggerChar: Char, val triggerIndex: Int, val query: String) |  | 111 |
| `ChatViewModel.MentionDeletionNormalization` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | class MentionDeletionNormalization(val value: TextFieldValue, val removedMentionToken: String?) |  | 117 |
| `FloatingWindowDelegate` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` | class FloatingWindowDelegate(private val context: Context, private val coroutineScope: CoroutineScope, private val inputProcessingState: StateFlow<InputProcessingStat…) | 委托类，负责管理悬浮窗交互 | 28 |
| `PendingMessageQueueState` | `PendingMessageQueueState` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | class PendingMessageQueueState(val messages: List<PendingQueueMessageItem>, val isExpanded: Boolean, val wasBlocked: Boolean, val suppressNextAutoDequeue: Boolean) |  | 9 |
| `PendingMessageQueueStore` | `PendingMessageQueueStore` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | class PendingMessageQueueStore |  | 16 |
| `PendingMessageQueueStoreTest` | `PendingMessageQueueStoreTest` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStoreTest.kt` | class PendingMessageQueueStoreTest |  | 8 |
| `UiStateDelegate` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` | class UiStateDelegate | 委托类，负责管理UI状态相关功能 | 17 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `ChatViewModel.speechPreview` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | text: String | String |  | 122 |
| `ChatViewModel.logSpeechState` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | event: String<br>extra: String? | Unit |  | 126 |
| `ChatViewModel.onChatHistorySearchQueryChange` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | query: String | Unit |  | 325 |
| `ChatViewModel.setHistoryDisplayMode` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | mode: ChatHistoryDisplayMode | Unit |  | 329 |
| `ChatViewModel.setAutoSwitchCharacterCard` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | enabled: Boolean | Unit |  | 333 |
| `ChatViewModel.toggleAutoSwitchCharacterCard` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 337 |
| `ChatViewModel.setAutoSwitchChatOnCharacterSelect` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | enabled: Boolean | Unit |  | 341 |
| `ChatViewModel.initializeDelegates` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 454 |
| `ChatViewModel.updateWebServerForCurrentChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String | Unit |  | 467 |
| `ChatViewModel.resetAttachmentPanelState` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 471 |
| `ChatViewModel.clearReplyToMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 475 |
| `ChatViewModel.getReplyToMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | ChatMessage? |  | 479 |
| `ChatViewModel.setupPermissionSystemCollection` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 496 |
| `ChatViewModel.setupAttachmentDelegateToastCollection` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 504 |
| `ChatViewModel.checkIfShouldCreateNewChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 510 |
| `ChatViewModel.setupInputProcessingStateListener` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | service: EnhancedAIService | Unit | 设置输入处理状态监听 当 EnhancedAIService 初始化或更新时调用 | 524 |
| `ChatViewModel.updateApiKey` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | key: String | Unit | API配置相关方法 | 568 |
| `ChatViewModel.updateApiEndpoint` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | endpoint: String | Unit |  | 570 |
| `ChatViewModel.updateModelName` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | modelName: String | Unit |  | 572 |
| `ChatViewModel.updateApiProviderType` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | providerType: ApiProviderType | Unit |  | 574 |
| `ChatViewModel.saveApiSettings` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 575 |
| `ChatViewModel.saveDeepSeekConfiguration` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | configId: String<br>apiKey: String | Unit |  | 576 |
| `ChatViewModel.useDefaultConfig` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 579 |
| `ChatViewModel.toggleFeature` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | featureKey: String | Unit |  | 587 |
| `ChatViewModel.toggleThinkingMode` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 切换思考模式的方法现在委托给ApiConfigDelegate | 592 |
| `ChatViewModel.updateThinkingOptionId` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | optionId: String | Unit |  | 596 |
| `ChatViewModel.toggleMemoryAutoUpdate` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 切换记忆自动更新的方法现在委托给ApiConfigDelegate | 601 |
| `ChatViewModel.updateContextLength` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | length: Float | Unit | 更新上下文长度 | 606 |
| `ChatViewModel.updateMaxContextLength` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | length: Float | Unit |  | 610 |
| `ChatViewModel.toggleEnableMaxContextMode` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 614 |
| `ChatViewModel.updateSummaryTokenThreshold` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | threshold: Float | Unit |  | 618 |
| `ChatViewModel.toggleEnableSummary` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 622 |
| `ChatViewModel.toggleEnableSummaryByMessageCount` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 626 |
| `ChatViewModel.updateSummaryMessageCountThreshold` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | threshold: Int | Unit |  | 630 |
| `ChatViewModel.toggleTools` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 634 |
| `ChatViewModel.saveToolPromptVisibility` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | toolName: String<br>isVisible: Boolean | Unit |  | 638 |
| `ChatViewModel.saveToolPromptVisibilityMap` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | visibilityMap: Map<String, Boolean> | Unit |  | 642 |
| `ChatViewModel.saveToolPromptOrder` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | order: List<String> | Unit |  | 648 |
| `ChatViewModel.toggleDisableStreamOutput` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 652 |
| `ChatViewModel.toggleDisableUserPreferenceDescription` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 656 |
| `ChatViewModel.createNewChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | characterCardName: String??<br>characterGroupId: String?? | Unit | 聊天历史相关方法 | 661 |
| `ChatViewModel.createNewChatWithDraft` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | draft: String | Unit |  | 665 |
| `ChatViewModel.switchChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String | Unit |  | 685 |
| `ChatViewModel.loadOlderMessagesForCurrentChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 711 |
| `ChatViewModel.loadNewerMessagesForCurrentChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 717 |
| `ChatViewModel.showLatestMessagesForCurrentChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 723 |
| `ChatViewModel.loadChatMessageLocatorPreviews` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>query: String? | List<ChatMessageLocatorPreview> |  | 729 |
| `ChatViewModel.revealMessageForCurrentChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | targetTimestamp: Long | Boolean |  | 735 |
| `ChatViewModel.deleteChatHistory` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String | Unit |  | 738 |
| `ChatViewModel.clearCurrentChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 748 |
| `ChatViewModel.toggleChatHistorySelector` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 757 |
| `ChatViewModel.showChatHistorySelector` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | show: Boolean | Unit |  | 758 |
| `ChatViewModel.switchActiveCharacterTarget` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | target: CharacterSelectorTarget | Unit |  | 762 |
| `ChatViewModel.autoSwitchCharacterTargetForChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String | Unit |  | 779 |
| `ChatViewModel.autoSwitchChatForCharacterTarget` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | target: CharacterSelectorTarget | Unit |  | 791 |
| `ChatViewModel.findLatestChatForCharacterCard` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | targetCard: com.ai.assistance.operit.data.model… | ChatHistory? |  | 824 |
| `ChatViewModel.createBranch` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | upToMessageTimestamp: Long?? | Unit | 创建对话分支 | 844 |
| `ChatViewModel.insertSummary` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | message: ChatMessage | Unit | 插入总结 | 850 |
| `ChatViewModel.performInsertSummary` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | message: ChatMessage | Unit |  | 854 |
| `ChatViewModel.deleteMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | index: Int | Unit | 删除单条消息 | 952 |
| `ChatViewModel.deleteMessagesFrom` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | index: Int | Unit | 从指定索引删除后续所有消息 | 965 |
| `ChatViewModel.deleteMessages` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | indices: Set<Int> | Unit | 批量删除消息 | 973 |
| `ChatViewModel.setMessageFavorite` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | timestamp: Long<br>isFavorite: Boolean | Unit |  | 1000 |
| `ChatViewModel.shareMessages` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | context: Context<br>messageIndices: Set<Int><br>userMessageColor: Color<br>aiMessageColor: Color<br>userTextColor: Color<br>aiTextColor: Color<br>systemMessageColor: Color<br>systemTextColor: Color<br>thinkingBackgroundColor: Color<br>thin… | Unit | 分享消息为图片 | 1005 |
| `ChatViewModel.saveCurrentChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 1096 |
| `ChatViewModel.updateMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | index: Int<br>editedMessage: ChatMessage | Unit | 添加消息编辑方法 | 1105 |
| `ChatViewModel.regenerateSingleAiMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | index: Int | Unit |  | 1128 |
| `ChatViewModel.switchMessageVariant` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | index: Int<br>targetVariantIndex: Int | Unit |  | 1143 |
| `ChatViewModel.deleteCurrentMessageVariant` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | index: Int | Unit |  | 1167 |
| `ChatViewModel.rewindAndResendMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | index: Int<br>editedContent: String | Unit | 回档到指定消息并重新发送 | 1205 |
| `ChatViewModel.previewWorkspaceChangesForMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | index: Int | List<WorkspaceBackupManager.WorkspaceFileChange> |  | 1277 |
| `ChatViewModel.rollbackToMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | index: Int | Unit |  | 1310 |
| `ChatViewModel.updateUserMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | value: TextFieldValue | Unit | 消息处理相关方法 | 1364 |
| `ChatViewModel.insertRoleMention` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | roleName: String | Unit |  | 1381 |
| `ChatViewModel.replaceCurrentMentionToken` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | token: String | Unit |  | 1408 |
| `ChatViewModel.selectMentionPackage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | packageName: String | Unit |  | 1432 |
| `ChatViewModel.selectMentionWorkspaceEntry` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | relativePath: String | Unit |  | 1441 |
| `ChatViewModel.sendUserMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | promptFunctionType: PromptFunctionType? | Unit |  | 1461 |
| `ChatViewModel.sendTextMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | text: String<br>promptFunctionType: PromptFunctionType? | Unit |  | 1469 |
| `ChatViewModel.sendTextMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | text: String<br>chatId: String<br>promptFunctionType: PromptFunctionType? | Unit |  | 1478 |
| `ChatViewModel.enqueuePendingQueueMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>text: String<br>isQueueBlocked: Boolean | Unit |  | 1491 |
| `ChatViewModel.removePendingQueueMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>messageId: Long | PendingQueueMessageItem? |  | 1495 |
| `ChatViewModel.restorePendingQueueMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>message: PendingQueueMessageItem | Unit |  | 1498 |
| `ChatViewModel.setPendingQueueExpanded` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>expanded: Boolean | Unit |  | 1502 |
| `ChatViewModel.consumePendingQueueAutoDequeueSignal` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>isQueueBlocked: Boolean | Boolean |  | 1506 |
| `ChatViewModel.suppressNextPendingQueueAutoDequeue` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String | Unit |  | 1509 |
| `ChatViewModel.removeLastVisibleUserMessageFromCurrentChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | text: String | Boolean |  | 1513 |
| `ChatViewModel.addVisibleUserMessageToCurrentChat` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | text: String | Unit |  | 1531 |
| `ChatViewModel.normalizeMentionDeletion` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | previous: TextFieldValue<br>proposed: TextFieldValue | MentionDeletionNormalization |  | 1567 |
| `ChatViewModel.attachMentionPackage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | packageName: String | Unit |  | 1598 |
| `ChatViewModel.attachMentionWorkspaceEntry` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | workspacePath: String<br>relativePath: String<br>workspaceEnv: String? | Unit |  | 1612 |
| `ChatViewModel.containsMentionToken` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | text: String<br>token: String | Boolean |  | 1634 |
| `ChatViewModel.cancelCurrentMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 1643 |
| `ChatViewModel.cancelMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String | Unit |  | 1650 |
| `ChatViewModel.showErrorMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | message: String | Unit | UI状态相关方法 | 1658 |
| `ChatViewModel.clearError` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 1659 |
| `ChatViewModel.dismissErrorDialog` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 1660 |
| `ChatViewModel.popupMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | message: String | Unit |  | 1668 |
| `ChatViewModel.clearPopupMessage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 1669 |
| `ChatViewModel.showToast` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | message: String | Unit |  | 1670 |
| `ChatViewModel.clearToastEvent` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | eventId: Long | Unit |  | 1671 |
| `ChatViewModel.onFloatingButtonClick` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | mode: FloatingMode<br>permissionLauncher: ActivityResultLauncher<String><br>colorScheme: ColorScheme<br>typography: Typography<br>moveTaskToBackOnReady: Boolean? | Unit | 悬浮窗相关方法 | 1674 |
| `ChatViewModel.toggleFloatingMode` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | colorScheme: ColorScheme??<br>typography: Typography?? | Unit |  | 1717 |
| `ChatViewModel.setMasterPermissionLevel` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | level: PermissionLevel | Unit |  | 1721 |
| `ChatViewModel.handleAttachment` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | filePath: String | Unit | Handles a file or image attachment selected by the user | 1729 |
| `ChatViewModel.attachPastedText` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | text: String | Boolean |  | 1759 |
| `ChatViewModel.removeAttachment` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | filePath: String | Unit | Removes an attachment by its file path | 1776 |
| `ChatViewModel.insertAttachmentReference` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | attachment: AttachmentInfo | Unit | Inserts a reference to an attachment at the current cursor position in the user's message | 1781 |
| `ChatViewModel.hideMentionSuggestionPanel` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 隐藏 @ mention 建议面板 | 1795 |
| `ChatViewModel.captureScreenContent` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | Captures the current screen content and attaches it to the message | 1800 |
| `ChatViewModel.captureNotifications` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 获取设备当前通知数据并添加为附件 | 1831 |
| `ChatViewModel.captureLocation` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 获取设备当前位置数据并添加为附件 | 1862 |
| `ChatViewModel.captureMemoryFolders` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | folderPaths: List<String> | Unit | 捕获记忆文件夹作为附件 | 1895 |
| `ChatViewModel.handleTakenPhoto` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | uri: Uri | Unit | Handles a photo taken by the camera | 1924 |
| `ChatViewModel.attachPackage` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | packageName: String | Unit | Attaches a package's prompt content to the current message as an attachment | 1931 |
| `ChatViewModel.updateMentionSuggestionState` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | value: TextFieldValue | Unit |  | 1942 |
| `ChatViewModel.clearMentionSuggestionState` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 1954 |
| `ChatViewModel.findActiveMentionTrigger` | `ChatViewModel` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | value: TextFieldValue | ActiveMentionTrigger? |  | 1960 |
| `awaitCurrentChat` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>maxWaitCount: Int? | Boolean |  | 1996 |
| `resolveTargetChatIdForSharedContent` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | targetChatId: String? | String? |  | 2005 |
| `handleSharedText` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | text: String<br>targetChatId: String?? | Unit | Handles shared files from external apps Attaches files to the selected chat or a newly cr… | 2053 |
| `handleSharedFiles` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | uris: List<Uri><br>targetChatId: String??<br>sharedText: String?? | Unit |  | 2080 |
| `ensureAiServiceAvailable` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 确保AI服务可用，如果当前实例为空则创建一个默认实例 | 2146 |
| `resetAttachmentPanelState` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 重置附件面板状态 - 在发送消息后关闭附件面板 | 2178 |
| `updateAttachmentPanelState` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | isExpanded: Boolean | Unit | 更新附件面板状态 | 2183 |
| `toggleWebView` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | WebView控制方法 | 2188 |
| `awaitWorkspaceChatId` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | String? |  | 2235 |
| `isWorkspaceServerEnabled` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | workspacePath: String<br>workspaceEnv: String? | Boolean |  | 2249 |
| `prepareWorkspaceServer` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | workspacePath: String<br>workspaceEnv: String? | Boolean |  | 2256 |
| `prepareWorkspaceServerForCurrentChat` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String | Unit |  | 2276 |
| `updateWebServerForCurrentChat` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String | Unit | 更新当前聊天ID的Web服务器工作空间 | 2295 |
| `refreshWebView` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 强制WebView刷新 | 2309 |
| `notifyWorkspacePreviewRefresh` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | workspacePath: String<br>workspaceEnv: String?<br>affectedPaths: List<String><br>source: String | Unit |  | 2313 |
| `resolveWorkspaceEnvForPath` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | workspacePath: String | String? |  | 2329 |
| `startFileChooserForResult` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | intent: Intent<br>callback: (Int, Intent?) -> Unit | Unit | 用于启动文件选择器并处理结果 | 2342 |
| `handleFileChooserResult` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | resultCode: Int<br>data: Intent? | Unit | 供Activity调用，处理文件选择结果 | 2349 |
| `setPermissionSystemColorScheme` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | colorScheme: ColorScheme? | Unit | 设置权限系统的颜色方案 | 2355 |
| `launchFloatingModeIn` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | mode: FloatingMode<br>colorScheme: ColorScheme??<br>typography: Typography??<br>moveTaskToBackOnReady: Boolean? | Unit |  | 2359 |
| `launchFloatingWindowInMode` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | mode: FloatingMode | Unit | 从Widget启动悬浮窗到指定模式（使用默认主题） | 2371 |
| `launchWindowFloatingModeAfterMicPermissionGranted` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | colorScheme: ColorScheme??<br>typography: Typography??<br>moveTaskToBackOnReady: Boolean? | Unit |  | 2375 |
| `launchFloatingWindowWithPermissionCheck` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | launcher: ActivityResultLauncher<String><br>onPermissionGranted: () -> Unit | Unit |  | 2393 |
| `launchFullscreenVoiceModeWithPermissionCheck` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | launcher: ActivityResultLauncher<String><br>colorScheme: ColorScheme??<br>typography: Typography?? | Unit |  | 2411 |
| `openOverlayPermissionSettings` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 2431 |
| `onCleared` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 2442 |
| `updateChatTitle` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>newTitle: String | Unit | 更新指定聊天的标题 | 2463 |
| `updateChatCharacterCardBinding` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>characterCardName: String? | Unit | 更新指定聊天绑定的角色卡 | 2468 |
| `updateChatCharacterGroupBinding` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>characterGroupId: String? | Unit | 更新指定聊天绑定的群组角色卡 | 2473 |
| `updateChatCharacterBinding` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>characterCardName: String?<br>characterGroupId: String? | Unit | 同时更新指定聊天绑定的角色卡与群组 | 2478 |
| `bindChatToWorkspace` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>workspace: String<br>workspaceEnv: String?? | Unit | 更新指定聊天的标题 | 2487 |
| `unbindChatFromWorkspace` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String | Unit | 解绑聊天的工作区 | 2512 |
| `renameWorkspace` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | chatId: String<br>newWorkspaceName: String | WorkspaceRenameResult |  | 2538 |
| `executeCommandInWorkspace` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | command: CommandConfig<br>workspacePath: String | Unit | 在工作区中执行命令（来自 config.json 按钮） | 2567 |
| `executeBackgroundWorkspaceCommand` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | command: CommandConfig<br>workspacePath: String<br>commandText: String | Unit |  | 2691 |
| `openAiComputerForTerminalSession` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 2725 |
| `dismissWorkspaceCommandExecutionDialog` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | workspacePath: String | Unit |  | 2733 |
| `cancelWorkspaceCommandExecution` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 2747 |
| `executeWorkspaceTool` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | command: CommandConfig<br>workspacePath: String<br>toolName: String | Unit |  | 2773 |
| `resolveWorkspaceToolParameterValue` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | name: String<br>rawValue: String<br>workspaceDir: File | String |  | 2821 |
| `isPathLikeToolParameter` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | name: String | Boolean |  | 2844 |
| `updateChatOrderAndGroup` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | reorderedHistories: List<ChatHistory><br>movedItem: ChatHistory<br>targetGroup: String? | Unit | 更新聊天顺序和分组 | 2850 |
| `createGroup` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | groupName: String<br>characterCardName: String?<br>characterGroupId: String?? | Unit | 创建新分组（通过创建新聊天实现） | 2859 |
| `updateGroupName` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | oldName: String<br>newName: String<br>characterCardName: String? | Unit | 重命名分组 | 2864 |
| `deleteGroup` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | groupName: String<br>deleteChats: Boolean<br>characterCardName: String? | Unit | 删除分组 | 2869 |
| `onWorkspaceButtonClick` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 2873 |
| `onAiComputerButtonClick` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 2877 |
| `toggleAiComputer` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | AI电脑控制方法 | 2882 |
| `initializeVoiceService` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 初始化语音服务 | 2913 |
| `recreateVoiceService` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Boolean |  | 2933 |
| `ensureActiveVoiceService` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | VoiceService? |  | 2950 |
| `cancelSpeechControlsHide` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | reason: String | Unit |  | 2975 |
| `observeVoiceState` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | service: VoiceService | Unit |  | 2983 |
| `speakMessage` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | message: String | Unit | 朗读消息内容 | 3016 |
| `speakMessage` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | message: String<br>interrupt: Boolean | Unit |  | 3020 |
| `stopSpeaking` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 停止朗读 | 3101 |
| `pauseSpeaking` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 3119 |
| `resumeSpeaking` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 3143 |
| `toggleAutoRead` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 3163 |
| `disableAutoRead` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 3178 |
| `enableAutoReadAndSpeak` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | content: String | Unit |  | 3186 |
| `setReplyToMessage` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | message: ChatMessage | Unit | 设置回复目标消息 | 3195 |
| `clearReplyToMessage` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit | 清除回复状态 | 3200 |
| `manuallyUpdateMemory` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 3204 |
| `enqueueSelectedMessagesForMemoryAutoSave` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | messages: List<ChatMessage> | Unit |  | 3208 |
| `manuallySummarizeConversation` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` |  | Unit |  | 3212 |
| `FloatingWindowDelegate.onReceive` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` | context: Context?<br>intent: Intent? | Unit |  | 53 |
| `FloatingWindowDelegate.onServiceConnected` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` | name: ComponentName?<br>service: IBinder? | Unit |  | 78 |
| `FloatingWindowDelegate.onServiceDisconnected` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` | name: ComponentName? | Unit |  | 88 |
| `FloatingWindowDelegate.onNullBinding` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` | name: ComponentName? | Unit |  | 98 |
| `FloatingWindowDelegate.tryBindToRunningService` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` |  | Unit |  | 126 |
| `FloatingWindowDelegate.clearFloatingCrashDisableFlag` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` |  | Unit | 用户在主界面显式进入悬浮窗，视为对崩溃停用保护的重新授权： 清除停用标记与持久化崩溃计数，让服务可以再次启动。 若同一崩溃仍在，服务会再次连崩 4 次后重新停用，形成闭环。 | 147 |
| `FloatingWindowDelegate.toggleFloatingMode` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` | colorScheme: ColorScheme??<br>typography: Typography?? | Unit | 切换悬浮窗模式 | 162 |
| `FloatingWindowDelegate.launchInMode` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` | mode: FloatingMode<br>colorScheme: ColorScheme??<br>typography: Typography??<br>moveTaskToBackOnReady: Boolean? | Unit | 启动悬浮窗并指定一个初始模式 | 195 |
| `FloatingWindowDelegate.closeFloatingWindow` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` |  | Unit | 由服务回调或用户操作调用，用于关闭悬浮窗并更新状态 | 238 |
| `FloatingWindowDelegate.disconnectFromService` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` | updateFloatingMode: Boolean | Unit |  | 242 |
| `FloatingWindowDelegate.setupInputStateCollection` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` |  | Unit |  | 262 |
| `FloatingWindowDelegate.cleanup` | `FloatingWindowDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `FloatingWindowDelegate.kt` |  | Unit | 清理资源 | 274 |
| `PendingMessageQueueStore.enqueue` | `PendingMessageQueueStore` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | chatId: String<br>text: String<br>isQueueBlocked: Boolean | Unit |  | 23 |
| `PendingMessageQueueStore.remove` | `PendingMessageQueueStore` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | chatId: String<br>messageId: Long | PendingQueueMessageItem? |  | 35 |
| `PendingMessageQueueStore.restore` | `PendingMessageQueueStore` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | chatId: String<br>message: PendingQueueMessageItem | Unit |  | 47 |
| `PendingMessageQueueStore.setExpanded` | `PendingMessageQueueStore` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | chatId: String<br>expanded: Boolean | Unit |  | 59 |
| `PendingMessageQueueStore.suppressNextAutoDequeue` | `PendingMessageQueueStore` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | chatId: String | Unit |  | 65 |
| `PendingMessageQueueStore.consumeAutoDequeueSignal` | `PendingMessageQueueStore` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | chatId: String<br>isQueueBlocked: Boolean | Boolean |  | 71 |
| `PendingMessageQueueStore.removeChat` | `PendingMessageQueueStore` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | chatId: String | Unit |  | 89 |
| `PendingMessageQueueStore.updateState` | `PendingMessageQueueStore` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStore.kt` | chatId: String<br>transform: (PendingMessageQueueState) -> Pendi… | Unit |  | 97 |
| `UiStateDelegate.showErrorMessage` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` | message: String | Unit | 显示错误消息 | 39 |
| `UiStateDelegate.clearError` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` |  | Unit | 清除错误消息 | 44 |
| `UiStateDelegate.showPopupMessage` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` | message: String | Unit | 显示弹出消息 | 49 |
| `UiStateDelegate.clearPopupMessage` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` |  | Unit | 清除弹出消息 | 54 |
| `UiStateDelegate.showToast` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` | message: String | Unit | 显示Toast消息 | 59 |
| `UiStateDelegate.clearToastEvent` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` | eventId: Long | Unit | 清除Toast消息 | 72 |
| `UiStateDelegate.updateMasterPermissionLevel` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` | level: PermissionLevel | Unit | 更新主权限级别 | 82 |
| `UiStateDelegate.requestFileChooser` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` | intent: Intent | Unit | 请求文件选择器 | 87 |
| `UiStateDelegate.clearFileChooserRequest` | `UiStateDelegate` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `UiStateDelegate.kt` |  | Unit | 清除文件选择器请求 | 92 |
| `PendingMessageQueueStoreTest.queueRemainsAvailableWhenAnotherChatIsVisited` | `PendingMessageQueueStoreTest` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStoreTest.kt` |  | Unit |  | 10 ⚑ |
| `PendingMessageQueueStoreTest.cancellingCurrentTurnConsumesOnlyTheNextAutoDequeue` | `PendingMessageQueueStoreTest` | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `PendingMessageQueueStoreTest.kt` |  | Unit |  | 21 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `query` | — | `com.ai.assistance.operit.ui.features.chat.viewmodel` | `ChatViewModel.kt` | inferred |  | 1982 |
