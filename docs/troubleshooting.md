# Troubleshooting

**English** | [Tiếng Việt](vi/troubleshooting.md)

To send a useful bug report, open OpenDash › Settings (gear) › **Export log** right after the
problem happens and send the file. It includes OpenDash's recent log from every process and your
phone model and Android, Android Auto and Shizuku versions. With a computer, `adb logcat -s OpenDash`
shows the same log live.

## Setup

**"Start Shizuku" stays unticked after a restart.** Shizuku stops whenever the phone restarts. Make
sure Wireless debugging is on and the phone is on Wi-Fi, open Shizuku and tap **Start**.

**Wireless debugging turns itself off.** It needs a Wi-Fi connection and turns off when Wi-Fi
drops or you change networks. Turn it back on (and allow the network) before starting Shizuku.

**"Allow OpenDash" shows permission denied.** You chose Deny earlier. Open Shizuku › Authorized
applications and turn OpenDash on.

**An app is missing from the app list.** The list shows apps with a launcher icon. Apps you have
disabled (Settings › Apps › the app › Enable) do not appear.

## Android Auto

**OpenDash is not in the car's app launcher.** Turn on Android Auto developer mode and **Unknown
sources** (install guide, step 7), then disconnect and reconnect the car.

**Android Auto shows "Communication error 14" with the Desktop Head Unit.** The DHU's certificate
has expired for older Android Auto versions; update Android Auto (17.x works).

**Android Auto closes after changing Settings › Car screen.** Its bar at the bottom can keep
OpenDash's old icon for a few minutes, and tapping that icon closes Android Auto. Open OpenDash from
Android Auto's list of apps instead; if Android Auto closed, reconnect the phone.

**The car screen shows an old picture after updating or reinstalling OpenDash.** OpenDash asks the
car for a new surface after about 3 seconds (you may see "Reconnecting…" briefly). If it stays
frozen, open the car's app launcher and choose OpenDash again.

**OpenDash's buttons on the car screen.** They are behind the round OpenDash button on the line
between two cells (the line between columns, or between rows for cells above each other), so it
covers no app: tap it to open Layout, Back, Apps and Info, tap it again to close them; they also
close after 10 seconds. The button follows the line when the cells are resized. With a single cell
(or one cell enlarged or hidden) it sits on an edge of the screen instead. Android Auto also shows
one OpenDash button of its own in the top corner (it hides after a few seconds; tap the screen to
show it): it opens the same menu.

