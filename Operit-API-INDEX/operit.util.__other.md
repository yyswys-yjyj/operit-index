# operit.util.（其余零散）

> 函数 206 · 类型 47 · 顶层常量 7 · 共 260 条
> 每日定时任务自动生成。

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `Action` | `Action` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` | class Action(val type: MarkdownProcessorType?, val text: String?) |  | 103 |
| `Action` | `Action` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` | class Action(val type: MarkdownProcessorType?, val text: String?) |  | 302 |
| `BaseJsonPlugin` | `BaseJsonPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `BaseJsonPlugin.kt` | class BaseJsonPlugin : StreamPlugin |  | 5 |
| `BaseJsonPlugin.JsonType` | `BaseJsonPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `BaseJsonPlugin.kt` | class JsonType |  | 16 |
| `IndexItem` | `IndexItem` | `com.ai.assistance.operit.util.vector` | `IndexItem.kt` | class IndexItem(private val id: Id, private val vector: FloatArray, private val version: Long, val value: T) : Any, T> | A generic wrapper for any object that needs to be stored in an HNSW index. It holds a uni… | 11 |
| `MarkdownNode` | `MarkdownNode` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | class MarkdownNode(val type: MarkdownProcessorType, initialContent: String, val nodeId: Long) |  | 57 |
| `MarkdownNodeProcessor` | `MarkdownNodeProcessor` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | class MarkdownNodeProcessor(private val type: MarkdownProcessorType) : StreamProcessor<String, MarkdownNode> | Markdown结果处理器 - 生成MarkdownNode模型 | 105 |
| `MarkdownNodeStable` | `MarkdownNodeStable` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | class MarkdownNodeStable(val type: MarkdownProcessorType, val content: String, val children: List<MarkdownNodeStable>, val nodeId: Long) |  | 67 |
| `MarkdownProcessorType` | `MarkdownProcessorType` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | class MarkdownProcessorType | Markdown处理器类型枚举 | 24 |
| `MarkdownUIBinder` | `MarkdownUIBinder` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | class MarkdownUIBinder(private val component: T, private val renderStrategy: suspend (T, MarkdownNode) -> …) : suspend | UI绑定器 - 将处理后的StreamGroup绑定到UI渲染组件 这里使用抽象类型T表示UI组件，你可以实现具体的渲染逻辑 | 181 |
| `NativeMarkdownSplitter` | `NativeMarkdownSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` | object NativeMarkdownSplitter |  | 41 |
| `NativeMarkdownSplitter.Session` | `NativeMarkdownSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` | class Session(private val handle: Long) |  | 52 |
| `NativeRipgrep` | `NativeRipgrep` | `com.ai.assistance.operit.util.ripgrep` | `NativeRipgrep.kt` | object NativeRipgrep |  | 3 |
| `NativeXmlSplitter` | `NativeXmlSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeXmlSplitter.kt` | object NativeXmlSplitter |  | 3 |
| `NestedMarkdownProcessor` | `NestedMarkdownProcessor` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | object NestedMarkdownProcessor | 递归Markdown处理器 - 在各级嵌套中应用不同的处理逻辑 | 116 |
| `PluginState` | `PluginState` | `com.ai.assistance.operit.util.stream.plugins` | `StreamPlugin.kt` | class PluginState | The possible states of a stream processing plugin. | 6 |
| `SmartString` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` | class SmartString(initialContent: String) | 智能字符串类 - 高性能的字符串构建器，带缓存优化 特性： 1. 重载 `+` 操作符为高效的 append 操作 2. 缓存 toString() 结果，只在内容变化时重新生成… | 14 |
| `StreamJsonPlugin` | `StreamJsonPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPlugin.kt` | class StreamJsonPlugin : BaseJsonPlugin | A stream processing plugin that identifies and extracts complete JSON objects or arrays. … | 9 |
| `StreamJsonPluginTest` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` | class StreamJsonPluginTest |  | 12 |
| `StreamJsonPluginTest.GroupInfo` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` | class GroupInfo(val tag: StreamPlugin?, val content: String) |  | 158 |
| `StreamMarkdownFencedCodeBlockPlugin` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownFencedCodeBlockPlugin(private val includeFences: Boolean) : StreamPlugin | A stream plugin for identifying Markdown fenced code blocks. This plugin identifies a blo… | 36 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownBoldPlugin` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownBoldPlugin(private val includeAsterisks: Boolean) : StreamPlugin | A stream plugin for identifying bold text using double asterisks (`**text**`). | 223 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownInlineCodePlugin` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownInlineCodePlugin(private val includeTicks: Boolean) : StreamPlugin | A stream plugin for identifying Markdown inline code snippets (`code` or ``code``). It ma… | 143 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownItalicPlugin` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownItalicPlugin(private val includeAsterisks: Boolean) : StreamPlugin | A stream plugin for identifying italic text using single asterisks (`*text*`)。 | 295 |
| `StreamMarkdownHeaderPlugin` | `StreamMarkdownHeaderPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownHeaderPlugin(private val includeMarker: Boolean) : StreamPlugin | Identifies ATX-style Markdown headers (e.g., "# My Header"). A header is defined as 1-6 '… | 382 |
| `StreamMarkdownLinkPlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownLinkPlugin : StreamPlugin | A stream plugin for identifying Markdown links in the format [text](url). | 469 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownImagePlugin(private val includeDelimiters: Boolean) : StreamPlugin | A stream plugin for identifying Markdown images in the format ![alt text](url). | 559 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.StreamMarkdownBlockQuotePlugin` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownBlockQuotePlugin(private val includeMarker: Boolean) : StreamPlugin | A stream plugin for identifying Markdown blockquotes (lines starting with >). | 666 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.StreamMarkdownHorizontalRulePlugin` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownHorizontalRulePlugin(private val includeMarker: Boolean) : StreamPlugin | A stream plugin for identifying Markdown horizontal rules (---, ***, ___). | 751 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownInlineLaTeXPlugin(private val includeDelimiters: Boolean) : StreamPlugin | A stream plugin for identifying LaTeX inline math expressions using single dollar signs (… | 1106 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockBracketLaTeXPlugin` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownBlockBracketLaTeXPlugin(private val includeDelimiters: Boolean) : StreamPlugin | LaTeX block math using \[ ... \] delimiters. | 1308 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockLaTeXPlugin` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownBlockLaTeXPlugin(private val includeDelimiters: Boolean) : StreamPlugin | A stream plugin for identifying LaTeX block math expressions using double dollar signs ($… | 1246 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownInlineParenLaTeXPlugin` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownInlineParenLaTeXPlugin(private val includeDelimiters: Boolean) : StreamPlugin | LaTeX inline math using \( ... \) delimiters. | 1175 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownTablePlugin` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownTablePlugin(private val includeDelimiters: Boolean) : StreamPlugin | A stream plugin for identifying Markdown tables. It recognizes complete table blocks with… | 1374 |
| `StreamMarkdownLinkPlugin.StreamMarkdownOrderedListPlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownOrderedListPlugin(private val includeMarker: Boolean) : StreamPlugin | A stream plugin for identifying Markdown ordered lists (lines starting with a number foll… | 965 |
| `StreamMarkdownLinkPlugin.StreamMarkdownStrikethroughPlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownStrikethroughPlugin(private val includeDelimiters: Boolean) : StreamPlugin | A stream plugin for identifying Markdown strikethrough text using double tildes (`~~text~… | 819 |
| `StreamMarkdownLinkPlugin.StreamMarkdownUnderlinePlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownUnderlinePlugin(private val includeDelimiters: Boolean) : StreamPlugin | A stream plugin for identifying Markdown underlined text using double underscores (`__tex… | 892 |
| `StreamMarkdownLinkPlugin.StreamMarkdownUnorderedListPlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | class StreamMarkdownUnorderedListPlugin(private val includeMarker: Boolean) : StreamPlugin | A stream plugin for identifying Markdown unordered lists (lines starting with *, - or + f… | 1037 |
| `StreamMarkdownPluginTest` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` | class StreamMarkdownPluginTest |  | 12 |
| `StreamMarkdownPluginTest.GroupInfo` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` | class GroupInfo(val tag: StreamPlugin?, val content: String) |  | 556 |
| `StreamPlugin` | `StreamPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamPlugin.kt` | interface StreamPlugin | 流处理插件接口 用于实现各种针对字符流的处理逻辑 | 24 |
| `StreamPureJsonPlugin` | `StreamPureJsonPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamPureJsonPlugin.kt` | class StreamPureJsonPlugin : BaseJsonPlugin | A stream processing plugin to identify JSON structures and extract only their content, fi… | 10 |
| `StreamXmlPlugin` | `StreamXmlPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` | class StreamXmlPlugin(private val includeTagsInOutput: Boolean) : StreamPlugin | A stream processing plugin to identify and process XML-formatted data streams. This imple… | 17 |
| `StreamXmlPluginTest` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` | class StreamXmlPluginTest | StreamXmlPlugin的Android测试类 | 11 |
| `StringCollectorProcessor` | `StringCollectorProcessor` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | class StringCollectorProcessor : StreamProcessor<String, String> | 字符串收集处理器 - 简单地将流收集为字符串 | 15 |
| `UserCancellationException` | `UserCancellationException` | `com.ai.assistance.operit.util.exceptions` | `UserCancellationException.kt` | class UserCancellationException(message: String, cause: Throwable?) : CancellationException | An exception to indicate that an operation was explicitly cancelled by the user. This hel… | 11 |
| `VectorIndexManager` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` | class VectorIndexManager(private val dimensions: Int, private val maxElements: Int, private val indexFile: File?) : Any> | 精简的HNSW向量索引管理器，支持初始化、添加、查询、保存、加载。 | 14 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `StreamJsonPluginTest.testSimpleJsonObject` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` |  | Unit | --- Tests for StreamJsonPlugin (extracts full JSON) --- | 17 ⚑ |
| `StreamJsonPluginTest.testSimpleJsonArray` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` |  | Unit |  | 36 ⚑ |
| `StreamJsonPluginTest.testNestedJsonObject` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` |  | Unit |  | 50 ⚑ |
| `StreamJsonPluginTest.testJsonWithEscapedChars` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` |  | Unit |  | 63 ⚑ |
| `StreamJsonPluginTest.testJsonWithStringsContainingBraces` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` |  | Unit |  | 74 ⚑ |
| `StreamJsonPluginTest.testSimpleJsonObject_Pure` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` |  | Unit | --- Tests for StreamPureJsonPlugin (extracts and filters content) --- | 87 ⚑ |
| `StreamJsonPluginTest.testSimpleJsonArray_Pure` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` |  | Unit |  | 100 ⚑ |
| `StreamJsonPluginTest.testNestedJsonObject_Pure` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` |  | Unit |  | 113 ⚑ |
| `StreamJsonPluginTest.testPureWithEscapedChars` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` |  | Unit |  | 134 ⚑ |
| `StreamJsonPluginTest.collectGroups` | `StreamJsonPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPluginTest.kt` | stream: com.ai.assistance.operit.util.strea…<br>plugin: StreamPlugin | List<GroupInfo> | --- Helper function --- | 145 ⚑ |
| `StreamMarkdownPluginTest.testBoldPlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试基本的 Markdown 粗体插件 --- | 16 ⚑ |
| `StreamMarkdownPluginTest.testItalicPlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试基本的 Markdown 斜体插件 --- | 40 ⚑ |
| `StreamMarkdownPluginTest.testInlineCodePlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试行内代码插件 --- | 64 ⚑ |
| `StreamMarkdownPluginTest.testFencedCodeBlockPlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试代码块插件 --- | 84 ⚑ |
| `StreamMarkdownPluginTest.testHeaderPlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试标题插件 --- | 119 ⚑ |
| `StreamMarkdownPluginTest.testLinkPlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试链接插件 --- | 154 ⚑ |
| `StreamMarkdownPluginTest.testImagePlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试图片插件 --- | 178 ⚑ |
| `StreamMarkdownPluginTest.testBlockQuotePlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试引用块插件 --- | 202 ⚑ |
| `StreamMarkdownPluginTest.testHorizontalRulePlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试水平线插件 --- | 239 ⚑ |
| `StreamMarkdownPluginTest.testStrikethroughPlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试删除线插件 --- | 279 ⚑ |
| `StreamMarkdownPluginTest.testUnderlinePlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试下划线插件 --- | 303 ⚑ |
| `StreamMarkdownPluginTest.testOrderedListPlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试有序列表插件 --- | 327 ⚑ |
| `StreamMarkdownPluginTest.testUnorderedListPlugin` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试无序列表插件 --- | 363 ⚑ |
| `StreamMarkdownPluginTest.testMultipleMarkdownPlugins` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试多个插件共同工作 --- | 399 ⚑ |
| `StreamMarkdownPluginTest.testPluginsWithoutDelimiters` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试不包含分隔符 --- | 468 ⚑ |
| `StreamMarkdownPluginTest.testEdgeCases` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` |  | Unit | --- 测试异常情况 --- | 504 ⚑ |
| `StreamMarkdownPluginTest.collectGroups` | `StreamMarkdownPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPluginTest.kt` | stream: com.ai.assistance.operit.util.strea…<br>plugin: StreamPlugin | List<GroupInfo> | --- Helper function --- | 543 ⚑ |
| `StreamXmlPluginTest.setup` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` |  | Unit |  | 16 ⚑ |
| `StreamXmlPluginTest.testInitialState` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` |  | Unit |  | 22 ⚑ |
| `StreamXmlPluginTest.testStartTagDetection` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` |  | Unit |  | 28 ⚑ |
| `StreamXmlPluginTest.testCompleteTagRecognitionAndProcessingEnter` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` |  | Unit |  | 38 ⚑ |
| `StreamXmlPluginTest.testTagWithAttributes` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` |  | Unit |  | 46 ⚑ |
| `StreamXmlPluginTest.testEndTagRecognition` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` |  | Unit |  | 53 ⚑ |
| `StreamXmlPluginTest.testFailedMatch` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` |  | Unit |  | 61 ⚑ |
| `StreamXmlPluginTest.testResetFunction` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` |  | Unit |  | 90 ⚑ |
| `StreamXmlPluginTest.testFullXmlProcessingAndCharacterConsumption` | `StreamXmlPluginTest` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPluginTest.kt` |  | Unit |  | 105 ⚑ |
| `StringCollectorProcessor.process` | `StringCollectorProcessor` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | stream: Stream<String> | String |  | 16 |
| `toCharStream` | — | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` |  | Stream<Char> | 将字符串转换为字符流 | 75 |
| `MarkdownNodeProcessor.process` | `MarkdownNodeProcessor` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | stream: Stream<String> | MarkdownNode |  | 107 |
| `NestedMarkdownProcessor.getBlockPlugins` | `NestedMarkdownProcessor` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` |  | List<StreamPlugin> | 块级插件列表 | 119 |
| `NestedMarkdownProcessor.getInlinePlugins` | `NestedMarkdownProcessor` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` |  | List<StreamPlugin> | 内联插件列表 | 138 |
| `NestedMarkdownProcessor.getTypeForPlugin` | `NestedMarkdownProcessor` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | plugin: StreamPlugin? | MarkdownProcessorType | 根据插件获取对应的Markdown处理器类型 | 154 |
| `MarkdownUIBinder.bind` | `MarkdownUIBinder` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | group: StreamGroup<MarkdownProcessorType> | Unit | 绑定StreamGroup到UI组件 | 186 |
| `MarkdownUIBinder.processGroupToNodes` | `MarkdownUIBinder` | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | group: StreamGroup<MarkdownProcessorType> | MarkdownNode | 将StreamGroup转换为MarkdownNode树 | 193 |
| `SmartString.plus` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` | content: String | SmartString | 追加字符串内容 | 24 |
| `SmartString.plus` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` | char: Char | SmartString | 追加字符内容 | 37 |
| `SmartString.toString` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` |  | String | 智能 toString - 只在内容变化时重新生成字符串 | 47 |
| `SmartString.isEmpty` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` |  | Boolean | 判断是否为空 | 70 |
| `SmartString.isNotEmpty` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` |  | Boolean | 判断是否非空 | 75 |
| `SmartString.clear` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` |  | Unit | 清空内容 | 80 |
| `SmartString.truncate` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` | length: Int | SmartString | Truncates accumulated content without creating an immutable String snapshot. | 87 |
| `SmartString.replace` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` | content: String | SmartString | Replaces accumulated content while preserving this buffer instance. | 100 |
| `SmartString.take` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` | n: Int | String | 截取字符串 | 111 |
| `SmartString.append` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` | content: String | SmartString | 追加内容（兼容 StringBuilder 风格） | 122 |
| `SmartString.append` | `SmartString` | `com.ai.assistance.operit.util.markdown` | `SmartString.kt` | char: Char | SmartString | 追加字符（兼容 StringBuilder 风格） | 129 |
| `NativeRipgrep.searchJson` | `NativeRipgrep` | `com.ai.assistance.operit.util.ripgrep` | `NativeRipgrep.kt` | path: String<br>patterns: Array<String><br>filePattern: String<br>caseInsensitive: Boolean<br>literal: Boolean<br>contextLines: Int<br>maxResults: Int | String |  | 9 |
| `BaseJsonPlugin.processChar` | `BaseJsonPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `BaseJsonPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 22 |
| `handleCharInProcessing` | — | `com.ai.assistance.operit.util.stream.plugins` | `BaseJsonPlugin.kt` | c: Char | Boolean |  | 48 |
| `finishProcessing` | — | `com.ai.assistance.operit.util.stream.plugins` | `BaseJsonPlugin.kt` |  | Unit |  | 85 |
| `initPlugin` | — | `com.ai.assistance.operit.util.stream.plugins` | `BaseJsonPlugin.kt` |  | Boolean |  | 91 |
| `destroy` | — | `com.ai.assistance.operit.util.stream.plugins` | `BaseJsonPlugin.kt` |  | Unit |  | 96 |
| `reset` | — | `com.ai.assistance.operit.util.stream.plugins` | `BaseJsonPlugin.kt` |  | Unit |  | 98 |
| `shouldEmit` | — | `com.ai.assistance.operit.util.stream.plugins` | `BaseJsonPlugin.kt` | c: Char | Boolean | Abstract method for subclasses to decide whether a character should be emitted. | 110 |
| `StreamJsonPlugin.shouldEmit` | `StreamJsonPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamJsonPlugin.kt` | c: Char | Boolean | Determines that all characters within the JSON structure should be emitted. | 14 |
| `StreamMarkdownFencedCodeBlockPlugin.processChar` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 57 |
| `StreamMarkdownFencedCodeBlockPlugin.initPlugin` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 120 |
| `StreamMarkdownFencedCodeBlockPlugin.destroy` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 125 |
| `StreamMarkdownFencedCodeBlockPlugin.reset` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 127 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownInlineCodePlugin.processChar` | `StreamMarkdownInlineCodePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 158 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownInlineCodePlugin.initPlugin` | `StreamMarkdownInlineCodePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 204 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownInlineCodePlugin.destroy` | `StreamMarkdownInlineCodePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 209 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownInlineCodePlugin.reset` | `StreamMarkdownInlineCodePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 211 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownBoldPlugin.processChar` | `StreamMarkdownBoldPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 243 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownBoldPlugin.initPlugin` | `StreamMarkdownBoldPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 276 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownBoldPlugin.destroy` | `StreamMarkdownBoldPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 281 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownBoldPlugin.reset` | `StreamMarkdownBoldPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 283 |
| `StreamMarkdownFencedCodeBlockPlugin.StreamMarkdownItalicPlugin.processChar` | `StreamMarkdownItalicPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 316 |
| `StreamMarkdownFencedCodeBlockPlugin.initPlugin` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 362 |
| `StreamMarkdownFencedCodeBlockPlugin.destroy` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 367 |
| `StreamMarkdownFencedCodeBlockPlugin.reset` | `StreamMarkdownFencedCodeBlockPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 369 |
| `StreamMarkdownHeaderPlugin.processChar` | `StreamMarkdownHeaderPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 398 |
| `StreamMarkdownHeaderPlugin.handleMatch` | `StreamMarkdownHeaderPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char | Boolean |  | 419 |
| `StreamMarkdownHeaderPlugin.initPlugin` | `StreamMarkdownHeaderPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 444 |
| `StreamMarkdownHeaderPlugin.destroy` | `StreamMarkdownHeaderPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 449 |
| `StreamMarkdownHeaderPlugin.reset` | `StreamMarkdownHeaderPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit | The problematic call from splitBy will now only perform a soft reset of the matching stat… | 453 |
| `StreamMarkdownHeaderPlugin.resetInternal` | `StreamMarkdownHeaderPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit | Internal reset that doesn't touch atStartOfLine | 458 |
| `StreamMarkdownLinkPlugin.processChar` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 492 |
| `StreamMarkdownLinkPlugin.initPlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 540 |
| `StreamMarkdownLinkPlugin.destroy` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 545 |
| `StreamMarkdownLinkPlugin.reset` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 547 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.processChar` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 586 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.initPlugin` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 647 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.destroy` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 652 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.reset` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 654 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.StreamMarkdownBlockQuotePlugin.processChar` | `StreamMarkdownBlockQuotePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 679 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.handleMatch` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char | Boolean |  | 712 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.initPlugin` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 729 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.destroy` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 734 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.reset` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 736 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.resetInternal` | `StreamMarkdownImagePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 740 |
| `StreamMarkdownLinkPlugin.StreamMarkdownImagePlugin.StreamMarkdownHorizontalRulePlugin.processChar` | `StreamMarkdownHorizontalRulePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 758 |
| `StreamMarkdownLinkPlugin.initPlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 796 |
| `StreamMarkdownLinkPlugin.destroy` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 801 |
| `StreamMarkdownLinkPlugin.reset` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 803 |
| `StreamMarkdownLinkPlugin.resetInternal` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 807 |
| `StreamMarkdownLinkPlugin.StreamMarkdownStrikethroughPlugin.processChar` | `StreamMarkdownStrikethroughPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 840 |
| `StreamMarkdownLinkPlugin.StreamMarkdownStrikethroughPlugin.initPlugin` | `StreamMarkdownStrikethroughPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 873 |
| `StreamMarkdownLinkPlugin.StreamMarkdownStrikethroughPlugin.destroy` | `StreamMarkdownStrikethroughPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 878 |
| `StreamMarkdownLinkPlugin.StreamMarkdownStrikethroughPlugin.reset` | `StreamMarkdownStrikethroughPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 880 |
| `StreamMarkdownLinkPlugin.StreamMarkdownUnderlinePlugin.processChar` | `StreamMarkdownUnderlinePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 912 |
| `StreamMarkdownLinkPlugin.StreamMarkdownUnderlinePlugin.initPlugin` | `StreamMarkdownUnderlinePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 945 |
| `StreamMarkdownLinkPlugin.StreamMarkdownUnderlinePlugin.destroy` | `StreamMarkdownUnderlinePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 950 |
| `StreamMarkdownLinkPlugin.StreamMarkdownUnderlinePlugin.reset` | `StreamMarkdownUnderlinePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 952 |
| `StreamMarkdownLinkPlugin.StreamMarkdownOrderedListPlugin.processChar` | `StreamMarkdownOrderedListPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 980 |
| `StreamMarkdownLinkPlugin.handleMatch` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char | Boolean |  | 997 |
| `StreamMarkdownLinkPlugin.initPlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 1014 |
| `StreamMarkdownLinkPlugin.destroy` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1019 |
| `StreamMarkdownLinkPlugin.reset` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1021 |
| `StreamMarkdownLinkPlugin.resetInternal` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1025 |
| `StreamMarkdownLinkPlugin.StreamMarkdownUnorderedListPlugin.processChar` | `StreamMarkdownUnorderedListPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 1050 |
| `StreamMarkdownLinkPlugin.handleMatch` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char | Boolean |  | 1067 |
| `StreamMarkdownLinkPlugin.initPlugin` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 1084 |
| `StreamMarkdownLinkPlugin.destroy` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1089 |
| `StreamMarkdownLinkPlugin.reset` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1091 |
| `StreamMarkdownLinkPlugin.resetInternal` | `StreamMarkdownLinkPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1095 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.processChar` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 1123 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.initPlugin` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 1158 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.destroy` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1163 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.reset` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1165 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownInlineParenLaTeXPlugin.processChar` | `StreamMarkdownInlineParenLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 1192 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownInlineParenLaTeXPlugin.initPlugin` | `StreamMarkdownInlineParenLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 1227 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownInlineParenLaTeXPlugin.destroy` | `StreamMarkdownInlineParenLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1232 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownInlineParenLaTeXPlugin.reset` | `StreamMarkdownInlineParenLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1234 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockLaTeXPlugin.processChar` | `StreamMarkdownBlockLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 1256 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockLaTeXPlugin.initPlugin` | `StreamMarkdownBlockLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 1291 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockLaTeXPlugin.destroy` | `StreamMarkdownBlockLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1296 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockLaTeXPlugin.reset` | `StreamMarkdownBlockLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1298 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockBracketLaTeXPlugin.processChar` | `StreamMarkdownBlockBracketLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 1319 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockBracketLaTeXPlugin.initPlugin` | `StreamMarkdownBlockBracketLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 1354 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockBracketLaTeXPlugin.destroy` | `StreamMarkdownBlockBracketLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1359 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownBlockBracketLaTeXPlugin.reset` | `StreamMarkdownBlockBracketLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1361 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.StreamMarkdownTablePlugin.processChar` | `StreamMarkdownTablePlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean |  | 1405 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.initPlugin` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Boolean |  | 1494 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.destroy` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1499 |
| `StreamMarkdownLinkPlugin.StreamMarkdownInlineLaTeXPlugin.reset` | `StreamMarkdownInlineLaTeXPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` |  | Unit |  | 1501 |
| `StreamPlugin.processChar` | `StreamPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean | 处理单个字符，并决定是否应将其发射到流中。 | 37 |
| `StreamPlugin.initPlugin` | `StreamPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamPlugin.kt` |  | Boolean | 初始化插件 | 43 |
| `StreamPlugin.destroy` | `StreamPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamPlugin.kt` |  | Unit | 销毁插件，释放资源 | 48 |
| `StreamPlugin.reset` | `StreamPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamPlugin.kt` |  | Unit | 重置插件状态 | 53 |
| `StreamPureJsonPlugin.shouldEmit` | `StreamPureJsonPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamPureJsonPlugin.kt` | c: Char | Boolean | Determines whether a character should be emitted based on whether it is part of the JSON … | 17 |
| `StreamXmlPlugin.processChar` | `StreamXmlPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` | c: Char<br>atStartOfLine: Boolean | Boolean | Processes a single character for XML stream parsing and decides if it should be emitted. … | 65 |
| `StreamXmlPlugin.finish` | `StreamXmlPlugin` | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` | result: Boolean | Boolean |  | 66 |
| `initPlugin` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` |  | Boolean | Initializes the plugin to its default state. | 169 |
| `destroy` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` |  | Unit | Destroys the plugin. No-op as listener is removed. | 175 |
| `reset` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` |  | Unit | Resets the plugin state. | 178 |
| `handleDefaultCharacter` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` | c: Char | Boolean |  | 185 |
| `updatePunctuationAllowance` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` | c: Char | Unit |  | 190 |
| `isEmojiTrigger` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` | c: Char | Boolean |  | 204 |
| `isEmojiContinuationChar` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` | c: Char | Boolean |  | 213 |
| `toMarkdownTypeOrNull` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` |  | MarkdownProcessorType? |  | 6 |
| `toInlineStableNodes` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` | content: String | List<MarkdownNodeStable> |  | 9 |
| `NativeMarkdownSplitter.nativeCreateBlockSession` | `NativeMarkdownSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` |  | Long |  | 47 |
| `NativeMarkdownSplitter.nativeCreateInlineSession` | `NativeMarkdownSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` |  | Long |  | 48 |
| `NativeMarkdownSplitter.nativeDestroySession` | `NativeMarkdownSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` | handle: Long | Unit |  | 49 |
| `NativeMarkdownSplitter.nativePush` | `NativeMarkdownSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` | handle: Long<br>chunk: String | IntArray |  | 50 |
| `NativeMarkdownSplitter.Session.push` | `Session` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` | chunk: String | IntArray |  | 55 |
| `NativeMarkdownSplitter.Session.destroy` | `Session` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` |  | Unit |  | 56 |
| `NativeMarkdownSplitter.createBlockSession` | `NativeMarkdownSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` |  | Session |  | 59 |
| `NativeMarkdownSplitter.createInlineSession` | `NativeMarkdownSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` |  | Session |  | 60 |
| `NativeMarkdownSplitter.parseInlineToStableNodes` | `NativeMarkdownSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownSplitter.kt` | content: String | List<MarkdownNodeStable> |  | 62 |
| `toMarkdownTypeOrNull` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | MarkdownProcessorType? |  | 18 |
| `lock` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 37 |
| `unlock` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 38 |
| `clearBuffer` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 39 |
| `collect` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` | collector: StreamCollector<StreamGroup<Markdow… | Unit |  | 41 |
| `openDefaultChannel` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 62 |
| `closeDefaultChannel` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 71 |
| `openPluginChannel` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` | tag: MarkdownProcessorType | Unit |  | 76 |
| `closePluginChannel` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 84 |
| `flushDelta` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 90 |
| `lock` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 236 |
| `unlock` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 237 |
| `clearBuffer` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 238 |
| `collect` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` | collector: StreamCollector<StreamGroup<Markdow… | Unit |  | 240 |
| `openDefaultChannel` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 261 |
| `closeDefaultChannel` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 270 |
| `openPluginChannel` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` | tag: MarkdownProcessorType | Unit |  | 275 |
| `closePluginChannel` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 283 |
| `flushDelta` | — | `com.ai.assistance.operit.util.streamnative` | `NativeMarkdownStreamOperators.kt` |  | Unit |  | 289 |
| `NativeXmlSplitter.nativeSplitXmlSegments` | `NativeXmlSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeXmlSplitter.kt` | content: String | IntArray |  | 9 |
| `NativeXmlSplitter.splitXmlTag` | `NativeXmlSplitter` | `com.ai.assistance.operit.util.streamnative` | `NativeXmlSplitter.kt` | content: String | List<List<String>> |  | 11 |
| `IndexItem.id` | `IndexItem` | `com.ai.assistance.operit.util.vector` | `IndexItem.kt` |  | Id |  | 18 |
| `IndexItem.vector` | `IndexItem` | `com.ai.assistance.operit.util.vector` | `IndexItem.kt` |  | FloatArray |  | 19 |
| `IndexItem.dimensions` | `IndexItem` | `com.ai.assistance.operit.util.vector` | `IndexItem.kt` |  | Int |  | 20 |
| `IndexItem.version` | `IndexItem` | `com.ai.assistance.operit.util.vector` | `IndexItem.kt` |  | Long |  | 21 |
| `IndexItem.equals` | `IndexItem` | `com.ai.assistance.operit.util.vector` | `IndexItem.kt` | other: Any? | Boolean |  | 23 |
| `IndexItem.hashCode` | `IndexItem` | `com.ai.assistance.operit.util.vector` | `IndexItem.kt` |  | Int |  | 31 |
| `VectorIndexManager.initIndex` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` |  | Unit | 初始化索引（新建或加载） | 26 |
| `VectorIndexManager.addItem` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` | item: T | Unit | 添加一个向量项 | 48 |
| `VectorIndexManager.removeItem` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` | id: Id<br>version: Long? | Boolean | 删除一个向量项。 | 54 |
| `VectorIndexManager.findNearest` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` | query: FloatArray<br>k: Int | List<T> | 查询最近的K个邻居 | 59 |
| `VectorIndexManager.size` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` |  | Int |  | 63 |
| `VectorIndexManager.maxItemCount` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` |  | Int |  | 65 |
| `VectorIndexManager.ensureCapacity` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` | minCapacity: Int | Unit |  | 67 |
| `VectorIndexManager.save` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` |  | Unit | 保存索引到文件 | 75 |
| `VectorIndexManager.close` | `VectorIndexManager` | `com.ai.assistance.operit.util.vector` | `VectorIndexManager.kt` |  | Unit | 关闭索引（可选） | 88 |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `GROUP_CONTENT` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` | inferred |  | 6 |
| `GROUP_DELIMITER` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | inferred | A collection of StreamPlugins for parsing various Markdown constructs. To use t… | 25 |
| `GROUP_HEADER_HASHES` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | inferred |  | 26 |
| `GROUP_TAG_NAME` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamXmlPlugin.kt` | inferred |  | 5 |
| `GROUP_TEXT` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | inferred |  | 27 |
| `GROUP_URL` | — | `com.ai.assistance.operit.util.stream.plugins` | `StreamMarkdownPlugin.kt` | inferred |  | 28 |
| `markdownNodeIdGenerator` | — | `com.ai.assistance.operit.util.markdown` | `MarkdownProcessor.kt` | inferred | Markdown数据模型 | 55 |
