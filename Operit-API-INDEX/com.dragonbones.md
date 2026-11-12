# com.dragonbones

> 函数 47 · 类型 7 · 顶层常量 2 · 共 56 条
> 自动生成，请勿手改。重新生成：`node indexer/index.mjs`

## 类型

| 类型 | 类名 | 包名 | 文件名 | 签名 / 字段 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `AnimationCommand` | `AnimationCommand` | `com.dragonbones` | `DragonBonesController.kt` | interface AnimationCommand : AnimationCommand | Represents a command to be executed on the DragonBones view. | 191 |
| `DragonBonesController` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` | class DragonBonesController(val coroutineScope: CoroutineScope) | A controller for the [DragonBonesViewCompose] composable. This controller provides a way … | 27 |
| `DragonBonesModel` | `DragonBonesModel` | `com.dragonbones` | `DragonBonesView.kt` | class DragonBonesModel(val skeletonPath: String, val textureJsonPath: String, val textureImagePath: String) | DragonBones 模型信息数据类 | 242 |
| `DragonBonesView` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | class DragonBonesView(context: Context, attrs: AttributeSet?, zOrderOnTop: Boolean) : GLSurfaceView | DragonBones 骨骼动画视图组件 使用 C++ JNI 和 OpenGL ES 进行渲染，以获得高性能 | 30 |
| `DragonBonesView.DragonBonesRenderer` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | class DragonBonesRenderer(private val onSurfaceCreated: () -> Unit, private val onDrawFrame: () -> Unit, private val onSurfaceDestroyed: () -> Unit) : Renderer | GL渲染器，负责调用JNI代码执行实际的OpenGL绘制 | 112 |
| `JniBridge` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | object JniBridge |  | 3 |
| `StopAnimationCommand` | `StopAnimationCommand` | `com.dragonbones` | `DragonBonesController.kt` | class StopAnimationCommand(val name: String, val id: Long) : AnimationCommand | Represents a command to stop a specific DragonBones animation. | 214 |

## 函数

| 函数 | 类名 | 包名 | 文件名 | 参数 | 返回 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `DragonBonesController.destroyView` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` |  | Unit | Destroys the currently associated view, if any. | 56 |
| `DragonBonesController.fetchAnimationNames` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` |  | Unit | Asynchronously fetches the animation names from the current view and updates the state. T… | 66 |
| `DragonBonesController.setView` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` | dragonBonesView: DragonBonesView? | Unit |  | 89 |
| `DragonBonesController.fadeInAnimation` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` | name: String<br>layer: Int<br>loop: Int<br>fadeInTime: Float? | Unit | Plays an animation on a specific track (layer) with looping and fade-in control. This is … | 119 |
| `DragonBonesController.stopAnimation` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` | name: String | Unit |  | 126 |
| `DragonBonesController.clearAnimationQueue` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` |  | Unit | Clears all pending animation commands from the queue. This should be called before loadin… | 137 |
| `DragonBonesController.consumeNextAnimationCommand` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` |  | AnimationCommand? | Atomically retrieves and removes the next command from the queue. Returns null if the que… | 146 |
| `DragonBonesController.playAnimation` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` | name: String<br>fadeInTime: Float? | Unit | Plays the specified animation. | 156 |
| `DragonBonesController.overrideBonePosition` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` | boneName: String<br>x: Float<br>y: Float | Unit |  | 160 |
| `DragonBonesController.resetBone` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` | boneName: String | Unit |  | 166 |
| `DragonBonesController.setAnimationNames` | `DragonBonesController` | `com.dragonbones` | `DragonBonesController.kt` | names: List<String> | Unit |  | 171 |
| `rememberDragonBonesController` | — | `com.dragonbones` | `DragonBonesController.kt` |  | DragonBonesController | Creates and remembers a [DragonBonesController]. | 183 |
| `DragonBonesView.isInstanceActive` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` |  | Boolean |  | 44 |
| `DragonBonesView.onSingleTapUp` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | e: MotionEvent | Boolean |  | 87 |
| `DragonBonesView.DragonBonesRenderer.onSurfaceCreated` | `DragonBonesRenderer` | `com.dragonbones` | `DragonBonesView.kt` | gl: GL10?<br>config: EGLConfig? | Unit |  | 117 |
| `DragonBonesView.DragonBonesRenderer.onSurfaceChanged` | `DragonBonesRenderer` | `com.dragonbones` | `DragonBonesView.kt` | gl: GL10?<br>width: Int<br>height: Int | Unit |  | 122 |
| `DragonBonesView.DragonBonesRenderer.onDrawFrame` | `DragonBonesRenderer` | `com.dragonbones` | `DragonBonesView.kt` | gl: GL10? | Unit |  | 126 |
| `DragonBonesView.readBytesFromPath` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | path: String | ByteArray |  | 132 |
| `DragonBonesView.loadModel` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | model: DragonBonesModel<br>onComplete: (() -> Unit)?? | Unit |  | 144 |
| `DragonBonesView.onPause` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` |  | Unit |  | 161 |
| `DragonBonesView.onResume` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` |  | Unit |  | 168 |
| `DragonBonesView.destroy` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` |  | Unit |  | 175 |
| `DragonBonesView.getAnimationNames` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | callback: (List<String>) -> Unit | Unit | 异步获取当前模型所有可播放的动画名称列表。 | 194 |
| `DragonBonesView.fadeInAnimation` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | name: String<br>layer: Int<br>loop: Int<br>fadeInTime: Float | Unit | 播放指定名称的动画。 如果动画名称不存在，将不会播放任何动画（并会在logcat中打印警告）。 | 208 |
| `DragonBonesView.stopAnimation` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | name: String | Unit |  | 213 |
| `DragonBonesView.setWorldScale` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | scale: Float | Unit |  | 218 |
| `DragonBonesView.setWorldTranslation` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | x: Float<br>y: Float | Unit |  | 222 |
| `DragonBonesView.overrideBonePosition` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | boneName: String<br>x: Float<br>y: Float | Unit |  | 226 |
| `DragonBonesView.resetBone` | `DragonBonesView` | `com.dragonbones` | `DragonBonesView.kt` | boneName: String | Unit |  | 230 |
| `DragonBonesViewCompose` | — | `com.dragonbones` | `DragonBonesView.kt` | modifier: Modifier?<br>model: DragonBonesModel?<br>controller: DragonBonesController<br>zOrderOnTop: Boolean?<br>onError: (String) -> Unit?<br>onRenderStart: () -> Unit?<br>onRenderFrame: () -> Unit?<br>onRenderEnd: () -> Unit? | Unit |  | 249 |
| `JniBridge.init` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` |  | Unit |  | 8 |
| `JniBridge.loadDragonBones` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | skeletonData: ByteArray<br>textureJsonData: ByteArray<br>texturePngData: ByteArray | Unit |  | 11 |
| `JniBridge.onPause` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` |  | Unit |  | 17 |
| `JniBridge.onResume` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` |  | Unit |  | 19 |
| `JniBridge.onDestroy` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` |  | Unit |  | 21 |
| `JniBridge.onSurfaceCreated` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` |  | Unit |  | 23 |
| `JniBridge.onSurfaceChanged` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | width: Int<br>height: Int | Unit |  | 25 |
| `JniBridge.onDrawFrame` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` |  | Unit |  | 27 |
| `JniBridge.getAnimationNames` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` |  | Array<String>? |  | 29 |
| `JniBridge.getAnimationDuration` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | animationName: String | Float |  | 31 |
| `JniBridge.fadeInAnimation` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | name: String<br>layer: Int<br>loop: Int<br>fadeInTime: Float | Unit |  | 33 |
| `JniBridge.containsPoint` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | x: Float<br>y: Float | String? |  | 35 |
| `JniBridge.setWorldScale` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | scale: Float | Unit |  | 37 |
| `JniBridge.setWorldTranslation` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | x: Float<br>y: Float | Unit |  | 39 |
| `JniBridge.overrideBonePosition` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | boneName: String<br>x: Float<br>y: Float | Unit |  | 41 |
| `JniBridge.resetBone` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | boneName: String | Unit |  | 43 |
| `JniBridge.stopAnimation` | `JniBridge` | `com.dragonbones` | `JniBridge.kt` | name: String | Unit |  | 45 |

## 常量 / 顶层属性

| 名称 | 类名 | 包名 | 文件名 | 类型 | 说明 | 行 |
| --- | --- | --- | --- | --- | --- | --- |
| `TAG` | — | `com.dragonbones` | `DragonBonesController.kt` | inferred |  | 16 |
| `TAG` | — | `com.dragonbones` | `DragonBonesView.kt` | inferred |  | 27 |
