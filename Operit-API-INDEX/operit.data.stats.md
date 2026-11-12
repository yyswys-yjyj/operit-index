# operit.data.stats

> 函数 183 · 类型 51 · 顶层常量 14 · 共 248 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `JvmCursor` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | class JvmCursor(private val resultSet: ResultSet, private val closeable: AutoCloseable?) : Cursor | 最小 android.database.Cursor 实现：迁移路径只用到读取行与列。 | 194 |
| `JvmSupportSQLiteDatabase` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | class JvmSupportSQLiteDatabase(private val connection: Connection) : SupportSQLiteDatabase | 纯 JVM 的最小 [SupportSQLiteDatabase] 测试替身（基于 sqlite-jdbc）， 用于直接驱动生产 `Migration.migrate(Suppo… | 29 |
| `ModelPriceSettings` | `ModelPriceSettings` | `com.ai.assistance.operit.data.stats` | `TokenPriceResolver.kt` | class ModelPriceSettings(val billingMode: BillingMode?, val currency: PricingCurrency?, val inputPricePerMillion: Double?, val cachedInputPricePerMillion: Double?, val cacheWritePrice… |  | 7 |
| `PricingSource` | `PricingSource` | `com.ai.assistance.operit.data.stats` | `TokenStatTypes.kt` | class PricingSource | Price-resolution provenance kept for calculation tests and diagnostics. | 4 |
| `ProviderUsageNormalizer` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | object ProviderUsageNormalizer | provider 原始 usage → 阶段 1 契约的归一化（provider 适配层）。 语义事实： - OpenAI 兼容系：`prompt_tokens`/`comple… | 74 |
| `ProviderUsageNormalizerTest` | `ProviderUsageNormalizerTest` | `com.ai.assistance.operit.data.stats` | `ProviderUsageNormalizerTest.kt` | class ProviderUsageNormalizerTest | provider 原始 usage → 阶段 1 契约归一化测试。 语义要点： - 未知（缺失字段）→ null；确认 0 → 0（例如无缓存读取、无缓存写入）； - OpenA… | 21 |
| `ProviderUsageSnapshot` | `ProviderUsageSnapshot` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | class ProviderUsageSnapshot(val uncachedInputTokens: Long?, val cachedInputTokens: Long?, val cacheWriteTokens: Long?, val totalInputTokens: Long?, val outputTokens: Long?, val reasoning… | provider 适配层规范化后的 usage 快照（阶段 1 契约 + 诊断标签）。 - null 字段表示“未知”（provider 未提供），0 表示 provider 确… | 32 |
| `QuantileLevels` | `QuantileLevels` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | class QuantileLevels(private val thresholds: LongArray) |  | 124 |
| `ReleasedProviderModelKey` | `ReleasedProviderModelKey` | `com.ai.assistance.operit.data.stats` | `ReleasedProviderModelKeyDecoder.kt` | class ReleasedProviderModelKey(val storedProviderModel: String, val provider: String, val model: String) |  | 6 |
| `ReleasedProviderModelKeyDecoder` | `ReleasedProviderModelKeyDecoder` | `com.ai.assistance.operit.data.stats` | `ReleasedProviderModelKeyDecoder.kt` | object ReleasedProviderModelKeyDecoder | Decodes released `provider:model` keys stored as `provider_model`. | 13 |
| `ReleasedProviderModelKeyDecoderTest` | `ReleasedProviderModelKeyDecoderTest` | `com.ai.assistance.operit.data.stats` | `ReleasedProviderModelKeyDecoderTest.kt` | class ReleasedProviderModelKeyDecoderTest |  | 7 |
| `ResolvedTokenPricing` | `ResolvedTokenPricing` | `com.ai.assistance.operit.data.stats` | `TokenPriceResolver.kt` | class ResolvedTokenPricing(val billingMode: BillingMode, val currency: PricingCurrency, val inputPricePerMillion: Double, val cachedInputPricePerMillion: Double, val cacheWritePricePerM… |  | 51 |
| `TokenActivityAggregator` | `TokenActivityAggregator` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | object TokenActivityAggregator |  | 38 |
| `TokenActivityAggregatorTest` | `TokenActivityAggregatorTest` | `com.ai.assistance.operit.data.stats` | `TokenActivityAggregatorTest.kt` | class TokenActivityAggregatorTest |  | 8 |
| `TokenActivityDay` | `TokenActivityDay` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | class TokenActivityDay(val date: LocalDate, val tokens: Long, val level: Int) |  | 15 |
| `TokenActivityRangeData` | `TokenActivityRangeData` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | class TokenActivityRangeData(val daily: List<TokenActivityDay>, val weekly: List<TokenActivityWeek>, val cumulative: List<TokenActivityDay>, val stats: TokenActivityStats) |  | 31 |
| `TokenActivitySnapshot` | `TokenActivitySnapshot` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | class TokenActivitySnapshot(val zone: ZoneId, val dayTotals: Map<LocalDate, Long>) |  | 10 |
| `TokenActivityStats` | `TokenActivityStats` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | class TokenActivityStats(val totalTokens: Long, val peakTokens: Long, val currentStreak: Int, val longestStreak: Int) |  | 24 |
| `TokenActivityViewMode` | `TokenActivityViewMode` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | class TokenActivityViewMode |  | 8 |
| `TokenCostCalculator` | `TokenCostCalculator` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculator.kt` | object TokenCostCalculator |  | 7 |
| `TokenCostCalculatorTest` | `TokenCostCalculatorTest` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculatorTest.kt` | class TokenCostCalculatorTest |  | 9 |
| `TokenCostCurrency` | `TokenCostCurrency` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculator.kt` | object TokenCostCurrency |  | 78 |
| `TokenPriceResolver` | `TokenPriceResolver` | `com.ai.assistance.operit.data.stats` | `TokenPriceResolver.kt` | object TokenPriceResolver | Resolves only the current price: user setting first, then the built-in model table. | 63 |
| `TokenPriceSettingsSnapshot` | `TokenPriceSettingsSnapshot` | `com.ai.assistance.operit.data.stats` | `TokenPriceResolver.kt` | class TokenPriceSettingsSnapshot(val providerModels: Map<String, ModelPriceSetting…, val configs: Map<String, ModelPriceSetting…) |  | 26 |
| `TokenStatsAnnualSummary` | `TokenStatsAnnualSummary` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsAnnualSummary(val totals: TokenStatsTotals, val displayModels: List<TokenStatsDisplayModelBr…, val monthTotals: List<Long>, val dayTotals: Map<java.time.LocalDate, Long>) | 年度报告的 token 汇总：全年合计、按模型、按月和按本地日期。 | 79 |
| `TokenStatsCostSummary` | `TokenStatsCostSummary` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsCostSummary(val currency: PricingCurrency, val knownAmount: Double, val unknownContributionCount: Long, val totalContributionCount: Long, val rateUsed: Double, val origin… |  | 11 |
| `TokenStatsDisplayModelBreakdown` | `TokenStatsDisplayModelBreakdown` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsDisplayModelBreakdown(val displayModelId: String, val displayName: String, val normalizedModel: String, val totals: TokenStatsTotals, val identities: List<TokenStatsIdentityBreakd…… |  | 69 |
| `TokenStatsDisplayUnit` | `TokenStatsDisplayUnit` | `com.ai.assistance.operit.data.stats` | `TokenStatsDisplayUnit.kt` | class TokenStatsDisplayUnit |  | 5 |
| `TokenStatsDisplayUnitTest` | `TokenStatsDisplayUnitTest` | `com.ai.assistance.operit.data.stats` | `TokenStatsDisplayUnitTest.kt` | class TokenStatsDisplayUnitTest |  | 6 |
| `TokenStatsGranularity` | `TokenStatsGranularity` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | class TokenStatsGranularity | 图表桶粒度：10 分钟 / 1 小时 / 1 自然日（本地时区对齐）。 | 21 |
| `TokenStatsIdentityBreakdown` | `TokenStatsIdentityBreakdown` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsIdentityBreakdown(val configId: String, val provider: String, val model: String, val totals: TokenStatsTotals) |  | 62 |
| `TokenStatsLifetimeOverview` | `TokenStatsLifetimeOverview` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsLifetimeOverview(val totals: TokenStatsTotals, val displayModels: List<TokenStatsDisplayModelBr…) |  | 39 |
| `TokenStatsModelBucket` | `TokenStatsModelBucket` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsModelBucket(val requests: Long, val uncachedInput: Long, val cachedInput: Long, val output: Long, val totalTokens: Long, val totalTokensUnknownEventCount: Long, val unkno… |  | 51 |
| `TokenStatsPreferences` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` | class TokenStatsPreferences(context: Context) | Scalar statistics settings. Structured usage, grouping, and pricing stay in Room. | 18 |
| `TokenStatsPreferencesStore` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | class TokenStatsPreferencesStore(context: Context) : TokenStatsSettingsStore | Statistics-only Preferences implementation; structured data remains in Room. | 29 |
| `TokenStatsPriceDraft` | `TokenStatsPriceDraft` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | class TokenStatsPriceDraft(val scope: TokenStatsPriceScope, val provider: String, val model: String, val configId: String?, val billingMode: BillingMode, val currency: PricingCurrency, … |  | 12 |
| `TokenStatsPriceScope` | `TokenStatsPriceScope` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | class TokenStatsPriceScope |  | 10 |
| `TokenStatsPriceScopeTest` | `TokenStatsPriceScopeTest` | `com.ai.assistance.operit.data.stats` | `TokenStatsPriceScopeTest.kt` | class TokenStatsPriceScopeTest |  | 6 |
| `TokenStatsPriceSetting` | `TokenStatsPriceSetting` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | class TokenStatsPriceSetting(val scope: TokenStatsPriceScope, val providerModel: String, val provider: String, val model: String, val configId: String?, val billingMode: BillingMode, val … |  | 26 |
| `TokenStatsQueryParams` | `TokenStatsQueryParams` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsQueryParams(val targetCurrency: PricingCurrency, val manualRate: Double, val providerModels: Set<String>?) |  | 5 |
| `TokenStatsQueryService` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | object TokenStatsQueryService | SQL-backed statistics queries. Only aggregate rows leave Room. | 14 |
| `TokenStatsRangeData` | `TokenStatsRangeData` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsRangeData(val range: TokenStatsTimeRange, val granularity: TokenStatsGranularity, val eventCount: Long, val summary: TokenStatsTotals, val buckets: List<TokenStatsTrend… |  | 86 |
| `TokenStatsSettingsManager` | `TokenStatsSettingsManager` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | class TokenStatsSettingsManager(context: Context) |  | 41 |
| `TokenStatsSettingsStore` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | interface TokenStatsSettingsStore |  | 6 |
| `TokenStatsTimeRange` | `TokenStatsTimeRange` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | class TokenStatsTimeRange(val startMs: Long, val endMs: Long) | 时间范围，**半开区间** `[startMs, endMs)`：`startedAtMs == endMs` 的事件 不属于该范围；endMs 是下一边界（如次日 0 点），不… | 11 |
| `TokenStatsTimeRanges` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | object TokenStatsTimeRanges | 日历范围的图表桶对齐计算。 桶边界在**本地时间**上对齐（10 分钟整点、整点小时、自然日 0 点），并用 java.time 的 plusMinutes/plusHours/… | 35 |
| `TokenStatsTimeRangeTest` | `TokenStatsTimeRangeTest` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRangeTest.kt` | class TokenStatsTimeRangeTest | 日历范围及桶边界测试，覆盖 DST 和半开区间语义。 | 11 |
| `TokenStatsTokenAggregate` | `TokenStatsTokenAggregate` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsTokenAggregate(val knownSum: Long, val knownEventCount: Long, val unknownEventCount: Long, val totalEventCount: Long) |  | 20 |
| `TokenStatsTotals` | `TokenStatsTotals` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsTotals(val requests: Long, val uncachedInput: TokenStatsTokenAggregate, val cachedInput: TokenStatsTokenAggregate, val totalInput: TokenStatsTokenAggregate, val outp… |  | 29 |
| `TokenStatsTrendBucket` | `TokenStatsTrendBucket` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryModels.kt` | class TokenStatsTrendBucket(val bucketStartMs: Long, val bucketEndMs: Long, val totals: TokenStatsTotals, val byModel: Map<String, TokenStatsModelBu…) |  | 44 |
| `TokenUsageRepository` | `TokenUsageRepository` | `com.ai.assistance.operit.data.stats` | `TokenUsageRepository.kt` | class TokenUsageRepository(context: Context) | Room owner for successful formal-inference usage and pricing. | 15 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `ProviderUsageSnapshot.hasKnownFields` | `ProviderUsageSnapshot` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` |  | Boolean | 是否有任何已知用量分量（含明确 0；完全无已知字段才为 false）。 | 46 |
| `ProviderUsageNormalizer.openAiChatCompletions` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | usage: JSONObject?<br>completeSnapshot: Boolean? | ProviderUsageSnapshot? | OpenAI chat/completions 系（含 DeepSeek、Kimi、Qwen、Mistral 等兼容端点）。 单次上报即该 attempt 的完整最终 usage… | 86 |
| `ProviderUsageNormalizer.openAiResponses` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | usage: JSONObject?<br>completeSnapshot: Boolean? | ProviderUsageSnapshot? | OpenAI Responses API：`input_tokens_details.cached_tokens` + `output_tokens_details.reason… | 140 |
| `ProviderUsageNormalizer.anthropic` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | usage: JSONObject?<br>completeSnapshot: Boolean? | ProviderUsageSnapshot? | Anthropic Messages API。`input_tokens` 不含缓存分量（官方文档：总量 = input_tokens + cache_read_input_to… | 193 |
| `ProviderUsageNormalizer.gemini` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | usageMetadata: JSONObject?<br>completeSnapshot: Boolean? | ProviderUsageSnapshot? | Gemini：`usageMetadata`；`candidatesTokenCount` 为 response candidates token， `thoughtsToken… | 242 |
| `ProviderUsageNormalizer.local` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | uncachedInputTokens: Long<br>outputTokens: Long<br>source: String | ProviderUsageSnapshot | 本地模型（llama.cpp/MNN）：本地实测计数，缓存分量明确为 0；单次完整上报。 | 283 |
| `ProviderUsageNormalizer.toolPkg` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | input: Long?<br>cachedInput: Long?<br>output: Long?<br>completeSnapshot: Boolean | ProviderUsageSnapshot | ToolPkg JS provider：`input` 视为总量（含缓存命中），uncached 为差值。 [completeSnapshot] 由协议版本决定：新协议（携带 a… | 308 |
| `ProviderUsageNormalizer.sumNumericFields` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | jsonObject: JSONObject | Long |  | 334 |
| `ReleasedProviderModelKeyDecoder.decode` | `ReleasedProviderModelKeyDecoder` | `com.ai.assistance.operit.data.stats` | `ReleasedProviderModelKeyDecoder.kt` | encoded: String<br>additionalProviderAliases: Map<String, String>? | ReleasedProviderModelKey |  | 17 |
| `ReleasedProviderModelKeyDecoder.decodeOrNull` | `ReleasedProviderModelKeyDecoder` | `com.ai.assistance.operit.data.stats` | `ReleasedProviderModelKeyDecoder.kt` | encoded: String<br>additionalProviderAliases: Map<String, String>? | ReleasedProviderModelKey? | Used by migration code for released keys from before provider/model identities existed. | 50 |
| `TokenActivityAggregator.rangeData` | `TokenActivityAggregator` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | snapshot: TokenActivitySnapshot<br>range: TokenStatsTimeRange | TokenActivityRangeData | Builds all three activity views from the same explicit calendar range. | 40 |
| `TokenActivityAggregator.rangeData` | `TokenActivityAggregator` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | dayTotals: Map<LocalDate, Long><br>start: LocalDate<br>end: LocalDate | TokenActivityRangeData |  | 49 |
| `TokenActivityAggregator.stats` | `TokenActivityAggregator` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | days: List<TokenActivityDay> | TokenActivityStats |  | 92 |
| `TokenActivityAggregator.barHeights` | `TokenActivityAggregator` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | values: List<Long> | IntArray |  | 112 |
| `QuantileLevels.level` | `QuantileLevels` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | value: Long | Int |  | 125 |
| `QuantileLevels.from` | `QuantileLevels` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | values: List<Long> | QuantileLevels |  | 132 |
| `QuantileLevels.nearest` | `QuantileLevels` | `com.ai.assistance.operit.data.stats` | `TokenActivityModels.kt` | percentile: Double | Long |  | 137 |
| `TokenCostCalculator.saturatedAdd` | `TokenCostCalculator` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculator.kt` | left: Long<br>right: Long | Long |  | 8 |
| `TokenCostCalculator.currentCost` | `TokenCostCalculator` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculator.kt` | row: TokenUsageModelAggregateRow<br>pricing: ResolvedTokenPricing<br>targetCurrency: PricingCurrency<br>usdToCnyRate: Double | TokenStatsCostSummary |  | 11 |
| `TokenCostCalculator.add` | `TokenCostCalculator` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculator.kt` | tokens: Long<br>known: Long<br>price: Double | Unit |  | 30 |
| `TokenCostCurrency.convertTo` | `TokenCostCurrency` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculator.kt` | amount: Double<br>source: PricingCurrency<br>target: PricingCurrency<br>usdToCnyRate: Double | Double |  | 81 |
| `ModelPriceSettings.hasAnyUserSetting` | `ModelPriceSettings` | `com.ai.assistance.operit.data.stats` | `TokenPriceResolver.kt` |  | Boolean |  | 16 |
| `TokenPriceSettingsSnapshot.settingFor` | `TokenPriceSettingsSnapshot` | `com.ai.assistance.operit.data.stats` | `TokenPriceResolver.kt` | providerModel: String<br>configId: String? | ModelPriceSettings? |  | 30 |
| `tokenPriceConfigKey` | — | `com.ai.assistance.operit.data.stats` | `TokenPriceResolver.kt` | providerModel: String<br>configId: String | String |  | 48 |
| `TokenPriceResolver.resolve` | `TokenPriceResolver` | `com.ai.assistance.operit.data.stats` | `TokenPriceResolver.kt` | providerModel: String<br>user: ModelPriceSettings? | ResolvedTokenPricing |  | 64 |
| `TokenStatsDisplayUnit.toggled` | `TokenStatsDisplayUnit` | `com.ai.assistance.operit.data.stats` | `TokenStatsDisplayUnit.kt` |  | TokenStatsDisplayUnit |  | 9 |
| `formatTokenCount` | — | `com.ai.assistance.operit.data.stats` | `TokenStatsDisplayUnit.kt` | value: Long<br>unit: TokenStatsDisplayUnit | String |  | 16 |
| `TokenStatsPreferences.importedAtMs` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` |  | Long? |  | 31 |
| `TokenStatsPreferences.completeMigration` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` | importedAtMs: Long<br>releasedUsdToCnyRate: Double? | Unit |  | 33 |
| `TokenStatsPreferences.loadRateWithEstimate` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` |  | Pair<Double, Boolean> |  | 40 |
| `TokenStatsPreferences.saveRate` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` | rate: Double | Unit |  | 50 |
| `TokenStatsPreferences.loadTargetCurrency` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` |  | PricingCurrency |  | 55 |
| `TokenStatsPreferences.saveTargetCurrency` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` | currency: PricingCurrency | Unit |  | 60 |
| `TokenStatsPreferences.loadTokenDisplayUnit` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` |  | TokenStatsDisplayUnit |  | 64 |
| `TokenStatsPreferences.saveTokenDisplayUnit` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` | unit: TokenStatsDisplayUnit | Unit |  | 70 |
| `TokenStatsPreferences.loadActivityViewMode` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` |  | TokenActivityViewMode |  | 74 |
| `TokenStatsPreferences.saveActivityViewMode` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` | mode: TokenActivityViewMode | Unit |  | 79 |
| `TokenStatsPreferences.loadTimeRange` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` |  | TokenStatsTimeRange? |  | 83 |
| `TokenStatsPreferences.saveTimeRange` | `TokenStatsPreferences` | `com.ai.assistance.operit.data.stats` | `TokenStatsPreferences.kt` | range: TokenStatsTimeRange? | Unit |  | 90 |
| `TokenStatsQueryService.lifetimeOverview` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | context: Context<br>params: TokenStatsQueryParams | TokenStatsLifetimeOverview |  | 15 |
| `TokenStatsQueryService.rangeData` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | context: Context<br>range: TokenStatsTimeRange<br>params: TokenStatsQueryParams<br>zone: ZoneId | TokenStatsRangeData |  | 33 |
| `TokenStatsQueryService.annualSummary` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | context: Context<br>range: TokenStatsTimeRange<br>params: TokenStatsQueryParams<br>zone: ZoneId | TokenStatsAnnualSummary | 年度报告用的汇总：全年合计、按月合计和按日合计。 与 [rangeData] 共用模型规范化和花费计算，保证和 Token 统计页同一日期范围内的数字一致； 但不走按天分桶（一年… | 87 |
| `TokenStatsQueryService.earliestOccurredDate` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | context: Context<br>params: TokenStatsQueryParams<br>zone: ZoneId | LocalDate? |  | 140 |
| `TokenStatsQueryService.activitySnapshot` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | context: Context<br>range: TokenStatsTimeRange<br>params: TokenStatsQueryParams<br>zone: ZoneId | TokenActivitySnapshot |  | 154 |
| `TokenStatsQueryService.buildDisplayModels` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | rows: List<TokenUsageModelAggregateRow><br>prices: TokenPriceSettingsSnapshot<br>params: TokenStatsQueryParams | List<TokenStatsDisplayModelBreakdown> |  | 178 |
| `TokenStatsQueryService.toTotals` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | prices: TokenPriceSettingsSnapshot<br>params: TokenStatsQueryParams | TokenStatsTotals |  | 204 |
| `TokenStatsQueryService.combineTotals` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | values: List<TokenStatsTotals><br>params: TokenStatsQueryParams | TokenStatsTotals |  | 240 |
| `TokenStatsQueryService.toModelBucket` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` |  | Unit |  | 266 |
| `TokenStatsQueryService.emptyTotals` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | params: TokenStatsQueryParams | TokenStatsTotals |  | 281 |
| `TokenStatsQueryService.component` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | sum: Long<br>known: Long<br>total: Long | Unit |  | 301 |
| `TokenStatsQueryService.combineComponents` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | components: List<TokenStatsTokenAggregate><br>contributionCount: Long | TokenStatsTokenAggregate |  | 304 |
| `TokenStatsQueryService.displayModelIdFor` | `TokenStatsQueryService` | `com.ai.assistance.operit.data.stats` | `TokenStatsQueryService.kt` | model: String | String |  | 335 |
| `TokenStatsSettingsManager.validatePriceValue` | `TokenStatsSettingsManager` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | name: String<br>value: Double? | Double? |  | 45 |
| `TokenStatsSettingsManager.savePrice` | `TokenStatsSettingsManager` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | draft: TokenStatsPriceDraft | Unit |  | 53 |
| `TokenStatsSettingsManager.allPriceSettings` | `TokenStatsSettingsManager` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` |  | List<TokenStatsPriceSetting> |  | 107 |
| `TokenStatsSettingsManager.restoreBuiltInPrice` | `TokenStatsSettingsManager` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | providerModel: String | Unit |  | 122 |
| `TokenStatsSettingsManager.resetConfigPrice` | `TokenStatsSettingsManager` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | providerModel: String<br>configId: String | Unit |  | 130 |
| `TokenStatsSettingsManager.splitProviderModel` | `TokenStatsSettingsManager` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | providerModel: String | Pair<String, String> |  | 139 |
| `tokenStatsPriceScopeForConfigId` | — | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` | configId: String | TokenStatsPriceScope |  | 149 |
| `hasPriceSetting` | — | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` |  | Boolean |  | 152 |
| `toModelPriceSettings` | — | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` |  | ModelPriceSettings |  | 161 |
| `toPriceSetting` | — | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsManager.kt` |  | TokenStatsPriceSetting |  | 172 |
| `TokenStatsSettingsStore.loadRateWithEstimate` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | Pair<Double, Boolean> |  | 7 |
| `TokenStatsSettingsStore.saveRate` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | rate: Double | Unit |  | 9 |
| `TokenStatsSettingsStore.loadTargetCurrency` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | PricingCurrency |  | 11 |
| `TokenStatsSettingsStore.saveTargetCurrency` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | currency: PricingCurrency | Unit |  | 13 |
| `TokenStatsSettingsStore.loadTokenDisplayUnit` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | TokenStatsDisplayUnit |  | 15 |
| `TokenStatsSettingsStore.saveTokenDisplayUnit` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | unit: TokenStatsDisplayUnit | Unit |  | 17 |
| `TokenStatsSettingsStore.loadActivityViewMode` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | TokenActivityViewMode |  | 19 |
| `TokenStatsSettingsStore.saveActivityViewMode` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | mode: TokenActivityViewMode | Unit |  | 21 |
| `TokenStatsSettingsStore.loadTimeRange` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | TokenStatsTimeRange? |  | 23 |
| `TokenStatsSettingsStore.saveTimeRange` | `TokenStatsSettingsStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | range: TokenStatsTimeRange? | Unit |  | 25 |
| `TokenStatsPreferencesStore.loadRateWithEstimate` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | Pair<Double, Boolean> |  | 32 |
| `TokenStatsPreferencesStore.saveRate` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | rate: Double | Unit |  | 36 |
| `TokenStatsPreferencesStore.loadTargetCurrency` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | PricingCurrency |  | 40 |
| `TokenStatsPreferencesStore.saveTargetCurrency` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | currency: PricingCurrency | Unit |  | 44 |
| `TokenStatsPreferencesStore.loadTokenDisplayUnit` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | TokenStatsDisplayUnit |  | 48 |
| `TokenStatsPreferencesStore.saveTokenDisplayUnit` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | unit: TokenStatsDisplayUnit | Unit |  | 52 |
| `TokenStatsPreferencesStore.loadActivityViewMode` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | TokenActivityViewMode |  | 56 |
| `TokenStatsPreferencesStore.saveActivityViewMode` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | mode: TokenActivityViewMode | Unit |  | 60 |
| `TokenStatsPreferencesStore.loadTimeRange` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` |  | TokenStatsTimeRange? |  | 64 |
| `TokenStatsPreferencesStore.saveTimeRange` | `TokenStatsPreferencesStore` | `com.ai.assistance.operit.data.stats` | `TokenStatsSettingsStore.kt` | range: TokenStatsTimeRange? | Unit |  | 68 |
| `TokenStatsTimeRanges.customRange` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | startMs: Long<br>endMs: Long | TokenStatsTimeRange | 日历选择器提供显式边界，始终使用半开区间 `[startMs, endMs)`。 | 45 |
| `TokenStatsTimeRanges.granularityFor` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | range: TokenStatsTimeRange | TokenStatsGranularity | 按范围时长选择合理桶粒度：≤12h → 10 分钟；≤48h → 1 小时； 更长时间（7d/30d/月）→ 1 自然日。自定义范围同样适用。 | 52 |
| `TokenStatsTimeRanges.bucketStarts` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | range: TokenStatsTimeRange<br>granularity: TokenStatsGranularity<br>zone: ZoneId | List<Long> | 覆盖 [range] 的桶起点列表（本地时间对齐，升序、不相交）。 最后一个桶的终点是日历对齐的下一个桶起点，可能超出 range.endMs； 事件归属按 `[桶起点, 下个桶… | 64 |
| `TokenStatsTimeRanges.bucketEndMs` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | bucketStarts: List<Long><br>index: Int<br>granularity: TokenStatsGranularity<br>zone: ZoneId | Long | 桶 [index] 的结束时间：本地对齐的下一个桶起点（日历推进，非固定毫秒）。 | 86 |
| `TokenStatsTimeRanges.bucketIndexOf` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | ts: Long<br>bucketStarts: List<Long><br>granularity: TokenStatsGranularity<br>zone: ZoneId | Int? | 事件时间戳所属的桶下标（桶起点列表升序）。ts 落在 `[第一个桶起点, 最后一个桶终点)` 之外返回 null（防御，正常输入不触发）。 | 101 |
| `TokenStatsTimeRanges.truncateToBucket` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | zdt: ZonedDateTime<br>granularity: TokenStatsGranularity | ZonedDateTime |  | 114 |
| `TokenStatsTimeRanges.advanceBucket` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | zdt: ZonedDateTime<br>granularity: TokenStatsGranularity | ZonedDateTime |  | 127 |
| `normalizeLegacyCacheWriteUsage` | — | `com.ai.assistance.operit.data.stats` | `TokenUsageLegacyNormalizer.kt` | row: TokenUsageModelAggregateRow | TokenUsageModelAggregateRow | Repairs only the in-memory shape of v20->v21 history rows. The old import left cache-writ… | 13 |
| `TokenUsageRepository.getInstance` | `TokenUsageRepository` | `com.ai.assistance.operit.data.stats` | `TokenUsageRepository.kt` | context: Context | TokenUsageRepository |  | 22 |
| `TokenUsageRepository.withDatabaseAccess` | `TokenUsageRepository` | `com.ai.assistance.operit.data.stats` | `TokenUsageRepository.kt` | block: suspend () -> T | T | Prevent Room access while a restore replaces database files. | 28 |
| `TokenUsageRepository.withDatabaseRestore` | `TokenUsageRepository` | `com.ai.assistance.operit.data.stats` | `TokenUsageRepository.kt` | block: suspend () -> T | T |  | 31 |
| `TokenUsageRepository.ensureInitialized` | `TokenUsageRepository` | `com.ai.assistance.operit.data.stats` | `TokenUsageRepository.kt` |  | Unit |  | 43 |
| `TokenUsageRepository.withDao` | `TokenUsageRepository` | `com.ai.assistance.operit.data.stats` | `TokenUsageRepository.kt` | block: suspend (TokenUsageDao) -> T | T |  | 98 |
| `TokenUsageRepository.record` | `TokenUsageRepository` | `com.ai.assistance.operit.data.stats` | `TokenUsageRepository.kt` | record: TokenUsageRecordEntity | Unit |  | 103 |
| `JvmSupportSQLiteDatabase.execSQL` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | sql: String | Unit |  | 31 ⚑ |
| `JvmSupportSQLiteDatabase.execSQL` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | sql: String<br>bindArgs: Array<out Any?> | Unit |  | 35 ⚑ |
| `JvmSupportSQLiteDatabase.query` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | query: String | Cursor |  | 53 ⚑ |
| `JvmSupportSQLiteDatabase.query` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | query: String<br>bindArgs: Array<out Any?> | Cursor |  | 58 ⚑ |
| `JvmSupportSQLiteDatabase.query` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | query: SupportSQLiteQuery | Cursor |  | 75 ⚑ |
| `JvmSupportSQLiteDatabase.bindNull` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | index: Int | Unit |  | 78 ⚑ |
| `JvmSupportSQLiteDatabase.bindLong` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | index: Int<br>value: Long | Unit |  | 79 ⚑ |
| `JvmSupportSQLiteDatabase.bindDouble` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | index: Int<br>value: Double | Unit |  | 80 ⚑ |
| `JvmSupportSQLiteDatabase.bindString` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | index: Int<br>value: String | Unit |  | 81 ⚑ |
| `JvmSupportSQLiteDatabase.bindBlob` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | index: Int<br>value: ByteArray | Unit |  | 82 ⚑ |
| `JvmSupportSQLiteDatabase.clearBindings` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 83 ⚑ |
| `JvmSupportSQLiteDatabase.close` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 84 ⚑ |
| `JvmSupportSQLiteDatabase.query` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | query: SupportSQLiteQuery<br>cancellationSignal: CancellationSignal? | Cursor |  | 89 ⚑ |
| `JvmSupportSQLiteDatabase.close` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 92 ⚑ |
| `JvmSupportSQLiteDatabase.setMaximumSize` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | numBytes: Long | Long |  | 112 ⚑ |
| `JvmSupportSQLiteDatabase.compileStatement` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | sql: String | SupportSQLiteStatement |  | 130 ⚑ |
| `JvmSupportSQLiteDatabase.beginTransaction` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 133 ⚑ |
| `JvmSupportSQLiteDatabase.beginTransactionNonExclusive` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 135 ⚑ |
| `JvmSupportSQLiteDatabase.beginTransactionWithListener` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | listener: android.database.sqlite.SQLiteTrans… | Unit |  | 137 ⚑ |
| `JvmSupportSQLiteDatabase.beginTransactionWithListenerNonExclusive` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | listener: android.database.sqlite.SQLiteTrans… | Unit |  | 140 ⚑ |
| `JvmSupportSQLiteDatabase.endTransaction` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 144 ⚑ |
| `JvmSupportSQLiteDatabase.setTransactionSuccessful` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 146 ⚑ |
| `JvmSupportSQLiteDatabase.inTransaction` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 148 ⚑ |
| `JvmSupportSQLiteDatabase.yieldIfContendedSafely` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 150 ⚑ |
| `JvmSupportSQLiteDatabase.yieldIfContendedSafely` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | sleepAfterYieldDelayMillis: Long | Boolean |  | 152 ⚑ |
| `JvmSupportSQLiteDatabase.insert` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | table: String<br>conflictAlgorithm: Int<br>values: ContentValues | Long |  | 155 ⚑ |
| `JvmSupportSQLiteDatabase.delete` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | table: String<br>whereClause: String?<br>whereArgs: Array<out Any?>? | Int |  | 158 ⚑ |
| `JvmSupportSQLiteDatabase.update` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | table: String<br>conflictAlgorithm: Int<br>values: ContentValues<br>whereClause: String?<br>whereArgs: Array<out Any?>? | Int |  | 161 ⚑ |
| `JvmSupportSQLiteDatabase.needUpgrade` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | newVersion: Int | Boolean |  | 169 ⚑ |
| `JvmSupportSQLiteDatabase.setLocale` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | locale: Locale | Unit |  | 171 ⚑ |
| `JvmSupportSQLiteDatabase.setMaxSqlCacheSize` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | cacheSize: Int | Unit |  | 173 ⚑ |
| `JvmSupportSQLiteDatabase.setForeignKeyConstraintsEnabled` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | enable: Boolean | Unit |  | 175 ⚑ |
| `JvmSupportSQLiteDatabase.enableWriteAheadLogging` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 178 ⚑ |
| `JvmSupportSQLiteDatabase.disableWriteAheadLogging` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 180 ⚑ |
| `JvmSupportSQLiteDatabase.unsupported` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | method: String | Nothing |  | 182 ⚑ |
| `JvmSupportSQLiteDatabase.open` | `JvmSupportSQLiteDatabase` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | dbPath: String | JvmSupportSQLiteDatabase |  | 188 ⚑ |
| `JvmCursor.getCount` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Int |  | 206 ⚑ |
| `JvmCursor.getPosition` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Int |  | 208 ⚑ |
| `JvmCursor.move` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | position: Int | Boolean |  | 210 ⚑ |
| `JvmCursor.moveToPosition` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | position: Int | Boolean |  | 212 ⚑ |
| `JvmCursor.moveToFirst` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 221 ⚑ |
| `JvmCursor.moveToLast` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 223 ⚑ |
| `JvmCursor.moveToNext` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 225 ⚑ |
| `JvmCursor.moveToPrevious` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 227 ⚑ |
| `JvmCursor.isFirst` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 229 ⚑ |
| `JvmCursor.isLast` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 231 ⚑ |
| `JvmCursor.isBeforeFirst` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 233 ⚑ |
| `JvmCursor.isAfterLast` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 235 ⚑ |
| `JvmCursor.getColumnCount` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Int |  | 237 ⚑ |
| `JvmCursor.getColumnIndex` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnName: String | Int |  | 239 ⚑ |
| `JvmCursor.getColumnIndexOrThrow` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnName: String | Int |  | 242 ⚑ |
| `JvmCursor.getColumnName` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | String |  | 248 ⚑ |
| `JvmCursor.getColumnNames` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Array<String> |  | 250 ⚑ |
| `JvmCursor.getString` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | String |  | 252 ⚑ |
| `JvmCursor.getLong` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | Long |  | 261 ⚑ |
| `JvmCursor.getInt` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | Int |  | 270 ⚑ |
| `JvmCursor.getShort` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | Short |  | 272 ⚑ |
| `JvmCursor.getFloat` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | Float |  | 274 ⚑ |
| `JvmCursor.getDouble` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | Double |  | 283 ⚑ |
| `JvmCursor.getBlob` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | ByteArray |  | 292 ⚑ |
| `JvmCursor.isNull` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | Boolean |  | 294 ⚑ |
| `JvmCursor.getType` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int | Int |  | 296 ⚑ |
| `JvmCursor.close` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 307 ⚑ |
| `JvmCursor.isClosed` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 315 ⚑ |
| `JvmCursor.deactivate` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Unit |  | 317 ⚑ |
| `JvmCursor.requery` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 319 ⚑ |
| `JvmCursor.copyStringToBuffer` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | columnIndex: Int<br>buffer: android.database.CharArrayBuffer | Unit |  | 321 ⚑ |
| `JvmCursor.getWantsAllOnMoveCalls` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Boolean |  | 324 ⚑ |
| `JvmCursor.getExtras` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Bundle? |  | 326 ⚑ |
| `JvmCursor.setExtras` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | extras: Bundle? | Unit |  | 328 ⚑ |
| `JvmCursor.respond` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | extras: Bundle? | Bundle? |  | 330 ⚑ |
| `JvmCursor.getNotificationUri` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Uri? |  | 332 ⚑ |
| `JvmCursor.setNotificationUri` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | cr: android.content.ContentResolver<br>notifyUri: Uri? | Unit |  | 334 ⚑ |
| `JvmCursor.registerContentObserver` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | observer: android.database.ContentObserver | Unit |  | 336 ⚑ |
| `JvmCursor.unregisterContentObserver` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | observer: android.database.ContentObserver | Unit |  | 338 ⚑ |
| `JvmCursor.registerDataSetObserver` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | observer: android.database.DataSetObserver | Unit |  | 340 ⚑ |
| `JvmCursor.unregisterDataSetObserver` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | observer: android.database.DataSetObserver | Unit |  | 342 ⚑ |
| `JvmCursor.row` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` |  | Array<Any?> |  | 344 ⚑ |
| `JvmCursor.unsupported` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | method: String | Nothing |  | 351 ⚑ |
| `JvmCursor.materialize` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | resultSet: ResultSet | List<Array<Any?>> |  | 355 ⚑ |
| `JvmCursor.columnNames` | `JvmCursor` | `com.ai.assistance.operit.data.stats` | `JvmSupportSQLiteDatabase.kt` | metaData: ResultSetMetaData | Array<String> |  | 368 ⚑ |
| `TokenActivityAggregatorTest.dateRange` | `TokenActivityAggregatorTest` | `com.ai.assistance.operit.data.stats` | `TokenActivityAggregatorTest.kt` | start: String<br>inclusiveEnd: String | TokenStatsTimeRange |  | 59 ⚑ |
| `TokenCostCalculatorTest.tokenPricing` | `TokenCostCalculatorTest` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculatorTest.kt` | inputPricePerMillion: Double?<br>cachedInputPricePerMillion: Double?<br>outputPricePerMillion: Double?<br>source: PricingSource? | Unit |  | 188 ⚑ |
| `TokenCostCalculatorTest.aggregateRow` | `TokenCostCalculatorTest` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculatorTest.kt` | requests: Long?<br>provider: String?<br>configId: String?<br>uncachedInputTokens: Long?<br>uncachedInputKnown: Long?<br>cachedInputTokens: Long?<br>cachedInputKnown: Long?<br>cacheWriteTokens: Long?<br>cacheWriteKnown: Long?<br>totalInputT… | Unit |  | 204 ⚑ |
| `TokenStatsTimeRangeTest.localMs` | `TokenStatsTimeRangeTest` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRangeTest.kt` | dateTime: String<br>zone: ZoneId | Long |  | 16 ⚑ |
| `TokenStatsTimeRangeTest.local` | `TokenStatsTimeRangeTest` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRangeTest.kt` | epochMs: Long<br>zone: ZoneId | LocalDateTime |  | 19 ⚑ |
| `TokenStatsTimeRangeTest.granularityOf` | `TokenStatsTimeRangeTest` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRangeTest.kt` | hours: Long | Unit |  | 41 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ProviderUsageNormalizer.SOURCE_ANTHROPIC` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | inferred |  | 78 |
| `ProviderUsageNormalizer.SOURCE_GEMINI` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | inferred |  | 79 |
| `ProviderUsageNormalizer.SOURCE_LLAMA` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | inferred |  | 80 |
| `ProviderUsageNormalizer.SOURCE_MNN` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | inferred |  | 81 |
| `ProviderUsageNormalizer.SOURCE_OPENAI_CHAT_COMPLETIONS` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | inferred |  | 76 |
| `ProviderUsageNormalizer.SOURCE_OPENAI_RESPONSES` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | inferred |  | 77 |
| `ProviderUsageNormalizer.SOURCE_TOOLPKG` | `ProviderUsageNormalizer` | `com.ai.assistance.operit.data.stats` | `ProviderUsageSnapshot.kt` | inferred |  | 82 |
| `ReleasedProviderModelKeyDecoder.builtInProviderAliases` | `ReleasedProviderModelKeyDecoder` | `com.ai.assistance.operit.data.stats` | `ReleasedProviderModelKeyDecoder.kt` | inferred |  | 14 |
| `ReleasedProviderModelKeyDecoder.preProviderFunctionKeys` | `ReleasedProviderModelKeyDecoder` | `com.ai.assistance.operit.data.stats` | `ReleasedProviderModelKeyDecoder.kt` | inferred |  | 15 |
| `TokenCostCurrency.DEFAULT_USD_TO_CNY_RATE` | `TokenCostCurrency` | `com.ai.assistance.operit.data.stats` | `TokenCostCalculator.kt` | inferred |  | 79 |
| `TokenStatsTimeRanges.DAY_MS` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | Long |  | 39 |
| `TokenStatsTimeRanges.HOUR_MS` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | Long |  | 38 |
| `TokenStatsTimeRanges.MAX_BUCKETS` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | inferred | 防御：自定义范围过大时限制桶数量，避免病态输入拖垮内存/UI。 | 42 |
| `TokenStatsTimeRanges.TEN_MINUTES_MS` | `TokenStatsTimeRanges` | `com.ai.assistance.operit.data.stats` | `TokenStatsTimeRange.kt` | Long |  | 37 |
