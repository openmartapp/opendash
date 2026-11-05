# OpenDash

**English** | [Tiếng Việt](README.vi.md) · Website: [opendash.openmart.app](https://opendash.openmart.app)

**Your phone's apps and views on the car screen, side by side, through Android Auto.**

OpenDash is an Android app by OpenMart, free to download, with a paid version (a licence code). It runs the apps you choose in virtual displays (through
[Shizuku](https://shizuku.rikka.app/), no root) or shows its own views (YouTube, a media library,
websites), puts them together in one frame and shows that frame on the car screen, with touch from
the car going to the right app.

This repository holds OpenDash's releases and user guides. OpenDash is not open source.

> [!WARNING]
> **Drive safely.** OpenDash shows apps that were not designed for use while driving. Set it up
> while parked, keep your eyes on the road, and follow the law where you drive. You are
> responsible for how you use it.

## Features

Three display modes, each with its own setup:

| Mode | Shows | Needs |
| --- | --- | --- |
| **Direct** (default) | YouTube or the media library, drawn straight onto the car screen for the smoothest picture, with the speed, the speed limit and the next turn | Nothing extra |
| **Built-in** | Up to 4 of OpenDash's own views: websites, a media player, pages made for OpenDash | Nothing extra: banking apps that refuse to run with debugging on keep working |
| **Virtual displays** | Up to 4 of your installed apps, each laid out for its cell | Shizuku, started with Wireless debugging or root |

- **Layouts:** full screen, side by side, stacked, 1 large + 2 small, or 2 × 2; cells can be resized
  or hidden, on the phone or the car.
- **Touch on the car screen:** tap, drag, fling and pinch go to the app under your finger. A floating
  OpenDash button opens Layout, Back, Apps and Info, so you need not touch the phone.
- **Keeps running** when you change the layout, lock the phone or the wireless link drops for a moment.
  When Android Auto ends, the apps close and OpenDash stops; they open again on the next drive.
- **Dash Player**, a small companion app, brings the car's media card, steering-wheel media keys and
  Android Auto's search to the player.
- **Voice commands** from the 🎤 button on the car screen: play, pause, skip, search YouTube, or get
  directions in your navigation app. Commands are plain text rules you can edit in the app, for any
  language; English and Vietnamese are included.
- **Speed and speed limit** from the phone's GPS, OpenStreetMap or WazeMod.
- **Setup wizard** that checks each step itself. English and Vietnamese.

**Status:** early development (0.x). It works on Google's Desktop Head Unit and on the phones it was
tried on. Reports from real cars and head units are very welcome.

## Requirements

- Android 11 or newer.
- Android Auto, with its developer mode and **Unknown sources** on (OpenDash is not on the Play Store).
- A car or head unit with Android Auto (wired or wireless), or Google's Desktop Head Unit to try it.
- Virtual-display mode only: [Shizuku](https://shizuku.rikka.app/) 11 or newer.

## Install

1. Download `opendash-<version>.apk`, and `dashplayer-<version>.apk` if you want the car's media
   controls, from the [latest release](../../releases/latest). Only download OpenDash from here:
   copies offered elsewhere, especially for money, may have been changed.
2. Install them, then open OpenDash: its setup wizard walks you through the rest.

Step by step, with what each mode needs: [`docs/install.md`](docs/install.md). Then:
[`docs/user-guide.md`](docs/user-guide.md). Each release lists the SHA-256 of its APKs (`SHA256SUMS`).

## Documentation

| For | Read |
| --- | --- |
| Installing and setting up | [`docs/install.md`](docs/install.md) |
| Using OpenDash: modes, the car screen, buttons, settings | [`docs/user-guide.md`](docs/user-guide.md) |
| Voice commands and their rules | [`docs/voice-commands.md`](docs/voice-commands.md) |
| Speed and speed limit from WazeMod | [`docs/wazemod.md`](docs/wazemod.md) |
| Something does not work | [`docs/troubleshooting.md`](docs/troubleshooting.md) |
| What changed | [`CHANGELOG.md`](CHANGELOG.md) |

## Privacy

OpenDash has no account, no ads, no analytics and no crash reporting. It sends nothing about you to
its developers. What it does with the permissions it asks for:

- **Location:** only while the car shows the speed, to measure it with the phone's GPS. It stays on
  the phone, except that the OpenStreetMap speed-limit source asks a public
  [Overpass](https://overpass-api.de/) server for the roads of the area you are in (map tiles about
  2 km wide around the car), cached on the phone for 30 days.
- **Microphone:** only while the voice screen listens. The audio goes to the phone's speech
  recognizer (usually Google's, under Google's terms), not to OpenDash's developers.
- **Notifications** (optional): to know which navigation app is guiding and to show its next turn
  on the car. OpenDash looks only at ongoing notifications and reads only the navigation app's: which
  app it is and its next turn, never stored.
- **Network:** the websites and streams you open, YouTube for the player and its search, and the
  Overpass server above.
- **Display over other apps** (optional): only to open directions asked for on the car, with a
  1-pixel clear window for a moment.
- **Logs:** kept on the phone. Settings › Export log makes a file you can choose to share; it holds
  OpenDash's log and your phone's model and Android, Android Auto and Shizuku versions.

## Community

News, release notes and questions: the [website](https://opendash.openmart.app) and the [Táp Lô - OpenDash Facebook page](https://www.facebook.com/taplo.opendash)
(mostly in Vietnamese). Bugs go to [GitHub issues](../../issues), where they don't get lost.

## Terms of use

Copyright © 2026 OpenMart. All rights reserved. OpenDash is free to download; its paid version
needs a licence code from OpenMart. Selling it or its codes, changing or repackaging it, getting
around its licence check, or reverse engineering it is not allowed: see [`LICENSE`](LICENSE). The
third-party software it uses and their licenses are listed in the app, in Settings › Third-party
licenses. Speed limits © [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors (ODbL).

OpenDash is not affiliated with or endorsed by Google or YouTube. Android Auto and YouTube are
trademarks of Google LLC.
