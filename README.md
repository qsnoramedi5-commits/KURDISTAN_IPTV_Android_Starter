# KURDISTAN IPTV — Android starter project

A dark Kurdish IPTV Android starter using Kotlin and AndroidX Media3 ExoPlayer for HLS/M3U8 playback.

## Open and build
1. Install Android Studio (stable version).
2. Open this folder as an existing Gradle project.
3. Let Gradle sync, then run on an Android device or emulator.
4. To create an APK: **Build → Build APK(s)**.

## Included
- Portrait-first channel list, search, category filters, Kurdish dark theme.
- HLS/M3U8 playback using Media3 ExoPlayer.
- Fullscreen landscape toggle.
- A starter subset of channel URLs in `app/src/main/java/com/kurdistan/iptv/Channel.kt`.

## Important
- This is source code, not a prebuilt APK. Build it in Android Studio to generate the APK.
- The `Channels.all` list currently includes a starter subset; append remaining channels in `Channel.kt` using `Channel("CHANNEL NAME", "https://...m3u8", "category")`.
- Streams can fail if a provider has changed its URL, requires a specific network/headers, blocks playback, or the user lacks permission. Only use streams you are authorized to access.
- `android:usesCleartextTraffic="true"` is enabled because the supplied list contains HTTP URLs. For production, remove HTTP streams where possible and disable cleartext traffic.
