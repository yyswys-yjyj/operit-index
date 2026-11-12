# com.k2fsa.sherpa

> 函数 72 · 类型 22 · 顶层常量 0 · 共 94 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `DecoderConfig` | `DecoderConfig` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | class DecoderConfig(var method: String, var numActivePaths: Int) |  | 23 |
| `EndpointConfig` | `EndpointConfig` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class EndpointConfig(var rule1: EndpointRule, var rule2: EndpointRule, var rule3: EndpointRule) |  | 11 |
| `EndpointRule` | `EndpointRule` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class EndpointRule(var mustContainNonSilence: Boolean, var minTrailingSilence: Float, var minUtteranceLength: Float) |  | 5 |
| `FeatureConfig` | `FeatureConfig` | `com.k2fsa.sherpa.mnn` | `FeatureConfig.kt` | class FeatureConfig(var sampleRate: Int, var featureDim: Int) |  | 3 |
| `FeatureExtractorConfig` | `FeatureExtractorConfig` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | class FeatureExtractorConfig(var sampleRate: Float, var featureDim: Int) |  | 5 |
| `ModelConfig` | `ModelConfig` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | class ModelConfig(var encoderParam: String, var encoderBin: String, var decoderParam: String, var decoderBin: String, var joinerParam: String, var joinerBin: String, var tokens… |  | 11 |
| `OnlineCtcFstDecoderConfig` | `OnlineCtcFstDecoderConfig` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineCtcFstDecoderConfig(var graph: String, var maxActive: Int) |  | 55 |
| `OnlineLMConfig` | `OnlineLMConfig` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineLMConfig(var model: String, var scale: Float) |  | 50 |
| `OnlineModelConfig` | `OnlineModelConfig` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineModelConfig(var transducer: OnlineTransducerModelConfig, var paraformer: OnlineParaformerModelConfig, var zipformer2Ctc: OnlineZipformer2CtcModelConfig, var neMoCtc: Onli… |  | 36 |
| `OnlineNeMoCtcModelConfig` | `OnlineNeMoCtcModelConfig` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineNeMoCtcModelConfig(var model: String) |  | 32 |
| `OnlineParaformerModelConfig` | `OnlineParaformerModelConfig` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineParaformerModelConfig(var encoder: String, var decoder: String) |  | 23 |
| `OnlineRecognizer` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineRecognizer(assetManager: AssetManager?, val config: OnlineRecognizerConfig) |  | 83 |
| `OnlineRecognizerConfig` | `OnlineRecognizerConfig` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineRecognizerConfig(var featConfig: FeatureConfig, var modelConfig: OnlineModelConfig, var lmConfig: OnlineLMConfig, var ctcFstDecoderConfig: OnlineCtcFstDecoderConfig, var endpo… |  | 61 |
| `OnlineRecognizerResult` | `OnlineRecognizerResult` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineRecognizerResult(val text: String, val tokens: Array<String>, val timestamps: FloatArray) |  | 77 |
| `OnlineStream` | `OnlineStream` | `com.k2fsa.sherpa.mnn` | `OnlineStream.kt` | class OnlineStream(var ptr: Long) |  | 3 |
| `OnlineTransducerModelConfig` | `OnlineTransducerModelConfig` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineTransducerModelConfig(var encoder: String, var decoder: String, var joiner: String) |  | 17 |
| `OnlineZipformer2CtcModelConfig` | `OnlineZipformer2CtcModelConfig` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | class OnlineZipformer2CtcModelConfig(var model: String) |  | 28 |
| `RecognizerConfig` | `RecognizerConfig` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | class RecognizerConfig(var featConfig: FeatureExtractorConfig, var modelConfig: ModelConfig, var decoderConfig: DecoderConfig, var enableEndpoint: Boolean, var rule1MinTrailingSilen… |  | 28 |
| `SherpaNcnn` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | class SherpaNcnn(var config: RecognizerConfig, assetManager: AssetManager?) |  | 40 |
| `SileroVadModelConfig` | `SileroVadModelConfig` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | class SileroVadModelConfig(var model: String, var threshold: Float, var minSilenceDuration: Float, var minSpeechDuration: Float, var windowSize: Int, var maxSpeechDuration: Float) |  | 6 |
| `SpeechSegment` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | class SpeechSegment(val start: Int, val samples: FloatArray) |  | 23 |
| `VadModelConfig` | `VadModelConfig` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | class VadModelConfig(var sileroVadModelConfig: SileroVadModelConfig, var sampleRate: Int, var numThreads: Int, var provider: String, var debug: Boolean) |  | 15 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `getFeatureConfig` | — | `com.k2fsa.sherpa.mnn` | `FeatureConfig.kt` | sampleRate: Int<br>featureDim: Int | FeatureConfig |  | 8 |
| `OnlineRecognizer.finalize` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` |  | Unit |  | 97 |
| `OnlineRecognizer.release` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` |  | Unit |  | 104 |
| `OnlineRecognizer.createStream` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | hotwords: String? | OnlineStream |  | 106 |
| `OnlineRecognizer.reset` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | stream: OnlineStream | Unit |  | 111 |
| `OnlineRecognizer.decode` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | stream: OnlineStream | Unit |  | 112 |
| `OnlineRecognizer.isEndpoint` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | stream: OnlineStream | Unit |  | 113 |
| `OnlineRecognizer.isReady` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | stream: OnlineStream | Unit |  | 114 |
| `OnlineRecognizer.getResult` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | stream: OnlineStream | OnlineRecognizerResult |  | 116 |
| `OnlineRecognizer.delete` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | ptr: Long | Unit |  | 126 |
| `OnlineRecognizer.newFromAsset` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | assetManager: AssetManager<br>config: OnlineRecognizerConfig | Long |  | 128 |
| `OnlineRecognizer.newFromFile` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | config: OnlineRecognizerConfig | Long |  | 133 |
| `OnlineRecognizer.createStream` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | ptr: Long<br>hotwords: String | Long |  | 137 |
| `OnlineRecognizer.reset` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | ptr: Long<br>streamPtr: Long | Unit |  | 138 |
| `OnlineRecognizer.decode` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | ptr: Long<br>streamPtr: Long | Unit |  | 139 |
| `OnlineRecognizer.isEndpoint` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | ptr: Long<br>streamPtr: Long | Boolean |  | 140 |
| `OnlineRecognizer.isReady` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | ptr: Long<br>streamPtr: Long | Boolean |  | 141 |
| `OnlineRecognizer.getResult` | `OnlineRecognizer` | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | ptr: Long<br>streamPtr: Long | Array<Any> |  | 142 |
| `getModelConfig` | — | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | type: Int | OnlineModelConfig? |  | 191 |
| `getOnlineLMConfig` | — | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` | type: Int | OnlineLMConfig |  | 394 |
| `getEndpointConfig` | — | `com.k2fsa.sherpa.mnn` | `OnlineRecognizer.kt` |  | EndpointConfig |  | 407 |
| `OnlineStream.acceptWaveform` | `OnlineStream` | `com.k2fsa.sherpa.mnn` | `OnlineStream.kt` | samples: FloatArray<br>sampleRate: Int | Unit |  | 4 |
| `OnlineStream.inputFinished` | `OnlineStream` | `com.k2fsa.sherpa.mnn` | `OnlineStream.kt` |  | Unit |  | 7 |
| `OnlineStream.finalize` | `OnlineStream` | `com.k2fsa.sherpa.mnn` | `OnlineStream.kt` |  | Unit |  | 9 |
| `OnlineStream.release` | `OnlineStream` | `com.k2fsa.sherpa.mnn` | `OnlineStream.kt` |  | Unit |  | 16 |
| `OnlineStream.use` | `OnlineStream` | `com.k2fsa.sherpa.mnn` | `OnlineStream.kt` | block: (OnlineStream) -> Unit | Unit |  | 18 |
| `OnlineStream.acceptWaveform` | `OnlineStream` | `com.k2fsa.sherpa.mnn` | `OnlineStream.kt` | ptr: Long<br>samples: FloatArray<br>sampleRate: Int | Unit |  | 26 |
| `OnlineStream.inputFinished` | `OnlineStream` | `com.k2fsa.sherpa.mnn` | `OnlineStream.kt` | ptr: Long | Unit |  | 27 |
| `OnlineStream.delete` | `OnlineStream` | `com.k2fsa.sherpa.mnn` | `OnlineStream.kt` | ptr: Long | Unit |  | 28 |
| `SpeechSegment.finalize` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` |  | Unit |  | 39 |
| `SpeechSegment.release` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` |  | Unit |  | 46 |
| `SpeechSegment.acceptWaveform` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | samples: FloatArray | Unit |  | 48 |
| `SpeechSegment.empty` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` |  | Boolean |  | 50 |
| `SpeechSegment.pop` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` |  | Unit |  | 51 |
| `SpeechSegment.front` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` |  | SpeechSegment |  | 53 |
| `SpeechSegment.clear` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` |  | Unit |  | 58 |
| `SpeechSegment.isSpeechDetected` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` |  | Boolean |  | 60 |
| `SpeechSegment.reset` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` |  | Unit |  | 62 |
| `SpeechSegment.flush` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` |  | Unit |  | 64 |
| `SpeechSegment.delete` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | ptr: Long | Unit |  | 66 |
| `SpeechSegment.newFromAsset` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | assetManager: AssetManager<br>config: VadModelConfig | Long |  | 68 |
| `SpeechSegment.newFromFile` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | config: VadModelConfig | Long |  | 73 |
| `SpeechSegment.acceptWaveform` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | ptr: Long<br>samples: FloatArray | Unit |  | 77 |
| `SpeechSegment.empty` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | ptr: Long | Boolean |  | 78 |
| `SpeechSegment.pop` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | ptr: Long | Unit |  | 79 |
| `SpeechSegment.clear` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | ptr: Long | Unit |  | 80 |
| `SpeechSegment.front` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | ptr: Long | Array<Any> |  | 81 |
| `SpeechSegment.isSpeechDetected` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | ptr: Long | Boolean |  | 82 |
| `SpeechSegment.reset` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | ptr: Long | Unit |  | 83 |
| `SpeechSegment.flush` | `SpeechSegment` | `com.k2fsa.sherpa.mnn` | `Vad.kt` | ptr: Long | Unit |  | 84 |
| `getVadModelConfig` | — | `com.k2fsa.sherpa.mnn` | `Vad.kt` | type: Int | VadModelConfig? | Please visit https://github.com/snakers4/silero-vad/raw/master/src/silero_vad/data/silero… | 98 |
| `SherpaNcnn.finalize` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` |  | Unit |  | 54 |
| `SherpaNcnn.release` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` |  | Unit |  | 59 |
| `SherpaNcnn.acceptSamples` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | samples: FloatArray | Unit |  | 66 |
| `SherpaNcnn.isReady` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` |  | Unit |  | 69 |
| `SherpaNcnn.decode` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` |  | Unit |  | 71 |
| `SherpaNcnn.inputFinished` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` |  | Unit |  | 73 |
| `SherpaNcnn.isEndpoint` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` |  | Boolean |  | 74 |
| `SherpaNcnn.reset` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | recreate: Boolean? | Unit |  | 75 |
| `SherpaNcnn.newFromAsset` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | assetManager: AssetManager<br>config: RecognizerConfig | Long |  | 80 |
| `SherpaNcnn.newFromFile` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | config: RecognizerConfig | Long |  | 85 |
| `SherpaNcnn.delete` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | ptr: Long | Unit |  | 89 |
| `SherpaNcnn.acceptWaveform` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | ptr: Long<br>samples: FloatArray<br>sampleRate: Float | Unit |  | 90 |
| `SherpaNcnn.inputFinished` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | ptr: Long | Unit |  | 91 |
| `SherpaNcnn.isReady` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | ptr: Long | Boolean |  | 92 |
| `SherpaNcnn.decode` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | ptr: Long | Unit |  | 93 |
| `SherpaNcnn.isEndpoint` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | ptr: Long | Boolean |  | 94 |
| `SherpaNcnn.reset` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | ptr: Long<br>recreate: Boolean | Unit |  | 95 |
| `SherpaNcnn.getText` | `SherpaNcnn` | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | ptr: Long | String |  | 96 |
| `getFeatureExtractorConfig` | — | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | sampleRate: Float<br>featureDim: Int | FeatureExtractorConfig |  | 105 |
| `getDecoderConfig` | — | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | method: String<br>numActivePaths: Int | DecoderConfig |  | 115 |
| `getModelConfig` | — | `com.k2fsa.sherpa.ncnn` | `SherpaNcnn.kt` | type: Int<br>useGPU: Boolean | ModelConfig? |  | 146 |
