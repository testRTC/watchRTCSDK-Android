//[watch-rtc-sdk](../../../index.md)/[com.spearline.watchrtc.logger](../index.md)/[ILogger](index.md)

# ILogger

[androidJvm]\
interface [ILogger](index.md)

ILogger is interface for logging in WatchRTC SDK. Please implement this interface and pass object reference on watchRTC.setLoggerImpl(iLogger: ILogger) function.

## Functions

| Name | Summary |
|---|---|
| [error](error.md) | [androidJvm]<br>abstract fun [error](error.md)(@[NonNull](https://developer.android.com/reference/kotlin/androidx/annotation/NonNull.html)tag: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), @[NonNull](https://developer.android.com/reference/kotlin/androidx/annotation/NonNull.html)message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html))<br>abstract fun [error](error.md)(@[NonNull](https://developer.android.com/reference/kotlin/androidx/annotation/NonNull.html)tag: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), @[Nullable](https://developer.android.com/reference/kotlin/androidx/annotation/Nullable.html)message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) = &quot;&quot;, @[NonNull](https://developer.android.com/reference/kotlin/androidx/annotation/NonNull.html)t: [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)) |
| [info](info.md) | [androidJvm]<br>abstract fun [info](info.md)(@[NonNull](https://developer.android.com/reference/kotlin/androidx/annotation/NonNull.html)tag: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), @[NonNull](https://developer.android.com/reference/kotlin/androidx/annotation/NonNull.html)message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)) |
| [log](log.md) | [androidJvm]<br>abstract fun [log](log.md)(@[NonNull](https://developer.android.com/reference/kotlin/androidx/annotation/NonNull.html)tag: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), @[NonNull](https://developer.android.com/reference/kotlin/androidx/annotation/NonNull.html)message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)) |

## Inheritors

| Name |
|---|
| [WatchRTCLoggerImpl](../-watch-r-t-c-logger-impl/index.md) |
