# OBS YouTube Playlist Player (GitHub Pages, no hardcoded playlist)

## Setup (GitHub Pages)
1. Create a repo (e.g., `obs-youtube-player`) and upload `index.html` to the root of `main`.
2. Settings → Pages → Source: **Deploy from a branch**, Branch: **main** / **root** → Save.
3. Use the Pages URL in OBS (**Browser** source, uncheck *Local file*).

## URL (playlist param required)
```
https://<user>.github.io/obs-youtube-player/?playlist=YOUR_PLAYLIST_ID&volume=75
```
- `playlist` is **required** (ID from the YouTube URL after `list=`).
- `volume` is optional (0–100, default 50).

## Notes
- No playlist ID is hardcoded in the code.
- Player remembers index + time per `playlist` on each machine via localStorage.
- HTTPS origin (Pages) avoids YouTube error 153.
