# Installing OpenDash

**English** | [Tiếng Việt](vi/install.md)

Do this once, at home or parked, with the phone on Wi-Fi. It takes about 10 minutes. The OpenDash
app walks you through the same steps and ticks each one when it sees it done.

## 1. Install OpenDash

Download `opendash-<version>.apk` from the [Releases page](../../../releases/latest) and open it. Allow your browser or file
manager to install apps when asked.

Google Play Protect may show **App scan recommended** ("Play Protect hasn't seen this app before"),
also when OpenDash updates itself: it has not seen this new file yet. Tap **Scan app** to have
Google check it first, or **More details** › **Install without scanning**.

Also install `dashplayer-<version>.apk` from the same release if you want the car's media card,
the steering-wheel media keys and Android Auto's search to control OpenDash's player. It has no
screen of its own; Android Auto lists it with its media apps as **Dash Player**.

On a phone set to Vietnamese, the apps are named **Táp Lô** (OpenDash) and **Kênh Xe** (Dash
Player): words Google's Vietnamese voice recognition hears well.

Steps 2 to 6 are only for virtual-display mode (your installed apps in the cells). For Direct mode
(YouTube, the default) and built-in mode, skip to step 7.

## 2. Install Shizuku

Shizuku gives OpenDash the permissions it needs to create virtual displays, without root.
Install it from [Google Play](https://play.google.com/store/apps/details?id=moe.shizuku.privileged.api)
or [GitHub](https://github.com/RikkaApps/Shizuku/releases) (the "Get Shizuku" button in OpenDash
opens the download page).

## 3. Turn on Developer options

Settings › About phone › tap **Build number** 7 times (enter your PIN if asked).

| Phone | Where "Build number" is |
| --- | --- |
| Pixel, most phones | Settings › About phone |
| Samsung | Settings › About phone › Software information |
| Xiaomi, Redmi, POCO | Settings › About phone › tap **MIUI version** / **OS version** |

## 4. Turn on Wireless debugging

Settings › System › Developer options › **Wireless debugging** › on. Allow it for your Wi-Fi network.
Your phone must be on Wi-Fi (any network; it does not need internet).

## 5. Start Shizuku

Open Shizuku › **Start via Wireless debugging** › **Pairing**, then follow its steps: it asks you to
open "Pair device with pairing code" in Wireless debugging and type the code into Shizuku's
notification. Pairing is needed once; then tap **Start**.

Shizuku stops when the phone restarts. Open Shizuku and tap **Start** again after every restart
(Wireless debugging must be on and the phone on Wi-Fi for that moment). With root, Shizuku can start
by itself instead.

## 6. Allow OpenDash

In OpenDash, tap **Grant permission** and choose **Allow all the time**. The setup card now shows
"Service connected".

## 7. Show OpenDash in Android Auto

Android Auto only lists apps from outside the Play Store in its developer mode:

1. Open Android Auto settings (the button in OpenDash opens them).
2. Scroll down and tap **Version** 10 times; allow development settings.
3. ⋮ (top right) › **Developer settings** › turn on **Unknown sources**.

If Android Auto is turned off on your phone, the button opens its store page instead: turn it back
on there. Update Android Auto if it is older than version 17.

## 8. Choose your apps and connect the car

In OpenDash, choose the display mode in Settings. In virtual-display or built-in mode, pick a
layout and an app or view for each cell. Then connect the car (cable or wireless), open the app
launcher on the car screen and choose **OpenDash**. The last setup step ticks itself the first
time OpenDash opens on the car.

With cells, on the car screen: tap a cell to select it (blue outline), then use the round OpenDash
button for **Layout**, **Back** and **Apps**.

## Voice commands

The first time you tap 🎤 on the car screen, the phone asks to allow the microphone (or allow it
beforehand in OpenDash › Settings › Voice commands). See [`voice-commands.md`](voice-commands.md).

## Battery settings

Some phones close background apps aggressively. If apps in the cells stop or restart while the
screen is off, allow OpenDash to run in the background: Settings › Apps › OpenDash › Battery ›
**Unrestricted** (Xiaomi: also turn on **Autostart**).

## Trying it without a car

Google's Desktop Head Unit (DHU) shows Android Auto on a computer. Install "Android Auto Desktop
Head Unit Emulator" with the Android SDK manager, turn on Android Auto developer mode (step 7), then
in Android Auto settings ⋮ › **Start head unit server**, and on the computer:

```sh
adb forward tcp:5277 tcp:5277
$ANDROID_HOME/extras/google/auto/desktop-head-unit
```

On Linux the DHU may fail with `libc++.so.1: cannot open shared object file`. Install libc++ from
your distribution, or point it at the NDK's copy:
`LD_LIBRARY_PATH=$ANDROID_HOME/ndk/<version>/toolchains/llvm/prebuilt/linux-x86_64/lib/x86_64-unknown-linux-gnu`.
