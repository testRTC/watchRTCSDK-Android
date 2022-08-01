//[watch-rtc-sdk](../../../index.md)/[com.spearline.watchrtc.sdk](../index.md)/[WatchRTCConfig](index.md)

# WatchRTCConfig

[androidJvm]\
class [WatchRTCConfig](index.md)(val rtcApiKey: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), val rtcRoomId: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), val rtcPeerId: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), keys: [HashMap](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-hash-map/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), [ArrayList](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-array-list/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)&gt;&gt;? = null, var proxyUrl: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)? = null)

## Parameters

androidJvm

| | |
|---|---|
| rtcApiKey | WatchRTC api key |
| rtcPeerId | Peer connection id |
| rtcRoomId | RTC room id |
| keys | optional key-value pairs to be sent to WatchRTC's backend |

## Constructors

| | |
|---|---|
| [WatchRTCConfig](-watch-r-t-c-config.md) | [androidJvm]<br>fun [WatchRTCConfig](-watch-r-t-c-config.md)(rtcApiKey: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), rtcRoomId: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), rtcPeerId: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), keys: [HashMap](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-hash-map/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), [ArrayList](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-array-list/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)&gt;&gt;? = null, proxyUrl: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)? = null) |

## Properties

| Name | Summary |
|---|---|
| [proxyUrl](proxy-url.md) | [androidJvm]<br>var [proxyUrl](proxy-url.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)? = null |
| [rtcApiKey](rtc-api-key.md) | [androidJvm]<br>@SerializedName(value = &quot;rtcApiKey&quot;)<br>val [rtcApiKey](rtc-api-key.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [rtcPeerId](rtc-peer-id.md) | [androidJvm]<br>@SerializedName(value = &quot;rtcPeerId&quot;)<br>val [rtcPeerId](rtc-peer-id.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [rtcRoomId](rtc-room-id.md) | [androidJvm]<br>@SerializedName(value = &quot;rtcRoomId&quot;)<br>val [rtcRoomId](rtc-room-id.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
