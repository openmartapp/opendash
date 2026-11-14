# Changelog

Notable changes, newest first. Versions follow `MAJOR.MINOR.PATCH`; each release on GitHub also
lists its commits.

## Unreleased

First public version.

- Three display modes: Direct (YouTube drawn straight onto the car screen), Built-in (OpenDash's
  views in up to 4 cells) and Virtual displays (installed apps in up to 4 cells, through Shizuku).
- Layouts, resizing and hiding cells on the phone and the car; touch, gestures and a floating menu
  on the car screen.
- Car, phone and Bluetooth remote buttons bound to OpenDash keys, per car.
- Websites, a media player for the phone's music, videos and streams, and pages made for OpenDash.
- YouTube in Direct mode, on YouTube's mobile site or its embedded player, with search on the phone
  and the car.
- Speed and speed limit over the video from the phone's GPS, OpenStreetMap or WazeMod.
- Dash Player: the car's media card, steering-wheel media keys and the Assistant's "play … on …".
- Voice commands from the car's 🎤, with rules the user can edit, shipped for English and
  Vietnamese; directions sent to the navigation app that is guiding.
- Setup wizard, log export, English and Vietnamese (Táp Lô and Kênh Xe on Vietnamese phones).

### 0.3.5 (2026-11-14)

- The free version now has every feature except voice commands and the YouTube player's controls
  and extra options: the media library, radio, split screens and your apps, the car's buttons, the
  speed and the next turn are free.
- New in the library: Radio, with your country's radio stations, and Shoutcast, with its most
  listened stations. Sound-only streams show a music note instead of a black screen.
- New on the car: **Browse**, lists of YouTube, the media library, radio and Shoutcast that a
  rotary knob or touchpad can use as well as a finger, with videos' pictures and album covers.
- For cars without a touch screen: a setting that puts Browse, Play/Pause and Next on the car's
  buttons.
- Album covers and video pictures in the media library.
- The phone's YouTube search has a microphone button: say what to find.
- Fixed: some streams added to the library did not play.

### 0.3.5-rc.6 (2026-11-14)

- Album covers and video pictures in the media library, on the car screen and in the car's lists.

### 0.3.5-rc.5 (2026-11-14)

- The car's lists show YouTube videos' pictures.
- The phone's YouTube search has a microphone button: say what to find.

### 0.3.5-rc.4 (2026-11-14)

- New on the car: **Browse**, lists of YouTube, the media library, radio and Shoutcast that a
  rotary knob or touchpad can use as well as a finger.
- For cars without a touch screen: a setting that puts Browse, Play/Pause and Next on the car's
  buttons.

### 0.3.5-rc.3 (2026-11-14)

- The free version now has every feature except voice commands and the YouTube player's controls
  and extra options: the media library, radio, split screens and your apps, the car's buttons, the
  speed and the next turn are free.
- Radio and other sound-only streams show a music note instead of a black screen.

### 0.3.5-rc.2 (2026-11-13)

- New in the library: Radio, with your country's radio stations, and Shoutcast, with its most
  listened stations.
- Fixed: some streams added to the library did not play.

### 0.3.5-rc.1 (2026-11-12)

- Test version: the exported log tells more about how the video plays, to find why it stutters on
  some phones.

### 0.3.4 (2026-11-11)

- Fixed: on Android 11, OpenDash closed by itself as YouTube opened on the car (0.3.2 and 0.3.3).

### 0.3.3 (2026-11-11)

- The video stutters less when the phone gets hot in the car.

### 0.3.2 (2026-11-11)

- Fixed: after a phone call, YouTube on the car could play on without sound. It now pauses for the
  call and plays again with its sound once the call is over.

### 0.3.1 (2026-11-10)

- Fixed: Play on the media card did nothing while another app filled the car screen. It now plays
  what you played last.
- The media card's picture shows only the speed limit sign.
- The phone stays cooler while playing on the car.

### 0.3.0 (2026-11-09)

- The speed bubble over the YouTube video can be moved: tap it on the car screen, then drag it.
  It stays where you leave it and never covers the voice button. Settings › Speed bubble size ›
  **Put it back on the driver's side** returns it to where it started.
