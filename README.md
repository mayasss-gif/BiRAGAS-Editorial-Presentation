# BiRAGAS Editorial Presentation · 32 Slides

A click-through HTML presentation of the BiRAGAS Causal Atlas content (25 modules · 8 causal engines · 3 stacked tiers) rendered in the **Editorial Issue 01** aesthetic: cream newsprint, hot red ink, Fraunces variable italic serif, Newsreader body, DM Mono marginalia.

## Files

| | |
|---|---|
| `index.html` | Self-contained 32-slide deck — open in any browser |
| `audio/` | 31 per-slide MP3 narrations (Ava Multilingual Neural via edge-tts) |

## Slide order

| # | Slide | Audio |
|---|---|---|
| 1 | Cover — `BiRAGAS.` | *(silent)* |
| 2 | Platform overview · 25 / 08 / 03 | `a01_open.mp3` |
| 3 | Chapter 01 banner · Causal Stack | `a02_t1_intro.mp3` |
| 4–11 | T1·01–08 module spreads | `t1_m1.mp3` … `t1_m8.mp3` |
| 12 | Chapter 02 banner · Core Analysis | `a04_t2_intro.mp3` |
| 13–22 | T2·01–10 module spreads | `t2_m1.mp3` … `t2_m10.mp3` |
| 23 | Chapter 03 banner · Data & Processing | `a06_t3_intro.mp3` |
| 24–30 | T3·01–07 module spreads | `t3_m1.mp3` … `t3_m7.mp3` |
| 31 | End-to-end pipeline fold | `a08_pipeline.mp3` |
| 32 | Editors' Note · manifesto | `a09_close.mp3` |

## Navigation

| Action | Key / button |
|---|---|
| Next slide | `→` · `SPACE` · `PgDn` · `→` button |
| Previous slide | `←` · `PgUp` · `←` button |
| Jump to start / end | `Home` / `End` |
| Jump to any slide | Click a pip in the bottom scrubber |
| Toggle audio | `A` key · `AUDIO · OFF/ON` button (top-right) |
| Toggle auto-advance | `AUTO · OFF/ON` button — when on, the deck auto-advances when each narration finishes |
| Fullscreen | `F` key · `⛶ FULLSCREEN` button |
| Replay current narration | Click any title, numeral, or headline on the slide |

## Audio behavior

- **Default OFF** to respect browser autoplay policies. Click `AUDIO · OFF` to enable; from that point each slide change auto-plays its narration.
- **Now-playing chip** appears bottom-left with animated EQ bars and the slide label while audio plays.
- **Auto-advance**: pair with audio ON to run hands-free — narration plays, then deck auto-jumps to next slide.

## Editorial aesthetic decisions

| | |
|---|---|
| **Paper** | `#F4EFE7` cream newsprint with SVG fractal-noise grain (multiply blend, 42% opacity) |
| **Ink** | `#0F0F0F` |
| **Tier accents** | T1 red `#E63946` · T2 ink `#0F0F0F` · T3 cobalt `#1E40AF` (mustard `#D4A017` available for callouts) |
| **Display type** | [Fraunces](https://fonts.google.com/specimen/Fraunces) variable — `opsz` 144, `wght` 380–760, `SOFT` 100, `WONK` 1 (italic) |
| **Body** | [Newsreader](https://fonts.google.com/specimen/Newsreader) |
| **Marginalia / pills / folios** | [DM Mono](https://fonts.google.com/specimen/DM+Mono) |
| **Module spread** | Giant italic Fraunces serial numeral (~450pt) on one side with rotated tier-color splash blocks behind; italic name + accent-rule deck + numbered ① ② ASSAY/METHOD bullets + ❡ italic action line on the other. Left/right alternates by even/odd index. |
| **Tier banners** | Chapter dividers with massive italic headline + splash + ghost mark (I / II / III) at 13% opacity |
| **Pipeline & close** | Full-bleed ink panel for dramatic contrast against the cream paper |
| **Manifesto** | "We're not building ~~another AI~~ that finds *associations.*" / "We're building **the infrastructure** that finally tells biology's *actual story.*●" |

## Preview

```bash
open "/Users/mohamadammarayass/Desktop/Ayass _ Strategic Planning/Videos/Commercials/05.17.2026/Presentation/index.html"
```

Or serve locally so the audio files load with proper MIME types in some browsers:

```bash
cd "/Users/mohamadammarayass/Desktop/Ayass _ Strategic Planning/Videos/Commercials/05.17.2026/Presentation"
python3 -m http.server 8000
# → http://localhost:8000/
```

## Live URL

**https://mayasss-gif.github.io/BiRAGAS-Editorial-Presentation/**

## Deployment commands used (for reference)

```bash
cd "/Users/mohamadammarayass/Desktop/Ayass _ Strategic Planning/Videos/Commercials/05.17.2026/Presentation"
git init && git add . && git commit -m "Initial: BiRAGAS Editorial Presentation"
gh repo create mayasss-gif/BiRAGAS-Editorial-Presentation --public --source=. --push
gh api repos/mayasss-gif/BiRAGAS-Editorial-Presentation/pages --method POST \
  -f source[branch]=main -f source[path]=/
```

Suggested URL: `https://mayasss-gif.github.io/BiRAGAS-Editorial-Presentation/`

## Source materials

- **Content**: `BiRAGAS-Causal-Atlas-III` (25 modules, 8 causal engines, 3 tiers + Causion agent)
- **Aesthetic**: `BiRAGAS-Editorial-Issue-01` (cream / Fraunces / hot red)
- **Audio**: 31 MP3s (Ava Multilingual Neural, edge-tts) from `../audio_3min/`
