# Intentional Pause

A tiny, original static webpage for redirecting distracting sites.

Flow:

1. One second of stillness
2. Two automatic breaths
3. “What is important right now?”
4. Type one intention and press Enter

There are no dependencies, accounts, analytics, cookies, builds, or backend.
Everything—including the original ambient soundscape—is generated inside `index.html`.

The page tries to begin the sound automatically. Most browsers block audible autoplay
until the visitor interacts with the page, so a small **tap for sound** control appears
when necessary. Once enabled, the sound follows the breathing rhythm and softens during
the reflection screen.

## Fastest publishing method: Netlify Drop

1. Unzip this folder.
2. Open Netlify Drop in your browser.
3. Drag the entire `intentional-pause` folder into the drop area.
4. Netlify gives you a public URL.
5. Paste that URL into your page blocker's redirect setting.

To update the page, edit `index.html` and drag the folder into Netlify again.

## GitHub Pages

1. Create a new public GitHub repository.
2. Upload `index.html` to the repository root.
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. GitHub will show the public site URL in the Pages settings.

## Easy customization

Near the bottom of `index.html`, find:

```js
const SETTINGS = {
  pauseBeforeStart: 1000,
  inhaleDuration: 4000,
  exhaleDuration: 6000,
  breaths: 2
};
```

Durations are in milliseconds. The prompt and closing text can be edited directly
in the HTML just above the script.
