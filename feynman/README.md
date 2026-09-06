# 费曼学习法 · The Feynman Technique

Seven animated handwritten slides. Chinese is the default; the **English / 中文** button changes language in place. Share English with `?lang=en#topics` (or any slide hash). The selected slide, beat, running animation, auto-preview timer, theme, camera placeholder, and recording state survive a language change. Language is explicit in the URL; no browser-language detection or saved preference overrides the Chinese default.

From the repository root:

```sh
python3 -m http.server 8766
```

Open `http://localhost:8766/feynman/` or `http://localhost:8766/feynman/?lang=en#topics`. All assets use relative paths, including on GitHub Pages under `/open-learning-notes/`. Opening `index.html` directly also works. `straw.html` redirects to the straw slide while preserving the language query.

- Click the board, Right / N / Space / PageDown: next beat, then next slide.
- Left / P / PageUp: previous beat, then the previous slide’s final beat.
- R: replay the current beat. Beat dots select a beat.
- Auto preview: restart and preview the current slide; pause or navigate to stop.
- F: recording/fullscreen view. Escape: exit. The language control is hidden along with the other chrome during recording; use **L** to change language without leaving recording.
- Theme and camera-space buttons retain the original whiteboard/blackboard and webcam-space controls.

Order: `#cover`, `#taiji`, `#straw`, `#benefits`, `#limits`, `#outro`, `#topics`. The wish list has one beat per column, after the thanks slide.

## Assets and attribution

- `assets/xiaolai.ttf`: Xiaolai handwriting font, distributed with its [SIL Open Font License](assets/OFL-Xiaolai.txt). Both languages use it; English uses measured glyph advances.
- `assets/feynman-sketch-simple.png`: Richard Feynman portrait generated and simplified with OpenAI image generation for this deck. The original SVG alpha filter and dark-mode treatment are preserved.
- `assets/zaige-avatar.webp`: author avatar of @载哥硅谷笔记, from zzn.im.
- Deck text and illustrations follow the repository’s [CC BY 4.0 license](../LICENSE); the font retains its own license.

The integrated Chinese deck comes from the approved handoff snapshot (SHA-256 of its original `index.html`: `72cfb44b4a83c7efc3255c2c544e3db80741028eb1d3229323820af5665113a8`). Prototypes and unused assets are omitted. `i18n.js` holds equivalent English wording; slide geometry, Chinese wording, and lesson timing remain in `index.html`.
