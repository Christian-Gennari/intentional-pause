# Intentional Pause

A one-file static webpage for page-blocker redirects.

## Flow

1. One second of stillness
2. Two automatic breaths
3. “What is important right now?”
4. Type one intention and press Enter

## What changed in this version

- The visual cue is now a clear, elegant breathing circle that expands on inhale and contracts on exhale.
- The soundscape volume has been adjusted to be clearly audible and supportive while remaining soft.
- The typography uses a clean humanist sans-serif stack.
- The Web Audio soundscape features two layers:
  - a stereo binaural bed
  - a separate breath-synced swell for inhale/exhale movement

There are no dependencies, accounts, analytics, cookies, builds, or backend. Everything is generated inside `index.html`.

## Hosting

Fastest options:

- Netlify Drop: drag the folder in and get a URL immediately
- GitHub Pages: upload `index.html` to a repo and enable Pages from `main` / root

## Customize

Near the bottom of `index.html`:

```js
const SETTINGS = {
  pauseBeforeStart: 1000,
  inhaleDuration: 4000,
  exhaleDuration: 6000,
  breaths: 2
};
```

Durations are in milliseconds. You can also edit the reflection question, helper text, and closing sentence directly in the HTML.

## Sound

The ambient soundscape is generated in the browser with Web Audio. Some browsers block autoplay sound until the first interaction; when that happens, a small “tap for sound” control appears.
