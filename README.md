# Pixel Chapel

A tiny interactive pixel-art chapel built as a single-page HTML experience.

Pixel Chapel lets you light candles, decorate the altar, keep a local prayer journal, switch ambience modes, and take polaroid-style snapshots of the scene.

## Files

- `index.html` - the full app, including styles, markup, pixel art, interactions, and audio.
- `jesus-icon.jpg` - the pixel icon image used in the altar scene.

## How To Run

Open `index.html` in a browser.

The app is mostly self-contained, but it uses a few online resources:

- Google Fonts for the pixel font.
- `html2canvas` from CDN for the snapshot feature.
- YouTube embed playback for the alternate audio track.

For the best experience, use a browser with internet access and click the entry screen once to unlock audio.

## Controls

- `LIGHT` - lights candles one by one.
- `SNUFF` - removes the most recently lit candle.
- `FLOWERS` - toggles flower decorations.
- `CROSS` - toggles the altar cross.
- `ICON` - toggles the small saint icon.
- `GARLAND` - toggles garland and stars.
- `NIGHT` - toggles night lighting.
- `JOURNAL` - opens the prayer journal.
- `AUDIO` - cycles through chapel ambience, YouTube track, and off.
- `SNAP` - captures the chapel as a polaroid-style image with a camera snap sound.

## Prayer Journal

Prayer entries are saved locally in the browser using `localStorage`.

This means:

- Prayers stay after refreshing the page.
- Prayers are stored only in that browser on that device.
- `CLEAR ALL` removes the saved Pixel Chapel prayers from local storage.

## Audio Modes

The audio button cycles through:

- `AUDIO: CHAPEL` - synthesized choir, bells, candle sounds, holy-water chimes, and camera snap.
- `AUDIO: TRACK` - the embedded YouTube track, plus camera snap.
- `AUDIO: OFF` - mutes app sounds.

## Snapshot Notes

Snapshots use `html2canvas`, so the CDN script must load for `SNAP` to work. After taking a snapshot, use `SAVE` on the polaroid overlay to download the image.
