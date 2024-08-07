<p align="center">
  <img height="160" src="https://avatars.githubusercontent.com/u/16746133?s=200&v=4" />
</p>

# watchrtc-android-sdk

This repository contains the watchRTC android SDK.

The SDK is geared towards those who want to collect WebRTC related data from an android application, log and analyze it as part of the testRTC environment.

Here is the [documentation] of the watchRTC sdk.

## SDK support and requirement
* The min android version supported by the SDK is Android-7 (Api Level 24).
* The SDK only required Internet permission.
* Kotlin version 2.0.0

## How to add SDK in your app
  1. Add dependancy in app module build.gradle file.
      ```groovy
      implementation 'com.spearline:testrtc-watchrtc-sdk:1.40.2'
     ```
  2. Sync project
 
 ## How to implement SDK in your app
- Implement the `RtcDataProvider` interface and their method `getStats(callback: GetStatsCallback)` The method getStats jobs is to generate webrtc stats report and once the report is avaialble need to call `callback.onStatsAvailable()`. To convert webrtc stats report to RTCStatsReport you can check this [function].
```Kotlin
  private val rtcDataProvider = object : RtcDataProvider {
        override fun getStats(callback: GetStatsCallback) {
            // get stats report and call callback.onStatsAvailable(com.spearline.watchrtc.model.RTCStatsReport)
        }
    }
```
- Initialize WatchRTCConfig with your API Key and room id and other details
- Here is [how to create WatchRTC API key](https://testrtc.com/docs/create-a-watchrtc-api-key/)
```Kotlin
val config = WatchRTCConfig(
            "<api-key>",
            "<room-id>",
            "<peer-id>",
            "<keys>", //(optional)
            proxyUrl = "wss://yourproxyurl.com" //(optional)
        )
```
- Create WatchRTC object
```Kotlin
val watchRTC = WatchRTC(config, rtcDataProvider)
```
- Connect to watchRTC's servers. The connect() function may throw `IllegalStateException` if the valid config is not set and call this function.
```Kotlin
/**
* Please call connect() once the peer connection is active where watchRTCConfig parameter is an optional, 
* Please pass this argument only if you would like to use an updated configuration or not passed on constructor. 
*/
watchRTC.connect(context, watchRTCConfig?)
```

- Log webrtc events to watchRTC server you can use `watchRTC.trace()` function.
Here is the sample app code for the [same]. This function may throw [ConnectionException] when facing issue to connecting server. Please handle this exception.

- Disconnect the call
```Kotlin
//Please call disconnect() once the call have been disconnected.
watchRTC.disconnect()
```

## SDK logs for debug perspective
- To print sdk logs in your application you have to set logger via calling `watchRTC.setLoggerImpl(WatchRTCLoggerImpl())` function.
- You can use your custom logs implementation with use of [ILogger] interface implementation.


## You can also use some of the other functions of the WatchRTC SDK
- `watchRTC.setConfig(WatchRTCConfig)` //Set WatchRTC configuration
- `watchRTC.addKeys(HashMap<String, ArrayList<String>>)` //Will be sent to WatchRTC's backend.
- `watchRTC.setUserRating(Int, String)` //Set user provided rating with an optional comment.
- `watchRTC.log(LogLevel,String)` //Log debug messages to WatchRTC's server
- `watchRTC.trace(String, Any?)` : Boolean //Send RTC related events to WatchRTC's backend.
- `watchRTC.addEvent(String, EventType, Any?)` //Send custom events to WatchRTC's backend.
- `watchRTC.setLoggerImpl(iLogger: ILogger)` // To print SDK logs for debug perspective.


## WatchRTC SDK sample applications
- [WebRTC Sample app]
- [Twilio Sample App]
- [Vonage Sample App]

[here]: https://github.com/testRTC/watchRTCSDK-Android/raw/master/sdk/watch-rtc-sdk.aar
[WebRTC Sample app]: https://github.com/testRTC/watchRTCSDK-Android-SampleApp
[documentation]: https://github.com/testRTC/watchRTCSDK-Android/blob/master/documentation/gfm/watch-rtc-sdk/com.spearline.watchrtc.sdk/-watch-r-t-c/index.md
[function]: https://github.com/testRTC/watchRTCSDK-Android-SampleApp/blob/f58809a977026d4d4747add6efba33793d7d2f86/watchrtc-demo/src/main/java/com/spearline/webrtc/RTCActivity.kt#L329
[same]: https://github.com/testRTC/watchRTCSDK-Android-SampleApp/blob/f58809a977026d4d4747add6efba33793d7d2f86/watchrtc-demo/src/main/java/com/spearline/webrtc/RTCActivity.kt#L140
[ConnectionException]: https://github.com/testRTC/watchRTCSDK-Android/blob/master/documentation/gfm/watch-rtc-sdk/com.spearline.watchrtc.exception/-connection-exception/-connection-exception.md
[ILogger]: https://github.com/testRTC/watchRTCSDK-Android/blob/master/documentation/gfm/watch-rtc-sdk/com.spearline.watchrtc.logger/-i-logger/index.md
[Twilio Sample App]: https://github.com/testRTC/watchRTCSDK-Android-TwilioSampleApp
[Vonage Sample App]: https://github.com/testRTC/watchRTCSDK-Android-VonageSampleApp
