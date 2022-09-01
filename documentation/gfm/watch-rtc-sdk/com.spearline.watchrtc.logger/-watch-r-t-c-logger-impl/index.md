//[watch-rtc-sdk](../../../index.md)/[com.spearline.watchrtc.logger](../index.md)/[WatchRTCLoggerImpl](index.md)

# WatchRTCLoggerImpl

[androidJvm]\
class [WatchRTCLoggerImpl](index.md) : [ILogger](../-i-logger/index.md)

This class is the implementation of ILogger interface. This will print logs in your logcat with tag of WatchRTC.

## Constructors

| | |
|---|---|
| [WatchRTCLoggerImpl](-watch-r-t-c-logger-impl.md) | [androidJvm]<br>fun [WatchRTCLoggerImpl](-watch-r-t-c-logger-impl.md)() |

## Functions

| Name | Summary |
|---|---|
| [error](error.md) | [androidJvm]<br>open override fun [error](error.md)(tag: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html))<br>This function will print error logs with tag WatchRTC.<br>[androidJvm]<br>open override fun [error](error.md)(tag: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), t: [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html))<br>This function will print error logs with exception along with tag WatchRTC. |
| [info](info.md) | [androidJvm]<br>open override fun [info](info.md)(tag: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html))<br>This function is printing logs for debug build only. |
| [log](log.md) | [androidJvm]<br>open override fun [log](log.md)(tag: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html))<br>This function will print logs with tag WatchRTC. |
