//[watch-rtc-sdk](../../../index.md)/[com.spearline.watchrtc.model](../index.md)/[RTCStatsReport](index.md)

# RTCStatsReport

[androidJvm]\
data class [RTCStatsReport](index.md)(val report: [HashMap](https://developer.android.com/reference/kotlin/java/util/HashMap.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), [RTCStatsReport.RTCStat](-r-t-c-stat/index.md)&gt;, var timestamp: [Long](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html))

## Constructors

| | |
|---|---|
| [RTCStatsReport](-r-t-c-stats-report.md) | [androidJvm]<br>fun [RTCStatsReport](-r-t-c-stats-report.md)(report: [HashMap](https://developer.android.com/reference/kotlin/java/util/HashMap.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), [RTCStatsReport.RTCStat](-r-t-c-stat/index.md)&gt;, timestamp: [Long](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)) |

## Types

| Name | Summary |
|---|---|
| [Companion](-companion/index.md) | [androidJvm]<br>object [Companion](-companion/index.md) |
| [RTCStat](-r-t-c-stat/index.md) | [androidJvm]<br>data class [RTCStat](-r-t-c-stat/index.md)(val timestamp: [Long](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html), val properties: [HashMap](https://developer.android.com/reference/kotlin/java/util/HashMap.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)&gt;) |

## Functions

| Name | Summary |
|---|---|
| [toData](to-data.md) | [androidJvm]<br>fun [toData](to-data.md)(): [HashMap](https://developer.android.com/reference/kotlin/java/util/HashMap.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)&gt; |
| [toJson](to-json.md) | [androidJvm]<br>fun [toJson](to-json.md)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |

## Properties

| Name | Summary |
|---|---|
| [report](report.md) | [androidJvm]<br>val [report](report.md): [HashMap](https://developer.android.com/reference/kotlin/java/util/HashMap.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html), [RTCStatsReport.RTCStat](-r-t-c-stat/index.md)&gt; |
| [timestamp](timestamp.md) | [androidJvm]<br>var [timestamp](timestamp.md): [Long](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html) |
