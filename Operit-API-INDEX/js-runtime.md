# ToolPkg JS 运行时 API

数据源：`runtime/toolpkgapi/1.2.0/bootstrap/`（由上游 Kotlin 原始字符串提取，与真机同源）。

这是插件在 QuickJS 里**真正能调用**的那一层。Kotlin 侧的 15000 个函数插件碰不到，能碰到的就是下面这些。

| 全局 | 说明 |
| --- | --- |
| `Tools` | 内建工具的门面，每个方法最终转成 `toolCall("<工具名>", params)` |
| `ToolPkg` | 注册桶：工具、Hook、AI Provider |

---

## `Tools` — 内建工具门面

每个方法都是一层薄封装：组装参数后调用 `toolCall(工具名)`。**左列是你写的，右列是真正执行的工具**。

### `Tools.FFmpeg`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `execute(command)` | `command` | `ffmpeg_execute` |  |
| `info()` | — | `ffmpeg_info` |  |
| `convert(inputPath, outputPath, options = {})` | `inputPath` `outputPath` `options = {}` | `ffmpeg_convert` |  |

### `Tools.Files`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `list(path, environment)` | `path` `environment` | `list_files` |  |
| `read(pathOrOptions)` | `pathOrOptions` | `read_file_full` |  |
| `readBinary(path, environment)` | `path` `environment` | `read_file_binary` |  |
| `readPart(path, startLine, endLine, environment)` | `path` `startLine` `endLine` `environment` | `read_file_part` |  |
| `write(path, content, append, environment)` | `path` `content` `append` `environment` | `write_file` |  |
| `writeBinary(path, base64Content, environment)` | `path` `base64Content` `environment` | `write_file_binary` |  |
| `deleteFile(path, recursive, environment)` | `path` `recursive` `environment` | `delete_file` |  |
| `exists(path, environment)` | `path` `environment` | `file_exists` |  |
| `move(source, destination, environment)` | `source` `destination` `environment` | `move_file` |  |
| `copy(source, destination, recursive, sourceEnvironment, destEnvironment)` | `source` `destination` `recursive` `sourceEnvironment` `destEnvironment` | `copy_file` |  |
| `mkdir(path, create_parents, environment)` | `path` `create_parents` `environment` | `make_directory` |  |
| `find(path, pattern, options = {}, environment)` | `path` `pattern` `options = {}` `environment` | `find_files` |  |
| `grep(path, pattern, options = {})` | `path` `pattern` `options = {}` | `grep_code` |  |
| `grepContext(path, intent, options = {})` | `path` `intent` `options = {}` | `grep_context` |  |
| `info(path, environment)` | `path` `environment` | `file_info` |  |
| `apply(path, type, oldContent, newContent, environment)` | `path` `type` `oldContent` `newContent` `environment` | `apply_file` |  |
| `create(path, newContent, environment)` | `path` `newContent` `environment` | `create_file` |  |
| `edit(path, oldContent, newContent, environment)` | `path` `oldContent` `newContent` `environment` | `edit_file` |  |
| `zip(source, destination, environment, include_root_directory)` | `source` `destination` `environment` `include_root_directory` | `zip_files` |  |
| `unzip(source, destination, environment)` | `source` `destination` `environment` | `unzip_files` |  |
| `open(path, environment)` | `path` `environment` | `open_file` |  |
| `share(path, title, environment)` | `path` `title` `environment` | `share_file` |  |
| `download(urlOrOptions, destination, environment, headers)` | `urlOrOptions` `destination` `environment` `headers` | `download_file` |  |

