# RSVP Speed Reader

A single-page, dependency-free RSVP (rapid serial visual presentation) reader: paste text and read it one word at a time, with each word's recognition point pinned to a fixed red anchor.

Everything runs client-side. Pasted text never leaves the page.

## Features

- Quick speed presets (250 easy → 900 sprint) right under Play, plus a fine 100–1000 wpm slider (5 wpm steps)
- Tap or click the word itself to play / pause
- End-of-read summary: your average wpm, words and time, with **Go faster** (next preset, restart) and **Read again**
- Optional **Ramp up** mode: starts at 250 wpm and climbs linearly to your chosen speed over the first half of the passage (at most 300 words)
- A short ~70-word demo loads by default; a longer demo is one tap away
- Smart pauses at punctuation (including inside closing quotes/brackets) and on long words
- Optional 3·2·1 countdown
- Unicode-aware anchor letter (grapheme-based, works for non-Latin scripts and emoji)
- Long tokens shrink to fit; anything too long (URLs) wraps instead of clipping
- Remaining-time estimate uses the same per-word delays as playback

## Keyboard

| Key | Action |
|---|---|
| Space / K | Play / pause |
| ← / → | Back / forward 10 words |
| ↑ / ↓ | Speed ±25 wpm |
| Home | Back to the beginning |

Shortcuts apply when focus is on the reader, its transport buttons, or nothing. Focused settings, presets and text fields keep their normal keys. The shortcuts card is hidden on small or touch-first screens; the shortcuts themselves still work.

## Hosting

It's a single static `index.html`. Serve the folder with any static host.
