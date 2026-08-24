# PacTrac releases

Installable builds of [PacTrac](https://github.com/0z00z0/pactrac). Artifacts
only. The source repo is private; this one is public so the app can check for and
download its own updates without carrying a token that could read anything else.

## Layout

The platform is part of the tag, so both platforms live here side by side.

| Platform | Tag | Asset |
|---|---|---|
| Android | `android-v<versionName>+<versionCode>` | `pactrac-android-v<versionName>+<versionCode>.apk` |
| iOS | `ios-v<versionName>+<versionCode>` | `pactrac-ios-v<versionName>+<versionCode>.ipa` |

`versionCode` is one monotonic counter shared by both platforms, so a number
identifies one build of PacTrac rather than one build of one platform. The
update check reads the integer after the `+`.

## Installing on Android

Download the `.apk` from the newest `android-` release and open it on the
phone. Android asks for permission to install from this source the first time.

Every build is signed with the same key. An install refused as *App not
installed* or `INSTALL_FAILED_UPDATE_INCOMPATIBLE` means the installed copy
predates that key and has to be uninstalled first, which deletes its recorded
tracks. Export anything worth keeping before doing that.

## Release notes

Generated from the issues closed in the source repo since the previous release
of the same platform, grouped by category. A release that lists nothing had no
issues closed against it; it is still a real build.