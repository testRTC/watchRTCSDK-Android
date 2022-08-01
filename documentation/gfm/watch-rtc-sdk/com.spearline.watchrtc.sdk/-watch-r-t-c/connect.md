//[watch-rtc-sdk](../../../index.md)/[com.spearline.watchrtc.sdk](../index.md)/[WatchRTC](index.md)/[connect](connect.md)

# connect

[androidJvm]\
fun [connect](connect.md)(config: [WatchRTCConfig](../-watch-r-t-c-config/index.md)? = null)

Initialize connection to WatchRTC's backend. Should be called once peer connection is open

## Throws

| | |
|---|---|
| [kotlin.IllegalStateException](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-illegal-state-exception/index.html) | in case config is not set via constructor or @see setConfig |
| [kotlin.IllegalArgumentException](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-illegal-argument-exception/index.html) | in case one of the config values is invalid |