### `Tools.Memory`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `_normalizeCallerCardId(callerCardId)` | `callerCardId` | — |  |
| `query(query, folderPath, limit, startTime, endTime, snapshotId, threshold, callerCardId)` | `query` `folderPath` `limit` `startTime` `endTime` `snapshotId` `threshold` `callerCardId` | `query_memory` |  |
| `getByTitle(title, chunkIndex, chunkRange, query, limit, callerCardId)` | `title` `chunkIndex` `chunkRange` `query` `limit` `callerCardId` | `get_memory_by_title` |  |
| `create(title, content, contentType, source, folderPath, tags, callerCardId)` | `title` `content` `contentType` `source` `folderPath` `tags` `callerCardId` | `create_memory` |  |
| `update(oldTitle, updates = {}, callerCardId)` | `oldTitle` `updates = {}` `callerCardId` | `update_memory` |  |
| `deleteMemory(title, callerCardId)` | `title` `callerCardId` | `delete_memory` |  |
| `move(targetFolderPath, titles, sourceFolderPath, callerCardId)` | `targetFolderPath` `titles` `sourceFolderPath` `callerCardId` | `move_memory` |  |
| `link(sourceTitle, targetTitle, linkType, weight, description, callerCardId)` | `sourceTitle` `targetTitle` `linkType` `weight` `description` `callerCardId` | `link_memories` |  |
| `queryLinks(linkId, sourceTitle, targetTitle, linkType, limit, callerCardId)` | `linkId` `sourceTitle` `targetTitle` `linkType` `limit` `callerCardId` | `query_memory_links` |  |
| `updateLink(linkId, sourceTitle, targetTitle, linkType, newLinkType, weight, description, callerCardId)` | `linkId` `sourceTitle` `targetTitle` `linkType` `newLinkType` `weight` `description` `callerCardId` | `update_memory_link` |  |
| `deleteLink(linkId, sourceTitle, targetTitle, linkType, callerCardId)` | `linkId` `sourceTitle` `targetTitle` `linkType` `callerCardId` | `delete_memory_link` |  |

### `Tools.Net`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `httpGet(url, ignoreSsl)` | `url` `ignoreSsl` | `http_request` |  |
| `httpPost(url, body, ignoreSsl)` | `url` `body` `ignoreSsl` | `http_request` |  |
| `visit(params)` | `params` | `visit_web` |  |
| `browserNavigate(urlOrOptions)` | `urlOrOptions` | `browser_navigate` |  |
| `browserNavigateBack(options)` | `options` | `browser_navigate_back` |  |
| `browserClick(options)` | `options` | `browser_click` |  |
| `browserClose(options)` | `options` | `browser_close` |  |
| `browserCloseAll(options)` | `options` | `browser_close_all` |  |
| `browserConsoleMessages(options)` | `options` | `browser_console_messages` |  |
| `browserDrag(options)` | `options` | `browser_drag` |  |
| `browserEvaluate(options)` | `options` | `browser_evaluate` |  |
| `browserFileUpload(options)` | `options` | `browser_file_upload` |  |
| `browserFillForm(options)` | `options` | `browser_fill_form` |  |
| `browserHandleDialog(options)` | `options` | `browser_handle_dialog` |  |
| `browserHover(options)` | `options` | `browser_hover` |  |
| `browserNetworkRequests(options)` | `options` | `browser_network_requests` |  |
| `browserPressKey(keyOrOptions)` | `keyOrOptions` | `browser_press_key` |  |
| `browserResize(options)` | `options` | `browser_resize` |  |
| `browserRunCode(options)` | `options` | `browser_run_code` |  |
| `browserSelectOption(options)` | `options` | `browser_select_option` |  |
| `browserSnapshot(options)` | `options` | `browser_snapshot` |  |
| `browserTabs(options)` | `options` | `browser_tabs` |  |
| `browserTakeScreenshot(options)` | `options` | `browser_take_screenshot` |  |
| `browserType(options)` | `options` | `browser_type` |  |
| `browserWaitFor(options)` | `options` | `browser_wait_for` |  |
| `http(options)` | `options` | `http_request` |  |
| `uploadFile(options)` | `options` | `multipart_request` |  |

### `Tools.Net.cookies`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `get(domain)` | `domain` | `manage_cookies` |  |
| `set(domain, cookies)` | `domain` `cookies` | `manage_cookies` |  |
| `clear(domain)` | `domain` | `manage_cookies` |  |