- Settings › Speed sources › WazeMod (Wi-Fi HUD link) now says the link opens only while the car
  shows OpenDash; WazeMod cannot connect before that.
- Paid version: Settings › **Skip YouTube's ads**, off by default, leaves out YouTube's ads. YouTube's
  terms do not allow it, and YouTube may warn your Google account or stop playing videos. Nothing
  changes for a YouTube Premium account.

### 0.2.1 (2026-11-08)

- Fixed: after OpenDash was restarted, Update could fail with "Can't download" (a file name made
  from the release page). Updating to this version is enough; if it happens while updating to it,
  open OpenDash again later and tap Update.

- Fixed: on some phones (seen on a Sony, Android 11) voice commands on the car could not listen while
  the phone's screen was off. OpenDash now keeps the microphone while the car runs it (a quiet
  notification says so), and the car tells the phone's refusal apart from a missing permission.

- Buttons: the steering wheel's Play/Pause key can now be learnt and set like the others (update
  Dash Player too).

- The car's media keys reach OpenDash more reliably: OpenDash keeps Dash Player running while the
  car is connected, also when the phone closed it.

- Fixed: on some phones (seen on a vivo iQOO) voice commands always said to allow the microphone,
  though OpenDash had it: the phone's speech recognizer lacked it. The car now names the app that
  needs it, and Settings › Voice commands opens its settings.
- The buttons at the top of the car screen leave out the one for what is shown (YouTube, Library
  or Streams).
- Fixed: OpenDash could go a day or more without telling you about a new version when it had kept
  running in the background; it now looks for one whenever you open it (at most every 6 hours).
- Settings › Speed sources tells a Waze that cannot share its data (Google's Waze, or a WazeMod
  Legacy or Beta build) apart from no Waze at all, and says which WazeMod to install.
- Settings › Speed sources: WazeMod (Wi-Fi HUD link), for every WazeMod build, also those without
  the data API: OpenDash becomes WazeMod's Wi-Fi HUD on the phone itself. Off by default, for those
  who use a real HUD.
- Settings: the explanations of each setting now open from an (i) next to its title.
- Buttons: keys are called by their name and symbol ("⏭ Next button", "▲ Up button (phone,
  remote)") instead of Android's key codes.
- Settings › **Car screen**: **Classic** (as before) or **Alongside Google Maps** (recent
  Android Auto). With the second, Google Maps keeps showing its next turn after it was opened on
  the car, directions asked of OpenDash open Maps on the car screen while the music plays on, and a
  bar at the top of the car screen shows the next turn or what plays. OpenDash then opens from
  Android Auto's list of apps. The change applies from the next time the phone connects.
- The voice button works while another app (Google Maps) has the car screen: OpenDash listens
  without coming back and says what it heard and did in a notice on the car screen.
- Settings › **YouTube account**: sign in to YouTube on the phone. YouTube on the car then
  suggests videos for you, and the library on the car gets a **YouTube** tab with your liked
  videos, Watch later, playlists, mixes and history; a list plays on in its order.

### 0.1.6 (2026-11-06)

- When the car connects, OpenDash opens on the last YouTube video or library file you played and
  plays it (a stream is skipped for what played before it).
- Fixed: on some phones (seen on a Xiaomi), the paid version's buttons over the YouTube video did
  nothing and the video reloaded each time it came back on the car screen. Updating is enough; the
  licence code does not need to be entered again (the phone needs the internet once).
- Fixed: after OpenDash was updated, the paid version's buttons over the YouTube video could do
  nothing for up to a day.
- Fixed: in Direct mode, OpenDash kept the phone busy in the background once it had started (a
  warm phone and a draining battery), until it was next used on the car.

### 0.1.5 (2026-11-06)

- Settings › **Speed bubble size**: small (like the voice button), medium, large (as before, the
  default) or very large, for the speed and limit over the YouTube video.
- The speed bubble sits on the driver's side, in line with the voice button (on the right with
  Settings › Driver on the right).
