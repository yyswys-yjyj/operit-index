# operit.provider

> 函数 83 · 类型 7 · 顶层常量 3 · 共 93 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `DocRef` | `DocRef` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | class DocRef |  | 1178 |
| `DocRef.Memory` | `DocRef` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | class Memory(override val profileId: String, val uuid: String) : DocRef |  | 1194 |
| `DocRef.Profile` | `DocRef` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | class Profile(override val profileId: String) : DocRef |  | 1186 |
| `DocRef.Root` | `DocRef` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | object Root : DocRef |  | 1181 |
| `MemoryDocumentsProvider` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | class MemoryDocumentsProvider : DocumentsProvider |  | 29 |
| `OperitDataDocumentsProvider` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | class OperitDataDocumentsProvider : DocumentsProvider |  | 14 |
| `WorkspaceDocumentsProvider` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | class WorkspaceDocumentsProvider : DocumentsProvider | Workspace目录的DocumentsProvider 通过Storage Access Framework暴露内部存储的workspace目录 路径: /data/data… | 20 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `MemoryDocumentsProvider.requireProviderContext` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` |  | Context |  | 65 |
| `MemoryDocumentsProvider.attachInfo` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | context: Context?<br>info: ProviderInfo? | Unit |  | 69 |
| `MemoryDocumentsProvider.onCreate` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` |  | Boolean |  | 77 |
| `MemoryDocumentsProvider.moveDocument` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | sourceDocumentId: String<br>sourceParentDocumentId: String<br>targetParentDocumentId: String | String? |  | 91 |
| `MemoryDocumentsProvider.queryRoots` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | projection: Array<out String>? | Cursor |  | 220 |
| `MemoryDocumentsProvider.queryDocument` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | documentId: String<br>projection: Array<out String>? | Cursor |  | 241 |
| `MemoryDocumentsProvider.queryChildDocuments` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | parentDocumentId: String<br>projection: Array<out String>?<br>sortOrder: String? | Cursor |  | 248 |
| `MemoryDocumentsProvider.openDocument` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | documentId: String<br>mode: String<br>signal: CancellationSignal? | ParcelFileDescriptor |  | 329 |
| `MemoryDocumentsProvider.createDocument` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | parentDocumentId: String<br>mimeType: String<br>displayName: String | String? |  | 398 |
| `MemoryDocumentsProvider.deleteDocument` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | documentId: String | Unit |  | 467 |
| `MemoryDocumentsProvider.renameDocument` | `MemoryDocumentsProvider` | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | documentId: String<br>displayName: String | String? |  | 494 |
| `isChildDocument` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | parentDocumentId: String<br>documentId: String | Boolean |  | 565 |
| `includeDocument` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | result: MatrixCursor<br>documentId: String | Unit |  | 626 |
| `includeProfile` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | result: MatrixCursor<br>profile: MemorySpace | Unit |  | 700 |
| `includeDirectory` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | result: MatrixCursor<br>profileId: String<br>path: String<br>displayName: String | Unit |  | 714 |
| `includeMemoriesForFolder` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | result: MatrixCursor<br>profileId: String<br>memories: List<Memory><br>folderPath: String? | Unit |  | 729 |
| `getProfileDisplayName` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | profile: MemorySpace | String |  | 760 |
| `applyWrittenContentToMemory` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | repo: MemoryRepository<br>uuid: String<br>writtenText: String | Unit |  | 765 |
| `normalizeFolders` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | folderPaths: Collection<String> | List<String> |  | 809 |
| `buildMemoryDisplayName` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | title: String<br>uuid: String | String |  | 826 |
| `decodeRequestedTitle` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | memory: Memory<br>displayName: String | String |  | 831 |
| `buildMemoryJson` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | memory: com.ai.assistance.operit.data.model… | String |  | 841 |
| `parseDocumentId` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | documentId: String | DocRef |  | 859 |
| `parseDirectDocumentId` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | documentId: String | DocRef |  | 870 |
| `parseSyntheticTreeDocumentId` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | documentId: String | DocRef |  | 916 |
| `resolveSyntheticChild` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | parent: DocRef<br>displayName: String<br>originalDocumentId: String | DocRef |  | 929 |
| `resolveSyntheticChildInContainer` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | profileId: String<br>parentFolderPath: String?<br>displayName: String<br>repo: MemoryRepository<br>originalDocumentId: String | DocRef |  | 970 |
| `findDirectChildDirectoryPath` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | parentFolderPath: String?<br>childDisplayName: String<br>folderPaths: Collection<String> | String? |  | 998 |
| `childDisplayName` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | path: String | String |  | 1023 |
| `getRepository` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | profileId: String | MemoryRepository |  | 1027 |
| `documentExists` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | ref: DocRef | Boolean |  | 1034 |
| `profileExists` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | profileId: String | Boolean |  | 1049 |
| `requireProfileExists` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | profileId: String | Unit |  | 1054 |
| `loadAllMemories` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | repo: MemoryRepository | List<Memory> |  | 1060 |
| `loadRealFolderPaths` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | repo: MemoryRepository | Set<String> |  | 1066 |
| `loadDirectoryNodes` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | repo: MemoryRepository | Set<String> |  | 1070 |
| `directoryExists` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | repo: MemoryRepository<br>path: String | Boolean |  | 1074 |
| `requireDirectoryExists` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | repo: MemoryRepository<br>path: String | Unit |  | 1079 |
| `loadMemoriesInFolderTree` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | repo: MemoryRepository<br>folderPath: String | List<Memory> |  | 1085 |
| `collectRealFolderPaths` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | memories: List<Memory> | Set<String> |  | 1093 |
| `filterDirectMemories` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | memories: List<Memory><br>folderPath: String? | List<Memory> |  | 1099 |
| `buildProfileDocumentId` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | profileId: String | String |  | 1113 |
| `buildDirectoryDocumentId` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | profileId: String<br>path: String | String |  | 1117 |
| `buildMemoryDocumentId` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | profileId: String<br>uuid: String | String |  | 1123 |
| `stripJsonExtension` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | name: String | String |  | 1127 |
| `decodeMemoryTitleFromDisplayName` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | stem: String | String |  | 1135 |
| `buildVisibleMemoryName` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | title: String | String |  | 1139 |
| `encodeFileComponent` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | value: String | String |  | 1148 |
| `decodeFileComponent` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | value: String | String |  | 1157 |
| `OperitDataDocumentsProvider.onCreate` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` |  | Boolean |  | 47 |
| `OperitDataDocumentsProvider.queryRoots` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | projection: Array<out String>? | Cursor |  | 65 |
| `OperitDataDocumentsProvider.queryDocument` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | documentId: String<br>projection: Array<out String>? | Cursor |  | 83 |
| `OperitDataDocumentsProvider.queryChildDocuments` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | parentDocumentId: String<br>projection: Array<out String>?<br>sortOrder: String? | Cursor |  | 89 |
| `OperitDataDocumentsProvider.openDocument` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | documentId: String<br>mode: String<br>signal: CancellationSignal? | ParcelFileDescriptor |  | 107 |
| `OperitDataDocumentsProvider.createDocument` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | parentDocumentId: String<br>mimeType: String<br>displayName: String | String |  | 119 |
| `OperitDataDocumentsProvider.deleteDocument` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | documentId: String | Unit |  | 145 |
| `OperitDataDocumentsProvider.renameDocument` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | documentId: String<br>displayName: String | String |  | 161 |
| `OperitDataDocumentsProvider.moveDocument` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | sourceDocumentId: String<br>sourceParentDocumentId: String<br>targetParentDocumentId: String | String |  | 178 |
| `OperitDataDocumentsProvider.isChildDocument` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | parentDocumentId: String<br>documentId: String | Boolean |  | 208 |
| `OperitDataDocumentsProvider.includeFile` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | result: MatrixCursor<br>file: File | Unit |  | 214 |
| `OperitDataDocumentsProvider.getDocumentFlags` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | file: File<br>docId: String | Int |  | 226 |
| `OperitDataDocumentsProvider.getDisplayName` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | file: File<br>docId: String | String |  | 242 |
| `OperitDataDocumentsProvider.getMimeType` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | file: File | String |  | 250 |
| `OperitDataDocumentsProvider.getExistingFile` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | documentId: String | File |  | 265 |
| `OperitDataDocumentsProvider.getFileForDocId` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | documentId: String | File |  | 273 |
| `OperitDataDocumentsProvider.getDocIdForFile` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | file: File | String |  | 284 |
| `OperitDataDocumentsProvider.resolveChildFile` | `OperitDataDocumentsProvider` | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | parent: File<br>displayName: String | File |  | 293 |
| `ensureInsideDataRoot` | — | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | file: File | File |  | 307 |
| `isSameOrChild` | — | `com.ai.assistance.operit.provider` | `OperitDataDocumentsProvider.kt` | parent: File<br>child: File | Boolean |  | 315 |
| `WorkspaceDocumentsProvider.onCreate` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` |  | Boolean |  | 54 |
| `WorkspaceDocumentsProvider.queryRoots` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | projection: Array<out String>? | Cursor |  | 72 |
| `WorkspaceDocumentsProvider.queryDocument` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | documentId: String<br>projection: Array<out String>? | Cursor |  | 92 |
| `WorkspaceDocumentsProvider.queryChildDocuments` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | parentDocumentId: String<br>projection: Array<out String>?<br>sortOrder: String? | Cursor |  | 98 |
| `WorkspaceDocumentsProvider.openDocument` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | documentId: String<br>mode: String<br>signal: CancellationSignal? | ParcelFileDescriptor |  | 119 |
| `WorkspaceDocumentsProvider.createDocument` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | parentDocumentId: String<br>mimeType: String<br>displayName: String | String? |  | 134 |
| `WorkspaceDocumentsProvider.deleteDocument` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | documentId: String | Unit |  | 165 |
| `WorkspaceDocumentsProvider.renameDocument` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | documentId: String<br>displayName: String | String? |  | 177 |
| `WorkspaceDocumentsProvider.isChildDocument` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | parentDocumentId: String<br>documentId: String | Boolean |  | 188 |
| `WorkspaceDocumentsProvider.includeFile` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | result: MatrixCursor<br>documentId: String | Unit | 将文件信息添加到cursor | 203 |
| `WorkspaceDocumentsProvider.includeFile` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | result: MatrixCursor<br>file: File | Unit |  | 208 |
| `WorkspaceDocumentsProvider.getDocIdForFile` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | file: File | String | 根据文件获取Document ID 使用相对于workspace根目录的路径作为ID | 248 |
| `WorkspaceDocumentsProvider.getFileForDocId` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | documentId: String | File | 根据Document ID获取文件 | 264 |
| `WorkspaceDocumentsProvider.getMimeType` | `WorkspaceDocumentsProvider` | `com.ai.assistance.operit.provider` | `WorkspaceDocumentsProvider.kt` | file: File | String | 获取文件的MIME类型 | 283 |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `displayName` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | inferred |  | 898 |
| `normalizedPath` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | inferred |  | 893 |
| `path` | — | `com.ai.assistance.operit.provider` | `MemoryDocumentsProvider.kt` | inferred |  | 892 |
