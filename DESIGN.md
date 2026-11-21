---
name: Dr. Kiruthika's Skintillate Skin Clinic
description: A soft blush, rose and sage clinic site with serif headlines, pill buttons and arch-framed photography.
colors:
  logo-rose: "#A5354B"
  logo-rose-deep: "#852638"
  logo-rose-soft: "#D6687C"
  logo-leaf: "#5D6A3C"
  leaf-tint: "#EDEFE1"
  blush-paper: "#FDF5F3"
  blush-tint: "#F7E6E3"
  hairline-rose: "#EBD8D4"
  surface-white: "#FFFFFF"
  charcoal-ink: "#3A3131"
  muted-ink: "#6A5C5B"
  reception-maroon: "#5C1F29"
  on-maroon: "#F8ECE9"
  maroon-heading: "#E9B9C1"
typography:
  display:
    fontFamily: "Cormorant Garamond, Times New Roman, serif"
    fontSize: "clamp(2.3rem, 5.2vw, 3.7rem)"
    fontWeight: 600
    lineHeight: 1.12
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cormorant Garamond, Times New Roman, serif"
    fontSize: "clamp(1.85rem, 3.6vw, 2.6rem)"
    fontWeight: 600
    lineHeight: 1.12
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cormorant Garamond, Times New Roman, serif"
    fontSize: "1.45rem"
    fontWeight: 600
    lineHeight: 1.12
  body:
    fontFamily: "Jost, Segoe UI, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "Jost, Segoe UI, system-ui, sans-serif"
    fontSize: "0.8rem"
    fontWeight: 500
    letterSpacing: "0.16em"
rounded:
  sm: "10px"
  md: "18px"
  pill: "999px"
spacing:
  sm: "12px"
  md: "18px"
  lg: "24px"
  container-gutter: "20px"
components:
  button-primary:
    backgroundColor: "{colors.logo-rose}"
    textColor: "{colors.surface-white}"
    rounded: "{rounded.pill}"
    padding: "0.7em 1.4em"
    height: "48px"
  button-primary-hover:
    backgroundColor: "{colors.logo-rose-deep}"
    textColor: "{colors.surface-white}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.logo-rose}"
    rounded: "{rounded.pill}"
    padding: "0.7em 1.4em"
    height: "48px"
  button-outline-hover:
    backgroundColor: "{colors.logo-rose}"
    textColor: "{colors.surface-white}"
  card:
    backgroundColor: "{colors.surface-white}"
    textColor: "{colors.charcoal-ink}"
    rounded: "{rounded.md}"
    padding: "24px"
  info-card:
    backgroundColor: "{colors.surface-white}"
    textColor: "{colors.charcoal-ink}"
    rounded: "{rounded.md}"
    padding: "24px"
  footer:
    backgroundColor: "{colors.reception-maroon}"
    textColor: "{colors.on-maroon}"
---

# Design System: Dr. Kiruthika's Skintillate Skin Clinic

## Overview

**Creative North Star: "The Blush Parlour"**

The site feels like a soft, well-kept parlour: blush paper, a single deep rose for everything you can act on, small sage leaves for quiet supporting marks, and a maroon footer borrowed from the clinic's reception desk. The palette is taken from the logo, whose JPEG background is the page colour so the mark sits on the page with no box around it. Headlines are a high-contrast serif; everything else is a clean geometric sans.

It is calm and uncluttered. Sections breathe (56–96px vertical padding), text is capped near 70 characters, and imagery is held in arch silhouettes (a full semicircle on top, soft corners below) that echo the doorway-and-leaf character of the logo. Nothing shouts: no superlatives, no hard sell, no dark mode, no gradients.

**Key Characteristics:**
- Blush-paper ground with white cards and hairline rose borders.
- One action colour (logo rose); sage appears only as small icons and eyebrows.
- Serif display type over a light sans body.
- Arch-framed photography, pill buttons, 18px cards.
- Flat at rest; a faint maroon-tinted shadow only on hover and on floating surfaces.
- Tap-first on mobile: a fixed Call / WhatsApp bar under 760px.

## Colors

A warm, low-saturation palette: blush neutrals, one rose accent, one sage support, one maroon anchor.