### `Tools.SoftwareSettings`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `readEnvironmentVariable(key)` | `key` | `read_environment_variable` |  |
| `writeEnvironmentVariable(key, value)` | `key` `value` | `write_environment_variable` |  |
| `listSandboxPackages()` | — | `list_sandbox_packages` |  |
| `setSandboxPackageEnabled(packageName, enabled)` | `packageName` `enabled` | `set_sandbox_package_enabled` |  |
| `executeSandboxScriptDirect(options = {})` | `options = {}` | `execute_sandbox_script_direct` |  |
| `restartMcpWithLogs(timeoutMs)` | `timeoutMs` | `restart_mcp_with_logs` |  |
| `getSpeechServicesConfig()` | — | `get_speech_services_config` |  |
| `setSpeechServicesConfig(updates = {})` | `updates = {}` | `set_speech_services_config` |  |
| `testTtsPlayback(text, options = {})` | `text` `options = {}` | `test_tts_playback` |  |
| `listModelConfigs()` | — | `list_model_configs` |  |
| `createModelConfig(options = {})` | `options = {}` | `create_model_config` |  |
| `updateModelConfig(configId, updates = {})` | `configId` `updates = {}` | `update_model_config` |  |
| `deleteModelConfig(configId)` | `configId` | `delete_model_config` |  |
| `listFunctionModelConfigs()` | — | `list_function_model_configs` |  |
| `getFunctionModelConfig(functionType)` | `functionType` | `get_function_model_config` |  |
| `setFunctionModelConfig(functionType, configId, modelIndex)` | `functionType` `configId` `modelIndex` | `set_function_model_config` |  |
| `testModelConfigConnection(configId, modelIndex)` | `configId` `modelIndex` | `test_model_config_connection` |  |
| `listCharacterCards()` | — | `list_character_cards_settings` |  |
| `getCharacterCard(characterCardId)` | `characterCardId` | `get_character_card` |  |
| `createCharacterCard(options = {})` | `options = {}` | `create_character_card` |  |
| `updateCharacterCard(characterCardId, updates = {})` | `characterCardId` `updates = {}` | `update_character_card` |  |
| `deleteCharacterCard(characterCardId)` | `characterCardId` | `delete_character_card` |  |
| `setActiveCharacterCard(characterCardId)` | `characterCardId` | `set_active_character_card` |  |
| `clearActiveCharacterCard()` | — | `clear_active_character_card` |  |
| `importCharacterCardFromTavernJson(tavernJson)` | `tavernJson` | `import_character_card_from_tavern_json` |  |
| `exportCharacterCardToTavernJson(characterCardId)` | `characterCardId` | `export_character_card_to_tavern_json` |  |

### `Tools.System`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `sleep(milliseconds)` | `milliseconds` | `sleep` |  |
| `getSetting(setting, namespace)` | `setting` `namespace` | `get_system_setting` |  |
| `setSetting(setting, value, namespace)` | `setting` `value` `namespace` | `modify_system_setting` |  |
| `getDeviceInfo()` | — | `device_info` |  |
| `toast(message)` | `message` | `toast` |  |
| `sendNotification(message, title)` | `message` `title` | `send_notification` |  |
| `usePackage(packageName)` | `packageName` | `use_package` |  |
| `installApp(path)` | `path` | `install_app` |  |
| `uninstallApp(packageName)` | `packageName` | `uninstall_app` |  |
| `startApp(packageName, activity)` | `packageName` `activity` | `start_app` |  |
| `stopApp(packageName)` | `packageName` | `stop_app` |  |
| `listApps(includeSystem)` | `includeSystem` | `list_installed_apps` |  |
| `getNotifications(limit = 10, includeOngoing = false)` | `limit = 10` `includeOngoing = false` | `get_notifications` |  |
| `getAppUsageTime(options = {})` | `options = {}` | `get_app_usage_time` |  |
| `getLocation(highAccuracy = false, timeout = 10, includeAddress = true)` | `highAccuracy = false` `timeout = 10` `includeAddress = true` | `get_device_location` |  |
| `shell(command)` | `command` | `execute_shell` |  |
| `intent(options = {})` | `options = {}` | `execute_intent` |  |
| `sendBroadcast(options = {})` | `options = {}` | `send_broadcast` |  |

### `Tools.System.bluetooth`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `requestPermission()` | — | `request_bluetooth_permission` |  |
| `getState()` | — | `get_bluetooth_state` |  |
| `requestEnable()` | — | `request_enable_bluetooth` |  |
| `listBondedDevices()` | — | `list_bluetooth_bonded_devices` |  |
| `scan(options = {})` | `options = {}` | `scan_bluetooth_devices` |  |
| `connect(options)` | `options` | `bluetooth_connect` |  |
| `listen(options = {})` | `options = {}` | `bluetooth_listen` |  |
| `accept(listenerSessionId, timeoutMs)` | `listenerSessionId` `timeoutMs` | `bluetooth_accept` |  |
| `send(sessionId, options)` | `sessionId` `options` | `bluetooth_send` |  |
| `read(sessionId, options = {})` | `sessionId` `options = {}` | `bluetooth_read` |  |
| `sendAndRead(sessionId, options)` | `sessionId` `options` | `bluetooth_send_and_read` |  |
| `close(sessionId)` | `sessionId` | `bluetooth_close` |  |

