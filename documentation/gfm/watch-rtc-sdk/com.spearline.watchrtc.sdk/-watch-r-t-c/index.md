//[watch-rtc-sdk](../../../index.md)/[com.spearline.watchrtc.sdk](../index.md)/[WatchRTC](index.md)

# WatchRTC

[androidJvm]\
class [WatchRTC](index.md)(config: [WatchRTCConfig](../-watch-r-t-c-config/index.md)?, dataProvider: [RtcDataProvider](../-rtc-data-provider/index.md))

## Parameters

androidJvm

| | |
|---|---|
| config | @see WatchRTCConfig |
| dataProvider | implementation of RTC stats data collection |

## Constructors

| | |
|---|---|
| [WatchRTC](-watch-r-t-c.md) | [androidJvm]<br>fun [WatchRTC](-watch-r-t-c.md)(dataProvider: [RtcDataProvider](../-rtc-data-provider/index.md))<br>Note: setConfig must be called before connect in case config is not passed in the constructor |
| [WatchRTC](-watch-r-t-c.md) | [androidJvm]<br>fun [WatchRTC](-watch-r-t-c.md)(config: [WatchRTCConfig](../-watch-r-t-c-config/index.md)?, dataProvider: [RtcDataProvider](../-rtc-data-provider/index.md)) |

## Functions

| Name | Summary |
|---|---|
| [addEvent](add-event.md) | [androidJvm]<br>fun [addEvent](add-event.md)(name: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), type: [EventType](../-event-type/index.md), parameters: [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)? = null)<br>Send custom events to WatchRTC's backend. |
| [addKeys](add-keys.md) | [androidJvm]<br>fun [addKeys](add-keys.md)(keys: [HashMap](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-hash-map/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), [ArrayList](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-array-list/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)&gt;&gt;)<br>Will be sent to WatchRTC's backend. |
| [connect](connect.md) | [androidJvm]<br>fun [connect](connect.md)(context: [Context](https://developer.android.com/reference/kotlin/android/content/Context.html), config: [WatchRTCConfig](../-watch-r-t-c-config/index.md)? = null)<br>Initialize connection to WatchRTC's backend. Should be called once peer connection is open |
| [disconnect](disconnect.md) | [androidJvm]<br>fun [disconnect](disconnect.md)()<br>Closes connection to WatchRTC's backend. Should be called once the peer connection is closed. |
| [log](log.md) | [androidJvm]<br>fun [log](log.md)(logLevel: [LogLevel](../-log-level/index.md), text: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html))<br>Log debug messages to WatchRTC's server |
| [setConfig](set-config.md) | [androidJvm]<br>fun [setConfig](set-config.md)(config: [WatchRTCConfig](../-watch-r-t-c-config/index.md))<br>Set WatchRTC configuration |
| [setLoggerImpl](set-logger-impl.md) | [androidJvm]<br>fun [setLoggerImpl](set-logger-impl.md)(iLogger: [ILogger](../../com.spearline.watchrtc.logger/-i-logger/index.md))<br>Set implementation of ILogger here for printing logs on your application. You can also use default implementation WatchRTCLoggerImpl of ILogger. This will print logs in your logcat. Please call this function after creating object of WatchRTC class. |
| [setUserRating](set-user-rating.md) | [androidJvm]<br>fun [setUserRating](set-user-rating.md)(rating: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html), ratingComment: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) = &quot;&quot;)<br>Set user provided rating with an optional comment. |
| [trace](trace.md) | [androidJvm]<br>fun [trace](trace.md)(eventName: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), data: [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)?): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Send RTC related events to WatchRTC's backend. |
