# Stage & Stem — Stage Recordings Player

A branded audio player for the Stage pages of the Stage & Stem website (Performance Space & Bistro, 199–201 Richmond Road, Cardiff). Plain HTML, CSS and JavaScript — no build step, no libraries.

## Features
- Turntable with a spinning record (33⅓ rpm) and a tonearm that tracks through the set
- Play / pause, previous / next, draggable progress bar
- Mute button and volume slider
- Left / right arrow keys skip between recordings; space plays / pauses
- Archive list of past sets with date, performer and duration

## Adding a recording
1. Export the set as an MP3 (192 kbps is plenty) and upload it to `audio/`.
2. Add one line to the `RECORDINGS` list near the bottom of `index.html`:

```js
{ src: "audio/2026-10-10-artist-name.mp3", performer: "Artist Name", set: "Set description", date: "2026-10-10", genre: "Jazz" },
```

Newest recordings first. Only add sets the performer has agreed to publish.

## Demo content
The three recordings in `audio/` are short test tones and the performers are examples. Replace them before going live.

## Deploying
Upload `index.html` and the `audio/` folder to the site (e.g. Fasthosts `public_html`), or embed the player markup into the existing Stage page.