- The voice button sits level with the car's own buttons at the top of the screen.
- A licence code moves to the last phone it is entered on; the phone before turns back to the free
  version and says why.

### 0.1.4 (2026-11-05)

- Android Auto's Assistant: "navigate to …" while OpenDash is on the car screen now opens the
  directions in your navigation app on the phone (it used to do nothing), also in the free
  version. OpenDash stays on the car screen.
- Directions asked for on the car start at once when the phone's screen is off, or it is locked
  with a swipe or kept unlocked by Smart Lock.
- With the phone locked by a PIN, pattern or password, the car shows a short notice at the top:
  unlock the phone for the directions to start, or open the navigation app on the car and ask there.
- The new-version notification now shows on Android 11 and 12.
- OpenDash's notifications use the new icon.

### 0.1.3 (2026-11-05)

- A new icon for OpenDash, easier to see on the car's dark screen, and a matching one for Dash
  Player.

### 0.1.2 (2026-11-05)

- The paid version needs the phone's clock right: with the date set back, OpenDash says so and
  stays on the free version until automatic date and time is on again.
- YouTube: only real video addresses are opened.
- The update dialog gives the right download size (about 6 MB).

### 0.1.1 (2026-11-05)

- The paid version: the YouTube player's controls, its state on Dash Player's card and the car's
  keys work as soon as the code is activated, without restarting OpenDash, and keep working after
  switching player or when the player opens again.

### 0.1.0 (2026-11-05)

- OpenDash is no longer open source: the code is private and this repository holds the releases
  and the user guides. Versions up to 0.1.0-rc.8 keep the GPL they were published under.
- A free version and a paid one. Free: YouTube on the car screen in Direct mode, with the car's
  search. Paid (one payment, a licence code for one phone): everything else, the player's
  controls, voice commands, speed, the next turn, the media library, favorites, Built-in and
  Virtual displays modes, the car's buttons and Dash Player. The Unlock screen shows the price,
  how to pay and a check that the phone can take a licence, before paying. Moving the code to a
  new phone: message us.
- A setup guide on the first start (also in Settings): display mode, permissions, Shizuku when
  needed, Android Auto. New installs start in Direct mode.
- Favorites on the phone show the video's picture.
- The home screen ends with the official website, the only place to get OpenDash.
- Smaller downloads: OpenDash about 5 MB (was 30), Dash Player about 150 KB.
- A copy of OpenDash changed and signed again by someone else says so, on the phone and the car,
  with where to get the official app. Only download it from this page.
- Settings › Third-party licenses lists the software OpenDash uses and their licenses.
- Update: KingInstaller opens afresh with the file to install, even when it was left open on an
  earlier screen.

### 0.1.0-rc.8 (2026-11-04)

- Direct mode: the media library beside YouTube. The car's buttons are YouTube, Library and
  Streams (icons only while a turn shows), then search. One plays at a time: the other one
  pauses, and the car's media card and keys follow the one shown.
- The phone's home screen has a Media library card in Direct mode: access to music and videos,
  the streams and files added, and Favorites.
- Videos and songs pick up where they stopped, with a Start over button for a few seconds.
- Favorites: ☆ on the car while something plays, a Favorites tab in the library, and a
  Favorites screen on the phone (play on the car, rename, reorder, delete).
- Shuffle: every list in the library starts with a row that plays all of it in a new order.
- The next turn from Google Maps beside the voice button (read from its notification, once
  allowed; nothing is stored), green near the turn. Settings › Next turn in Dash Player's card
  shows it under the song there too (off by default).
- Voice "directions to …" opens the navigation app again on Android 14 and later: allow OpenDash
  to display over other apps (Settings › Voice commands). With the phone locked, they start once
  it is unlocked.
- The voice button shows on every OpenDash screen on the car, below the part some car screens
  hide; the speed stays in sight while the player's controls show.
- The library goes on to the next song or video when one cannot play.
- The voice screen says which microphone listens.
- WazeMod: it connects again when its link drops, says when Waze's map has to run once for
  data, and can open Waze then (on by default).
