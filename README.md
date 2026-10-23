<p align="center">
  <img src="images/icon.svg" width="96" alt="PacTrac app icon: a yellow Pac-Man eating two dots along a street on a blue background">
</p>

<h1 align="center">PacTrac</h1>

<p align="center"><b>Run every street in town, one dot at a time.</b><br>
Every street not yet run becomes a trail of dots on the map. Run past them and they are eaten, Pac-Man style.</p>

<p align="center">
  <img src="images/hero.jpg" width="100%" alt="Three PacTrac screens: a town map covered in yellow dots on every street, a run that has just completed the street Brattlien with 63 dots in 476 metres, and the statistics screen with kilometres per week, dots per week and a 58-week streak">
</p>

<p align="center"><i>Real screens from the app, shown with demo data in Bergen.</i></p>

## Every street is a dot to eat

<img src="images/dots-everywhere.jpg" width="260" align="right" alt="Map of a town centre with yellow dots along every street and the Pac-Man position marker in the middle">

Open the map and every street still to run lights up with dots, from the main road to the smallest alley.
An ordinary run turns into a hunt: there is always a new street in sight.

<br clear="right">

## Watch the map empty behind the run

<img src="images/dots-eaten.jpg" width="260" align="right" alt="A run in progress: a pink trail where the dots have been eaten, with dots still ahead and the dots of the current street ringed in red">

Dots vanish as the run passes them, and the score counts up live.
Eat them in a row and the streak multiplier climbs to ×5. The dots left on the street underfoot are ringed in red, and the last one on a street grows into a power pellet.

<br clear="right">

## The best moment: street complete

<img src="images/street-complete.jpg" width="260" align="right" alt="A banner reading Brattlien complete, 63 dots, 476 metres, above the live numbers: pace, distance, time, streak ×5 and 2 streets finished">

Eat the last dot and the street is announced by name: *Brattlien complete, 63 dots, 476 m.*
The panel counts the streets finished on this run and how many in the area are done.

<br clear="right">

## Numbers for the self-competitive

<img src="images/statistics.jpg" width="100%" alt="Statistics screens: kilometres run, walked and ridden for the week and for each year as bar charts, dots eaten per week, a 6-day and a 58-week streak">

- **Kilometres** run, walked and ridden, per week, month and year, or in total.
- **Dots eaten per week**, for the last twelve weeks.
- **Streaks** in days and in weeks, the kind that are hard to break.
- **Activities per month**, and every run in the list carries its score.

## Built on CityStrides

[CityStrides](https://citystrides.com) is the wonderful community project behind street running.
It records every street a runner has covered, in every city, and gives each run a purpose: finish all the streets.

- PacTrac is based on CityStrides statistics.
- Connect a CityStrides account, and the map shows the runner's own record: streets already finished in white, the rest still to eat, in any town the map is moved to.
- City percentages, the full record of places run and the league live on CityStrides, one tap away from the app.

CityStrides remains the record of which streets are finished. PacTrac is an independent app, not an official CityStrides product.

## A route full of new streets

The route planner builds a run that collects as many unrun streets as possible: a round trip from the door, a drawn area, or a route through chosen points.
Arrows on the map show the way, and the phone buzzes before each turn.

## Pick a look

<img src="images/designs.jpg" width="100%" alt="The same map in the three designs: Glass and Neon, CRT with 8-bit pixel icons, and Calm">

Glass + Neon, CRT + 8-bit pixel, or Calm, each with its own icons, plus a Daylight setting for bright sun.

## More on the run

<img src="images/welcome.jpg" width="220" align="right" alt="The welcome tour: a Pac-Man maze with dots being eaten, above the line: PacTrac puts a dot on every street not yet run">

- **Flags with spoken notes:** mark a place on the route and dictate a note while running.
- **Same dots on every phone:** settings and eaten dots follow the account, with sign-in by passkey.
- **A welcome tour** on the first start explains the map and the sign-ins.
- **Private by default:** recorded runs stay on the phone.

<br clear="right">

## Install on Android

1. Android 8 or newer is needed.
2. Open the newest `android-` release under [Releases](../../releases) on the phone and download the `.apk` file.
3. Open the file. Android asks once for permission to install apps from this source.

New versions arrive inside the app: it finds them and installs them itself.
A copy installed before the current signing key is refused as *App not installed*; remove it first, after exporting any runs worth keeping.

## This repository

Installable builds of PacTrac and nothing else. The source repository is private; this one is public so the app can check for and download its own updates.

| Platform | Tag | File |
|---|---|---|
| Android | `android-v<versionName>+<versionCode>` | `pactrac-android-v<versionName>.apk` |
| iOS | `ios-v<versionName>+<versionCode>` | `pactrac-ios-v<versionName>.ipa` |

The number after the `+` counts every build across both platforms, and the update check reads it.
Release notes list the issues closed since the previous release of the same platform; a release that lists nothing is still a real build.
