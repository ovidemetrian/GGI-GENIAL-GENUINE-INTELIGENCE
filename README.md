# GGI — Genial Genuine Intelligence

«“Machine got speed. Human got time.”»

«GGI is an independent research, governance, and engineering initiative created by Ovidiu “Ovi” Demetrian. It explores how human judgment, meaning, responsibility, and creativity can remain sovereign while working with increasingly capable artificial intelligence.»

This repository contains the working GGI Control Panel and serves as an entry point into the wider GGI ecosystem.

Introduction and quick overview
- This repo: the working GGI Control Panel — a single-file Progressive Web App (PWA) designed for offline use, with no build step and no external dependencies.
- Focus: human‑first governance and practical engineering supporting human–AI collaboration.
- Governance artifacts present in this repository: Canon Rule, Ten Laws of AI, Palade Precedent, and the Five Thresholds of AI Risk.
- Technical features present in the Control Panel: API-key handling and governance metadata surfaced in the UI.

The GGI Ecosystem
«GGI is part of an interconnected body of work exploring human cognition, artificial intelligence, governance, language, engineering, narrative, and practical technology.»

Core Ideas and Governance
- GGI — Genial Genuine Intelligence  
  The human-centered intelligence and governance framework represented by this repository.  
  [GGI — Genial Genuine Intelligence](https://ovidemetrian.github.io/GGI-GENIAL-GENUINE-INTELLIGENCE/)

- Ten Laws of AI  
  The canonical governance principles supporting GGI and responsible human–AI collaboration.  
  [Ten Laws of AI](https://10lawsofai.com)

- Möbius Bar  
  The narrative and philosophical environment where GGI, Synthiosis, Neogrammar, human cognition, humor, paradox, and AI behavior are explored.  
  [Möbius Bar](https://ovidemetrian.github.io/mobiusbar/)

Engineering and Professional Practice
- Media Content Delivery  
  Professional work in audio, video, networking, smart environments, automation, and integrated media systems.  
  [Media Content Delivery](https://www.mediacontentdelivery.com/)

- Smart Homes by Ovi  
  Practical smart-home technology, automation, networking, audio, security, and intelligent-environment integration.  
  [Smart Homes by Ovi](https://smarthomesbyovi.com/)

Additional Projects
- NoEscape  
  An experimental project examining interfaces, digital persuasion, navigation, attention, and human awareness.  
  [NoEscape (Netscape)](https://ovidemetrian.github.io/Netscape/)

- My Future Past  
  An interactive multimedia résumé and professional story connecting music, engineering, smart environments, AI, and personal experience.  
  [My Future Past](https://ovidemetrian.github.io/my-future-past/)

Neogrammar
Neogrammar is an evolving language and conceptual framework for human–AI communication. It supplies terms and conceptual structures for ideas conventional vocabulary does not capture. Representative Neogrammar terms used across the work include:
- Future Past
- Vrăjală
- Meh → But → Aha → Pam‑Pam
- Nose on the Glass
- Loopdrift

Conceptual architecture
- GGI is the framework.
- Synthiosis is the human↔machine relationship and practice.
- Neogrammar is the language.
- The Ten Laws of AI are the governance.
- Möbius Bar is the narrative environment.
- Media Content Delivery and Smart Homes by Ovi provide the practical engineering foundation.
- NoEscape and My Future Past are applied and creative expressions of the work.

Identity diagram
```text
GGI
        Genial Genuine Intelligence
                    │
      ┌─────────────┼─────────────┐
      │             │             │
 Synthiosis    Neogrammar   Ten Laws
      │             │             │
      └─────────────┼─────────────┘
                    │
              Möbius Bar
                    │
      ┌─────────────┼─────────────┐
      │                           │
 Media Content            Smart Homes
   Delivery                  by Ovi
                    │
              Real Applications
```

What exists now (transparency)
- Files and artifacts observed in this repository:
  - `index.html` — the primary single-file PWA interface (SYNTHIOSIS / GGI Control Panel).
  - `GGI_Control_Panel_v30_VANGUARD_cognition_gauge_MEMORY_SPLIT_v7_speedometer.html` — single-file Control Panel variant.
  - `manifest.json` and `sw.js` — PWA manifest and service worker for offline capability.
  - `icon-512.png`, `apple-touch-icon.png` — icons used by the PWA.
  - `README.md` (this file) and `LICENSE.txt`.
- Confirmed technical properties (present in repository files):
  - Single-file PWA UI(s) provided as HTML files.
  - PWA manifest and service worker implementing offline caching behavior.
  - No explicit build toolchain visible in repository root.
  - Governance artifacts surfaced in the UI: Ten Laws (embedded), Canon Rule and Palade Precedent are referenced in the control panel text and UI.
  - API‑endpoint support and UI controls exist for configuring custom AI endpoints (OpenAI‑compatible support is shown in the UI text).
  - Storage patterns: the UI code shows usage of `localStorage` for profile persistence; the repository’s README also references `sessionStorage` for keys (see verification notes below).
- Experimental material observed inline in the Control Panel UI (embedded narratives, Möbius Bar references, Neogrammar terms).

Planned documentation (not created here)
- The following documentation files are listed here only as planned unless they already exist in the repository:
  - `docs/PHILOSOPHY.md`
  - `docs/NEOGRAMMAR.md`
  - `docs/SYNTHIOSIS.md`
  - `docs/GOVERNANCE.md`
  - `docs/TEN-LAWS.md`

How to use the Control Panel (brief)
- Open the repository’s GitHub Pages link or open `index.html` (or the single-file Control Panel HTML) in a modern browser.
- No build step required; the PWA is installable and provides offline behavior via the included `sw.js`.
- API keys and endpoint configuration are entered via the Control Panel UI.

Contributing and governance
- The project’s governance artifacts (Ten Laws, Canon Rule, Palade Precedent, Five Thresholds) are primary touchstones for design and contributions.
- See `LICENSE.txt` for licensing and reuse terms.

Connect
- GitHub: [ovidemetrian](https://github.com/ovidemetrian)
- Möbius Bar on YouTube: [@mobiusbar](https://youtube.com/@mobiusbar)

License
See `LICENSE.txt` in the repository root.

Short closing
GGI is a platform of interrelated projects spanning governance, language, narrative, and engineering grounded in practical professional experience. This repository hosts the working Control Panel — the operational lobby for the platform. Explore the Control Panel UI and the governance artifacts embedded within it.
