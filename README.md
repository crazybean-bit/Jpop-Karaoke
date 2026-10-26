# Kashi Karaoke

A J-pop karaoke and study web app. Each lyric line is split into word tiles with furigana above, romaji below, part-of-speech colored underlines, and the English translation underneath, all synced to your own audio or video file.

## Features

- Load an audio or video file from your device. Video plays above the lyrics.
- **Find lyrics** searches [LRCLIB](https://lrclib.net), a free synced-lyrics library, from your browser when you ask. It ranks matches by title, artist and your file's length, and lists the options when it isn't sure.
- Paste lyrics yourself, with or without `[mm:ss.xx]` timestamps, and set timing with **Tap to sync**.
- Tap any word to see its reading, word type and a Jisho link.
- Songs are saved in your browser's local storage.

No lyrics are bundled with the app. The built-in sample song uses original text written for the demo.

## How it works

Japanese text is split into words with [kuromoji.js](https://github.com/takuyaa/kuromoji.js) and its IPADIC dictionary (in `dict/`, Apache 2.0). The dictionary files carry a `.wasm` suffix so any static host serves them as binary.

## Hosting

It is a single static page. On GitHub Pages: Settings → Pages → Deploy from a branch → `main`, folder `/ (root)`.
