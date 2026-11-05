# Voice commands

**English** | [Tiếng Việt](vi/voice-commands.md)

Tap 🎤 on the car screen and say what you want: "pause", a song to play, a place to drive to.
The phone's speech recognizer (usually Google's, which needs the internet) hears it, on the car's
microphone from Android 13 and on the phone's before that. The video pauses while it listens. The
car shows what was heard and what OpenDash does, then goes back to the video.

OpenDash does not use Android Auto's Assistant for this: the Assistant only passes requests to the
media app or navigation app it picks itself. With the Assistant, say Dash Player's name instead:
"play jazz on Dash Player" (on a phone set to Vietnamese: "phát nhạc jazz trên Kênh Xe"); Dash
Player hands the search to OpenDash, which plays the first video found.

## Settings

OpenDash › Settings › **Voice commands**:

- The switch shows or hides 🎤 on the car screen.
- **Language heard**: Vietnamese (the default) or English, or **Other** with a BCP 47 tag such
  as `fr-FR`. Each language has its own commands.
- **Edit commands**: the rules below, for the language heard.
- **App for directions**: **Automatic**, or one of the navigation apps on the phone. Automatic
  takes the app guiding now, else the one used last, else Google Maps. OpenDash knows WazeMod is
  guiding once WazeMod is connected as a speed source; for other apps, allow OpenDash to read
  notifications: it looks only at ongoing ones, and of the navigation app's reads only which app
  it is and its next turn (shown on the car, never stored).
- **Allow the microphone**, if you did not allow it the first time.
- **Allow display over other apps**: Android 14 and later keep an app in the background from
  opening another one, and OpenDash runs in the background while the car shows it. With this
  permission it shows a 1-pixel clear window for a moment to open the directions.

Directions open in the navigation app on the phone, which speaks through the car; with the phone
locked, they start once it is unlocked (within 5 minutes). The car screen
keeps showing OpenDash (Android Auto shows one navigation app at a time).

## The rules

Commands are plain text, one per line:

```
action: phrase | phrase | …
```

- `{text}` in a phrase takes what is said there: a song, a place. `youtube` and `navigate` need it
  in every phrase; the other actions must not have it.
- A phrase without `{text}` must be the whole sentence.
- When several phrases fit, one without `{text}` wins, then the one with the most words of its own.
- A sentence no phrase fits is searched on YouTube, whole.
- Case, punctuation and how accents are typed do not matter.
- A line starting with `#` is a comment. Lines OpenDash cannot read are listed under the editor
  and skipped; the others still work.

The actions:

| Action | Does |
| --- | --- |
| `youtube {text}` | Searches YouTube and plays the first video |
| `navigate {text}` | Directions to the place, in the app for directions |
| `play`, `pause` | Plays or pauses the video |
| `next`, `previous` | The next or previous video |
| `forward`, `rewind` | Jumps forward or back in the video |

For example, part of OpenDash's English rules:

```
# Keep the words that help the search: "play jazz music" searches "jazz music".
pause: pause | stop | be quiet
play: play | resume | continue
next: next | next song | skip
previous: previous | previous song | last song
forward: forward | skip ahead
rewind: rewind | back
navigate: directions to {text} | navigate to {text} | take me to {text} | drive to {text}
youtube: play {text} | open {text} | watch {text} | {text} on youtube
```

Under the editor, **Try a sentence** shows what a sentence would do with the rules as they are in
the editor, saved or not. **Save** keeps them for the next command; **Restore OpenDash's** goes back
to the rules OpenDash ships.

## Shipping rules for a language

OpenDash's own rules are files in `app/src/main/assets/voice/`, named by language (`vi.txt` is
used for `vi-VN` and any other Vietnamese). There are files for Vietnamese (`vi.txt`) and English
(`en.txt`). For other languages the rules start empty, and everything said is searched on YouTube
until you add commands. To share rules for your language, add a file there in a pull request.