- Phone keys: how to allow "restricted settings" on Android 13 and later.
- Direct mode on Android 11: switching between YouTube and the library no longer freezes the car
  screen.

### 0.1.0-rc.7 (2026-11-04)

- OpenDash checks GitHub for a new version (at most every 6 hours, when the app or the car starts)
  and says so on the phone, on the car screen and with a card on the home screen. Update downloads
  OpenDash and, if installed, Dash Player, checks them against the release's checksums and installs
  each one: through KingInstaller when OpenDash was installed with it (so it stays on Android
  Auto), else through the phone's own installer.
- Settings › Voice commands › A button for voice commands: Android Auto keeps the car's own voice
  key for Google Assistant, so another button can open OpenDash's voice commands instead (off by
  default; Previous unless another is picked). That button then only opens the voice commands.
- Buttons: tap a bound button to give it another function; the car's media buttons read "Car:
  Previous", "Car: Next", and so on.

### 0.1.0-rc.6 (2026-11-03)

- YouTube player: the controls hide again a few seconds after a video plays; since rc.5 they stayed
  on screen.
- Settings: a clear card when the microphone is not allowed, with a button to allow it, or to open
  the app's permissions once it was refused for good.
- YouTube player on small car screens (800x480): play/pause is an icon, text buttons keep to one
  line, icons are smaller, and the speed gauge hides under the controls.
- The voice button is red, apart from the car's own microphone (the Assistant's), easier to hit, and
  faded while the controls are hidden.
- A page that stays blank after the player is restored loads again; Reload opens the page that
  failed instead of the error page.

### 0.1.0-rc.5 (2026-11-02)

- The car's media keys and steering-wheel buttons (through Dash Player) can be learned and bound to
  OpenDash's keys; they drive the YouTube player by default, including forward and back 10 s.
- New keys: Forward 10 s, Back 10 s and Voice search, which opens the voice commands; search and
  assistant keys (SEARCH, VOICE_ASSIST, ASSIST) are bound to it by default.
- Previous starts the video again, and a second press goes back to the video before.
- YouTube player: a progress bar with the time and the length, to drag or tap to seek; icons for
  back and forward 10 s; a clearer player chooser (⚙).
- Direct mode: a voice button in the top corner on the driver's side, always shown; the car's action
  strip keeps only search. Skip ad moves to the driver's side too; Settings › Driver on the right
  for right-hand drive cars.
- Direct mode: buttons bound to keys (car buttons, phone, remote) work; they did nothing before.
- The "running" notification says what runs in each mode.

### 0.1.0-rc.4 (2026-11-02)

- Direct mode, YouTube website, Android 11 and 12: a video picked from the car's search now plays,
  instead of the one that played before (since 0.1.0-rc.3).
- Vietnamese install guide: the newer name of Android Auto's "Unknown sources" setting.

### 0.1.0-rc.3 (2026-11-01)

- Direct mode, YouTube website: no more "Loading YouTube…" that never ends when the player was left
  on YouTube's home page; it opens the last video or finds one.
- When Android Auto ends, the apps and the player close and the "running" notification goes away
  by itself; they open again on the next drive.
- WazeMod is found in both its builds: beside Waze, or installed in place of it (`com.waze`).
- A guide to installing WazeMod and connecting it ([`docs/wazemod.md`](docs/wazemod.md)).

### 0.1.0-rc.2 (2026-11-01)

A cooler phone and smoother video in Direct mode:

- YouTube's mobile site no longer draws its page under the player (ambient light, list spinner),
  which made the video drop frames.
- YouTube's quality is held to what the car screen needs (it kept 720p on a 480p screen).
- The YouTube page rests while it is hidden and not playing.
- On a phone with no YouTube history, the mobile-site player starts on a searched video instead of
  waiting on "Loading YouTube…".
- Docs: picture quality in the user guide; a 60 Hz phone screen for less heat and fewer dropped
  frames in Troubleshooting (English and Vietnamese).

### 0.1.0-rc.1 (2026-11-01)

The first test release, with everything above.
