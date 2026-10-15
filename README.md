# Discord LAN Voice - Android APK Project

## Why the old APK did not work
1. The previous `MainActivity.java` only contained two plain text boxes and a raw UDP DatagramSocket to `239.255.42.99`.
2. PC web browsers **cannot listen to raw UDP datagrams** because of browser security.
3. This updated project replaces the old two-textbox code with the real Discord Voice Call app using hardware microphone capture and the real-time WebSocket audio relay.

## How to build your APK on GitHub (Zero Install)
1. In your GitHub repository, ensure the contents of this ZIP are at the ROOT of the repository:
   - `build.gradle` (root)
   - `settings.gradle` (root)
   - `gradle.properties` (root)
   - `.github/workflows/build-apk.yml`
   - `app/` folder
   *(Do NOT upload a nested folder inside another folder)*
2. Go to the **Actions** tab on your GitHub repository.
3. Wait ~90 seconds for `build-apk` to finish.
4. Download the **DiscordVoice-Installable-APK** artifact.
5. Tap `app-debug.apk` on your Android phone to install!