### `Tools.System.bluetooth.ble`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `connect(options)` | `options` | `bluetooth_ble_connect` |  |
| `discoverServices(sessionId, timeoutMs)` | `sessionId` `timeoutMs` | `bluetooth_ble_discover_services` |  |
| `readCharacteristic(sessionId, options)` | `sessionId` `options` | `bluetooth_ble_read_characteristic` |  |
| `writeCharacteristic(sessionId, options)` | `sessionId` `options` | `bluetooth_ble_write_characteristic` |  |
| `writeAndReadCharacteristic(sessionId, options)` | `sessionId` `options` | `bluetooth_ble_write_and_read_characteristic` |  |
| `subscribe(sessionId, options)` | `sessionId` `options` | `bluetooth_ble_subscribe_characteristic` |  |
| `readNotifications(sessionId, limit)` | `sessionId` `limit` | `bluetooth_ble_read_notifications` |  |

### `Tools.System.music`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `play(options)` | `options` | `music_play` |  |
| `playQueue(options)` | `options` | `music_play_queue` |  |
| `pause()` | — | `music_pause` |  |
| `resume()` | — | `music_resume` |  |
| `stop()` | — | `music_stop` |  |
| `seek(positionMs)` | `positionMs` | `music_seek` |  |
| `setVolume(volume)` | `volume` | `music_set_volume` |  |
| `status()` | — | `music_status` |  |

### `Tools.System.terminal`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `create(sessionName)` | `sessionName` | `create_terminal_session` |  |
| `exec(sessionId, command, timeoutMs)` | `sessionId` `command` `timeoutMs` | `execute_in_terminal_session` |  |
| `execStreaming(sessionId, command, options = {})` | `sessionId` `command` `options = {}` | `execute_in_terminal_session_streaming` |  |
| `hiddenExec(command, options = {})` | `command` `options = {}` | `execute_hidden_terminal_command` |  |
| `screen(sessionId)` | `sessionId` | `get_terminal_session_screen` |  |
| `close(sessionId)` | `sessionId` | `close_terminal_session` |  |
| `input(sessionId, options = {})` | `sessionId` `options = {}` | `input_in_terminal_session` |  |

### `Tools.Tasker`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `triggerEvent(params)` | `params` | `trigger_tasker_event` |  |

### `Tools.UI`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `getPageInfo()` | — | `get_page_info` |  |
| `captureScreenshot()` | — | `capture_screenshot` |  |
| `tap(x, y)` | `x` `y` | `tap` |  |
| `longPress(x, y)` | `x` `y` | `long_press` |  |
| `clickElement(param1, param2, param3)` | `param1` `param2` `param3` | `click_element` |  |
| `setText(text, resourceId)` | `text` `resourceId` | `set_input_text` |  |
| `swipe(startX, startY, endX, endY, duration)` | `startX` `startY` `endX` `endY` `duration` | `swipe` |  |
| `pressKey(keyCode)` | `keyCode` | `press_key` |  |
| `runSubAgent(intent, maxSteps, agentId, targetApp)` | `intent` `maxSteps` `agentId` `targetApp` | `run_ui_subagent` |  |

### `Tools.Workflow`

