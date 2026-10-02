<p align="center">
  <img src="icon.png" width="120" alt="Minimal Music Controller Remote icon">
</p>

# Minimal Music Controller Remote

Control whatever is already playing on your Android device with a game controller, and get
back the tactile button feel of a dedicated music player.

The app does not play audio itself. It is a remote for the media app you already use
(Spotify, YouTube Music, podcast players, anything that exposes an Android media session)
with transport controls, track info, an animated visualizer and a lot of customisation.

**[Download the latest APK](https://github.com/handyandii/music-remote/releases/latest)**

- Android 12 or newer
- About 3 MB
- No ads, no accounts, no analytics, and no internet permission: everything stays on your device

## Features

**Physical controls**

- Bind any button, trigger, stick direction or D-pad input your controller reports to a media
  action: play/pause, play, pause, skip, previous, fast forward, rewind, volume up, volume down.
- Works with built-in handheld controls and connected controllers, including D-pads and
  triggers that only report as analog axes.
- Multiple named binding profiles, for example one per controller.
- A controller test screen that shows exactly what the device detects when you press something.
- Default profile: **L1** and **A** play/pause, **R1** skips, **R2** goes to the previous track.

**Make it yours**

- 9 built-in themes (Midnight, Mono, Sunset, Neon, Forest, Ocean, Berry, Amber, Lavender), a
  Device Colors theme that follows your wallpaper, and a custom theme builder with swatches,
  a full colour picker and hex input.
- Dark and light modes, tuned separately for each theme.
- Load your own `.ttf` or `.otf` font and adjust weight and letter spacing.
- Adjustable visualizer (bar count and width), play button style, and independent scale
  sliders for the visualizer, controls, track info, badge and corner buttons.
- Window position and height, so the remote can sit in the part of the screen you want.
- Save your whole setup as a named preset, and export or import presets as JSON.

**Extras**

- Lockscreen overlay: control playback without unlocking the device.
- Screen timeout control: follow the system, never sleep while the app is open, or a custom
  timeout from 5 to 300 seconds.
- Shortcut button that opens the app currently playing, or a default app you choose.
- Orientation lock and split-screen support.

## Install

1. Download the `.apk` file from the [latest release](https://github.com/handyandii/music-remote/releases/latest).
2. Open it on your device. If Android asks, allow your browser or file manager to install
   unknown apps.
3. Launch the app and tap **Open Notification Access Settings**.
4. Enable **Minimal Music Controller Remote** in the list, then go back. The app continues
   automatically.

### If Android says "Restricted setting"

On Android 13 and newer, apps installed from outside an app store are usually blocked from
Notification Access the first time you try to turn it on. To unblock it:

1. Open **Settings → Apps → Minimal Music Controller Remote**.
2. Tap the **⋮** menu in the top-right corner and choose **Allow restricted settings**.
3. Confirm with your PIN or fingerprint.
4. Return to the app and enable Notification Access again.

The **⋮** option only appears after you have seen the "Restricted setting" message once.
Menu names vary slightly between manufacturers.

## Permissions

| Permission | Needed for | Required |
|---|---|---|
| Notification Access | Seeing and controlling the active media session. This is the standard Android mechanism for media remotes. The app does not read your notification content. | Yes |
| Modify system settings | The custom screen timeout option | Only if you use it |
| Full-screen intent | The lockscreen overlay on Android 14+ | Only if you use it |

The optional permissions are requested inside Settings when you turn on the feature that
needs them.

## Troubleshooting

- **Nothing shows as playing:** start playback in your music app first, and confirm
  Notification Access is still enabled for this app.
- **Controller buttons do nothing:** check **Settings → Controls → Enable physical button
  controls**, then use **Test controller input** to see whether the device reports the press.
  If it does, add it under **Button bindings**.
- **"App not installed" when updating:** you have a copy signed with a different key (for
  example a development build). Uninstall it and install the release APK. This resets your
  settings, so export any presets first.

## About this project

This started as a personal project: I wanted a dedicated music remote for a small Android
handheld, and decided to release it publicly in case it is useful to anyone else.

It was built mostly by vibe coding with Claude. I directed the design and features and
tested it on my own devices, but most of the code was written by AI. It works well for me,
but it has not been tested across many devices, so expect rough edges and please report
anything that breaks.

## Feedback

Bug reports and feature requests are welcome in
[Issues](https://github.com/handyandii/music-remote/issues). Please include your device
model, Android version and the app version shown in **Settings → About**.

## License

Free to download and use. This repository hosts release builds only.
