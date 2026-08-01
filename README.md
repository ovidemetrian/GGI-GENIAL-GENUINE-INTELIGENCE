# SYNTHIOSIS — GGI Control Panel

**Genial Genuine Intelligence — the steering wheel for AGI.**
Lumină, nu vrăjeală.

`v34-3` · single file · no build step · no dependencies · no server · installable.

**Live:** https://ovidemetrian.github.io/GGI-GENIAL-GENUINE-INTELIGENCE/

---

## What it is

The Control Panel is the working instrument of the GGI framework: **Meh → But →
Aha → Pám Pám**, gated, with no skipping from Meh to Pám Pám without paying the
toll in the middle.

Bundled in the same file: the Synthiosis Info shelf — Direction Not Drift, the
Palade Precedent, the Five Thresholds of AI Risk, the Governance Seal, and the
Ten Laws of A.I.

> The Human provides Intent and Conscience.
> The Machine provides Compute and Scale.

## Installable, and offline

`manifest.json` and `sw.js` make this a real PWA. On Android Chrome, "Add to
Home screen" gives a standalone app with the GGI icon. On iOS, Share → Add to
Home Screen.

The service worker is network-first with a cache fallback: you always get the
latest version when online, and the panel still opens when you are not — because
without record there is no continuity (Law VIII).

## Files

```
index.html            the entire panel
manifest.json         PWA metadata
sw.js                 offline shell
icon-192.png          launcher icon
icon-512.png          launcher + maskable icon
apple-touch-icon.png  iOS home screen icon
.nojekyll             tells GitHub Pages to serve files as-is
README.md             this file
LICENSE               copyright terms
```

## Publishing to GitHub Pages

```bash
git init
git add .
git commit -m "SYNTHIOSIS GGI Control Panel v34-3"
git branch -M main
git remote add origin https://github.com/ovidemetrian/REPO-NAME.git
git push -u origin main
```

Then **Settings → Pages → Deploy from a branch → main / (root) → Save.**

Live in about a minute. Replace `REPO-NAME` in the live link above once it
resolves.

### After every update

Bump the cache name in `sw.js` (`ggi-panel-v34-3` → `ggi-panel-v34-4`) whenever
you push a new build. Otherwise installed copies may serve the old shell.

## License

**Proprietary. All rights reserved.** © 2026 Ovidiu Demetrian / Media Content
Delivery LLC.

Read it, study it, run it, link to it, quote it with credit. Do not copy,
mirror, modify, rebrand, or commercialize it without written permission —
which is available, so ask.

**This work may not be used to train, fine-tune, evaluate, or benchmark any
machine learning model.** Text and data mining rights are expressly reserved
under Article 4(3) of EU Directive 2019/790 and all other applicable law.
Being publicly reachable is not a license.

> Human input, creativity, and wisdom remain human property. The time humans
> invest is sacred; it must not be harvested as free labor for corporate gain.
> — The Tenth Law

Full terms in [LICENSE](LICENSE).

---

Built by **Ovidiu "Ovi" Demetrian** — Media Content Delivery LLC, Phoenix, AZ.
Framework submitted to NIST (2026-01-21) and CDAO / Tradewinds (2026-02-26).

- https://10lawsofai.com
- https://www.mediacontentdelivery.com
- https://www.smarthomesbyovi.com
- https://youtube.com/@mobiusbar
