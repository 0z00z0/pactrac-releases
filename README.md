# PacTrac

**Every street in town, run one dot at a time.** PacTrac shows the streets not yet run as dots on
the map, Pac-Man style. Each dot is eaten as the run passes it, so new streets are always in sight.

**Built on CityStrides.** [CityStrides](https://citystrides.com) is the community project that
records every street a runner has covered and gives every run a purpose: finish all the streets in
the city. PacTrac reads that CityStrides data and adds a live view and route planning on top.
CityStrides remains the record of which streets are finished. PacTrac is an independent app, not
an official CityStrides product.

## What it does

- **Dots in seconds.** Street data comes from PacTrac's own server, so the dots in view appear
  within seconds, finished streets in white beside the ones still to run.
- **Back at once after a restart.** Dots are stored on the phone, so they are on the map straight
  away, also with no signal, and can still be eaten.
- **Smooth over large areas.** Every dot in view is drawn, even across many dense neighbourhoods,
  and the map keeps moving smoothly.
- **A steady view zoomed out.** Far out, the map shows a sample of the dots that stays in place;
  zooming in shows them all.
- **One tap to refresh.** The dot button asks CityStrides again for everything in view, so streets
  CityStrides has just credited turn white.
- **Eat them live.** Dots disappear as the run passes them, the score counts up, and a notice
  shows each street finished.
- **Streets finished.** Beside the dots eaten, the panel counts the streets finished on this run
  and how many streets nearby are done.
- **Comparison after the run.** A report sets the run against what CityStrides counted, with a map
  of any gaps and the places where the two disagree.
- **Route planner for new streets.** A round trip, a drawn area or a route through points A to H,
  with a slider for how far a detour may go, each built to collect as many unrun streets as it can.
- **Turn-by-turn on the map.** Arrows show the way ahead, and the phone buzzes before each turn
  onto another street.
- **Three looks.** Glass + Neon, CRT + 8-bit pixel or Calm, each with its own icons, plus a
  Daylight setting for bright sun.
- **A new app icon.** Pac-Man eating dots along a street, also as an Android themed icon.
- **Statistics.** Kilometres run, walked and ridden, dots eaten per week, day and week streaks,
  and activities per month.
- **Flags with spoken notes.** A flag marks a place on the route, and its note can be dictated in
  Norwegian while running.
- **Sync between phones.** Settings and eaten dots follow the account, with sign-in by passkey.
- **Updates itself.** The app finds and installs new versions from this page.
- **A welcome tour** on the first start explains the map, the permissions and the sign-ins.

PacTrac runs on Android. Recorded tracks and activities stay on the phone.

## Installing on Android

Download the `.apk` from the newest `android-` release and open it on the
phone. Android asks for permission to install from this source the first time.
Later versions arrive through the app's own update check.

Every build is signed with the same key. An install refused as *App not
installed* or `INSTALL_FAILED_UPDATE_INCOMPATIBLE` means the installed copy
predates that key and has to be uninstalled first, which deletes its recorded
tracks. Export anything worth keeping before doing that.

## This repository

Installable builds of [PacTrac](https://github.com/0z00z0/pactrac). Artifacts
only. The source repo is private; this one is public so the app can check for and
download its own updates without carrying a token that could read anything else.

The platform is part of the tag, so both platforms live here side by side.

| Platform | Tag | Asset |
|---|---|---|
| Android | `android-v<versionName>+<versionCode>` | `pactrac-android-v<versionName>.apk` |
| iOS | `ios-v<versionName>+<versionCode>` | `pactrac-ios-v<versionName>.ipa` |

`versionCode` is one monotonic counter shared by both platforms, so a number
identifies one build of PacTrac rather than one build of one platform. The
update check reads the integer after the `+`.

## Release notes

Generated from the issues closed in the source repo since the previous release
of the same platform, grouped by category. A release that lists nothing had no
issues closed against it; it is still a real build.