### Primary
- **Logo Rose** (#A5354B): links, primary buttons, active nav, FAQ toggles and the mobile call bar. About 6:1 against blush paper, so it carries text as well as fills.
- **Logo Rose Deep** (#852638): hover state for links and primary buttons.
- **Logo Rose Soft** (#D6687C): decoration only (card hover border, list markers, doctor-card hover). Never for text.

### Secondary
- **Logo Leaf** (#5D6A3C): eyebrow labels, check marks and small icons. It marks "information", never "action".
- **Leaf Tint** (#EDEFE1): reserved for soft sage backgrounds.

### Neutral
- **Blush Paper** (#FDF5F3): page background and the header glass (92% opacity).
- **Blush Tint** (#F7E6E3): image placeholders, table headers, CTA band background.
- **Hairline Rose** (#EBD8D4): every border and divider.
- **Surface White** (#FFFFFF): cards, alternate sections, mobile bar.
- **Charcoal Ink** (#3A3131): body text and headings.
- **Muted Ink** (#6A5C5B): secondary text, captions, lead paragraphs.
- **Reception Maroon** (#5C1F29): footer background only, with **On Maroon** (#F8ECE9) text and **Maroon Heading** (#E9B9C1) for footer labels and icons.

### Named Rules
**The One Action Colour Rule.** If something is tappable and meaningful, it is Logo Rose. Sage and maroon never signal action.

**The Paper Rule.** Backgrounds are blush paper, white or blush tint. Pure grey and cool neutrals do not appear.

## Typography

**Display Font:** Cormorant Garamond (with Times New Roman, serif), weights 500–600, self-hosted variable WOFF2.
**Body Font:** Jost (with Segoe UI, system-ui, sans-serif), weights 400–500, self-hosted variable WOFF2.

**Character:** A refined, slightly literary serif for headings against a light, open geometric sans for reading. The serif carries warmth; the sans keeps medical information plain.

### Hierarchy
- **Display** (600, clamp 2.3–3.7rem, 1.12): page H1 and hero. Balanced wrapping, capped to 24ch on inner pages.
- **Headline** (600, clamp 1.85–2.6rem, 1.12): section H2.
- **Title** (600, 1.45rem, 1.12): card titles, H3, footer name (1.6rem).
- **Body** (400, 1.0625rem, 1.7): all running text; prose capped at 70ch, lead at 62ch.
- **Label** (500, 0.8rem, 0.16em tracking, uppercase): eyebrows (sage) and footer headings (maroon heading).

### Named Rules
**The Serif-For-Voice Rule.** Cormorant is used for headings, the brand name and the signature line. Never for UI labels, buttons or body text.

**The Self-Hosted Rule.** Fonts load from `/assets/fonts` as latin-subset WOFF2 with `font-display: swap`. No third-party font requests. Tamil will need its own self-hosted face.

## Layout

A single centred container (max 1160px, 20px gutters) with `narrow` at 760px for text pages. Sections use fluid vertical padding `clamp(56px, 8vw, 96px)`, and alternate sections switch to white with hairline top and bottom borders. Two-column compositions (hero 1.05fr/.95fr, split 0.8fr/1.2fr, service page content + 320px sticky aside) collapse to one column at 860–960px. Card grids use `auto-fill, minmax(260px, 1fr)` with 18px gaps. A sticky 72px header holds the logo lockup and nav, which becomes a drop-down panel at 900px and below. At 760px and below a fixed two-button bar (Call, WhatsApp) sits at the bottom and the body gains 64px bottom padding.

## Elevation & Depth

Flat by default, with hairline borders doing most of the separating. Shadows are a single maroon-tinted vocabulary and appear on hover or on surfaces that float.

### Shadow Vocabulary
- **Soft Lift** (`0 1px 2px rgba(92,31,41,.05), 0 8px 24px rgba(92,31,41,.07)`): card hover, arch photos, hero badge.
- **Menu Drop** (`0 12px 24px rgba(92,31,41,.08)`): mobile nav panel.
- **Bar Rise** (`0 -6px 20px rgba(92,31,41,.08)`): mobile call bar.

The header uses a 10px backdrop blur on 92% blush paper plus a hairline border.

### Named Rules
**The Flat-At-Rest Rule.** Cards have no shadow until hovered. Shadows are always tinted maroon, never neutral black.

## Shapes

Soft and rounded, nothing sharp. Buttons are full pills (999px); cards and info blocks use 18px; small tiles, credentials and the skip link use 10px. Photographs are arches (a full semicircle top, 18px bottom corners) at 4:5. Doctor thumbnails are circles. Borders are 1px hairline rose, buttons 1.5px.

## Components

### Buttons
- **Shape:** full pill (999px), min-height 48px (40px small).
- **Primary:** Logo Rose fill, white Jost 500 text, 0.7em × 1.4em padding.
- **Outline:** transparent with a Logo Rose 1.5px border and text; fills with rose on hover.
- **Hover / Focus:** fill moves to Logo Rose Deep over 150ms; focus is a 2px Logo Rose outline offset 3px.

### Cards / Containers
- **Corner Style:** 18px.
- **Background:** white (blush paper when placed inside a white alternate section).
- **Border:** 1px Hairline Rose; hover shifts to Logo Rose Soft with Soft Lift and a 2px rise.
- **Internal Padding:** 24px; whole card is clickable via a stretched title link.

### Navigation
Charcoal 500-weight links with a 1.5px underline in Logo Rose for hover and the current page. Language switch sits in the same row. Below 900px a 44px bordered toggle opens a full-width panel with divider-separated rows.

### FAQ
Native details/summary with hairline dividers and a rose "+" that becomes "–" when open; answers in Muted Ink.

### Hero Badge
A white 18px card with Soft Lift, overlapping the lower-left of the hero arch, showing a circular doctor photo, name and line.

### Mobile Call Bar
Two equal 56px targets: a Logo Rose filled Call and a white WhatsApp with rose text. Respects the iOS safe area.

### Footer
Reception Maroon ground, four-column grid collapsing to two then one. Links are On Maroon with a faint underline; labels are small tracked caps in Maroon Heading.

## Do's and Don'ts

### Do:
- **Do** use Logo Rose (#A5354B) for every link, primary action and active state.
- **Do** frame portrait and clinic photos in the arch shape at 4:5.
- **Do** keep text on blush paper at Charcoal Ink or Muted Ink; Logo Rose for text is allowed on blush paper and white.
- **Do** keep hit targets at 48px or larger, with a 40px minimum for small buttons.
- **Do** respect reduced motion: transitions are disabled under `prefers-reduced-motion`.
- **Do** tint every shadow with maroon (92,31,41).

### Don't:
- **Don't** use Logo Rose Soft (#D6687C) for text; it is decorative only.
- **Don't** use sage for anything tappable.
- **Don't** introduce gradients, gradient text, glows or a dark theme.
- **Don't** load web fonts from third-party hosts.
- **Don't** add visual claims the copy rules forbid: no price badges, award or "best" ribbons, star ratings, testimonial cards or before-and-after pairs.
