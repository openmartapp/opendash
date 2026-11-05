# WazeMod: speed and speed limit from Waze

**English** | [Tiếng Việt](vi/wazemod.md)

WazeMod is a modified Waze made by a community developer, not by OpenDash or Waze. It can share
its speed and the road's speed limit with other apps through its data API. OpenDash shows them
over the video in Direct mode and on the car's media card, like its other speed sources.

OpenDash does not host or vouch for WazeMod. Download it only from its official website,
[wazemod.io.vn](https://wazemod.io.vn/), and ask its own community for help with it (links at the
end).

## 1. Choose the build

On [wazemod.io.vn](https://wazemod.io.vn/), open **Download** (or **Tải APK Waze Mod** in the
menu), then pick:

- **The version.** Take the newest one marked stable or newest, not a Beta: a Beta build may not
  have the data API yet, and OpenDash then cannot read it.
- **Your Android version** (OpenDash itself needs Android 11 or newer).
- **"Có Android Auto"** if you also want Waze on the car screen; **"Đã gỡ AA"** removes it.
- **The install type:**
  - **DUAL** installs beside Google's Waze; both stay on the phone, each with its own data.
  - **Cài đè** (in place) replaces Google's Waze: uninstall Google's Waze first.

OpenDash finds WazeMod with either install type.

## 2. Install it

1. Allow your browser (or file manager) to install apps: Android asks the first time you open an
   APK; answer **Settings** › **Allow from this source**.
2. For **Cài đè**, uninstall Google's Waze first (your saved places stay in your Waze account).
3. Open the downloaded APK and tap **Install**.
4. Open WazeMod once, sign in or skip, and allow location.

The website's **Hướng dẫn cài đặt APK** page shows these steps with pictures.

## 3. Connect it to OpenDash

1. In OpenDash: Settings › **Speed sources**. WazeMod's row says **Connect WazeMod**.
2. Tap it: WazeMod asks whether OpenDash may read its data (speed, limit, turns, alerts, arrival
   time, street names; not your GPS position). Tap **Allow**.
3. Move **WazeMod** up the list if it should come before the phone's GPS and OpenStreetMap.

You can take the permission back in WazeMod: Settings › connected apps. OpenDash then shows the
next source in the list.

## If it does not work

- **"Not installed"** under WazeMod: the build has no data API (often a Beta). Install the newest
  stable build.
- **No speed while driving:** WazeMod gives a speed while it is open and has a GPS fix; start it
  once before the drive. Check that WazeMod is switched on in **Speed sources**.
- **Not allowed in WazeMod yet:** tap **Connect WazeMod** again and choose **Allow**.

For WazeMod itself (install problems, maps, alerts): the
[Facebook group](https://www.facebook.com/groups/wazevn) and the support chat linked on
[wazemod.io.vn](https://wazemod.io.vn/).
