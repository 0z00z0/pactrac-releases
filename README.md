<p align="center">
  <img src="images/icon.svg" width="96" alt="PacTrac app icon: a yellow Pac-Man eating two dots along a street on a blue background">
</p>

<h1 align="center">PacTrac</h1>

<p align="center"><b>Every street in town, one dot at a time.</b><br>
Each street not yet covered becomes a trail of dots. Run or walk it, and the dots are gone. Waka waka.</p>

<p align="center">
  <img src="images/hero.jpg" width="100%" alt="Three PacTrac screens: a town map covered in yellow dots on every street, an activity that has just completed the street Brattlien with 63 dots in 476 metres, and the statistics screen with distance per week, dots per week and a 58-week streak">
</p>

<p align="center"><i>Real screens from the app, with demo data from Bergen.</i></p>

## A town full of dots

<img src="images/dots-everywhere.jpg" width="260" align="right" alt="Map of a town centre with yellow dots along every street and the Pac-Man position marker in the middle">

Open the map and every street still to cover glows with dots, from the high street to the narrowest alley.
A routine outing turns into a hunt. There is always one more street in sight.

<br clear="right">

## The map empties behind every step

<img src="images/dots-eaten.jpg" width="260" align="right" alt="An activity in progress: a pink trail where the dots have been eaten, with dots still ahead and the dots of the current street ringed in red">

Dots vanish underfoot and the score ticks up live.
Eat them in a row and the streak multiplier climbs to ×5. Red rings mark what is left of the current street, and the last dot swells into a power pellet.

<br clear="right">

## Street complete

<img src="images/street-complete.jpg" width="260" align="right" alt="A banner reading Brattlien complete, 63 dots, 476 metres, above the live numbers: pace, distance, time, streak ×5 and 2 streets finished">

Swallow the last dot and the street gets its name in lights: *Brattlien complete, 63 dots, 476 m.*
The panel tallies the streets finished on this outing and how many in the area are done.

<br clear="right">

## Numbers to beat

<img src="images/statistics.jpg" width="100%" alt="Statistics screens: distance walked, run and ridden for the week and for each year as bar charts, dots eaten per week, a 6-day and a 58-week streak">

- **Distance** walked, run and ridden, per week, month and year, or in total.
- **Dots eaten** per week, for the last twelve weeks.
- **Streaks** in days and in weeks, and every one of them begs not to be broken.
- **Activities** per month, each one in the list carrying its score.

## Based on CityStrides

PacTrac is based on [CityStrides](https://citystrides.com) statistics, and CityStrides is the record of which streets are finished.
Connect a CityStrides account and the map shows that record: finished streets in white, the rest still waiting to be eaten.
City percentages and comparisons with others stay on CityStrides, one tap from the app.

PacTrac is an independent app, not an official CityStrides product.

## A route full of new streets

The route planner builds an outing that sweeps up as many uncovered streets as it can: a round trip from the door, a drawn area, or a line through chosen points.
Arrows point the way, and the phone buzzes before each turn.

## Pick a look

<img src="images/designs.jpg" width="100%" alt="The same map in the three designs: Glass and Neon, CRT with 8-bit pixel icons, and Calm">

## More on the way

<img src="images/welcome.jpg" width="220" align="right" alt="The welcome tour: a Pac-Man maze with dots being eaten, above the line: PacTrac puts a dot on every street not yet run">

<br clear="right">

## Install on Android

1. Android 8 or newer is needed.
2. Open the newest `android-` release under [Releases](../../releases) on the phone and download the `.apk` file.
3. Open the file. Android asks once for permission to install apps from this source.

New versions arrive inside the app: it finds them and installs them itself.
A copy installed before the current signing key is refused as *App not installed*; remove it first, after exporting any activities worth keeping.

## This repository

Installable builds of PacTrac and nothing else. The source repository is private; this one is public so the app can check for and download its own updates.

| Platform | Tag | File |
|---|---|---|
| Android | `android-v<versionName>+<versionCode>` | `pactrac-android-v<versionName>.apk` |
| iOS | `ios-v<versionName>+<versionCode>` | `pactrac-ios-v<versionName>.ipa` |

The number after the `+` counts every build across both platforms, and the update check reads it.
Release notes list the issues closed since the previous release of the same platform; a release that lists nothing is still a real build.