| 调用 | 参数 | → 工具 | 说明 |
| --- | --- | --- | --- |
| `getAll()` | — | `get_all_workflows` |  |
| `create(name, description = "", nodes = null, connections = null, enabled = true)` | `name` `description = ""` `nodes = null` `connections = null` `enabled = true` | `create_workflow` |  |
| `get(workflowId)` | `workflowId` | `get_workflow` |  |
| `update(workflowId, updates = {})` | `workflowId` `updates = {}` | `update_workflow` |  |
| `patch(workflowId, patch = {})` | `workflowId` `patch = {}` | `patch_workflow` |  |
| `setEnabled(workflowId, enabled)` | `workflowId` `enabled` | — |  |
| `enable(workflowId)` | `workflowId` | `enable_workflow` |  |
| `disable(workflowId)` | `workflowId` | `disable_workflow` |  |
| `trigger(workflowId)` | `workflowId` | `trigger_workflow` |  |
| `startService(options = {})` | `options = {}` | `start_chat_service` |  |
| `createNew(group, setAsCurrentChat, characterCardId)` | `group` `setAsCurrentChat` `characterCardId` | `create_new_chat` |  |
| `listAll()` | — | `list_chats` |  |
| `listChats(params = {})` | `params = {}` | `list_chats` |  |
| `findChat(params = {})` | `params = {}` | `find_chat` |  |
| `agentStatus(chatId)` | `chatId` | `agent_status` |  |
| `switchTo(chatId)` | `chatId` | `switch_chat` |  |
| `updateTitle(chatId, title)` | `chatId` `title` | `update_chat_title` |  |
| `deleteChat(chatId)` | `chatId` | `delete_chat` |  |
| `getMessages(chatId, options = {})` | `chatId` `options = {}` | `get_chat_messages` |  |
| `getMessagesRange(chatId, options = {})` | `chatId` `options = {}` | `get_chat_messages_range` |  |
| `sendMessage(message, chatId, roleCardId, senderName, options = {})` | `message` `chatId` `roleCardId` `senderName` `options = {}` | `send_message_to_ai` |  |
| `sendMessageStreaming(message, chatId, roleCardId, senderName, options = {})` | `message` `chatId` `roleCardId` `senderName` `options = {}` | `send_message_to_ai_streaming` |  |
| `listCharacterCards()` | — | `list_character_cards` |  |

## `ToolPkg` — 注册桶

注册即调用；返回值多数是 `boolean` 或无语义。`→ 宿主方法` 是它在 C++ 侧转发的 `NativeInterface` 方法名。

| API | 参数 | → 宿主方法 |
| --- | --- | --- |
| `ToolPkg.registerAiProvider` | `definition` | `registerToolPkgAiProvider` |
| `ToolPkg.registerAppLifecycleHook` | `...` | `registerToolPkgAppLifecycleHook` |
| `ToolPkg.registerChatInputHook` | `...` | `registerToolPkgChatInputHook` |
| `ToolPkg.registerChatMessageHook` | `...` | `registerToolPkgChatMessageHook` |
| `ToolPkg.registerChatViewHook` | `...` | `registerToolPkgChatViewHook` |
| `ToolPkg.registerInputMenuTogglePlugin` | `...` | `registerToolPkgInputMenuTogglePlugin` |
| `ToolPkg.registerMessageProcessingPlugin` | `...` | `registerToolPkgMessageProcessingPlugin` |
| `ToolPkg.registerPromptEstimateFinalizeHook` | `...` | `registerToolPkgPromptEstimateFinalizeHook` |
| `ToolPkg.registerPromptEstimateHistoryHook` | `...` | `registerToolPkgPromptEstimateHistoryHook` |
| `ToolPkg.registerPromptFinalizeHook` | `...` | `registerToolPkgPromptFinalizeHook` |
| `ToolPkg.registerPromptHistoryHook` | `...` | `registerToolPkgPromptHistoryHook` |
| `ToolPkg.registerPromptInputHook` | `...` | `registerToolPkgPromptInputHook` |
| `ToolPkg.registerSummaryGenerateHook` | `...` | `registerToolPkgSummaryGenerateHook` |
| `ToolPkg.registerSystemPromptComposeHook` | `...` | `registerToolPkgSystemPromptComposeHook` |
| `ToolPkg.registerToolLifecycleHook` | `...` | `registerToolPkgToolLifecycleHook` |
| `ToolPkg.registerToolPromptComposeHook` | `...` | `registerToolPkgToolPromptComposeHook` |
| `ToolPkg.registerXmlRenderPlugin` | `...` | `registerToolPkgXmlRenderPlugin` |

## 覆盖情况

`Tools` 门面共封装 **172** 个不同的底层工具。

上游工具目录共 162 个，其中 172 个有 `Tools` 便捷封装。

没有便捷封装、但可以 `toolCall("名字", {...})` 直接调的：

`update_user_profile` · `delete_workflow` · `stop_chat_service` · `close_all_virtual_displays` · `read_file`

---

## 与 CLI 实现的关系

`operitcli` 的工具执行器（`src/tools/`）实现的是**底层工具名**这一侧，也就是上表右列。
插件写 `Tools.Files.read(p)`，真机和 CLI 都会走到 `read_file_full`；差异只可能出在 `read_file_full` 的实现里。
