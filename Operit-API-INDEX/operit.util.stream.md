# operit.util.stream

> 函数 297 · 类型 60 · 顶层常量 12 · 共 369 条
> 每日定时任务自动生成。

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `AbstractStream` | `AbstractStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | class AbstractStream : Stream<T> | 默认Stream抽象实现，提供锁定功能 | 110 |
| `AndCondition` | `AndCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class AndCondition(private val conditions: List<KmpCondition>) : KmpCondition | 使用AND逻辑组合多个条件 | 88 |
| `CharCondition` | `CharCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class CharCondition(private val expectedChar: Char) : KmpCondition | 匹配特定字符的简单条件 | 25 |
| `CharRangeCondition` | `CharRangeCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class CharRangeCondition(private val from: Char, private val to: Char) : KmpCondition | 匹配指定范围内任何字符的条件 | 36 |
| `CharSetCondition` | `CharSetCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class CharSetCondition(private val charSet: Set<Char>) : KmpCondition | 匹配字符集中任何字符的条件 | 43 |
| `CompositeStreamProcessor` | `CompositeStreamProcessor` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | class CompositeStreamProcessor(private val processors: List<StreamProcessor<T, *>>, private val finalProcessor: StreamProcessor<T, R>) : StreamProcessor<T, R> | 复合型流处理器，可以组合多个处理器按顺序执行 | 26 |
| `DelegatingRevisableCharStream` | `DelegatingRevisableCharStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | class DelegatingRevisableCharStream(private val upstream: Stream<Char>, override val eventChannel: SharedStream<TextStreamEvent>) : RevisableCharStream |  | 123 |
| `DelegatingRevisableSharedTextStream` | `DelegatingRevisableSharedTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | class DelegatingRevisableSharedTextStream(private val upstream: SharedStream<String>, override val eventChannel: SharedStream<TextStreamEvent>) : RevisableSharedTextStream |  | 87 |
| `DelegatingRollbackPrefixCharStream` | `DelegatingRollbackPrefixCharStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | class DelegatingRollbackPrefixCharStream(private val upstream: Stream<Char>, override val rollbackPrefix: String) : Stream<Char> by upstream, StreamRollbackPrefix |  | 150 |
| `FlowAsStream` | `FlowAsStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | class FlowAsStream(private val flow: Flow<T>) : AbstractStream<T> | Flow到Stream的适配器，允许将Kotlin Flow转换为Stream | 191 |
| `GreedyStarCondition` | `GreedyStarCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class GreedyStarCondition(val condition: KmpCondition) : KmpCondition | 贪心星号匹配条件（内部使用） | 124 |
| `GroupCondition` | `GroupCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class GroupCondition(val groupId: Int, val conditions: List<KmpCondition>) : KmpCondition | A private marker condition used by the builder to handle capturing groups. | 131 |
| `HotStreamAndroidTest` | `HotStreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `HotStreamAndroidTest.kt` | class HotStreamAndroidTest | Android测试类，用于测试热流（HotStream）功能 | 30 |
| `HotStreamTest` | `HotStreamTest` | `com.ai.assistance.operit.util.stream` | `HotStreamTest.kt` | class HotStreamTest |  | 17 |
| `KmpCondition` | `KmpCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | interface KmpCondition | 条件接口，用于KMP图中的字符匹配 允许灵活的模式匹配，超越简单的字符相等性比较 | 4 |
| `KmpNode` | `KmpNode` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class KmpNode(val id: Int, val depth: Int, var isFinal: Boolean) | KMP状态机图中的节点 | 153 |
| `KmpNodeChangeListener` | `KmpNodeChangeListener` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | interface KmpNodeChangeListener | 节点变化监听器，用于监听KMP图中当前节点的变化 | 182 |
| `KmpPattern` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class KmpPattern | 简化的模式构建DSL，允许以更简洁的方式构建KMP匹配条件 | 493 |
| `MutableSharedStream` | `MutableSharedStream` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | interface MutableSharedStream : SharedStream<T> | 可变共享Stream接口，类似于MutableSharedFlow | 25 |
| `MutableSharedStreamImpl` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | class MutableSharedStreamImpl(replay: Int, extraBufferCapacity: Int, onBufferOverflow: BufferOverflow, private val propagateCompletionCause: Boolean) : MutableSharedStream<T> | MutableSharedFlow的包装器，实现MutableSharedStream | 65 |
| `MutableSharedStreamImpl.SharedEvent` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | interface SharedEvent |  | 71 |
| `MutableSharedStreamImpl.SharedEvent.Value` | `SharedEvent` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | class Value(val payload: T) : SharedEvent<T> data class Completion |  | 72 |
| `MutableStateStream` | `MutableStateStream` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | interface MutableStateStream : StateStream<T>, MutableSharedStream<T> | 可变状态Stream接口，类似于MutableStateFlow | 43 |
| `MutableStateStreamImpl` | `MutableStateStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | class MutableStateStreamImpl(initialValue: T) : MutableStateStream<T> | MutableStateFlow的包装器，实现MutableStateStream | 239 |
| `NotCondition` | `NotCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class NotCondition(private val condition: KmpCondition) : KmpCondition | 对另一个条件取反的条件 | 58 |
| `NoValue` | `NoValue` | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` | object NoValue : Exception | 用于表示没有值的标记对象 | 490 |
| `OrCondition` | `OrCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class OrCondition(private val conditions: List<KmpCondition>) : KmpCondition | 使用OR逻辑组合多个条件 | 77 |
| `PredicateCondition` | `PredicateCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class PredicateCondition(private val description: String, private val predicate: (Char) -> Boolean) : KmpCondition | 使用自定义谓词函数匹配字符的条件 | 99 |
| `RevisableTextStream` | `RevisableTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | interface RevisableTextStream : Stream<Char>, TextStreamEventCarrier private class Delegati… |  | 54 |
| `RevisionAppliedTextTest` | `RevisionAppliedTextTest` | `com.ai.assistance.operit.util.stream` | `RevisionAppliedTextTest.kt` | class RevisionAppliedTextTest |  | 10 |
| `RevisionEventRelayTest` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` | class RevisionEventRelayTest |  | 20 |
| `SharedStream` | `SharedStream` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | interface SharedStream : Stream<T> | 共享Stream接口，类似于SharedFlow | 13 |
| `StateStream` | `StateStream` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | interface StateStream : SharedStream<T> | 状态Stream接口，类似于StateFlow | 37 |
| `Stream` | `Stream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | interface Stream | Stream接口，类似于Kotlin Flow，用于表示异步计算的数据流 | 71 |
| `StreamAndroidTest` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` | class StreamAndroidTest | Android测试类，用于测试Stream的基本操作符和功能 | 26 |
| `StreamAsFlow` | `StreamAsFlow` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | class StreamAsFlow(private val stream: Stream<T>) : Flow<T> | Stream到Flow的适配器，允许将Stream转换为Kotlin Flow | 228 |
| `StreamCollector` | `StreamCollector` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | interface StreamCollector | Stream收集器接口，类似于FlowCollector | 104 |
| `StreamGroup` | `StreamGroup` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | class StreamGroup(val tag: TAG, val stream: Stream<String>, val processor: StreamProcessor<String, *>?, val children: MutableList<StreamGroup<*>>) | StreamGroup表示带有关联标签的流数据组，支持嵌套结构和处理器绑定 | 57 |
| `StreamGroupBuilder` | `StreamGroupBuilder` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | class StreamGroupBuilder | StreamGroupBuilder - 用于构建嵌套的StreamGroup结构 | 122 |
| `StreamInterceptor` | `StreamInterceptor` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | class StreamInterceptor(sourceStream: Stream<T>, private var onEach: (T) -> R) |  | 206 |
| `StreamKmpGraph` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class StreamKmpGraph | 实现基于图的Knuth-Morris-Pratt算法，支持自定义转换和灵活的模式匹配 | 193 |
| `StreamKmpGraphBuilder` | `StreamKmpGraphBuilder` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | class StreamKmpGraphBuilder | 简化的KMP图构建器 | 414 |
| `StreamKmpGraphTest` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` | class StreamKmpGraphTest |  | 14 |
| `StreamKmpMatchResult` | `StreamKmpMatchResult` | `com.ai.assistance.operit.util.stream` | `StreamKmpMatchResult.kt` | class StreamKmpMatchResult | Represents the outcome of processing a single character in a StreamKmpGraph. | 4 |
| `StreamKmpMatchResult.InProgress` | `StreamKmpMatchResult` | `com.ai.assistance.operit.util.stream` | `StreamKmpMatchResult.kt` | object InProgress : StreamKmpMatchResult |  | 9 |
| `StreamKmpMatchResult.NoMatch` | `StreamKmpMatchResult` | `com.ai.assistance.operit.util.stream` | `StreamKmpMatchResult.kt` | object NoMatch : StreamKmpMatchResult | The character was not part of any match and the state was reset. | 6 |
| `StreamLogger` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | object StreamLogger | 日志工具类，统一Stream相关日志 | 15 |
| `StreamProcessor` | `StreamProcessor` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | interface StreamProcessor | 流处理器接口，定义了如何处理流数据 | 12 |
| `StreamRealTimeSplitTest` | `StreamRealTimeSplitTest` | `com.ai.assistance.operit.util.stream` | `StreamRealTimeSplitTest.kt` | class StreamRealTimeSplitTest |  | 15 |
| `StreamRollbackPrefix` | `StreamRollbackPrefix` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | interface StreamRollbackPrefix | Marks a replacement stream with content already rendered before a rollback. | 50 |
| `StreamSplitByTest` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` | class StreamSplitByTest | Stream.splitBy功能的Android测试类 主要测试splitBy与XML插件结合使用的情况 | 16 |
| `StreamStart` | `StreamStart` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | class StreamStart | 流启动模式 | 444 |
| `TextStreamEvent` | `TextStreamEvent` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | class TextStreamEvent(val eventType: TextStreamEventType, val id: String, val contentLength: Int, val discardedLength: Int) | A revision event for a streamed text response. [contentLength] is the offset in the raw c… | 20 |
| `TextStreamEventCarrier` | `TextStreamEventCarrier` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | interface TextStreamEventCarrier |  | 45 |
| `TextStreamEventType` | `TextStreamEventType` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | class TextStreamEventType |  | 40 |
| `TextStreamRevisionTracker` | `TextStreamRevisionTracker` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTracker.kt` | class TextStreamRevisionTracker(initialContent: String) | Applies SAVEPOINT / ROLLBACK events to a locally accumulated copy of a streamed response.… | 20 |
| `TextStreamRevisionTracker.DiscardedRange` | `TextStreamRevisionTracker` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTracker.kt` | class DiscardedRange(val start: Int, val end: Int) |  | 26 |
| `TextStreamRevisionTrackerTest` | `TextStreamRevisionTrackerTest` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTrackerTest.kt` | class TextStreamRevisionTrackerTest |  | 8 |
| `TimeoutException` | `TimeoutException` | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` | class TimeoutException(message: String) : Exception | 超时异常 | 496 |
| `ToolTagStreamParsingTest` | `ToolTagStreamParsingTest` | `com.ai.assistance.operit.util.stream` | `ToolTagStreamParsingTest.kt` | class ToolTagStreamParsingTest | Regression coverage for issue #1375. Tool calls are emitted as `<tool_XXXX name="...">...… | 22 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `HotStreamAndroidTest.setUp` | `HotStreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `HotStreamAndroidTest.kt` |  | Unit |  | 40 ⚑ |
| `HotStreamAndroidTest.tearDown` | `HotStreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `HotStreamAndroidTest.kt` |  | Unit |  | 46 ⚑ |
| `HotStreamAndroidTest.testMutableSharedStream` | `HotStreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `HotStreamAndroidTest.kt` |  | Unit |  | 51 ⚑ |
| `HotStreamAndroidTest.testTryEmitToSharedStream` | `HotStreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `HotStreamAndroidTest.kt` |  | Unit |  | 88 ⚑ |
| `HotStreamAndroidTest.testMutableStateStream` | `HotStreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `HotStreamAndroidTest.kt` |  | Unit |  | 107 ⚑ |
| `HotStreamAndroidTest.testStreamShareInDifferentModes` | `HotStreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `HotStreamAndroidTest.kt` |  | Unit |  | 153 ⚑ |
| `HotStreamAndroidTest.testStreamStateInDifferentModes` | `HotStreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `HotStreamAndroidTest.kt` |  | Unit |  | 258 ⚑ |
| `HotStreamAndroidTest.testMultipleSubscribersToSharedStream` | `HotStreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `HotStreamAndroidTest.kt` |  | Unit |  | 326 ⚑ |
| `StreamAndroidTest.setUp` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 34 ⚑ |
| `StreamAndroidTest.testStreamCreation` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 39 ⚑ |
| `StreamAndroidTest.testStreamMap` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 57 ⚑ |
| `StreamAndroidTest.testStreamFilter` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 64 ⚑ |
| `StreamAndroidTest.testStreamTakeAndDrop` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 71 ⚑ |
| `StreamAndroidTest.testStreamFlatMap` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 84 ⚑ |
| `StreamAndroidTest.testStreamOnEach` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 91 ⚑ |
| `StreamAndroidTest.testStreamConcatenation` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 100 ⚑ |
| `StreamAndroidTest.testStreamErrorHandling` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 110 ⚑ |
| `StreamAndroidTest.testStreamDistinct` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 127 ⚑ |
| `StreamAndroidTest.testStreamFlowInteroperation` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 134 ⚑ |
| `StreamAndroidTest.testStreamFinally` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 153 ⚑ |
| `StreamAndroidTest.testStreamThrottle` | `StreamAndroidTest` | `com.ai.assistance.operit.util.stream` | `StreamAndroidTest.kt` |  | Unit |  | 175 ⚑ |
| `StreamKmpGraphTest.testCharCondition` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 17 ⚑ |
| `StreamKmpGraphTest.testCharRangeCondition` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 25 ⚑ |
| `StreamKmpGraphTest.testCharSetCondition` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 35 ⚑ |
| `StreamKmpGraphTest.testNotCondition` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 46 ⚑ |
| `StreamKmpGraphTest.testOrCondition` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 55 ⚑ |
| `StreamKmpGraphTest.testAndCondition` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 65 ⚑ |
| `StreamKmpGraphTest.testPredicateCondition` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 80 ⚑ |
| `StreamKmpGraphTest.testStreamKmpGraphProcessText` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 89 ⚑ |
| `StreamKmpGraphTest.testStreamKmpGraphBuilder` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 98 ⚑ |
| `StreamKmpGraphTest.testComplexPattern` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 128 ⚑ |
| `StreamKmpGraphTest.testFailureTransitions` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 158 ⚑ |
| `StreamKmpGraphTest.testKmpConditionOperators` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 170 ⚑ |
| `StreamKmpGraphTest.testCharOperators` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 190 ⚑ |
| `StreamKmpGraphTest.testKmpPatternDSL` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 211 ⚑ |
| `StreamKmpGraphTest.testPredefinedConditions` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 242 ⚑ |
| `StreamKmpGraphTest.testNegationFunctions` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 266 ⚑ |
| `StreamKmpGraphTest.testInversePredefinedConditions` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 285 ⚑ |
| `StreamKmpGraphTest.testKmpPatternNegationMethods` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 302 ⚑ |
| `StreamKmpGraphTest.testComplexDSLPattern` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 327 ⚑ |
| `StreamKmpGraphTest.testRepeat` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 366 ⚑ |
| `StreamKmpGraphTest.testGreedyStar` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 401 ⚑ |
| `StreamKmpGraphTest.testGreedyStarAtEnd` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 440 ⚑ |
| `StreamKmpGraphTest.testStreamingMatchCapture` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 459 ⚑ |
| `StreamKmpGraphTest.testAdvancedGroupCapture` | `StreamKmpGraphTest` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraphTest.kt` |  | Unit |  | 505 ⚑ |
| `StreamRealTimeSplitTest.setup` | `StreamRealTimeSplitTest` | `com.ai.assistance.operit.util.stream` | `StreamRealTimeSplitTest.kt` |  | Unit |  | 18 ⚑ |
| `StreamRealTimeSplitTest.generateLargeTestText` | `StreamRealTimeSplitTest` | `com.ai.assistance.operit.util.stream` | `StreamRealTimeSplitTest.kt` | sizeMultiplier: Int? | String | 生成混合内容的大文本 包含扁平的XML块和普通文本，重复多次以创建足够大的数据量 | 29 ⚑ |
| `StreamRealTimeSplitTest.testRealTimeSplitByProcessing` | `StreamRealTimeSplitTest` | `com.ai.assistance.operit.util.stream` | `StreamRealTimeSplitTest.kt` |  | Unit | 测试splitBy对大文本的实时流式处理能力 通过打印发送和接收的时间戳和内容，验证处理是否同步流式进行 | 53 ⚑ |
| `StreamRealTimeSplitTest.testRealTimeSplitByWithSlowProducer` | `StreamRealTimeSplitTest` | `com.ai.assistance.operit.util.stream` | `StreamRealTimeSplitTest.kt` |  | Unit | 测试在发送方添加延迟的情况下，是否仍然保持流式处理 这有助于更清晰地观察流式处理的行为 | 145 ⚑ |
| `StreamSplitByTest.setup` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` |  | Unit |  | 21 ⚑ |
| `StreamSplitByTest.testSplitByWithXmlPlugin` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` |  | Unit |  | 26 ⚑ |
| `StreamSplitByTest.testSplitByWithMultipleXmlTags` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` |  | Unit |  | 62 ⚑ |
| `StreamSplitByTest.testSplitByWithIncompleteXml` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` |  | Unit |  | 98 ⚑ |
| `StreamSplitByTest.testSplitByWithNestedLikeTags` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` |  | Unit |  | 130 ⚑ |
| `StreamSplitByTest.testSplitByWithEmptyInput` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` |  | Unit |  | 157 ⚑ |
| `StreamSplitByTest.testSplitByWithOnlyText` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` |  | Unit |  | 173 ⚑ |
| `StreamSplitByTest.testSplitByWithNestedContentForReadme` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` |  | Unit |  | 199 ⚑ |
| `StreamSplitByTest.testSplitByWithEmojiTrigger` | `StreamSplitByTest` | `com.ai.assistance.operit.util.stream` | `StreamSplitByTest.kt` |  | Unit |  | 227 ⚑ |
| `asCharStream` | — | `com.ai.assistance.operit.util.stream` | `StreamTestExtensions.kt` |  | Stream<Char> | 测试用扩展函数：将字符串转换为字符流 | 6 ⚑ |
| `MutableSharedStream.emit` | `MutableSharedStream` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | value: T | Unit | 发射一个值到Stream | 27 |
| `MutableSharedStream.tryEmit` | `MutableSharedStream` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | value: T | Boolean | 尝试发射一个值，如果缓冲区已满返回false | 30 |
| `MutableSharedStream.resetReplayCache` | `MutableSharedStream` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` |  | Unit | 重置重放缓存 | 33 |
| `MutableStateStream.compareAndSet` | `MutableStateStream` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | expect: T<br>update: T | Boolean | 比较并设置值 | 48 |
| `MutableSharedStreamImpl.lock` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` |  | Unit |  | 90 |
| `MutableSharedStreamImpl.unlock` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` |  | Unit |  | 95 |
| `MutableSharedStreamImpl.clearBuffer` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` |  | Unit |  | 100 |
| `MutableSharedStreamImpl.emit` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | value: T | Unit |  | 114 |
| `MutableSharedStreamImpl.tryEmit` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | value: T | Boolean |  | 130 |
| `MutableSharedStreamImpl.resetReplayCache` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` |  | Unit |  | 146 |
| `MutableSharedStreamImpl.close` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | cause: Throwable?? | Unit |  | 152 |
| `MutableSharedStreamImpl.collect` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | collector: StreamCollector<T> | Unit |  | 169 |
| `MutableSharedStreamImpl.appendToReplayBufferLocked` | `MutableSharedStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | value: T | Unit |  | 227 |
| `MutableStateStreamImpl.lock` | `MutableStateStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` |  | Unit |  | 246 |
| `MutableStateStreamImpl.unlock` | `MutableStateStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` |  | Unit |  | 251 |
| `MutableStateStreamImpl.clearBuffer` | `MutableStateStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` |  | Unit |  | 256 |
| `MutableStateStreamImpl.emit` | `MutableStateStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | value: T | Unit |  | 276 |
| `MutableStateStreamImpl.tryEmit` | `MutableStateStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | value: T | Boolean |  | 280 |
| `MutableStateStreamImpl.resetReplayCache` | `MutableStateStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` |  | Unit |  | 284 |
| `MutableStateStreamImpl.compareAndSet` | `MutableStateStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | expect: T<br>update: T | Boolean |  | 288 |
| `MutableStateStreamImpl.collect` | `MutableStateStreamImpl` | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | collector: StreamCollector<T> | Unit |  | 292 |
| `MutableSharedStream` | — | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | replay: Int?<br>extraBufferCapacity: Int?<br>onBufferOverflow: BufferOverflow?<br>context: CoroutineContext?<br>propagateCompletionCause: Boolean? | MutableSharedStream<T> | 创建一个MutableSharedStream | 298 |
| `MutableStateStream` | — | `com.ai.assistance.operit.util.stream` | `HotStream.kt` | initialValue: T | MutableStateStream<T> | 创建一个MutableStateStream | 314 |
| `shiftedBy` | — | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | offset: Int | TextStreamEvent | Moves an event recorded in a single request's coordinate space into the coordinate space … | 35 |
| `RevisableTextStream.lock` | `RevisableTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` |  | Unit |  | 70 |
| `RevisableTextStream.unlock` | `RevisableTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` |  | Unit |  | 74 |
| `RevisableTextStream.clearBuffer` | `RevisableTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` |  | Unit |  | 78 |
| `RevisableTextStream.collect` | `RevisableTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | collector: StreamCollector<String> | Unit |  | 82 |
| `DelegatingRevisableSharedTextStream.lock` | `DelegatingRevisableSharedTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` |  | Unit |  | 106 |
| `DelegatingRevisableSharedTextStream.unlock` | `DelegatingRevisableSharedTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` |  | Unit |  | 110 |
| `DelegatingRevisableSharedTextStream.clearBuffer` | `DelegatingRevisableSharedTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` |  | Unit |  | 114 |
| `DelegatingRevisableSharedTextStream.collect` | `DelegatingRevisableSharedTextStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | collector: StreamCollector<String> | Unit |  | 118 |
| `DelegatingRevisableCharStream.lock` | `DelegatingRevisableCharStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` |  | Unit |  | 133 |
| `DelegatingRevisableCharStream.unlock` | `DelegatingRevisableCharStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` |  | Unit |  | 137 |
| `DelegatingRevisableCharStream.clearBuffer` | `DelegatingRevisableCharStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` |  | Unit |  | 141 |
| `DelegatingRevisableCharStream.collect` | `DelegatingRevisableCharStream` | `com.ai.assistance.operit.util.stream` | `RevisableTextStream.kt` | collector: StreamCollector<Char> | Unit |  | 145 |
| `applyRevisionEvents` | — | `com.ai.assistance.operit.util.stream` | `RevisionAppliedText.kt` | rawContent: String<br>events: List<TextStreamEvent> | String | Removes every discarded attempt from [rawContent]. | 35 |
| `forwardEvent` | — | `com.ai.assistance.operit.util.stream` | `RevisionEventRelay.kt` | event: TextStreamEvent | Unit |  | 42 |
| `StreamLogger.setEnabled` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | enabled: Boolean | Unit | 启用或禁用日志 | 21 |
| `StreamLogger.setVerboseEnabled` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | enabled: Boolean | Unit | 启用或禁用详细日志 | 26 |
| `StreamLogger.d` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | component: String<br>message: String | Unit | 记录调试信息 | 31 |
| `StreamLogger.i` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | component: String<br>message: String | Unit | 记录信息 | 38 |
| `StreamLogger.v` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | component: String<br>message: String | Unit | 记录详细信息 | 45 |
| `StreamLogger.w` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | component: String<br>message: String | Unit | 记录警告 | 52 |
| `StreamLogger.e` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | component: String<br>message: String<br>throwable: Throwable?? | Unit | 记录错误 | 59 |
| `Stream.lock` | `Stream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` |  | Unit | 锁定流 - 暂停接收新数据但继续发送 | 79 |
| `Stream.unlock` | `Stream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` |  | Unit | 解锁流 - 恢复接收并发送缓存的数据 | 82 |
| `Stream.clearBuffer` | `Stream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` |  | Unit | 清空缓存的数据 | 85 |
| `Stream.collect` | `Stream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | collector: StreamCollector<T> | Unit | 收集Stream发出的值 | 88 |
| `Stream.collect` | `Stream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | onEach: suspend (T) -> Unit | Unit | Stream的标准收集方法，简化使用 | 91 |
| `Stream.emit` | `Stream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | value: T | Unit |  | 94 |
| `StreamCollector.emit` | `StreamCollector` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | value: T | Unit | 发射一个值到Stream | 106 |
| `AbstractStream.lock` | `AbstractStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` |  | Unit |  | 119 |
| `AbstractStream.unlock` | `AbstractStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` |  | Unit |  | 130 |
| `AbstractStream.clearBuffer` | `AbstractStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` |  | Unit |  | 156 |
| `AbstractStream.tryBuffer` | `AbstractStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | value: T | Boolean | 当流被锁定时，将值存入缓冲区 | 163 |
| `AbstractStream.emitBufferedItem` | `AbstractStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | item: T | Unit | 在流解锁时处理缓冲区中的项目 | 173 |
| `AbstractStream.markClosed` | `AbstractStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` |  | Unit | 标记流已关闭，此方法应在流完成或发生错误时调用 如果流处于锁定状态，此方法将允许处理缓冲区数据 | 179 |
| `AbstractStream.isClosed` | `AbstractStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` |  | Boolean | 检查流是否已关闭 | 187 |
| `FlowAsStream.collect` | `FlowAsStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | collector: StreamCollector<T> | Unit |  | 194 |
| `FlowAsStream.emitBufferedItem` | `FlowAsStream` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | item: T | Unit |  | 221 |
| `StreamAsFlow.collect` | `StreamAsFlow` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | collector: FlowCollector<T> | Unit |  | 229 |
| `emptyStream` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` |  | Stream<T> | 创建一个空的Stream | 9 |
| `collect` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | collector: StreamCollector<T> | Unit |  | 10 |
| `emitBufferedItem` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | item: T | Unit |  | 15 |
| `streamOf` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | value: T | Stream<T> | 从单个值创建Stream | 23 |
| `collect` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | collector: StreamCollector<T> | Unit |  | 26 |
| `emitBufferedItem` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | item: T | Unit |  | 34 |
| `streamOf` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | values: T | Stream<T> | 从多个值创建Stream | 42 |
| `collect` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | collector: StreamCollector<T> | Unit |  | 45 |
| `emitBufferedItem` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | item: T | Unit |  | 56 |
| `collect` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | collector: StreamCollector<T> | Unit |  | 67 |
| `emitBufferedItem` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | item: T | Unit |  | 79 |
| `collect` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | collector: StreamCollector<T> | Unit |  | 90 |
| `emitBufferedItem` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | item: T | Unit |  | 104 |
| `stream` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | block: suspend StreamCollector<T>.() -> Un… | Stream<T> | 通过调用构建器创建Stream | 112 |
| `emit` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | value: T | Unit |  | 115 |
| `collect` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | collector: StreamCollector<T> | Unit |  | 122 |
| `emitBufferedItem` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | item: T | Unit |  | 150 |
| `intervalStream` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | period: Duration<br>initialDelay: Duration? | Stream<Long> | 创建固定间隔发射整数的Stream | 159 |
| `rangeStream` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | start: Int<br>count: Int | Stream<Int> | 创建固定次数的Stream | 173 |
| `streamError` | — | `com.ai.assistance.operit.util.stream` | `StreamBuilders.kt` | exception: Throwable | Stream<T> | 从异常创建Stream | 185 |
| `StreamProcessor.process` | `StreamProcessor` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | stream: Stream<T> | R | 处理流数据 | 18 |
| `CompositeStreamProcessor.process` | `CompositeStreamProcessor` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | stream: Stream<T> | R |  | 30 |
| `CompositeStreamProcessor.compose` | `CompositeStreamProcessor` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | processors: StreamProcessor<T, *><br>final: StreamProcessor<T, R> | CompositeStreamProcessor<T, R> | 构建复合处理器的工厂方法 | 39 |
| `StreamGroup.collect` | `StreamGroup` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | collector: suspend (String) -> Unit | Unit | 收集这个组的流数据 | 67 |
| `StreamGroup.collect` | `StreamGroup` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | collector: StreamCollector<String> | Unit | 使用StreamCollector收集这个组的流数据 | 80 |
| `StreamGroup.addChild` | `StreamGroup` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | child: StreamGroup<*> | StreamGroup<TAG> | 添加子分组 | 90 |
| `StreamGroup.processRecursively` | `StreamGroup` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | action: suspend (StreamGroup<*>) -> Unit | Unit | 递归处理当前组和所有子组 | 99 |
| `StreamGroup.processWithBoundProcessor` | `StreamGroup` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` |  | R? | 使用绑定的处理器处理这个流 | 108 |
| `StreamGroup.toPair` | `StreamGroup` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` |  | Pair<TAG, Stream<String>> | 将这个流组转换为标签和流的Pair | 116 |
| `StreamGroup.toString` | `StreamGroup` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` |  | String |  | 118 |
| `StreamGroupBuilder.tag` | `StreamGroupBuilder` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | tag: TAG | StreamGroupBuilder<TAG> | 设置组的标签 | 129 |
| `StreamGroupBuilder.stream` | `StreamGroupBuilder` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | stream: Stream<String> | StreamGroupBuilder<TAG> | 设置组的数据流 | 135 |
| `StreamGroupBuilder.processor` | `StreamGroupBuilder` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | processor: StreamProcessor<String, *> | StreamGroupBuilder<TAG> | 设置组的处理器 | 141 |
| `StreamGroupBuilder.addChild` | `StreamGroupBuilder` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | child: StreamGroup<*> | StreamGroupBuilder<TAG> | 添加子组 | 147 |
| `StreamGroupBuilder.child` | `StreamGroupBuilder` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | init: StreamGroupBuilder<CHILD_TAG>.() ->… | StreamGroupBuilder<TAG> | 使用嵌套构建器添加子组 | 153 |
| `StreamGroupBuilder.build` | `StreamGroupBuilder` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | context: Context?? | StreamGroup<TAG> | 根据配置构建StreamGroup | 164 |
| `streamGroup` | — | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | init: StreamGroupBuilder<TAG>.() -> Unit | StreamGroup<TAG> | 创建StreamGroup的便捷扩展函数 | 182 |
| `StreamInterceptor.setOnEach` | `StreamInterceptor` | `com.ai.assistance.operit.util.stream` | `StreamGroup.kt` | onEach: (T) -> R | Unit |  | 219 |
| `KmpCondition.matches` | `KmpCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean | 检查给定字符是否匹配此条件 | 6 |
| `KmpCondition.getDescription` | `KmpCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String | 获取此条件的描述（用于调试） | 9 |
| `KmpCondition.plus` | `KmpCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | other: KmpCondition | KmpCondition | 与另一个条件进行OR组合 | 12 |
| `KmpCondition.times` | `KmpCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | other: KmpCondition | KmpCondition | 与另一个条件进行AND组合 | 15 |
| `KmpCondition.not` | `KmpCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | KmpCondition | 对此条件取反 | 18 |
| `KmpCondition.toRegexPattern` | `KmpCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String | 转换为等效的正则表达式模式字符串 | 21 |
| `CharCondition.matches` | `CharCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean |  | 26 |
| `CharCondition.getDescription` | `CharCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 27 |
| `CharCondition.toRegexPattern` | `CharCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 28 |
| `CharRangeCondition.matches` | `CharRangeCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean |  | 37 |
| `CharRangeCondition.getDescription` | `CharRangeCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 38 |
| `CharRangeCondition.toRegexPattern` | `CharRangeCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 39 |
| `CharSetCondition.matches` | `CharSetCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean |  | 46 |
| `CharSetCondition.getDescription` | `CharSetCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 47 |
| `CharSetCondition.toRegexPattern` | `CharSetCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 48 |
| `NotCondition.matches` | `NotCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean |  | 59 |
| `NotCondition.getDescription` | `NotCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 60 |
| `NotCondition.toRegexPattern` | `NotCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 61 |
| `OrCondition.matches` | `OrCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean |  | 80 |
| `OrCondition.getDescription` | `OrCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 81 |
| `OrCondition.toRegexPattern` | `OrCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 83 |
| `AndCondition.matches` | `AndCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean |  | 91 |
| `AndCondition.getDescription` | `AndCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 92 |
| `AndCondition.toRegexPattern` | `AndCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 94 |
| `PredicateCondition.matches` | `PredicateCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean |  | 103 |
| `PredicateCondition.getDescription` | `PredicateCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 104 |
| `PredicateCondition.toRegexPattern` | `PredicateCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 105 |
| `GreedyStarCondition.matches` | `GreedyStarCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean |  | 125 |
| `GreedyStarCondition.getDescription` | `GreedyStarCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 126 |
| `GreedyStarCondition.toRegexPattern` | `GreedyStarCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 127 |
| `GroupCondition.matches` | `GroupCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Boolean |  | 132 |
| `GroupCondition.getDescription` | `GroupCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 137 |
| `GroupCondition.toRegexPattern` | `GroupCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String |  | 138 |
| `GroupCondition.getAllGroupIds` | `GroupCondition` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | List<Int> |  | 141 |
| `KmpNode.addTransition` | `KmpNode` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | condition: KmpCondition<br>targetNode: KmpNode | Unit | 添加从此节点到另一个节点的转换 | 163 |
| `KmpNode.getNextNode` | `KmpNode` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | KmpNode? | 基于输入字符查找下一个节点 | 168 |
| `KmpNode.getTransitions` | `KmpNode` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Map<KmpCondition, KmpNode> | 获取此节点的所有出站转换 | 178 |
| `KmpNodeChangeListener.onNodeChanged` | `KmpNodeChangeListener` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | previousNode: KmpNode<br>currentNode: KmpNode<br>triggeredChar: Char | Unit | 当当前节点发生变化时调用 | 189 |
| `StreamKmpGraph.addNodeChangeListener` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | listener: KmpNodeChangeListener | Unit | 添加节点变化监听器 | 209 |
| `StreamKmpGraph.removeNodeChangeListener` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | listener: KmpNodeChangeListener | Unit | 移除节点变化监听器 | 214 |
| `StreamKmpGraph.notifyNodeChanged` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | previousNode: KmpNode<br>currentNode: KmpNode<br>triggeredChar: Char | Unit | 通知所有监听器节点变化 | 219 |
| `StreamKmpGraph.createNode` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | depth: Int<br>isFinal: Boolean? | KmpNode | 在图中创建新节点 | 230 |
| `StreamKmpGraph.addTransition` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | fromNode: KmpNode<br>toNode: KmpNode<br>condition: KmpCondition | Unit | 添加两个节点之间的转换 | 237 |
| `StreamKmpGraph.setFailure` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | node: KmpNode<br>failureNode: KmpNode | Unit | 设置节点的失败转换 | 242 |
| `StreamKmpGraph.processChar` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | StreamKmpMatchResult | 处理单个字符并更新当前状态 | 247 |
| `StreamKmpGraph.performRegexMatchingIfNeeded` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | isFullMatch: Boolean | StreamKmpMatchResult | 在KMP匹配成功后使用正则表达式进行二次匹配以提取捕获组 | 292 |
| `StreamKmpGraph.processText` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | text: String | List<Int> | 处理一串字符 | 325 |
| `StreamKmpGraph.reset` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 重置图到初始状态 | 341 |
| `StreamKmpGraph.getCurrentNode` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | KmpNode | 获取当前状态节点 | 348 |
| `StreamKmpGraph.getStartNode` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | KmpNode | 获取起始节点 | 351 |
| `StreamKmpGraph.getNodes` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | List<KmpNode> | 获取图中的所有节点 | 354 |
| `StreamKmpGraph.findMatches` | `StreamKmpGraph` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | text: String | List<String> | 查找并返回文本中所有匹配的子字符串。 此方法会处理整个文本并返回一个包含所有非重叠匹配项的列表。 | 362 |
| `StreamKmpGraphBuilder.build` | `StreamKmpGraphBuilder` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | pattern: KmpPattern | StreamKmpGraph |  | 415 |
| `StreamKmpGraphBuilder.buildRecursive` | `StreamKmpGraphBuilder` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | graph: StreamKmpGraph<br>startNode: KmpNode<br>conditions: List<KmpCondition><br>depth: Int | Pair<KmpNode, Int> |  | 425 |
| `StreamKmpGraphBuilder.setupFailureTransitions` | `StreamKmpGraphBuilder` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | graph: StreamKmpGraph | Unit | 设置图的失败转换（简化版） | 476 |
| `KmpPattern.add` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | condition: KmpCondition<br>isTopLevel: Boolean? | Unit | 添加一个匹配条件 | 498 |
| `KmpPattern.add` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | condition: KmpCondition | Unit | 添加一个匹配条件 | 506 |
| `KmpPattern.group` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | id: Int<br>builder: KmpPattern.() -> Unit | Unit | 定义一个捕获组 | 511 |
| `KmpPattern.toRegexPattern` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | String | 将模式转换为等效的正则表达式 | 518 |
| `KmpPattern.char` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Unit | 添加一个字符匹配条件 | 523 |
| `KmpPattern.charIgnoreCase` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Unit | 添加一个忽略大小写的字符匹配条件 | 528 |
| `KmpPattern.range` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | from: Char<br>to: Char | Unit | 添加一个字符范围匹配条件 | 533 |
| `KmpPattern.anyOf` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | chars: Char | Unit | 添加一个字符集匹配条件 | 538 |
| `KmpPattern.notChar` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | c: Char | Unit | 添加一个不匹配指定字符的条件 | 543 |
| `KmpPattern.noneOf` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | chars: Char | Unit | 添加一个不匹配指定字符集的条件 | 548 |
| `KmpPattern.notInRange` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | from: Char<br>to: Char | Unit | 添加一个不匹配指定范围的条件 | 553 |
| `KmpPattern.predicate` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | description: String<br>predicate: (Char) -> Boolean | Unit | 添加一个自定义匹配条件 | 558 |
| `KmpPattern.digit` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 添加一个数字匹配条件 | 563 |
| `KmpPattern.notDigit` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 添加一个非数字匹配条件 | 568 |
| `KmpPattern.letter` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 添加一个字母匹配条件 | 573 |
| `KmpPattern.notLetter` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 添加一个非字母匹配条件 | 578 |
| `KmpPattern.letterOrDigit` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 添加一个字母或数字匹配条件 | 583 |
| `KmpPattern.notLetterOrDigit` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 添加一个非字母非数字匹配条件 | 588 |
| `KmpPattern.whitespace` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 添加一个空白字符匹配条件 | 593 |
| `KmpPattern.notWhitespace` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 添加一个非空白字符匹配条件 | 598 |
| `KmpPattern.any` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | Unit | 添加任意字符匹配条件（通配符） | 603 |
| `KmpPattern.literal` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | sequence: CharSequence | Unit | Adds a literal string to the pattern by converting each character into a CharCondition. | 611 |
| `KmpPattern.greedyStar` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | conditionBuilder: KmpPattern.() -> Unit | Unit | 添加一个贪心匹配（*），匹配零个或多个满足条件的字符。 这将尽可能多地匹配字符。 注意：为了避免歧义，循环条件会自动排除掉紧随其后的第一个非贪心匹配条件。 | 621 |
| `KmpPattern.repeat` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | count: Int<br>builder: KmpPattern.() -> Unit | Unit | 重复一个模式指定的次数。 | 640 |
| `KmpPattern.not` | `KmpPattern` | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | condition: KmpCondition | Unit | 添加对条件的反向匹配 | 650 |
| `unaryPlus` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` |  | KmpCondition | 扩展函数，简化单个字符匹配条件的创建 | 656 |
| `or` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | other: Char | KmpCondition | 忽略大小写的字符匹配 | 672 |
| `to` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | other: Char | KmpCondition | 字符范围匹配 | 675 |
| `chars` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | chars: Char | KmpCondition | 字符集匹配 | 678 |
| `notChars` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | chars: Char | KmpCondition | 字符集不匹配 | 681 |
| `notInRange` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | from: Char<br>to: Char | KmpCondition | 不在字符范围内 | 684 |
| `not` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | condition: KmpCondition | KmpCondition | 自由函数形式的否定 | 687 |
| `kmpPattern` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | init: KmpPattern.() -> Unit | KmpPattern | DSL构建器 | 690 |
| `lock` | — | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` |  | Unit | 实现Stream接口必须的方法 | 238 |
| `unlock` | — | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` |  | Unit |  | 239 |
| `clearBuffer` | — | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` |  | Unit |  | 240 |
| `collect` | — | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` | collector: StreamCollector<StreamGroup<StreamP… | Unit |  | 242 |
| `openDefaultChannel` | — | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` |  | Unit |  | 273 |
| `closeDefaultChannel` | — | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` |  | Unit |  | 283 |
| `openPluginChannel` | — | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` | plugin: StreamPlugin | Unit |  | 288 |
| `closePluginChannel` | — | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` |  | Unit |  | 296 |
| `collect` | — | `com.ai.assistance.operit.util.stream` | `StreamOperators.kt` | collector: StreamCollector<String> | Unit |  | 472 |
| `stream` | — | `com.ai.assistance.operit.util.stream` | `StringExtensions.kt` |  | Stream<Char> | 将字符串转换为字符流 用于在MarkdownTextComposable中将普通字符串转换为所需的字符流 | 4 |
| `TextStreamRevisionTracker.append` | `TextStreamRevisionTracker` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTracker.kt` | chunk: String | SmartString |  | 30 |
| `TextStreamRevisionTracker.savepoint` | `TextStreamRevisionTracker` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTracker.kt` | id: String<br>contentLength: Int | Unit | Registers a savepoint at [contentLength], the raw offset the producer recorded when it em… | 48 |
| `TextStreamRevisionTracker.rollback` | `TextStreamRevisionTracker` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTracker.kt` | id: String<br>contentLength: Int<br>discardedLength: Int | SmartString? | Removes the attempt recorded for [id]. [contentLength] is the raw offset where the attemp… | 61 |
| `TextStreamRevisionTracker.replace` | `TextStreamRevisionTracker` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTracker.kt` | content: String | Unit |  | 72 |
| `TextStreamRevisionTracker.applyEventHistory` | `TextStreamRevisionTracker` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTracker.kt` | events: List<TextStreamEvent> | SmartString | Recomputes the visible text from every chunk received so far and the complete [events] hi… | 88 |
| `TextStreamRevisionTracker.rebuildVisibleContent` | `TextStreamRevisionTracker` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTracker.kt` |  | Unit |  | 102 |
| `HotStreamTest.disableAndroidSystemLogForJvmTests` | `HotStreamTest` | `com.ai.assistance.operit.util.stream` | `HotStreamTest.kt` |  | Unit |  | 22 ⚑ |
| `HotStreamTest.restoreAndroidSystemLog` | `HotStreamTest` | `com.ai.assistance.operit.util.stream` | `HotStreamTest.kt` |  | Unit |  | 28 ⚑ |
| `HotStreamTest.shareForwardsUpstreamFailureAfterReplayingPartialContent` | `HotStreamTest` | `com.ai.assistance.operit.util.stream` | `HotStreamTest.kt` |  | Unit |  | 33 ⚑ |
| `HotStreamTest.shareCanRecordUpstreamFailureWithoutFailingObservers` | `HotStreamTest` | `com.ai.assistance.operit.util.stream` | `HotStreamTest.kt` |  | Unit |  | 59 ⚑ |
| `RevisionAppliedTextTest.disableAndroidSystemLogForJvmTests` | `RevisionAppliedTextTest` | `com.ai.assistance.operit.util.stream` | `RevisionAppliedTextTest.kt` |  | Unit |  | 15 ⚑ |
| `RevisionAppliedTextTest.restoreAndroidSystemLog` | `RevisionAppliedTextTest` | `com.ai.assistance.operit.util.stream` | `RevisionAppliedTextTest.kt` |  | Unit |  | 21 ⚑ |
| `RevisionAppliedTextTest.plainStreamWithoutEventsIsConcatenated` | `RevisionAppliedTextTest` | `com.ai.assistance.operit.util.stream` | `RevisionAppliedTextTest.kt` |  | Unit |  | 26 ⚑ |
| `RevisionAppliedTextTest.rollbackRemovesTheAbortedAttemptFromTheCollectedText` | `RevisionAppliedTextTest` | `com.ai.assistance.operit.util.stream` | `RevisionAppliedTextTest.kt` |  | Unit |  | 35 ⚑ |
| `RevisionAppliedTextTest.rollbackKeepsTextProducedBeforeTheSavepoint` | `RevisionAppliedTextTest` | `com.ai.assistance.operit.util.stream` | `RevisionAppliedTextTest.kt` |  | Unit |  | 56 ⚑ |
| `RevisionAppliedTextTest.collectForwardsEveryChunk` | `RevisionAppliedTextTest` | `com.ai.assistance.operit.util.stream` | `RevisionAppliedTextTest.kt` |  | Unit |  | 75 ⚑ |
| `RevisionAppliedTextTest.rollbackOfALaterRoundKeepsEarlierRounds` | `RevisionAppliedTextTest` | `com.ai.assistance.operit.util.stream` | `RevisionAppliedTextTest.kt` |  | Unit | One response can contain several provider requests, and each provider numbers its revisio… | 105 ⚑ |
| `RevisionAppliedTextTest.shiftedByMovesBothEventCoordinates` | `RevisionAppliedTextTest` | `com.ai.assistance.operit.util.stream` | `RevisionAppliedTextTest.kt` |  | Unit |  | 135 ⚑ |
| `RevisionEventRelayTest.disableAndroidSystemLogForJvmTests` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` |  | Unit |  | 24 ⚑ |
| `RevisionEventRelayTest.restoreAndroidSystemLog` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` |  | Unit |  | 30 ⚑ |
| `RevisionEventRelayTest.queuedFinalRollbackIsForwardedBeforeCompletionOnOneDispatcher` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` |  | Unit |  | 35 ⚑ |
| `RevisionEventRelayTest.livePrefixAndQueuedLaterRoundEventsAreShiftedOnceInOrder` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` |  | Unit |  | 76 ⚑ |
| `RevisionEventRelayTest.textFailureDrainsQueuedEventsAndPropagatesOriginalFailure` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` |  | Unit |  | 145 ⚑ |
| `RevisionEventRelayTest.cancellationDrainsProviderFinalizerEventsAndRemovesSubscription` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` |  | Unit |  | 179 ⚑ |
| `RevisionEventRelayTest.liveRelayFailurePropagatesWithoutReemittingItsDeliveredEvents` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` |  | Unit |  | 227 ⚑ |
| `RevisionEventRelayTest.eventChannelCancellationPropagatesAndStillFinalizesRound` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` |  | Unit |  | 262 ⚑ |
| `RevisionEventRelayTest.plainTextStreamForwardsChunksAndFinalizesContent` | `RevisionEventRelayTest` | `com.ai.assistance.operit.util.stream` | `RevisionEventRelayTest.kt` |  | Unit |  | 293 ⚑ |
| `TextStreamRevisionTrackerTest.appendReturnsSharedSmartString` | `TextStreamRevisionTrackerTest` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTrackerTest.kt` |  | Unit |  | 10 ⚑ |
| `TextStreamRevisionTrackerTest.rollbackTruncatesToSavedLength` | `TextStreamRevisionTrackerTest` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTrackerTest.kt` |  | Unit |  | 21 ⚑ |
| `TextStreamRevisionTrackerTest.rollbackInvalidatesSavepointsInDiscardedSuffix` | `TextStreamRevisionTrackerTest` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTrackerTest.kt` |  | Unit |  | 34 ⚑ |
| `TextStreamRevisionTrackerTest.rollbackUsesProducerOffsetWhenConsumerAlreadyAppendedDiscardedChunks` | `TextStreamRevisionTrackerTest` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTrackerTest.kt` |  | Unit | Regression for the HTTP/API truncation of issue #1375. The event channel and the text cha… | 57 ⚑ |
| `TextStreamRevisionTrackerTest.rollbackKeepsContentThatPrecedesTheProducerOffset` | `TextStreamRevisionTrackerTest` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTrackerTest.kt` |  | Unit |  | 75 ⚑ |
| `TextStreamRevisionTrackerTest.rollbackBeforeDiscardedChunksArriveDropsThemAsTheyArrive` | `TextStreamRevisionTrackerTest` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTrackerTest.kt` |  | Unit |  | 93 ⚑ |
| `TextStreamRevisionTrackerTest.rollbackAfterRetriedChunksArriveKeepsOnlyTheDiscardedRange` | `TextStreamRevisionTrackerTest` | `com.ai.assistance.operit.util.stream` | `TextStreamRevisionTrackerTest.kt` |  | Unit |  | 105 ⚑ |
| `ToolTagStreamParsingTest.disableAndroidSystemLogForJvmTests` | `ToolTagStreamParsingTest` | `com.ai.assistance.operit.util.stream` | `ToolTagStreamParsingTest.kt` |  | Unit |  | 27 ⚑ |
| `ToolTagStreamParsingTest.restoreAndroidSystemLog` | `ToolTagStreamParsingTest` | `com.ai.assistance.operit.util.stream` | `ToolTagStreamParsingTest.kt` |  | Unit |  | 33 ⚑ |
| `ToolTagStreamParsingTest.everyTwoChunkSplitKeepsToolBlockIntact` | `ToolTagStreamParsingTest` | `com.ai.assistance.operit.util.stream` | `ToolTagStreamParsingTest.kt` |  | Unit |  | 46 ⚑ |
| `ToolTagStreamParsingTest.everySingleCharacterSplitKeepsToolBlockIntact` | `ToolTagStreamParsingTest` | `com.ai.assistance.operit.util.stream` | `ToolTagStreamParsingTest.kt` |  | Unit |  | 54 ⚑ |
| `ToolTagStreamParsingTest.toolTagSplitAcrossManySmallChunksKeepsToolBlockIntact` | `ToolTagStreamParsingTest` | `com.ai.assistance.operit.util.stream` | `ToolTagStreamParsingTest.kt` |  | Unit |  | 60 ⚑ |
| `ToolTagStreamParsingTest.assertParsed` | `ToolTagStreamParsingTest` | `com.ai.assistance.operit.util.stream` | `ToolTagStreamParsingTest.kt` | chunks: List<String><br>splitPosition: Int | Unit |  | 68 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ALPHANUMERIC` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | KmpCondition |  | 661 |
| `ANY_CHAR` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | KmpCondition |  | 663 |
| `DIGITS` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | KmpCondition | 扩展属性，用于常见字符组 | 659 |
| `LETTERS` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | KmpCondition |  | 660 |
| `NOT_ALPHANUMERIC` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | KmpCondition |  | 668 |
| `NOT_DIGITS` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | KmpCondition | 反向的预定义条件 | 666 |
| `NOT_LETTERS` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | KmpCondition |  | 667 |
| `NOT_WHITESPACE` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | KmpCondition |  | 669 |
| `StreamLogger.enabled` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | inferred |  | 17 |
| `StreamLogger.TAG` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | inferred |  | 16 |
| `StreamLogger.verboseEnabled` | `StreamLogger` | `com.ai.assistance.operit.util.stream` | `Stream.kt` | inferred |  | 18 |
| `WHITESPACE` | — | `com.ai.assistance.operit.util.stream` | `StreamKmpGraph.kt` | KmpCondition |  | 662 |
