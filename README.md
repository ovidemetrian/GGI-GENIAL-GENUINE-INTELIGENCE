# SYNTHIOSIS — GGI Control Panel

**Genial Genuine Intelligence — the steering wheel for AGI.**
Lumină, nu vrăjeală.

`v34-4` · single file · no build step · no dependencies · no server · installable.

**Live:** https://ovidemetrian.github.io/GGI-GENIAL-GENUINE-INTELIGENCE/

---

## What it is

The Control Panel is the working instrument of the GGI framework: **Meh → But →
Aha → Pám Pám**, gated, with no skipping from Meh to Pám Pám without paying the
toll in the middle.

Bundled in the same file: the Synthiosis Info shelf — Direction Not Drift, the
Palade Precedent, the Five Thresholds of AI Risk, and the Governance Seal.

> The Human provides Intent and Conscience.
> The Machine provides Compute and Scale.

## The canon rule

**The Ten Laws exist in exactly one place in this repository:** the
`📜 10 LAWS OF AI GOVERNANCE` modal, carrying both the Human-Facing and
Developer's Editions. Canonical published text lives at
[10lawsofai.com](https://10lawsofai.com).

Do not restate the Laws anywhere else in `index.html`. Reference the modal
instead. A framework whose Ninth Law is *Trust but Verify, Save to Verify*
cannot ship two versions of itself on one page.

*Why this rule exists: it happened.* A second, divergent Ten Laws lived in the
Synthiosis Info shelf and drifted — dropping Preservation of Record and Trust
but Verify entirely, the two laws the Governance Seal rests on. Removed
2026-08-01. The rule is here so the next edit doesn't reintroduce it.

## Installable, and offline

`manifest.json` and `sw.js` make this a real PWA. On Android Chrome, "Add to
Home screen" gives a standalone app with the GGI icon. On iOS, Share → Add to
Home Screen.

The service worker is network-first with a cache fallback: you always get the
latest version when online, and the panel still opens when you are not — because
without record there is no continuity (Law VIII).

## API keys

Keys are held in `sessionStorage` and die with the browser session. Non-secret
model configuration persists in `localStorage`. Any legacy plaintext key found
in `localStorage` from an older build is migrated to session storage and
deleted on load.

**Never reintroduce `localStorage.setItem` for an API key.** If a diff shows a
key being written to `localStorage`, that build is older than it looks.

## Files

```
index.html            the entire panel
manifest.json         PWA metadata
sw.js                 offline shell
icon-512.png          launcher + maskable icon
apple-touch-icon.png  iOS home screen icon
README.md             this file
LICENSE.txt           copyright terms
```

### Known repo hygiene items

- `manifest.json` references `icon-192.png`, which is **not in the repo**. Add
  it or drop the entry — a missing icon can fail the install prompt.
- `.nojekyll` is **not in the repo**. Add it if any path ever starts with an
  underscore.
- `GGI_Control_Panel_v30_VANGUARD_cognition_gauge_MEMORY_SPLIT_v7_speedometer.html`
  is a stale second panel sitting next to `index.html`. Two panel files in one
  repo is how the two-canon problem started. Archive or delete it.

## Deploy discipline

Before any push:

1. **Walk the fence line.** Read `index.html` end to end once, editing nothing.
   Surgical property-level edits are the right way to build this file and the
   reason nobody ever sees the whole document. Schedule the whole read as its
   own step or it never happens.
2. **Diff local against live** before assuming the deploy is behind or ahead:

   ```bash
   curl -sL https://raw.githubusercontent.com/ovidemetrian/GGI-GENIAL-GENUINE-INTELIGENCE/main/index.html -o live.html
   diff live.html index.html
   ```

   A fresh `pushed_at` timestamp on the repo does **not** mean `index.html`
   moved. It only means *something* moved. Verified the hard way, 2026-08-01.
3. **Bump the cache name** in `sw.js` (`ggi-panel-v34-3` → `ggi-panel-v34-4`)
   on every build, or installed copies keep serving the old shell.
4. **Bump the version string** in the Info shelf footer and the header comment
   in `index.html`. They have disagreed before (footer v34, header v30).
5. **Hard-refresh the live URL** and confirm: the Info shelf reads
   "One canon. One place.", and group titles render with their shadow.

## Changelog

### v34-4 — 2026-08-01
- Removed the duplicate, divergent Ten Laws from the Synthiosis Info shelf;
  replaced with a pointer to the single canon. Added the canon rule above.
- API keys moved to `sessionStorage`, with migration and deletion of legacy
  plaintext keys in `localStorage`.
- Fixed self-referential CSS custom property `--m3_group_title_color`, which
  had a stranded `text-shadow` declaration inside its value.
- Theme state now uses `classList.toggle` instead of overwriting
  `document.body.className`, which was silently dropping `lumina-theme`.
- Profile reset preserves API configuration instead of neutralizing it.
- Custom endpoints fall back to a generic OpenAI-compatible request shape
  instead of throwing for any provider without a built-in config.

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

Full terms in [LICENSE.txt](LICENSE.txt).

---

Built by **Ovidiu "Ovi" Demetrian** — Media Content Delivery LLC, Phoenix, AZ.
Framework submitted to NIST (2026-01-21) and CDAO / Tradewinds (2026-02-26).

- https://10lawsofai.com
- https://www.mediacontentdelivery.com
- https://www.smarthomesbyovi.com
- https://youtube.com/@mobiusbar
- https://ovidemetrian.github.io/mobiusbar/