**Resizing the cells.** On the phone preview, drag the grey handle on the line between two cells (on
the line that holds the car's OpenDash button, the handle sits just below or beside where the button
goes). A cell keeps at least a third of the screen; drag past that and it shows "Release to hide". A
hidden cell's handle stays at the screen edge: drag it back to show the app again (it kept running).
On the car screen, tap the handle: the line moves to a third, half, then two thirds of the screen,
then to the far edge (the cell before it fills the screen and the other hides), then to the near
edge (the cell after it fills the screen), and round again to a third. A hidden cell's handle stays
at the screen edge so you can tap it. Only
the handle (and a finger's width around it) does this: a tap elsewhere on the line goes to the app
under it. Android Auto does not tell apps where a drag starts, so the car cannot drag the line
itself. Cells above each other stay half and half unless the car screen is taller than wide.

**The steering wheel's arrow or media buttons do nothing in OpenDash.** Android Auto keeps the
car's arrow keys and rotary knob for its own focus, and sends media keys to its media app, so apps
like OpenDash never get them. What works instead: OpenDash's extra buttons on the car screen
(the knob can select them), swipes and pinches on the car's touch screen, and keys on the phone or
a Bluetooth remote. Set them up in Settings › **Set up buttons** (or Info › Car buttons on the
car). Keys on the phone need Settings › Accessibility › **OpenDash buttons** turned on; they only
act while the car shows OpenDash.

**Back or Apps acts on the wrong cell.** They act on the selected cell, the one with the blue
outline: the last one you tapped on the car screen.

**Scrolling in one cell moves another.** Tap the cell first, then scroll or swipe. Android Auto
tells apps where a tap is, but only how far a drag or swipe moved, not where the finger is, so
OpenDash sends drags, scrolls and swipes to the selected cell (blue outline). A tap selects the
cell under it. Pinches are not affected: they say where they are.

## Direct mode and YouTube

**"Loading YouTube…" stays, or "Can't load YouTube".** Tap **Retry**, or Reload in OpenDash's
controls (tap the video). With nothing to resume, the player starts on a video it searches for, so
it also needs the internet for that. Check that the phone has internet. If you have both a release and a debug
build of OpenDash installed, Android Auto may open the other one: keep only one.

**A video does not play in the IFrame player.** Its owner does not allow it on other sites. Choose
the YouTube website in Settings › **YouTube player**.

**The sound stops when a map takes the car screen.** That is the default. Turn on Settings › **Play
on behind other apps** to keep it going.

**No speed or limit over the video.** Settings › **Speed sources**: turn one on and allow what it
asks (location for GPS and OpenStreetMap, WazeMod's consent for WazeMod). OpenStreetMap only knows
the limits mapped there, and a road driven for the first time needs the internet once.

**The phone gets hot, or the video stutters on the car.** If the phone's screen runs at 90 or 120 Hz,
OpenDash and the WebView keep that pace while the car shows the video, even with the phone screen
off. Set the phone to 60 Hz: on Samsung, Settings › Display › **Motion smoothness** › **Standard**; on
Pixel, turn off Settings › Display › **Smooth Display**; on other phones, look for **Refresh rate**
under Display. On a test phone this left fewer dropped video frames and less work for the phone.
Charging, wireless Android Auto and sun on the phone also warm it up: a cable and a shaded,
ventilated holder help.

## Dash Player and the car's media controls

**Dash Player is not in Android Auto's media apps.** Install `dashplayer-<version>.apk` from the
same release as OpenDash: Dash Player only works with an OpenDash signed alike. Android Auto may need
a reconnect to list it, and "Unknown sources" on (install guide, step 7).

**The media card says "Open OpenDash on the car".** Dash Player only passes things on: open
OpenDash on the car screen once, then the card and the steering-wheel keys control it.

**The steering-wheel keys do nothing (often on vivo, iQOO, Xiaomi, OPPO).** Android Auto sends them
to its media app, Dash Player, which must be running. OpenDash keeps it running, but some phones only
let Android Auto start it. Make Dash Player Android Auto's media app: open **Dash Player** once from
Android Auto's app list on the car; Android Auto then starts it each time the car connects. If you
play another music app, open Dash Player again afterwards.

**"Play … on Dash Player" plays something else.** Say the name as the phone shows it (**Kênh Xe** on
a phone set to Vietnamese). The Assistant picks apps by that name; OpenDash's own 🎤 needs no name.

## Voice commands

**"Allow OpenDash to use the microphone".** Allow it on the phone when asked, or in Settings ›
Voice commands › **Allow the microphone**.

**"Allow the microphone for Speech Recognition and Synthesis from Google" (or another app's name),
though OpenDash has it.** The phone's speech recognizer hears the commands, and Android gives it
the sound only if it may use the microphone too, even when the car's microphone listens. On some
phones it may not, out of the box. Settings › Voice commands › **Open its settings**, then
Permissions › Microphone › Allow.

**"Speech recognition needs the internet" or "is not available".** OpenDash uses the phone's speech
recognizer, usually Google's: it needs the internet and must support the language heard. Check that
speech recognition works in another app, such as the keyboard's microphone.

**It hears the wrong thing, or does the wrong command.** Check Settings › Voice commands ›
**Language heard**. In **Edit commands**, type what it heard into **Try a sentence** to see which
rule fits, then add the words you say ([`voice-commands.md`](voice-commands.md)).

**Directions open the wrong app.** Settings › Voice commands › **App for directions**: choose one,
or allow reading navigation notifications so Automatic knows which app is guiding.

## Apps in the cells

**A cell is black with "This app blocks screen projection".** The app (often banking or payment
apps, or private browser tabs) forbids screen capture, so the system shows it as black in any
virtual display. Use another app in that cell.

**An app keeps restarting.** OpenDash restarts apps that stop, up to 5 times in a row, then shows
an error for the cell. The app may not support running on a second display; try it on its own in
the Full layout.

**An app shows letterboxed (bars at the sides) or does not fill its cell.** Apps that only support
portrait, such as the YouTube Shorts player, are shown upright with bars instead of sideways.

**Text is too small or too large.** OpenDash picks the density from the car screen size and the
cell size. Change it for every cell in Settings › **Text and icon size**.

**Cells show "Paused while the phone is locked".** Some phones turn OpenDash's displays off, or
show them black, while the phone is locked: seen on Android 17 and on some Samsung
phones with Android 16. The apps continue when you unlock the phone. Turn on Settings › **Keep apps running with the
screen off**: while the car shows OpenDash, the power key (or the screen timeout) then darkens the
phone screen instead of turning it off, so the apps keep running. Press the power key to see the
phone again; the lock screen shows as usual. When the car disconnects, the phone goes back to
normal.

**Websites or the player stop when the phone is locked (built-in mode).** They should not:
OpenDash's views draw on displays of their own that Android never turns off with the phone screen
(checked on Android 11, 13, 15 and 17). If they do on your phone, export a log (Settings › Export
log) and tell us the phone model. Also allow OpenDash to run in the background, as below.

**The phone screen stays on while a cell plays a video.** A website playing a video asks Android to
keep the screen on, and Android applies that to the phone screen. OpenDash undoes it unless
Settings › **Let videos keep the phone screen on** is on; turn that off and the phone screen times
out as usual while the video keeps playing on the car.

**Apps stop or restart when the screen is off (other phones).** Allow OpenDash to run in the
background: Settings › Apps › OpenDash › Battery › Unrestricted (Xiaomi: also Autostart).

## Phone app

**The preview says "Showing on the car screen".** While the car shows OpenDash, the phone preview
pauses; use the car screen.

**The app search in landscape.** With the keyboard open there is no room for the list, so the
matching apps show as buttons above the search field; the search key opens the app if only one
matches.
