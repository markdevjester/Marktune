<p align="center">
  <img src="https://markdev.app/media/tools/marktune-icon.png" width="128" alt="Marktune icon">
</p>

<h1 align="center">Marktune</h1>

<p align="center">
  <b>A retro music player that lives on the edge of your Mac's screen.</b><br>
  Pull the little tab, and the player slides out over any window. Free, no account.
</p>

<p align="center">
  <a href="https://markdev.app/tools/#marktune">Download</a> ·
  <a href="#styles">Styles</a> ·
  <a href="#services">Services</a> ·
  <a href="#privacy">Privacy</a> ·
  <a href="README.ru.md">Русский</a>
</p>

<p align="center">
  <img src="https://markdev.app/media/tools/marktune-player.jpg" width="900" alt="Marktune player slid out from the right edge of a Mac desktop">
</p>

## Why

To skip a song you usually have to find the right browser tab or app window, click, and go back to what you were doing. Marktune keeps the player one pull away: a small tab sits on the edge of the screen, above every window and on every desktop. Pull it, and the player springs out. Push it back, and it's gone.

## Styles

<p align="center">
  <img src="https://markdev.app/media/tools/marktune-skins.jpg" width="900" alt="Four player styles: Digital, Disc, Cassette and Glass">
</p>

- **Digital.** A brushed-aluminium MP3 player. Turn the click wheel to scrub: every notch is 2 seconds and clicks like a revolver drum.
- **Disc.** A round CD player in spun metal. Grab the disc and spin it to scrub, with a vinyl scratch sound.
- **Cassette.** Drag the cassette left or right to wind the tape. The piano keys clunk like real ones.
- **Glass.** A modern card that takes its colours from the album cover.

Each style comes in several finishes. Pick one in the menu bar ♪ → **Player Style**, or right-click the player. The sounds are synthesized live and can be turned off in ♪ → **Player Sounds**.

## Services

Choose in the menu bar ♪ → **Source**:

- **YouTube Music**, **Spotify** and **Yandex Music** play from their own websites inside Marktune. Sign in once on the service's page, and the sign-in is kept.
- **Apple Music** controls the Music app on your Mac.

Press ≡ (or **Menu**) and a panel opens next to the player: the queue, your playlists and search. Pick any song from a playlist and it plays.

<p align="center">
  <img src="https://markdev.app/media/tools/marktune-queue.jpg" width="900" alt="Queue panel next to the player">
</p>

## How to use

- **The tab:** click to show or hide the player. Pull it away from the edge to open, push it back to hide.
- **Move it:** drag the player up or down along the edge. Left or right edge: ♪ → **Screen Edge**.
- **Resize:** drag the corner handle, or ♪ → **Size**.
- **Hide When Clicking Outside**, **Player Sounds** and **Launch at Login**: all in the ♪ menu.

## Install

1. Download `Marktune-1.0.0.zip` from [markdev.app](https://markdev.app/tools/#marktune) or [Releases](https://github.com/markdevjester/Marktune/releases/latest), unzip it and move `Marktune.app` to **Applications**.
2. First launch: the app isn't notarized by Apple yet, so macOS says it can't verify the developer. Open **System Settings → Privacy & Security**, scroll down and click **Open Anyway**.
3. A ♪ appears in the menu bar and the tab appears on the right edge of the screen. Pull it, press ▶ and sign in to your service.

Requires macOS 14 or later. Apple Silicon and Intel.

## Privacy

- Marktune never sees your password: you sign in on the service's own page (Google, Spotify or Yandex) inside the app, and the session is kept in the app's web storage.
- There's no account, no analytics and no servers of mine. The app talks only to the music service you chose.
- Apple Music: macOS asks once for permission to control the Music app.
- Marktune doesn't download music or block ads. It plays your own subscription through the service's official web player.

## How it works

YouTube Music, Spotify and Yandex Music have no public playback API for desktop apps, so Marktune opens their regular website in an invisible `WKWebView`. It reads the title, cover and time from the page and presses the page's own buttons with JavaScript. Queue, playlists and search use the same requests the website makes. Apple Music is controlled with AppleScript. Native Swift and SwiftUI.

## License

Free to download and use, including at work. The source code is closed. See [LICENSE](LICENSE).

Made by [markdev](https://markdev.app). Bugs and ideas: open an issue.
