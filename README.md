# Nightmare TV: official installers

Nightmare TV is an IPTV player for Windows, macOS, Android TV, Google TV, Fire TV and Android phones and tablets. This repository is the official public mirror of its installers: every direct download linked from [nightmaretv.net](https://nightmaretv.net) is a file in the [Releases](https://github.com/zeze89/nightmare-tv-releases/releases/latest) tab here.

**Player only.** Nightmare TV plays your own M3U playlist or Xtream Codes login. It provides no channels, playlists or subscriptions.

**[Download the latest release](https://github.com/zeze89/nightmare-tv-releases/releases/latest)** · [Website](https://nightmaretv.net) · [Docs](https://nightmaretv.net/docs) · [Changelog](https://nightmaretv.net/changelog)

![Live TV screen: the channel keeps playing on top, with now and next for every channel below](https://nightmaretv.net/screenshots/rev-live-guide-720.webp)

*Capture from the Windows build, with demo channels playing open-license films.*

## Which file do I need?

Where a store build exists, use it first: store builds update themselves. Direct files are on the [latest release](https://github.com/zeze89/nightmare-tv-releases/releases/latest) page. `<version>` in the file names below is the release number, for example `Nightmare-2.2.6-Setup.exe`.

| Device | Recommended source | Direct file | Notes |
| --- | --- | --- | --- |
| Windows 10 and 11, 64-bit | [Microsoft Store](https://apps.microsoft.com/detail/9PLPLGHTVB5G) | `Nightmare-<version>-Setup.exe` (installer) or `Nightmare-<version>-Portable.zip` (no install) | The Store build is signed by Microsoft. The direct builds are not code-signed yet, so Windows may show "Windows protected your PC": choose More info, then Run anyway. The installer is also on winget: `winget install NightmareTv.NightmareTV`. |
| Android phone or tablet, Android 7 or newer | [Google Play](https://play.google.com/store/apps/details?id=tv.nightmare.app) | `NightmareTV-<version>-arm64-v8a.apk` | Allow installs from your browser or file manager once. |
| Google TV or Android TV | Play Store on the TV | `NightmareTV-<version>-arm64-v8a.apk` on 64-bit boxes, `NightmareTV-<version>-armeabi-v7a.apk` on older or budget boxes | If the app is not listed in the Play Store on your TV, type `nightmaretv.net/apk-android-tv` in the Downloader app. [TV install steps](https://nightmaretv.net/android#tv) |
| Fire TV and Firestick, Fire OS 6 or newer | Downloader app: code `6766124` or address `nightmaretv.net/fire` | `NightmareTV-<version>-armeabi-v7a.apk` | Fire OS needs the 32-bit file. The 64-bit file shows "App not installed". Fire TV models that run Vega OS cannot install Android apps. [Fire TV guide](https://nightmaretv.net/firestick) |
| Mac, macOS 13 or newer, Apple Silicon and Intel | This repository | `Nightmare-<version>-macos.dmg` | The .dmg is not notarized yet. Right-click the app and choose Open, then confirm once. On macOS 15 and later choose Open Anyway in System Settings, Privacy and Security. [First-launch help](https://nightmaretv.net/mac) |
| Android emulator or x86 device | This repository | `NightmareTV-<version>-x86_64.apk` | |
| Any ARM Android device, if unsure | This repository | `NightmareTV-<version>-universal.apk` | One larger file that covers every ARM device. |

Each release also carries `Nightmare-<version>.msix` (a Windows package; the Microsoft Store listing is the simpler route for most people) and `SHA256SUMS.txt`.

Nightmare TV is distributed through the Microsoft Store, Google Play and this repository, and nowhere else. A "cracked", "modded" or pre-loaded-playlist copy from another site is not an official build. The full list with sizes and checksums is on the [download page](https://nightmaretv.net/where-to-download).

## Verify a download

Every release includes `SHA256SUMS.txt`. Compute the SHA-256 of the file you downloaded and compare it with the entry for that file name. Replace the example file name with yours.

Windows (PowerShell):

```powershell
Get-FileHash .\Nightmare-2.2.6-Setup.exe -Algorithm SHA256
```

macOS:

```sh
shasum -a 256 Nightmare-2.2.6-macos.dmg
```

Linux:

```sh
sha256sum NightmareTV-2.2.6-arm64-v8a.apk
```

The comparison is not case-sensitive. If the values match, the file is exactly the one that was published. If they do not, delete the file and download it again from one of the sources above.

## Trial and licence

- Every feature is unlocked for 7 days, with no card and no account. The 7 days start with your first playback, not at install.
- After the trial you choose a plan: Lifetime, Yearly, Monthly or Lifetime for 1 device. Every plan includes every feature, and one licence works on Windows, Mac and Android.
- Current prices, device counts and the refund policy are on the [pricing page](https://nightmaretv.net/pricing). A purchase made in Google Play or the Microsoft Store unlocks the app on that store account.

## What it does

- Plays M3U and M3U8 playlists (link or file) and Xtream Codes logins. Stalker portals are not supported.
- Programme guide from your XMLTV source: now and next, plus a 12-hour timeline.
- Recording: one press records the live channel to disk. Scheduling a recording from the guide is available on Windows and Android, not on Mac.
- Timeshift: pause and rewind live TV from a rolling buffer on your own device.
- Multi-view: up to four channels at once, fewer on low-memory TV devices.
- HDR tone-mapping (BT.2390) on Windows and macOS, and hardware decoding for 4K HEVC and AV1 where your device supports it.
- Dolby Atmos and DTS-X passthrough to a receiver on Windows and Android TV. It is off by default and is not available on Mac.
- Parental controls with PIN-protected profiles, and Cloud Sync for favourites, watch history, profiles and settings. Playlists and logins are not synced: you add them on each device.

Full list: [features](https://nightmaretv.net/features). Per-device details: [supported devices](https://nightmaretv.net/devices).

## Not supported

There is no iPhone, iPad, Apple TV, Samsung (Tizen), LG (webOS), Roku or Linux version. On a TV that cannot run Android apps, an Android TV or Fire TV device on a spare HDMI input runs the full app. Fire TV models on Fire OS 5 or Vega OS cannot install it.

## Help

- [Docs](https://nightmaretv.net/docs), [FAQ](https://nightmaretv.net/faq) and the [support page](https://nightmaretv.net/support) cover setup and the common fixes.
- Questions and bug reports: [GitHub Discussions](https://github.com/zeze89/nightmare-tv-releases/discussions). Include your platform and app version.
- Feature requests and voting: [nightmaretv.featurebase.app](https://nightmaretv.featurebase.app).
- Licensing, billing or anything private: [support@nightmaretv.net](mailto:support@nightmaretv.net).

Please do not share, request or link IPTV streams, playlists or providers in Discussions.

## About this repository

This repository holds installers only. Nightmare TV is closed source and is distributed under an [end user licence agreement](https://nightmaretv.net/eula); the source code is not published here. The third-party open-source components it uses are listed in the EULA and in the app under About, Open Source Licenses.

## Legal

Nightmare TV is a media player. It does not provide, host, distribute, recommend or resell streams, channels, films, series, guide data or any other content. You bring your own M3U or Xtream Codes source that you have the legal right to use.

[Terms](https://nightmaretv.net/terms) · [Privacy](https://nightmaretv.net/privacy) · [EULA](https://nightmaretv.net/eula) · [Refund policy](https://nightmaretv.net/refund) · [Bring your own playlist](https://nightmaretv.net/legal/byo-playlist)
