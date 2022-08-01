//[watch-rtc-sdk](../../../index.md)/[com.spearline.watchrtc.sdk](../index.md)/[RtcDataProvider](index.md)/[getStats](get-stats.md)

# getStats

[androidJvm]\
abstract fun [getStats](get-stats.md)(callback: [GetStatsCallback](../-get-stats-callback/index.md))

Used by WatchRTC to periodically fetch statistics of the current peer connection. Implementation of this interface should collect stats and once available, call callback.onStatsAvailable(stats). Output is expected to be a JSON string, structured as an RTCStatsReport object. [docs](https://developer.mozilla.org/en-US/docs/Web/API/RTCStatsReport)
