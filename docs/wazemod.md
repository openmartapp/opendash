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

- **The version.** Take the newest one marked stable or newest (V14 or newer), not a Beta or a
  **Legacy** build: those may not have the data API, and OpenDash then cannot read them.
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

## Without the data API: OpenDash as WazeMod's Wi-Fi HUD

Some WazeMod builds (the **Legacy** ones) have no data API, but every build can drive a HUD over
Wi-Fi. OpenDash can pose as that HUD, on the phone itself:

1. In OpenDash: Settings › **Speed sources**, turn on **WazeMod (Wi-Fi HUD link)**.
2. In WazeMod's settings: **Kết nối với thiết bị** › tab **HUD WazeMod (Wi-Fi)**:
   - **Địa chỉ IP / hostname HUD**: `127.0.0.1`
   - **Cổng WebSocket**: `8765`
   - **Đường dẫn WebSocket**: `/hlp`
   - then turn on **Bật HUD WazeMod**.
3. Open Waze's map. The row in OpenDash says **Connected** once the car screen shows OpenDash.

OpenDash opens this link only while the car screen shows OpenDash (as every speed source). Before
that, at home without the car, WazeMod says it cannot connect: that is expected. Its row in
OpenDash then says **Opens when the car shows OpenDash**.

WazeMod drives only one HUD. If you use a real HUD with WazeMod, leave this source off and keep the
data API source, or pick one of the two. When WazeMod finds no HUD for 2 minutes it stops looking
until Waze's map opens again; OpenDash opens Waze for it when the car screen starts (the **Open Waze
when it has no data** choice).

## If it does not work

- **"This Waze does not share its data"** under WazeMod: the Waze on the phone is Google's, or a
  WazeMod build without the data API (a Legacy or Beta build, or one older than V14). Install the
  newest stable build.
- **"Not installed"** under WazeMod: no Waze was found on the phone.
- **No speed while driving:** WazeMod gives a speed while it is open and has a GPS fix; start it
  once before the drive. Check that WazeMod is switched on in **Speed sources**.
- **Not allowed in WazeMod yet:** tap **Connect WazeMod** again and choose **Allow**.

For WazeMod itself (install problems, maps, alerts): the
[Facebook group](https://www.facebook.com/groups/wazevn) and the support chat linked on
[wazemod.io.vn](https://wazemod.io.vn/).
