# com.ai.assistance

> 函数 324 · 类型 63 · 顶层常量 31 · 共 418 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `ExampleInstrumentedTest` | `ExampleInstrumentedTest` | `com.ai.assistance.operit` | `ExampleInstrumentedTest.kt` | class ExampleInstrumentedTest | Instrumented test, which will execute on an Android device. See [testing documentation](h… | 17 |
| `ExampleInstrumentedTest` | `ExampleInstrumentedTest` | `com.ai.assistance.shower` | `ExampleInstrumentedTest.kt` | class ExampleInstrumentedTest | Instrumented test, which will execute on an Android device. See [testing documentation](h… | 17 |
| `ExampleUnitTest` | `ExampleUnitTest` | `com.ai.assistance.shower` | `ExampleUnitTest.kt` | class ExampleUnitTest | Example local unit test, which will execute on the development machine (host). See [testi… | 12 |
| `FbxGlSurfaceView` | `FbxGlSurfaceView` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | class FbxGlSurfaceView(context: Context, attrs: AttributeSet?) : GLSurfaceView |  | 28 |
| `FbxInspector` | `FbxInspector` | `com.ai.assistance.fbx` | `FbxInspector.kt` | object FbxInspector |  | 17 |
| `FbxLibraryLoader` | `FbxLibraryLoader` | `com.ai.assistance.fbx` | `FbxLibraryLoader.kt` | object FbxLibraryLoader |  | 3 |
| `FbxModelInfo` | `FbxModelInfo` | `com.ai.assistance.fbx` | `FbxInspector.kt` | class FbxModelInfo(val modelName: String, val animationNames: List<String>, val animationDurationMillisByName: Map<String, Long>, val requiredExternalFiles: List<String>, val mi… |  | 6 |
| `FbxNative` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` | object FbxNative |  | 3 |
| `FbxPreviewInfo` | `FbxPreviewInfo` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | class FbxPreviewInfo(val centerX: Float, val centerY: Float, val centerZ: Float, val radius: Float, val vertexCount: Int, val animationNames: List<String>, val animationDurationMi… |  | 112 |
| `FbxPreviewMaterial` | `FbxPreviewMaterial` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | class FbxPreviewMaterial(val textureIndex: Int, val baseColor: FloatArray, val alphaBlend: Boolean) |  | 100 |
| `FbxPreviewRenderer` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | class FbxPreviewRenderer(private val appContext: Context) : GLSurfaceView.Renderer |  | 220 |
| `FbxPreviewRenderer.Handle` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | object Handle |  | 228 |
| `FbxPreviewSegment` | `FbxPreviewSegment` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | class FbxPreviewSegment(val vertexOffset: Int, val vertexCount: Int, val materialIndex: Int) |  | 106 |
| `FbxPreviewTextureSlot` | `FbxPreviewTextureSlot` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | class FbxPreviewTextureSlot(val label: String, val path: String?, val embedded: Boolean) |  | 94 |
| `LlamaLibraryLoader` | `LlamaLibraryLoader` | `com.ai.assistance.llama` | `LlamaLibraryLoader.kt` | object LlamaLibraryLoader |  | 3 |
| `LlamaNative` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | object LlamaNative |  | 3 |
| `LlamaNative.GenerationCallback` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | interface GenerationCallback |  | 80 |
| `LlamaSession` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | class LlamaSession(private var sessionPtr: Long) |  | 3 |
| `LlamaSession.Config` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | class Config(val nThreads: Int, val nCtx: Int, val nBatch: Int, val nUBatch: Int, val nGpuLayers: Int, val useMmap: Boolean, val flashAttention: Boolean, val kvUnified: Bo… |  | 7 |
| `LoadedTextureSlot` | `LoadedTextureSlot` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | class LoadedTextureSlot(val textureId: Int, val hasAlpha: Boolean) |  | 215 |
| `MainActivity` | `MainActivity` | `com.ai.assistance.shower` | `MainActivity.kt` | class MainActivity : ComponentActivity |  | 17 |
| `MmdGlSurfaceView` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | class MmdGlSurfaceView(context: Context, attrs: AttributeSet?) : GLSurfaceView |  | 16 |
| `MmdInspector` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` | object MmdInspector |  | 31 |
| `MmdLibraryLoader` | `MmdLibraryLoader` | `com.ai.assistance.mmd` | `MmdLibraryLoader.kt` | object MmdLibraryLoader |  | 3 |
| `MmdModelFormat` | `MmdModelFormat` | `com.ai.assistance.mmd` | `MmdInspector.kt` | class MmdModelFormat |  | 3 |
| `MmdModelInfo` | `MmdModelInfo` | `com.ai.assistance.mmd` | `MmdInspector.kt` | class MmdModelInfo(val format: MmdModelFormat, val modelName: String, val vertexCount: Int, val faceCount: Int, val materialCount: Int, val boneCount: Int, val morphCount: Int, … |  | 9 |
| `MmdNative` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | object MmdNative |  | 5 |
| `MNNForwardType` | `MNNForwardType` | `com.ai.assistance.mnn` | `MNNForwardType.kt` | class MNNForwardType(val type: Int) | MNN Forward Type 推理执行的硬件类型 | 7 |
| `MNNImageProcess` | `MNNImageProcess` | `com.ai.assistance.mnn` | `MNNImageProcess.kt` | object MNNImageProcess | MNN Image Process MNN 图像处理工具类 | 10 |
| `MNNImageProcess.Config` | `MNNImageProcess` | `com.ai.assistance.mnn` | `MNNImageProcess.kt` | class Config(var mean: FloatArray, var normal: FloatArray, var source: Format, var dest: Format, var filter: Filter, var wrap: Wrap) | 图像处理配置 | 59 |
| `MNNImageProcess.Filter` | `MNNImageProcess` | `com.ai.assistance.mnn` | `MNNImageProcess.kt` | class Filter(val type: Int) | 滤波器类型 | 35 |
| `MNNImageProcess.Format` | `MNNImageProcess` | `com.ai.assistance.mnn` | `MNNImageProcess.kt` | class Format(val type: Int) | 图像格式 | 15 |
| `MNNImageProcess.Wrap` | `MNNImageProcess` | `com.ai.assistance.mnn` | `MNNImageProcess.kt` | class Wrap(val type: Int) | 边界处理方式 | 47 |
| `MNNLibraryLoader` | `MNNLibraryLoader` | `com.ai.assistance.mnn` | `MNNLibraryLoader.kt` | object MNNLibraryLoader | MNN 库加载器 确保 MNN 和 MNNWrapper 库只被加载一次 | 9 |
| `MNNLlmContextInfo` | `MNNLlmContextInfo` | `com.ai.assistance.mnn` | `MNNLlmContextInfo.kt` | class MNNLlmContextInfo(val promptLen: Int, val generatedSeqLen: Int, val totalSeqLen: Int, val loadUs: Long, val visionUs: Long, val audioUs: Long, val prefillUs: Long, val decodeUs… | 最近一次推理上下文的快照。 | 8 |
| `MNNLlmNative` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | object MNNLlmNative | MNN LLM Engine Native JNI 接口 基于 MNN 官方 LLM 引擎实现 | 7 |
| `MNNLlmNative.AudioDataCallback` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | interface AudioDataCallback | 当模型输出音频波形时触发。 返回 true 表示继续，false 表示停止音频输出。 | 210 |
| `MNNLlmNative.GenerationCallback` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | interface GenerationCallback | 生成回调接口 | 197 |
| `MNNLlmSession` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | class MNNLlmSession(private var llmPtr: Long, private val modelPath: String) | MNN LLM 会话封装 提供高级 API 来管理 LLM 推理会话 | 11 |
| `MNNModule` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | class MNNModule(private var modulePtr: Long, private val inputNames: List<String>, private val outputNames: List<String>) | MNN Module 高级封装 用于处理动态形状模型和复杂推理场景 | 9 |
| `MNNModule.Config` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | class Config(val inputNames: List<String>, val outputNames: List<String>, val forwardType: Int, val numThread: Int, val precision: Int, val memoryMode: Int) | 模型配置 | 48 |
| `MNNModule.DataFormat` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | object DataFormat | 数据格式 | 78 |
| `MNNModule.DataType` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | object DataType | 数据类型编码 | 87 |
| `MNNModule.MemoryMode` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | object MemoryMode | 内存模式 | 70 |
| `MNNModule.PrecisionMode` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | object PrecisionMode | 精度模式 | 60 |
| `MNNModule.Variable` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | class Variable(private var varPtr: Long) | 变量（张量）包装类 | 98 |
| `MNNModuleNative` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | object MNNModuleNative | MNN Module Native JNI 接口 用于处理动态形状模型和需要输入内容计算形状的模型 | 7 |
| `MNNNetInstance` | `MNNNetInstance` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | class MNNNetInstance(private var netInstance: Long) | MNN Net Instance MNN 网络实例，封装了 MNN 推理引擎的核心功能 | 9 |
| `MNNNetInstance.Config` | `MNNNetInstance` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | class Config(var forwardType: Int, var numThread: Int, var saveTensors: Array<String>?, var outputTensors: Array<String>?) | Session 配置 | 48 |
| `MNNNetInstance.Session` | `MNNNetInstance` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | class Session(private var sessionInstance: Long) | Session 会话 | 86 |
| `MNNNetInstance.Session.Tensor` | `Session` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | class Tensor(private val tensorInstance: Long) | Tensor 张量 | 91 |
| `MNNNetNative` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | object MNNNetNative | MNN Native JNI Interface MNN 原生 JNI 接口层 | 9 |
| `NativeMmdRenderer` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | class NativeMmdRenderer(private val appContext: Context, private val instanceId: Int) : GLSurfaceView.Renderer |  | 126 |
| `ShellCommandResult` | `ShellCommandResult` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | class ShellCommandResult(val success: Boolean, val stdout: String, val stderr: String, val exitCode: Int) | Result of executing a shell command. | 17 |
| `ShellIdentity` | `ShellIdentity` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | class ShellIdentity | Identity for executing shell commands. | 8 |
| `ShowerBinderRegistry` | `ShowerBinderRegistry` | `com.ai.assistance.showerclient` | `ShowerBinderRegistry.kt` | object ShowerBinderRegistry | Global registry for the active Shower Binder service. Host apps should update this from t… | 12 |
| `ShowerController` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | class ShowerController | Lightweight controller to talk to the Shower server running locally on the device. Respon… | 22 |
| `ShowerEnvironment` | `ShowerEnvironment` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | object ShowerEnvironment | Global environment configuration for the Shower client library. | 47 |
| `ShowerLog` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | object ShowerLog | Logging facade for Shower client. This avoids hardcoding host logger implementations insi… | 72 |
| `ShowerServerManager` | `ShowerServerManager` | `com.ai.assistance.showerclient` | `ShowerServerManager.kt` | object ShowerServerManager | Helper to manage the lifecycle of the Shower server (shower-server.jar) on the device. Th… | 18 |
| `ShowerSurfaceView` | `ShowerSurfaceView` | `com.ai.assistance.showerclient.ui` | `ShowerSurfaceView.kt` | class ShowerSurfaceView(context: Context, attrs: AttributeSet?) : SurfaceView | SurfaceView used inside a virtual display overlay to render the Shower video stream. | 19 |
| `ShowerVideoRenderer` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` | class ShowerVideoRenderer | H.264 decoder that renders the Shower video stream onto a Surface. Each instance handles … | 23 |
| `VmdMotionInfo` | `VmdMotionInfo` | `com.ai.assistance.mmd` | `MmdInspector.kt` | class VmdMotionInfo(val modelName: String, val motionCount: Int, val morphCount: Int, val cameraCount: Int, val lightCount: Int, val shadowCount: Int, val ikCount: Int) |  | 21 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `ExampleInstrumentedTest.useAppContext` | `ExampleInstrumentedTest` | `com.ai.assistance.operit` | `ExampleInstrumentedTest.kt` |  | Unit |  | 19 ⚑ |
| `FbxGlSurfaceView.setModelPath` | `FbxGlSurfaceView` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | path: String | Unit |  | 46 |
| `FbxGlSurfaceView.setAnimationState` | `FbxGlSurfaceView` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | animationName: String?<br>isLooping: Boolean<br>playbackNonce: Long | Unit |  | 52 |
| `FbxGlSurfaceView.setCameraPose` | `FbxGlSurfaceView` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | pitchDegrees: Float<br>yawDegrees: Float<br>distanceScale: Float<br>targetHeightOffset: Float | Unit |  | 62 |
| `FbxGlSurfaceView.setOnRenderErrorListener` | `FbxGlSurfaceView` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | listener: ((String) -> Unit)? | Unit |  | 78 |
| `FbxGlSurfaceView.setOnAnimationsDiscoveredListener` | `FbxGlSurfaceView` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | listener: ((List<String>, Map<String, Long>) … | Unit |  | 82 |
| `FbxGlSurfaceView.onDetachedFromWindow` | `FbxGlSurfaceView` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` |  | Unit |  | 86 |
| `FbxPreviewInfo.fromJson` | `FbxPreviewInfo` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | rawJson: String | FbxPreviewInfo |  | 125 |
| `FbxPreviewRenderer.setOnErrorListener` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | listener: ((String) -> Unit)? | Unit |  | 307 |
| `FbxPreviewRenderer.setOnAnimationsDiscoveredListener` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | listener: ((List<String>, Map<String, Long>) … | Unit |  | 311 |
| `FbxPreviewRenderer.setModelPath` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | path: String | Unit |  | 315 |
| `FbxPreviewRenderer.setAnimationState` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | animationName: String?<br>isLooping: Boolean<br>playbackNonce: Long | Unit |  | 327 |
| `FbxPreviewRenderer.setCameraPose` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | pitchDegrees: Float<br>yawDegrees: Float<br>distanceScale: Float<br>targetHeightOffset: Float | Unit |  | 343 |
| `FbxPreviewRenderer.onSurfaceCreated` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | gl: GL10?<br>config: EGLConfig? | Unit |  | 355 |
| `FbxPreviewRenderer.onSurfaceChanged` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | gl: GL10?<br>width: Int<br>height: Int | Unit |  | 377 |
| `FbxPreviewRenderer.onDrawFrame` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | gl: GL10? | Unit |  | 382 |
| `FbxPreviewRenderer.release` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` |  | Unit |  | 418 |
| `FbxPreviewRenderer.loadPreviewAssets` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | modelPath: String | Unit |  | 424 |
| `FbxPreviewRenderer.loadTextureSlots` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | handle: Long<br>info: FbxPreviewInfo | List<LoadedTextureSlot> |  | 463 |
| `FbxPreviewRenderer.loadTextureFromBytes` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | bytes: ByteArray | LoadedTextureSlot |  | 475 |
| `FbxPreviewRenderer.loadTextureFromFile` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | path: String | LoadedTextureSlot |  | 480 |
| `FbxPreviewRenderer.uploadBitmapTexture` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | bitmap: Bitmap | LoadedTextureSlot |  | 490 |
| `FbxPreviewRenderer.updateVertexBuffer` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | frameVertices: FloatArray | Boolean |  | 511 |
| `FbxPreviewRenderer.updateCamera` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | info: FbxPreviewInfo | Unit |  | 539 |
| `FbxPreviewRenderer.drawScene` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | info: FbxPreviewInfo<br>handles: IntArray | Unit |  | 575 |
| `FbxPreviewRenderer.drawSegment` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | segment: FbxPreviewSegment<br>info: FbxPreviewInfo<br>handles: IntArray | Unit |  | 610 |
| `FbxPreviewRenderer.isSegmentTransparent` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | segment: FbxPreviewSegment | Boolean |  | 638 |
| `FbxPreviewRenderer.createProgramHandles` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` |  | IntArray? |  | 648 |
| `FbxPreviewRenderer.createProgram` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | vertexCode: String<br>fragmentCode: String | Int |  | 671 |
| `FbxPreviewRenderer.loadShader` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | type: Int<br>shaderCode: String | Int |  | 709 |
| `FbxPreviewRenderer.releaseSession` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` |  | Unit |  | 729 |
| `FbxPreviewRenderer.clearTextures` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` |  | Unit |  | 740 |
| `FbxPreviewRenderer.clearProgram` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` |  | Unit |  | 748 |
| `FbxPreviewRenderer.dispatchOnce` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | message: String | Unit |  | 755 |
| `FbxPreviewRenderer.dispatchError` | `FbxPreviewRenderer` | `com.ai.assistance.fbx` | `FbxGlSurfaceView.kt` | message: String | Unit |  | 763 |
| `FbxInspector.isAvailable` | `FbxInspector` | `com.ai.assistance.fbx` | `FbxInspector.kt` |  | Boolean |  | 19 |
| `FbxInspector.unavailableReason` | `FbxInspector` | `com.ai.assistance.fbx` | `FbxInspector.kt` |  | String |  | 21 |
| `FbxInspector.getLastError` | `FbxInspector` | `com.ai.assistance.fbx` | `FbxInspector.kt` |  | String |  | 23 |
| `FbxInspector.inspectModel` | `FbxInspector` | `com.ai.assistance.fbx` | `FbxInspector.kt` | pathModel: String | FbxModelInfo? |  | 25 |
| `FbxLibraryLoader.loadLibraries` | `FbxLibraryLoader` | `com.ai.assistance.fbx` | `FbxLibraryLoader.kt` |  | Unit |  | 9 |
| `FbxNative.nativeIsAvailable` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` |  | Boolean |  | 9 |
| `FbxNative.nativeGetUnavailableReason` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` |  | String |  | 11 |
| `FbxNative.nativeGetLastError` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` |  | String |  | 13 |
| `FbxNative.nativeInspectModel` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` | pathModel: String | String? |  | 15 |
| `FbxNative.nativeCreatePreviewSession` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` | pathModel: String | Long |  | 17 |
| `FbxNative.nativeDestroyPreviewSession` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` | sessionHandle: Long | Unit |  | 19 |
| `FbxNative.nativeReadPreviewInfo` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` | sessionHandle: Long | String? |  | 21 |
| `FbxNative.nativeBuildPreviewFrame` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` | sessionHandle: Long<br>animationName: String?<br>timeSeconds: Double | FloatArray? |  | 23 |
| `FbxNative.nativeReadEmbeddedTextureBytes` | `FbxNative` | `com.ai.assistance.fbx` | `FbxNative.kt` | sessionHandle: Long<br>textureIndex: Int | ByteArray? |  | 29 |
| `MmdGlSurfaceView.setModelPath` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | path: String | Unit |  | 43 |
| `MmdGlSurfaceView.setAnimationState` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | animationName: String?<br>isLooping: Boolean | Unit |  | 49 |
| `MmdGlSurfaceView.setModelRotation` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | rotationX: Float<br>rotationY: Float<br>rotationZ: Float | Unit |  | 55 |
| `MmdGlSurfaceView.setCameraDistanceScale` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | scale: Float | Unit |  | 61 |
| `MmdGlSurfaceView.setCameraTargetHeight` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | height: Float | Unit |  | 67 |
| `MmdGlSurfaceView.setOnRenderErrorListener` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | listener: ((String) -> Unit)? | Unit |  | 73 |
| `MmdGlSurfaceView.onResume` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` |  | Unit |  | 77 |
| `MmdGlSurfaceView.onPause` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` |  | Unit |  | 85 |
| `MmdGlSurfaceView.onDetachedFromWindow` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` |  | Unit |  | 92 |
| `MmdGlSurfaceView.requestHighRefreshRateIfSupported` | `MmdGlSurfaceView` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` |  | Unit |  | 103 |
| `NativeMmdRenderer.setOnErrorListener` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | listener: ((String) -> Unit)? | Unit |  | 151 |
| `NativeMmdRenderer.setModelPath` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | path: String | Unit |  | 155 |
| `NativeMmdRenderer.setAnimationState` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | animationName: String?<br>isLooping: Boolean | Unit |  | 167 |
| `NativeMmdRenderer.setModelRotation` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | rotationX: Float<br>rotationY: Float<br>rotationZ: Float | Unit |  | 189 |
| `NativeMmdRenderer.setCameraDistanceScale` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | scale: Float | Unit |  | 198 |
| `NativeMmdRenderer.setCameraTargetHeight` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | height: Float | Unit |  | 205 |
| `NativeMmdRenderer.pauseRenderer` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` |  | Unit |  | 212 |
| `NativeMmdRenderer.resumeRenderer` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` |  | Unit |  | 218 |
| `NativeMmdRenderer.releaseRenderer` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` |  | Unit |  | 224 |
| `NativeMmdRenderer.onSurfaceCreated` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | gl: GL10?<br>config: EGLConfig? | Unit |  | 232 |
| `NativeMmdRenderer.onSurfaceChanged` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | gl: GL10?<br>width: Int<br>height: Int | Unit |  | 246 |
| `NativeMmdRenderer.onDrawFrame` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | gl: GL10? | Unit |  | 254 |
| `NativeMmdRenderer.syncRequestedState` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` |  | Unit |  | 273 |
| `NativeMmdRenderer.dispatchError` | `NativeMmdRenderer` | `com.ai.assistance.mmd` | `MmdGlSurfaceView.kt` | message: String | Unit |  | 293 |
| `MmdInspector.isAvailable` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` |  | Boolean |  | 38 |
| `MmdInspector.unavailableReason` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` |  | String |  | 40 |
| `MmdInspector.getLastError` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` |  | String |  | 42 |
| `MmdInspector.inspectModel` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` | pathModel: String | MmdModelInfo? |  | 44 |
| `MmdInspector.inspectMotion` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` | pathMotion: String | VmdMotionInfo? |  | 69 |
| `MmdLibraryLoader.loadLibraries` | `MmdLibraryLoader` | `com.ai.assistance.mmd` | `MmdLibraryLoader.kt` |  | Unit |  | 9 |
| `MmdNative.nativeIsAvailable` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` |  | Boolean |  | 11 |
| `MmdNative.nativeGetUnavailableReason` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` |  | String |  | 13 |
| `MmdNative.nativeGetLastError` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` |  | String |  | 15 |
| `MmdNative.nativeReadModelName` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | pathModel: String | String? |  | 17 |
| `MmdNative.nativeReadModelSummary` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | pathModel: String | LongArray? |  | 19 |
| `MmdNative.nativeReadMotionModelName` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | pathMotion: String | String? |  | 21 |
| `MmdNative.nativeReadMotionSummary` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | pathMotion: String | LongArray? |  | 23 |
| `MmdNative.nativeReadMotionMaxFrame` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | pathMotion: String | Int |  | 25 |
| `MmdNative.nativeCreateRenderer` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` |  | Long |  | 27 |
| `MmdNative.nativeDestroyRenderer` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long | Unit |  | 29 |
| `MmdNative.nativeOnSurfaceCreated` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long<br>assetManager: AssetManager | Unit |  | 31 |
| `MmdNative.nativeOnSurfaceChanged` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long<br>width: Int<br>height: Int | Unit |  | 33 |
| `MmdNative.nativeRender` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long | Boolean |  | 35 |
| `MmdNative.nativePause` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long | Unit |  | 37 |
| `MmdNative.nativeResume` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long | Unit |  | 39 |
| `MmdNative.nativeSetModelPath` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long<br>pathModel: String? | Unit |  | 41 |
| `MmdNative.nativeSetAnimationState` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long<br>animationName: String?<br>isLooping: Boolean | Unit |  | 43 |
| `MmdNative.nativeSetModelRotation` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long<br>rotationX: Float<br>rotationY: Float<br>rotationZ: Float | Unit |  | 49 |
| `MmdNative.nativeSetCameraDistanceScale` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long<br>scale: Float | Unit |  | 56 |
| `MmdNative.nativeSetCameraTargetHeight` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long<br>height: Float | Unit |  | 58 |
| `MmdNative.nativeGetRendererLastError` | `MmdNative` | `com.ai.assistance.mmd` | `MmdNative.kt` | handle: Long | String |  | 60 |
| `LlamaLibraryLoader.loadLibraries` | `LlamaLibraryLoader` | `com.ai.assistance.llama` | `LlamaLibraryLoader.kt` |  | Unit |  | 9 |
| `LlamaNative.nativeIsAvailable` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` |  | Boolean |  | 9 |
| `LlamaNative.nativeGetUnavailableReason` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` |  | String |  | 11 |
| `LlamaNative.nativeCreateSession` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | pathModel: String<br>nThreads: Int<br>nCtx: Int<br>nBatch: Int<br>nUBatch: Int<br>nGpuLayers: Int<br>useMmap: Boolean<br>flashAttention: Boolean<br>kvUnified: Boolean<br>offloadKqv: Boolean | Long |  | 14 |
| `LlamaNative.nativeReleaseSession` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | sessionPtr: Long | Unit |  | 27 |
| `LlamaNative.nativeCancel` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | sessionPtr: Long | Unit |  | 29 |
| `LlamaNative.nativeCountTokens` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | sessionPtr: Long<br>text: String | Int |  | 31 |
| `LlamaNative.nativeSetSamplingParams` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | sessionPtr: Long<br>temperature: Float<br>topP: Float<br>topK: Int<br>repetitionPenalty: Float<br>frequencyPenalty: Float<br>presencePenalty: Float<br>penaltyLastN: Int | Boolean |  | 34 |
| `LlamaNative.nativeApplyChatTemplate` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | sessionPtr: Long<br>roles: Array<String><br>contents: Array<String><br>enableThinking: Boolean<br>addAssistant: Boolean | String? |  | 46 |
| `LlamaNative.nativeApplyStructuredChatTemplate` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | sessionPtr: Long<br>messagesJson: String<br>toolsJson: String?<br>enableThinking: Boolean<br>addAssistant: Boolean | String? |  | 55 |
| `LlamaNative.nativeGenerateStream` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | sessionPtr: Long<br>prompt: String<br>maxTokens: Int<br>callback: GenerationCallback | Boolean |  | 64 |
| `LlamaNative.nativeClearToolCallGrammar` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | sessionPtr: Long | Boolean |  | 72 |
| `LlamaNative.nativeParseToolCallResponse` | `LlamaNative` | `com.ai.assistance.llama` | `LlamaNative.kt` | sessionPtr: Long<br>content: String | String? |  | 75 |
| `LlamaNative.GenerationCallback.onToken` | `GenerationCallback` | `com.ai.assistance.llama` | `LlamaNative.kt` | token: String | Boolean |  | 81 |
| `LlamaSession.isAvailable` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` |  | Boolean |  | 20 |
| `LlamaSession.getUnavailableReason` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` |  | String |  | 22 |
| `LlamaSession.create` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | pathModel: String<br>config: Config | LlamaSession? |  | 25 |
| `LlamaSession.checkValid` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` |  | Unit |  | 52 |
| `LlamaSession.countTokens` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | text: String | Int |  | 58 |
| `LlamaSession.generateStream` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | prompt: String<br>maxTokens: Int<br>onToken: (String) -> Boolean | Boolean |  | 65 |
| `LlamaSession.onToken` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | token: String | Boolean |  | 77 |
| `LlamaSession.applyStructuredChatTemplate` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | messagesJson: String<br>toolsJson: String?<br>enableThinking: Boolean<br>addAssistant: Boolean | String? |  | 82 |
| `LlamaSession.clearToolCallGrammar` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` |  | Boolean |  | 103 |
| `LlamaSession.parseToolCallResponse` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | content: String | String? |  | 113 |
| `LlamaSession.applyChatTemplate` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | roles: List<String><br>contents: List<String><br>enableThinking: Boolean<br>addAssistant: Boolean | String? |  | 123 |
| `LlamaSession.setSamplingParams` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` | temperature: Float<br>topP: Float<br>topK: Int<br>repetitionPenalty: Float<br>frequencyPenalty: Float<br>presencePenalty: Float<br>penaltyLastN: Int? | Boolean |  | 144 |
| `LlamaSession.cancel` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` |  | Unit |  | 171 |
| `LlamaSession.release` | `LlamaSession` | `com.ai.assistance.llama` | `LlamaSession.kt` |  | Unit |  | 178 |
| `MNNImageProcess.Config.equals` | `Config` | `com.ai.assistance.mnn` | `MNNImageProcess.kt` | other: Any? | Boolean |  | 67 |
| `MNNImageProcess.Config.hashCode` | `Config` | `com.ai.assistance.mnn` | `MNNImageProcess.kt` |  | Int |  | 83 |
| `MNNImageProcess.convertBuffer` | `MNNImageProcess` | `com.ai.assistance.mnn` | `MNNImageProcess.kt` | buffer: ByteArray<br>width: Int<br>height: Int<br>tensor: MNNNetInstance.Session.Tensor<br>config: Config<br>matrix: Matrix?? | Boolean | 设置输入 buffer | 105 |
| `MNNImageProcess.convertBitmap` | `MNNImageProcess` | `com.ai.assistance.mnn` | `MNNImageProcess.kt` | sourceBitmap: Bitmap<br>tensor: MNNNetInstance.Session.Tensor<br>config: Config<br>matrix: Matrix?? | Boolean | 设置 bitmap 输入 | 133 |
| `MNNLibraryLoader.loadLibraries` | `MNNLibraryLoader` | `com.ai.assistance.mnn` | `MNNLibraryLoader.kt` |  | Unit | 加载 MNN 库 如果库已经加载，则不会重复加载 | 21 |
| `MNNLibraryLoader.isLoaded` | `MNNLibraryLoader` | `com.ai.assistance.mnn` | `MNNLibraryLoader.kt` |  | Boolean | 检查库是否已加载 | 51 |
| `MNNLlmContextInfo.fromJson` | `MNNLlmContextInfo` | `com.ai.assistance.mnn` | `MNNLlmContextInfo.kt` | json: String | MNNLlmContextInfo |  | 28 |
| `MNNLlmContextInfo.optIntArray` | `MNNLlmContextInfo` | `com.ai.assistance.mnn` | `MNNLlmContextInfo.kt` | name: String | IntArray |  | 51 |
| `MNNLlmNative.nativeCreateLlm` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | configPath: String | Long | 从配置文件创建 LLM 实例（不加载模型） | 20 |
| `MNNLlmNative.nativeLoadLlm` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long | Boolean | 加载 LLM 模型（必须在设置配置后调用） | 28 |
| `MNNLlmNative.nativeReleaseLlm` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long | Unit | 释放 LLM 实例 | 35 |
| `MNNLlmNative.nativeTokenize` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>text: String | IntArray? | 将文本编码为 token IDs | 44 |
| `MNNLlmNative.nativeDetokenize` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>token: Int | String? | 将单个 token ID 解码为文本 | 53 |
| `MNNLlmNative.nativeCountTokens` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>text: String | Int |  | 56 |
| `MNNLlmNative.nativeGenerate` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>prompt: String<br>maxTokens: Int<br>callback: GenerationCallback? | String? | 生成文本（非流式） | 67 |
| `MNNLlmNative.nativeGenerateStream` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>history: List<Pair<String, String>><br>maxTokens: Int<br>callback: GenerationCallback | Boolean | 流式生成文本（带历史记录） | 83 |
| `MNNLlmNative.nativeGenerateStreamStructured` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>messagesJson: String<br>toolsJson: String?<br>maxTokens: Int<br>callback: GenerationCallback | Boolean |  | 91 |
| `MNNLlmNative.nativeApplyChatTemplateWithHistory` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>history: List<Pair<String, String>> | String? |  | 100 |
| `MNNLlmNative.nativeApplyChatTemplateWithStructuredMessages` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>messagesJson: String<br>toolsJson: String? | String? |  | 106 |
| `MNNLlmNative.nativeCountTokensWithHistory` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>history: List<Pair<String, String>> | Int |  | 113 |
| `MNNLlmNative.nativeCountTokensWithStructuredMessages` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>messagesJson: String<br>toolsJson: String? | Int |  | 119 |
| `MNNLlmNative.nativeDumpConfig` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long | String? | 导出当前生效的 LLM 配置。 | 131 |
| `MNNLlmNative.nativeGetContextInfo` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long | String? | 导出最近一次推理上下文信息。 | 139 |
| `MNNLlmNative.nativeApplyChatTemplate` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>userContent: String | String? | 应用聊天模板 | 148 |
| `MNNLlmNative.nativeReset` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long | Unit | 重置 LLM 状态（清除 KV-Cache 和历史） | 155 |
| `MNNLlmNative.nativeSetConfig` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>configJson: String | Boolean | 设置 LLM 配置（用于运行时修改配置） | 164 |
| `MNNLlmNative.nativeSetAudioDataCallback` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long<br>callback: AudioDataCallback? | Boolean | 注册或清除音频数据回调。 | 173 |
| `MNNLlmNative.nativeGenerateWavform` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long | Boolean | 触发语音波形生成。 仅对支持语音输出的模型有效。 | 185 |
| `MNNLlmNative.nativeCancel` | `MNNLlmNative` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | llmPtr: Long | Unit | 取消当前的生成任务 | 192 |
| `MNNLlmNative.GenerationCallback.onToken` | `GenerationCallback` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | token: String | Boolean | 当生成新的 token 时调用 | 203 |
| `MNNLlmNative.AudioDataCallback.onAudioData` | `AudioDataCallback` | `com.ai.assistance.mnn` | `MNNLlmNative.kt` | audioData: FloatArray<br>isLastChunk: Boolean | Boolean |  | 211 |
| `MNNLlmSession.create` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | modelDir: String<br>backendType: String?<br>threadNum: Int?<br>precision: String?<br>memory: String?<br>tmpPath: String?? | MNNLlmSession? | 从模型目录创建 LLM 会话 | 29 |
| `MNNLlmSession.withActiveCall` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | block: (Long) -> T | T |  | 96 |
| `MNNLlmSession.checkValid` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | Unit | 检查会话是否有效 | 117 |
| `MNNLlmSession.tokenize` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | text: String | IntArray | 将文本编码为 token IDs | 126 |
| `MNNLlmSession.detokenize` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | token: Int | String | 将 token ID 解码为文本 | 136 |
| `MNNLlmSession.countTokens` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | text: String | Int |  | 143 |
| `MNNLlmSession.countTokensWithHistory` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | history: List<Pair<String, String>> | Int |  | 149 |
| `MNNLlmSession.countTokensStructured` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | messagesJson: String<br>toolsJson: String?? | Int |  | 155 |
| `MNNLlmSession.dumpConfig` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | String | 导出当前生效的配置。 | 164 |
| `MNNLlmSession.getContextInfo` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | MNNLlmContextInfo? | 获取最近一次推理的上下文统计。 在尚未执行推理时可能返回 null。 | 175 |
| `MNNLlmSession.applyChatTemplate` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | userContent: String | String | 应用聊天模板 | 184 |
| `MNNLlmSession.applyChatTemplate` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | history: List<Pair<String, String>> | String | 对完整历史应用聊天模板。 | 194 |
| `MNNLlmSession.applyChatTemplateStructured` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | messagesJson: String<br>toolsJson: String?? | String |  | 201 |
| `MNNLlmSession.generate` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | prompt: String<br>maxTokens: Int? | String | 非流式生成 | 214 |
| `MNNLlmSession.generateStream` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | history: List<Pair<String, String>><br>maxTokens: Int?<br>onToken: (String) -> Boolean | Boolean | 流式生成（带历史记录） | 228 |
| `MNNLlmSession.onToken` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | token: String | Boolean |  | 234 |
| `MNNLlmSession.generateStreamStructured` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | messagesJson: String<br>toolsJson: String??<br>maxTokens: Int?<br>onToken: (String) -> Boolean | Boolean |  | 249 |
| `MNNLlmSession.onToken` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | token: String | Boolean |  | 256 |
| `MNNLlmSession.chat` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | userContent: String<br>maxTokens: Int?<br>onToken: (String) -> Boolean | Boolean | 聊天生成（应用模板后生成） | 278 |
| `MNNLlmSession.reset` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | Unit | 重置会话（清除历史和 KV-Cache） | 291 |
| `MNNLlmSession.cancel` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | Unit | 取消当前的生成任务 这会立即中断正在进行的推理过程 | 302 |
| `MNNLlmSession.setConfig` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | configJson: String | Boolean | 设置 LLM 配置 | 318 |
| `MNNLlmSession.setMaxNewTokens` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | maxNewTokens: Int | Boolean | 更新 max_new_tokens 配置。 | 333 |
| `MNNLlmSession.setSystemPrompt` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | systemPrompt: String | Boolean | 更新 system_prompt 配置。 | 340 |
| `MNNLlmSession.setAssistantPromptTemplate` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | template: String | Boolean | 更新 assistant_prompt_template 配置。 | 347 |
| `MNNLlmSession.setThinkingMode` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | enabled: Boolean | Boolean | 启用或禁用 thinking 模式（仅对支持的模型有效，如 Qwen3） | 356 |
| `MNNLlmSession.setAudioDataCallback` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` | callback: MNNLlmNative.AudioDataCallback? | Boolean | 注册或清除音频波形回调。 | 372 |
| `MNNLlmSession.generateWavform` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | Boolean | 触发语音波形生成。 | 381 |
| `MNNLlmSession.release` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | Unit | 释放会话 | 390 |
| `MNNLlmSession.getModelPath` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | String | 获取模型路径 | 421 |
| `MNNLlmSession.isReleased` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | Boolean | 检查会话是否已释放 | 426 |
| `MNNLlmSession.finalize` | `MNNLlmSession` | `com.ai.assistance.mnn` | `MNNLlmSession.kt` |  | Unit |  | 428 |
| `MNNModule.load` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | filePath: String<br>config: Config | MNNModule? | 从文件加载模型 | 24 |
| `MNNModule.Variable.setFloatData` | `Variable` | `com.ai.assistance.mnn` | `MNNModule.kt` | data: FloatArray | Boolean | 设置浮点数据 | 103 |
| `MNNModule.Variable.setIntData` | `Variable` | `com.ai.assistance.mnn` | `MNNModule.kt` | data: IntArray | Boolean | 设置整型数据 | 111 |
| `MNNModule.Variable.getFloatData` | `Variable` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | FloatArray? | 获取浮点数据 | 119 |
| `MNNModule.Variable.getShape` | `Variable` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | IntArray? | 获取形状 | 127 |
| `MNNModule.Variable.release` | `Variable` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | Unit | 释放变量 | 135 |
| `MNNModule.Variable.getPtr` | `Variable` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | Long |  | 142 |
| `MNNModule.Variable.checkValid` | `Variable` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | Unit |  | 144 |
| `MNNModule.Variable.finalize` | `Variable` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | Unit |  | 150 |
| `MNNModule.createInputVariable` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | shape: IntArray<br>dataFormat: Int?<br>dataType: Int? | Variable? | 创建输入变量 | 162 |
| `MNNModule.forward` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` | inputs: List<Variable> | List<Variable>? | 执行前向推理 | 183 |
| `MNNModule.getInputNames` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | List<String> | 获取输入名称列表 | 208 |
| `MNNModule.getOutputNames` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | List<String> | 获取输出名称列表 | 213 |
| `MNNModule.release` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | Unit | 释放模块 | 218 |
| `MNNModule.checkValid` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | Unit |  | 226 |
| `MNNModule.finalize` | `MNNModule` | `com.ai.assistance.mnn` | `MNNModule.kt` |  | Unit |  | 232 |
| `MNNModuleNative.nativeCreateModuleFromFile` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | filePath: String<br>inputs: Array<String><br>outputs: Array<String><br>forwardType: Int<br>numThread: Int<br>precision: Int<br>memoryMode: Int | Long | 从文件创建 Module | 25 |
| `MNNModuleNative.nativeReleaseModule` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | modulePtr: Long | Unit | 释放 Module | 40 |
| `MNNModuleNative.nativeForward` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | modulePtr: Long<br>inputVarPtrs: LongArray | LongArray? | 执行前向推理 | 49 |
| `MNNModuleNative.nativeCreateInputVar` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | shape: IntArray<br>dataFormat: Int<br>dataType: Int | Long | 创建输入变量 | 59 |
| `MNNModuleNative.nativeSetVarFloatData` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | varPtr: Long<br>data: FloatArray | Boolean | 设置变量的浮点数据 | 68 |
| `MNNModuleNative.nativeSetVarIntData` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | varPtr: Long<br>data: IntArray | Boolean | 设置变量的整型数据 | 77 |
| `MNNModuleNative.nativeGetVarFloatData` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | varPtr: Long | FloatArray? | 获取变量的浮点数据 | 85 |
| `MNNModuleNative.nativeGetVarShape` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | varPtr: Long | IntArray? | 获取变量的形状 | 93 |
| `MNNModuleNative.nativeReleaseVar` | `MNNModuleNative` | `com.ai.assistance.mnn` | `MNNModuleNative.kt` | varPtr: Long | Unit | 释放变量 | 100 |
| `MNNNetInstance.createFromFile` | `MNNNetInstance` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | fileName: String | MNNNetInstance? | 从文件创建 MNN 网络实例 | 20 |
| `MNNNetInstance.createFromBuffer` | `MNNNetInstance` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | buffer: ByteArray | MNNNetInstance? | 从字节数组创建 MNN 网络实例 | 35 |
| `MNNNetInstance.Config.equals` | `Config` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | other: Any? | Boolean |  | 54 |
| `MNNNetInstance.Config.hashCode` | `Config` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | Int |  | 74 |
| `MNNNetInstance.Session.Tensor.instance` | `Tensor` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | Long |  | 96 |
| `MNNNetInstance.Session.Tensor.reshape` | `Tensor` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | dims: IntArray | Unit | 重塑张量形状 | 101 |
| `MNNNetInstance.Session.Tensor.setInputIntData` | `Tensor` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | data: IntArray | Unit | 设置整型输入数据 | 109 |
| `MNNNetInstance.Session.Tensor.setInputFloatData` | `Tensor` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | data: FloatArray | Unit | 设置浮点输入数据 | 117 |
| `MNNNetInstance.Session.Tensor.getDimensions` | `Tensor` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | IntArray | 获取张量维度 | 125 |
| `MNNNetInstance.Session.Tensor.getFloatData` | `Tensor` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | FloatArray | 获取浮点数据 | 132 |
| `MNNNetInstance.Session.Tensor.getIntData` | `Tensor` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | IntArray | 获取整型数据 | 140 |
| `MNNNetInstance.Session.Tensor.getData` | `Tensor` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | Unit | 获取数据 | 152 |
| `MNNNetInstance.Session.Tensor.getUINT8Data` | `Tensor` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | ByteArray | 获取 UINT8 数据 | 163 |
| `MNNNetInstance.Session.reshape` | `Session` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | Unit | 在所有输入张量 reshape 后调用此方法 | 176 |
| `MNNNetInstance.Session.run` | `Session` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | Unit | 运行推理 | 183 |
| `MNNNetInstance.Session.runWithCallback` | `Session` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | names: Array<String> | Array<Tensor> | 使用回调运行推理 | 190 |
| `MNNNetInstance.Session.getInput` | `Session` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | name: String? | Tensor? | 获取输入张量 | 199 |
| `MNNNetInstance.Session.getOutput` | `Session` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | name: String? | Tensor? | 获取输出张量 | 211 |
| `MNNNetInstance.Session.release` | `Session` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | Unit | 从网络实例中释放会话，如果调用了 net.release() 则不需要调用此方法 | 223 |
| `MNNNetInstance.createSession` | `MNNNetInstance` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` | config: Config?? | Session? | 创建会话 | 233 |
| `MNNNetInstance.checkValid` | `MNNNetInstance` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | Unit |  | 252 |
| `MNNNetInstance.release` | `MNNNetInstance` | `com.ai.assistance.mnn` | `MNNNetInstance.kt` |  | Unit | 释放网络实例 | 261 |
| `MNNNetNative.nativeCreateNetFromFile` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | modelName: String | Long | Net | 17 |
| `MNNNetNative.nativeCreateNetFromBuffer` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | buffer: ByteArray | Long |  | 20 |
| `MNNNetNative.nativeReleaseNet` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long | Long |  | 23 |
| `MNNNetNative.nativeCreateSession` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>forwardType: Int<br>numThread: Int<br>saveTensors: Array<String>?<br>outputTensors: Array<String>? | Long | Session | 27 |
| `MNNNetNative.nativeReleaseSession` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>sessionPtr: Long | Unit |  | 36 |
| `MNNNetNative.nativeRunSession` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>sessionPtr: Long | Int |  | 39 |
| `MNNNetNative.nativeRunSessionWithCallback` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>sessionPtr: Long<br>nameArray: Array<String><br>tensorAddr: LongArray | Int |  | 42 |
| `MNNNetNative.nativeReshapeSession` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>sessionPtr: Long | Int |  | 50 |
| `MNNNetNative.nativeGetSessionInput` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>sessionPtr: Long<br>name: String? | Long |  | 53 |
| `MNNNetNative.nativeGetSessionOutput` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>sessionPtr: Long<br>name: String? | Long |  | 56 |
| `MNNNetNative.nativeReshapeTensor` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>tensorPtr: Long<br>dims: IntArray | Unit | Tensor | 60 |
| `MNNNetNative.nativeTensorGetDimensions` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | tensorPtr: Long | IntArray |  | 63 |
| `MNNNetNative.nativeSetInputIntData` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>tensorPtr: Long<br>data: IntArray | Unit |  | 66 |
| `MNNNetNative.nativeSetInputFloatData` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | netPtr: Long<br>tensorPtr: Long<br>data: FloatArray | Unit |  | 69 |
| `MNNNetNative.nativeTensorGetData` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | tensorPtr: Long<br>dest: FloatArray? | Int |  | 72 |
| `MNNNetNative.nativeTensorGetIntData` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | tensorPtr: Long<br>dest: IntArray? | Int |  | 75 |
| `MNNNetNative.nativeTensorGetUINT8Data` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | tensorPtr: Long<br>dest: ByteArray? | Int |  | 78 |
| `MNNNetNative.nativeConvertBitmapToTensor` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | srcBitmap: Bitmap<br>tensorPtr: Long<br>destFormat: Int<br>filterType: Int<br>wrap: Int<br>matrixValue: FloatArray<br>mean: FloatArray<br>normal: FloatArray | Boolean | ImageProcess | 82 |
| `MNNNetNative.nativeConvertBufferToTensor` | `MNNNetNative` | `com.ai.assistance.mnn` | `MNNNetNative.kt` | bufferData: ByteArray<br>width: Int<br>height: Int<br>tensorPtr: Long<br>srcFormat: Int<br>destFormat: Int<br>filterType: Int<br>wrap: Int<br>matrixValue: FloatArray<br>mean: FloatArray<br>normal: FloatArray | Boolean |  | 94 |
| `run` | — | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | command: String<br>identity: ShellIdentity | ShellCommandResult |  | 31 |
| `log` | — | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | priority: Int<br>tag: String<br>message: String<br>throwable: Throwable? | Unit |  | 41 |
| `ShowerLog.emit` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | priority: Int<br>tag: String<br>message: String<br>throwable: Throwable?? | Unit |  | 74 |
| `ShowerLog.v` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String | Unit |  | 94 |
| `ShowerLog.v` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String<br>throwable: Throwable | Unit |  | 95 |
| `ShowerLog.d` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String | Unit |  | 96 |
| `ShowerLog.d` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String<br>throwable: Throwable | Unit |  | 97 |
| `ShowerLog.i` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String | Unit |  | 98 |
| `ShowerLog.i` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String<br>throwable: Throwable | Unit |  | 99 |
| `ShowerLog.w` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String | Unit |  | 100 |
| `ShowerLog.w` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String<br>throwable: Throwable | Unit |  | 101 |
| `ShowerLog.e` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String | Unit |  | 102 |
| `ShowerLog.e` | `ShowerLog` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | tag: String<br>message: String<br>throwable: Throwable | Unit |  | 103 |
| `ShowerBinderRegistry.setService` | `ShowerBinderRegistry` | `com.ai.assistance.showerclient` | `ShowerBinderRegistry.kt` | newService: IShowerService? | Unit |  | 19 |
| `ShowerBinderRegistry.getService` | `ShowerBinderRegistry` | `com.ai.assistance.showerclient` | `ShowerBinderRegistry.kt` |  | IShowerService? |  | 25 |
| `ShowerBinderRegistry.hasAliveService` | `ShowerBinderRegistry` | `com.ai.assistance.showerclient` | `ShowerBinderRegistry.kt` |  | Boolean |  | 27 |
| `ShowerController.alignToCodecBlockSize` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | value: Int | Int |  | 31 |
| `ShowerController.getBinder` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | context: Context?? | IShowerService? |  | 34 |
| `ShowerController.clearDeadService` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` |  | Unit |  | 39 |
| `ShowerController.getDisplayId` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` |  | Int? |  | 90 |
| `ShowerController.getVideoSize` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` |  | Pair<Int, Int>? |  | 98 |
| `ShowerController.setBinaryHandler` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | handler: ((ByteArray) -> Unit)? | Unit |  | 107 |
| `ShowerController.onVideoFrame` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | data: ByteArray | Unit |  | 132 |
| `ShowerController.requestScreenshot` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | timeoutMs: Long? | ByteArray? |  | 147 |
| `ShowerController.prepareMainDisplay` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | context: Context | Boolean | Prepares this controller to inject input on the physical main display (displayId=0) witho… | 165 |
| `ShowerController.clearCachedBinder` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` |  | Unit |  | 166 |
| `ShowerController.resetLocalDisplayState` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` |  | Unit |  | 171 |
| `ShowerController.isBinderDied` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | e: Throwable | Boolean |  | 177 |
| `ShowerController.doPrepare` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | service: IShowerService | Boolean |  | 181 |
| `ShowerController.ensureDisplay` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | context: Context<br>width: Int<br>height: Int<br>dpi: Int<br>bitrateKbps: Int?? | Boolean |  | 234 |
| `ShowerController.clearCachedBinder` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` |  | Unit |  | 241 |
| `ShowerController.resetLocalDisplayState` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` |  | Unit |  | 246 |
| `ShowerController.isBinderDied` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | e: Throwable | Boolean |  | 252 |
| `ShowerController.doEnsure` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | service: IShowerService | Boolean |  | 260 |
| `ShowerController.launchApp` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | packageName: String | Boolean |  | 327 |
| `ShowerController.tap` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | x: Int<br>y: Int | Boolean |  | 340 |
| `ShowerController.swipe` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | startX: Int<br>startY: Int<br>endX: Int<br>endY: Int<br>durationMs: Long? | Boolean |  | 352 |
| `ShowerController.touchDown` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | x: Int<br>y: Int | Boolean |  | 370 |
| `ShowerController.touchMove` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | x: Int<br>y: Int | Boolean |  | 382 |
| `ShowerController.touchUp` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | x: Int<br>y: Int | Boolean |  | 394 |
| `ShowerController.injectTouchEvent` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | action: Int<br>x: Float<br>y: Float<br>downTime: Long<br>eventTime: Long<br>pressure: Float<br>size: Float<br>metaState: Int<br>xPrecision: Float<br>yPrecision: Float<br>deviceId: Int<br>edgeFlags: Int | Boolean |  | 406 |
| `ShowerController.shutdown` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` |  | Unit |  | 445 |
| `ShowerController.key` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | keyCode: Int | Boolean |  | 466 |
| `ShowerController.keyWithMeta` | `ShowerController` | `com.ai.assistance.showerclient` | `ShowerController.kt` | keyCode: Int<br>metaState: Int | Boolean |  | 470 |
| `ShowerServerManager.ensureServerStarted` | `ShowerServerManager` | `com.ai.assistance.showerclient` | `ShowerServerManager.kt` | context: Context | Boolean | Ensure the Shower server is started in the background. Returns true if the start command … | 32 |
| `ShowerServerManager.stopServer` | `ShowerServerManager` | `com.ai.assistance.showerclient` | `ShowerServerManager.kt` |  | Boolean | Stop the Shower server process if running. | 116 |
| `ShowerServerManager.copyJarToExternalDir` | `ShowerServerManager` | `com.ai.assistance.showerclient` | `ShowerServerManager.kt` | context: Context | File | Copy shower-server.jar from assets to an external directory. Host apps can override this … | 135 |
| `ShowerVideoRenderer.attach` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` | surface: Surface<br>videoWidth: Int<br>videoHeight: Int | Unit |  | 54 |
| `ShowerVideoRenderer.detach` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` |  | Unit |  | 65 |
| `ShowerVideoRenderer.releaseDecoderLocked` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` |  | Unit |  | 74 |
| `ShowerVideoRenderer.onFrame` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` | data: ByteArray | Unit | Called for each H.264 packet. | 90 |
| `ShowerVideoRenderer.findNalUnitType` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` | packet: ByteArray | Int |  | 129 |
| `ShowerVideoRenderer.queueFrameToDecoder` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` | packet: ByteArray | Unit |  | 148 |
| `ShowerVideoRenderer.maybeAvccToAnnexb` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` | packet: ByteArray | ByteArray |  | 176 |
| `ShowerVideoRenderer.captureCurrentFramePng` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` |  | ByteArray? |  | 205 |
| `ShowerVideoRenderer.initDecoderLocked` | `ShowerVideoRenderer` | `com.ai.assistance.showerclient` | `ShowerVideoRenderer.kt` |  | Unit |  | 243 |
| `ShowerSurfaceView.bindController` | `ShowerSurfaceView` | `com.ai.assistance.showerclient.ui` | `ShowerSurfaceView.kt` | controller: ShowerController | Unit | Bind a specific ShowerController to this view. This allows rendering a specific virtual d… | 41 |
| `ShowerSurfaceView.surfaceCreated` | `ShowerSurfaceView` | `com.ai.assistance.showerclient.ui` | `ShowerSurfaceView.kt` | holder: SurfaceHolder | Unit |  | 45 |
| `ShowerSurfaceView.surfaceChanged` | `ShowerSurfaceView` | `com.ai.assistance.showerclient.ui` | `ShowerSurfaceView.kt` | holder: SurfaceHolder<br>format: Int<br>width: Int<br>height: Int | Unit |  | 85 |
| `ShowerSurfaceView.surfaceDestroyed` | `ShowerSurfaceView` | `com.ai.assistance.showerclient.ui` | `ShowerSurfaceView.kt` | holder: SurfaceHolder | Unit |  | 89 |
| `ShowerSurfaceView.captureCurrentFramePng` | `ShowerSurfaceView` | `com.ai.assistance.showerclient.ui` | `ShowerSurfaceView.kt` |  | ByteArray? | Capture the current frame from the renderer. | 104 |
| `ExampleInstrumentedTest.useAppContext` | `ExampleInstrumentedTest` | `com.ai.assistance.shower` | `ExampleInstrumentedTest.kt` |  | Unit |  | 19 ⚑ |
| `MainActivity.onCreate` | `MainActivity` | `com.ai.assistance.shower` | `MainActivity.kt` | savedInstanceState: Bundle? | Unit |  | 18 |
| `Greeting` | — | `com.ai.assistance.shower` | `MainActivity.kt` | name: String<br>modifier: Modifier? | Unit |  | 36 |
| `GreetingPreview` | — | `com.ai.assistance.shower` | `MainActivity.kt` |  | Unit |  | 45 |
| `ShowerTheme` | — | `com.ai.assistance.shower.ui.theme` | `Theme.kt` | darkTheme: Boolean?<br>dynamicColor: Boolean?<br>content: () -> Unit | Unit |  | 37 |
| `ExampleUnitTest.addition_isCorrect` | `ExampleUnitTest` | `com.ai.assistance.shower` | `ExampleUnitTest.kt` |  | Unit |  | 14 ⚑ |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `DarkColorScheme` | — | `com.ai.assistance.shower.ui.theme` | `Theme.kt` | inferred |  | 14 |
| `FbxLibraryLoader.loaded` | `FbxLibraryLoader` | `com.ai.assistance.fbx` | `FbxLibraryLoader.kt` | inferred |  | 5 |
| `FbxLibraryLoader.lock` | `FbxLibraryLoader` | `com.ai.assistance.fbx` | `FbxLibraryLoader.kt` | inferred |  | 7 |
| `LightColorScheme` | — | `com.ai.assistance.shower.ui.theme` | `Theme.kt` | inferred |  | 20 |
| `LlamaLibraryLoader.loaded` | `LlamaLibraryLoader` | `com.ai.assistance.llama` | `LlamaLibraryLoader.kt` | inferred |  | 5 |
| `LlamaLibraryLoader.lock` | `LlamaLibraryLoader` | `com.ai.assistance.llama` | `LlamaLibraryLoader.kt` | inferred |  | 7 |
| `MmdInspector.FORMAT_PMD` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` | inferred |  | 35 |
| `MmdInspector.FORMAT_PMX` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` | inferred |  | 36 |
| `MmdInspector.MODEL_SUMMARY_SIZE` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` | inferred |  | 32 |
| `MmdInspector.MOTION_SUMMARY_SIZE` | `MmdInspector` | `com.ai.assistance.mmd` | `MmdInspector.kt` | inferred |  | 33 |
| `MmdLibraryLoader.loaded` | `MmdLibraryLoader` | `com.ai.assistance.mmd` | `MmdLibraryLoader.kt` | inferred |  | 5 |
| `MmdLibraryLoader.lock` | `MmdLibraryLoader` | `com.ai.assistance.mmd` | `MmdLibraryLoader.kt` | inferred |  | 7 |
| `MNNLibraryLoader.loaded` | `MNNLibraryLoader` | `com.ai.assistance.mnn` | `MNNLibraryLoader.kt` | inferred |  | 13 |
| `MNNLibraryLoader.lock` | `MNNLibraryLoader` | `com.ai.assistance.mnn` | `MNNLibraryLoader.kt` | inferred |  | 15 |
| `MNNLibraryLoader.TAG` | `MNNLibraryLoader` | `com.ai.assistance.mnn` | `MNNLibraryLoader.kt` | inferred |  | 10 |
| `Pink40` | — | `com.ai.assistance.shower.ui.theme` | `Color.kt` | inferred |  | 11 |
| `Pink80` | — | `com.ai.assistance.shower.ui.theme` | `Color.kt` | inferred |  | 7 |
| `Purple40` | — | `com.ai.assistance.shower.ui.theme` | `Color.kt` | inferred |  | 9 |
| `Purple80` | — | `com.ai.assistance.shower.ui.theme` | `Color.kt` | inferred |  | 5 |
| `PurpleGrey40` | — | `com.ai.assistance.shower.ui.theme` | `Color.kt` | inferred |  | 10 |
| `PurpleGrey80` | — | `com.ai.assistance.shower.ui.theme` | `Color.kt` | inferred |  | 6 |
| `ShowerBinderRegistry.service` | `ShowerBinderRegistry` | `com.ai.assistance.showerclient` | `ShowerBinderRegistry.kt` | IShowerService? |  | 17 |
| `ShowerBinderRegistry.TAG` | `ShowerBinderRegistry` | `com.ai.assistance.showerclient` | `ShowerBinderRegistry.kt` | inferred |  | 14 |
| `ShowerEnvironment.emitToSystemLog` | `ShowerEnvironment` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | Boolean | Keep writing logs to Android system logcat. Default is true to preserve existin… | 64 |
| `ShowerEnvironment.logSink` | `ShowerEnvironment` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | ShowerLogSink? | Optional sink used to mirror Shower client logs into host logging systems. | 56 |
| `ShowerEnvironment.shellRunner` | `ShowerEnvironment` | `com.ai.assistance.showerclient` | `ShellEnvironment.kt` | ShellRunner? |  | 50 |
| `ShowerServerManager.additionalTargetPackages` | `ShowerServerManager` | `com.ai.assistance.showerclient` | `ShowerServerManager.kt` | Set<String> |  | 25 |
| `ShowerServerManager.ASSET_JAR_NAME` | `ShowerServerManager` | `com.ai.assistance.showerclient` | `ShowerServerManager.kt` | inferred |  | 21 |
| `ShowerServerManager.LOCAL_JAR_NAME` | `ShowerServerManager` | `com.ai.assistance.showerclient` | `ShowerServerManager.kt` | inferred |  | 22 |
| `ShowerServerManager.TAG` | `ShowerServerManager` | `com.ai.assistance.showerclient` | `ShowerServerManager.kt` | inferred |  | 20 |
| `Typography` | — | `com.ai.assistance.shower.ui.theme` | `Type.kt` | inferred | Set of Material typography styles to start with | 10 |
