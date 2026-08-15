# Design

## Theme

Light-first academic page; dark theme provided via the site's built-in toggle.
Paper-like calm surface, ink-like text, one committed accent: International Klein Blue.
Neutral chrome; the accent carries identity.

## Color

Strategy: **Restrained** — blue-tinted neutrals + Klein blue accent.
All values OKLCH; neutrals tinted toward hue 264 (chroma 0.004–0.018).

### Light

| Role | OKLCH | Hex fallback | Notes |
|---|---|---|---|
| Background | `oklch(0.988 0.004 264)` | #FAFBFE | paper, faint blue tint |
| Text | `oklch(0.335 0.016 264)` | #32373F | 11.6:1 |
| Text light | `oklch(0.52 0.014 264)` | — | captions, meta |
| Border | `oklch(0.922 0.007 264)` | — | |
| Thead / footer bg | `oklch(0.952 0.007 264)` / `oklch(0.958 0.006 264)` | — | |
| Link (accent) | `oklch(0.452 0.208 264)` | #1444C7 | lifted IKB, 7.6:1 |
| Link hover | `oklch(0.36 0.15 264)` | #11338A | darker, 10.9:1 |
| Link visited | `oklch(0.452 0.09 264)` | #3C5488 | desaturated |
| Base (buttons, nav accent, selection) | `oklch(0.379 0.195 263.2)` | #002FA7 | pure IKB |

### Dark

| Role | OKLCH | Notes |
|---|---|---|
| Background | `oklch(0.205 0.018 264)` | #131720 |
| Text | `oklch(0.90 0.008 264)` | 13.3:1 |
| Border | `oklch(0.30 0.018 264)` | |
| Link | `oklch(0.70 0.15 262)` | #6A9CFB, 6.6:1 |
| Link hover | `oklch(0.78 0.13 262)` | |
| Link visited | `oklch(0.62 0.10 262)` | |

Selection: IKB background, near-white blue-tinted text (both themes).

## Typography

Inherits the template stack: sans-serif body with narrow sans headers.
Hierarchy via scale + weight contrast; body line length kept ≤ 75ch by the grid.

## Layout

12-column Susy grid; author sidebar 3 cols (capped 320px), content 9 cols.
Compact rhythm: heading top margin 1.4em, paragraph bottom 1.3em, page right suffix 1 col.

## Components

- Sidebar author card: avatar, name, bio, icon link list (Font Awesome / Academicons / inline SVG for TED)
- Link colors are the main interactive surface; underline on hover
- Buttons and nav accents take the pure IKB base color
