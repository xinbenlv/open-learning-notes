# System maps

Interactive architecture maps for the For You lecture, rendered with [archify](https://github.com/tt-a1i/archify) (MIT) from the typed JSON specs in `src/`. Each map is a self-contained HTML file with light/dark themes, guided views, search, and PNG/SVG export.

| Map | English | 中文 | Spec |
|---|---|---|---|
| A · Classic recommendation cascade (data flow) | [classic-recsys.en.html](classic-recsys.en.html) | [classic-recsys.zh.html](classic-recsys.zh.html) | `src/classic-recsys*.dataflow.json` |
| B · 𝕏 For You service architecture (nodes link to source at commit `45b48ba`) | [x-for-you.en.html](x-for-you.en.html) | [x-for-you.zh.html](x-for-you.zh.html) | `src/x-for-you*.architecture.json` |

Regenerate (needs Node ≥ 18 and a clone of archify):

```bash
node <archify>/bin/archify.mjs deliver dataflow src/classic-recsys.dataflow.json classic-recsys.en.html --quality showcase
node <archify>/bin/archify.mjs deliver architecture src/x-for-you.architecture.json x-for-you.en.html --quality showcase --repo-root <x-algorithm clone at 45b48ba>
```
