---
name: Ira Volunteer Fire Department
description: A printed-bulletin civic site for residents of a small Vermont town.
colors:
  almanac-cream: "#F5F1E8"
  mill-paper: "#EDE7D8"
  bulletin-ink: "#1C1C1A"
  slate-ink: "#3A3933"
  birch-gray: "#6B6A62"
  newsprint-rule: "#D9D2BF"
  heavy-rule: "#C3BCA7"
  vermont-pine: "#2D3E2C"
  deep-pine: "#1E2B1D"
  maple-bark: "#6B4423"
  dark-bark: "#54351A"
  ember-brick: "#B33A2A"
  banked-ember: "#8E2C1F"
  hollow-moss: "#5B6B3A"
  lantern-amber: "#C98A2B"
  pasture-green: "#3E6B3E"
  caution-ochre: "#C9762E"
typography:
  display:
    fontFamily: "'Public Sans', system-ui, sans-serif"
    fontSize: "64px"
    fontWeight: 800
    lineHeight: 1.02
    letterSpacing: "-0.025em"
  headline:
    fontFamily: "'Public Sans', system-ui, sans-serif"
    fontSize: "38px"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.015em"
  title:
    fontFamily: "'Public Sans', system-ui, sans-serif"
    fontSize: "22px"
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: "-0.005em"
  body:
    fontFamily: "'Public Sans', system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: "normal"
  label:
    fontFamily: "'Public Sans', system-ui, sans-serif"
    fontSize: "12.5px"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: "0.06em"
  eyebrow:
    fontFamily: "'Public Sans', system-ui, sans-serif"
    fontSize: "11px"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: "0.18em"
  italic-accent:
    fontFamily: "'Source Serif 4', Georgia, serif"
    fontSize: "inherit"
    fontWeight: 500
    lineHeight: "inherit"
    letterSpacing: "-0.01em"
rounded:
  none: "0px"
  sm: "4px"
  pill: "999px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "32px"
  xl: "56px"
  xxl: "72px"
  section: "96px"
components:
  button-primary:
    backgroundColor: "{colors.vermont-pine}"
    textColor: "{colors.mill-paper}"
    rounded: "{rounded.sm}"
    padding: "12px 20px"
  button-primary-hover:
    backgroundColor: "{colors.deep-pine}"
    textColor: "{colors.almanac-cream}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.bulletin-ink}"
    rounded: "{rounded.sm}"
    padding: "12px 20px"
  button-ghost-hover:
    backgroundColor: "{colors.mill-paper}"
    textColor: "{colors.bulletin-ink}"
  button-ember:
    backgroundColor: "{colors.ember-brick}"
    textColor: "{colors.almanac-cream}"
    rounded: "{rounded.sm}"
    padding: "12px 20px"
  chip-tag:
    backgroundColor: "transparent"
    textColor: "{colors.birch-gray}"
    rounded: "{rounded.pill}"
    padding: "6px 12px"
  chip-tag-ember:
    backgroundColor: "transparent"
    textColor: "{colors.ember-brick}"
    rounded: "{rounded.pill}"
    padding: "6px 12px"
  chip-tag-forest:
    backgroundColor: "transparent"
    textColor: "{colors.vermont-pine}"
    rounded: "{rounded.pill}"
    padding: "6px 12px"
  card-paper:
    backgroundColor: "{colors.almanac-cream}"
    textColor: "{colors.bulletin-ink}"
    rounded: "{rounded.none}"
    padding: "36px"
  alert-warn:
    backgroundColor: "#FBF3E2"
    textColor: "{colors.bulletin-ink}"
    rounded: "{rounded.none}"
    padding: "14px 20px"
  cta-card-ember:
    backgroundColor: "{colors.ember-brick}"
    textColor: "{colors.almanac-cream}"
    rounded: "{rounded.none}"
    padding: "48px 44px"
---

# Design System: Ira Volunteer Fire Department

## 1. Overview

**Creative North Star: "The Town Bulletin"**

The site reads like a printed civic notice posted outside the Ira town hall: dated, plain-spoken, and unmistakably *of this place*. The page is a public document first, a website second. Rules of authority come from the Vermont Division of Forestry and the Fire Warden, not from marketing. Editorial italic accents (Source Serif 4) do all of the warm, human work; everything else is set in a single utilitarian sans (Public Sans) with hairline rules carving the page into civic columns.

The system explicitly refuses the four reflex aesthetics named in PRODUCT.md: SaaS landing-page templating, slick corporate firefighter branding, dark-mode tech, and clipart-civic web. It does not perform "fire department." It performs the quiet, accurate authority of a department that has been answering calls since 1879 and intends to keep doing so. Trust comes from specificity: today's fire weather index, the Warden's actual phone number, the address of the station, the count of active volunteers (fourteen).

**Key Characteristics:**

- Earth-tone palette anchored on Almanac Cream paper and Bulletin Ink type, accented by Vermont Pine and Ember Brick.
- One sans family doing the structural work; one serif italic doing the editorial work. No third typeface.
- Hairline rules (1px Newsprint Rule) instead of cards, dividers, or container shadows. The page is a printed sheet, not a stack of floating panels.
- Sharp corners by default. Pill-shaped tags only. No rounded cards, no soft cards, no glass.
- Flat. Zero shadow vocabulary. Depth is conveyed by tonal shifts in paper (Almanac Cream → Mill Paper → Vermont Pine → Bulletin Ink).

## 2. Colors: The Almanac Palette

A warm, paper-based neutral system tinted toward maple bark, with disciplined accents drawn from the actual landscape: pine for steady authority, ember for danger and donations, ochre for caution. No blue. No purple. No grayscale-tech-neutrals.

### Primary

- **Vermont Pine** (`#2D3E2C`): The voice of the department. Used on primary buttons, the dark feature section that holds the Board of Directors, the gov-strip footer, and the crest banner. Carries authority without bravado.
- **Deep Pine** (`#1E2B1D`): Hover and pressed state for Vermont Pine. Also the gov-strip background.

### Secondary

- **Ember Brick** (`#B33A2A`): The single warning color. Used on the Donate CTA, the alert/danger states, the crest flame, and the active-fire-weather indicator. Restricted to ≤8% of any given screen, including the donate card. The crest's flame is small for a reason.
- **Banked Ember** (`#8E2C1F`): Hover state for Ember Brick, and the underline color for inline links so they read warm against Almanac Cream.

### Tertiary

- **Maple Bark** (`#6B4423`): Eyebrows, datelines, "EST. 1879" markers, secondary numerical labels. The voice of the printed dateline. Always uppercase, always letter-spaced.
- **Lantern Amber** (`#C98A2B`): Active-row highlight on the FWI legend, the gov-strip dot. Used sparingly as a focused-attention marker.
- **Caution Ochre** (`#C9762E`): The alert banner's accent color and the warn-state for the Fire Weather Index "moderate" tier.
- **Hollow Moss** (`#5B6B3A`): Tertiary tag color, used on the "Wildland" and "Training" event chips.
- **Pasture Green** (`#3E6B3E`): Reserved for "OK" / "Low danger" indicators on the FWI gauge only.

### Neutral

- **Almanac Cream** (`#F5F1E8`): The page itself. Body background. Card and surface fills. The paper.
- **Mill Paper** (`#EDE7D8`): One step warmer-darker than Almanac Cream. Used for the "cream" alternating section background, button-ghost hover, and the inverted-button text color on dark surfaces.
- **Bulletin Ink** (`#1C1C1A`): All headline and primary body type. Never `#000`.
- **Slate Ink** (`#3A3933`): Body copy and lede paragraphs. The footer's panel background border.
- **Birch Gray** (`#6B6A62`): Eyebrows, kickers, table labels, and any "support text" role.
- **Newsprint Rule** (`#D9D2BF`): The 1px hairline that does almost all the structural work on the page. Used between events, between FWI legend rows, around cards, between hero meta cells. If you reach for a shadow, reach for this instead.
- **Heavy Rule** (`#C3BCA7`): The same hairline at slightly more weight. Used for ghost-button borders and pill-tag outlines.

### Named Rules

- **The One Voice Rule.** Vermont Pine carries authority; Ember Brick carries danger. The two never share a screen surface as equals. If both must appear, pine is the structural color (button, header, frame) and ember is the highlight (donate badge, alert state, crest flame).
- **The No-Blue Rule.** Civic-American sites reach for navy by reflex. We never do. Every neutral is tinted toward maple/cream; every accent is grown from this landscape, not a corporate palette.
- **The Hairline Rule.** Newsprint Rule (`1px solid #D9D2BF`) replaces shadows, dropshadows, glows, and most card outlines. If a divider is needed, it is one pixel of Newsprint Rule. Anything heavier reads as a frame, not a separator.

## 3. Typography

**Display & Body Font:** Public Sans (with `system-ui, -apple-system, sans-serif` fallback).
**Editorial Accent Font:** Source Serif 4, italic only, weight 500 (with `Georgia, serif` fallback).

**Character.** Public Sans is a U.S. Web Design System face, designed to read clearly on government-issued public-information sites. That lineage matters here: it is not "designed to feel friendly," it is designed to be unambiguous on a phone in bright sunlight at 65 years old. Source Serif 4 italic is used like a printer's flourish: short phrases inside a Public Sans headline, a single tagline in the footer. It never carries running text.

### Hierarchy

- **Display** (Public Sans 800, 64px, line-height 1.02, letter-spacing -0.025em): Hero headline only. One per page. On screens below 920px, scales down to 44px.
- **Headline** (Public Sans 700, 38px, line-height 1.1, letter-spacing -0.015em): Section heads ("Today's Fire Weather Index", "Open burning in Ira", "Upcoming events & trainings").
- **Title** (Public Sans 700, 22px, line-height 1.25): Sub-section heads, FAQ summaries, event titles, board-card names.
- **Body** (Public Sans 400, 17px, line-height 1.6): Running paragraphs. Cap line length at 65–75ch on long-form sections; the lede uses 52ch for emphasis.
- **Label** (Public Sans 600, 12.5px, line-height 1.4, letter-spacing 0.06em, UPPERCASE): "Mono" eyebrows in legends and station-info chips. Always Birch Gray.
- **Eyebrow** (Public Sans 600, 11px, line-height 1.4, letter-spacing 0.18em, UPPERCASE): The widest-tracked label. Used for "VOLUNTEER FIRE & RESCUE · EST. 1879" and for "MO" date strips on event rows. Always Maple Bark.
- **Italic Accent** (Source Serif 4 italic, weight 500, inherits size from parent): Used inside Display and on the footer tagline. Color is Maple Bark inside the hero headline, Mill Paper in the footer.

### Named Rules

- **The Almanac-Italic Rule.** Source Serif 4 italic is reserved for two roles: a phrase or two inside a Display headline (e.g. "*hills, homes*"), and the footer tagline. It is never used for body type, button labels, eyebrows, or section headlines.
- **The Eyebrow Rule.** Every uppercase label is letter-spaced (≥0.06em for labels, 0.18em for eyebrows) and rendered in Birch Gray or Maple Bark. Uppercase without tracking reads as shouting.
- **The Single-Sans Rule.** Public Sans is the only sans on the page. No "humanist supplemental sans," no rounded display sans, no condensed accent. One civic face, six roles.

## 4. Elevation

**The system is flat.** No shadow vocabulary. Depth is conveyed entirely through tonal shifts in paper and 1px hairlines. A hover state may shift a row's background to Mill Paper; a card may sit on Almanac Cream with a Newsprint Rule border; the dark Board section sits on Vermont Pine with the type set in light cream. There are no `box-shadow` declarations in the system, and there should not be.

This matches the printed-bulletin metaphor exactly: a printed page has no shadows, only ink and paper of different weights.

### Named Rules

- **The Flat-Page Rule.** Surfaces sit on the page; they do not float above it. If a section needs separation from its neighbor, use a tonal shift (Almanac Cream → Mill Paper, or → Vermont Pine for the dark block) plus a 1px Newsprint Rule. Never a shadow.
- **The No-Glow Rule.** Focus states do not glow. Focus is communicated by a 2px solid Vermont Pine outline offset 2px from the element. No diffused colored shadows under buttons; no neon focus rings.

## 5. Components

### Buttons

- **Shape:** Subtly rounded (`4px`). Sharp enough to read as utilitarian, soft enough not to look brutalist.
- **Primary:** Vermont Pine fill, Mill Paper text, no border. Padding `12px 20px`. Right-arrow glyph that translates +3px on hover. Hover shifts to Deep Pine.
- **Ghost:** Transparent background, Bulletin Ink text, 1px Heavy Rule border. Hover swaps to Mill Paper background and Bulletin Ink border.
- **Ember (donate-only):** Used inside the donate CTA card. Inverted: Almanac Cream background, Banked Ember text. The button is the inverse of the surface it sits on.
- **States:** All buttons transition `background` and `border-color` over 150ms; the arrow glyph translates `transform` over 150ms. No scale, no bounce, no elastic.

### Chips & Tags

- **Style:** Pill-shaped (`999px`), 1px outline-only (no fill), uppercase Public Sans 600 at 10.5px with 0.14em letter-spacing.
- **Variants:** `chip-tag` (Birch Gray default), `chip-tag-ember` (events that are emergency-related), `chip-tag-forest` (volunteer/training events), `chip-tag-bark` (fundraising/community events). The variant communicates category without color flooding the screen.
- **Placement:** One per row maximum. Multiple chips per row dilutes the signal.

### Cards & Containers

- **Corner Style:** Sharp (`0px`). Cards are not rounded. Pill chips are. Buttons are slightly so. Nothing else.
- **Background:** Almanac Cream on light surfaces. On the dark Board section, a deep tonal pine (`#26351F`) with a `#3A4A31` hairline.
- **Shadow Strategy:** None. Always 1px Newsprint Rule on light surfaces, 1px tonal-pine on dark surfaces.
- **Border:** 1px Newsprint Rule. On the donate CTA, 1px Banked Ember.
- **Internal Padding:** `36px` on permit-grid cells, `32px–48px` on CTA cards, `20–28px` on inline call-out boxes. Padding varies by context; do not flatten to one number.

### Hairline Grids

The signature pattern. The hero meta row, the FWI conditions table, and the burn-permit grid are all built from cells separated by Newsprint Rule on every internal edge, with no outer container shadow. This pattern replaces what most sites would do with cards. **Do not card these. They are tables.**

### Alerts

- **Style:** Cream warn-tinted background (`#FBF3E2`). Sharp corners. **Full** 1px Caution Ochre border on all four sides — never a fat side-stripe (see Don'ts). Leading 36px-circle Caution Ochre icon containing a 20px exclamation glyph. Title in Title-class type, supporting copy in 14.5px Slate Ink.
- **Placement:** Directly under the masthead, full-width within the header band.
- **Variants:** `warn` (Caution Ochre, default), `danger` (Ember Brick — reserved for active-incident state).

### Navigation

- **Masthead:** Almanac Cream background, sticky, with a 1px Newsprint Rule bottom border. Brand crest (44px) + two-line wordmark on the left. Inline nav links on the right at Public Sans 600, 15px, Slate Ink, with 4px-rounded `padding: 10px 14px` hover backgrounds in Mill Paper.
- **Donate CTA in nav:** Ember Brick fill, Almanac Cream text, otherwise identical shape to the inline links.
- **Below 920px:** The inline nav collapses (currently to none — consider a disclosure pattern in future work).
- **Gov Strip:** Persistent strip above the masthead in Deep Pine (`#1E2B1D`) with a Lantern Amber 6px dot, 13px text in Public Sans 500. "An official site of the Town of Ira, Vermont · Established 1779."

### Departmental Crest

A custom inline SVG with: outer cream shield outlined in Bulletin Ink, Vermont Pine top banner reading "IRA · VERMONT", Vermont Pine pine-tree silhouette with a Maple Bark trunk, a small Ember Brick flame behind the tree, and a Maple Bark "est. 1879" footer. Used at 44px in the masthead, 56px in the footer, and 380px as the hero anchor. The crest is the system's only illustration and does the work that stock photography would do on a lesser site.

## 6. Do's and Don'ts

### Do

- **Do** lead every screen with a specific, dated public-information artifact. The fire weather index is updated daily and bears a timestamp. Future variants should keep that pattern: real, current, sourced.
- **Do** use Source Serif 4 italic for one or two phrases inside a Display headline. The contrast between the unfussy sans and the editorial italic is the system's single signature move.
- **Do** use Newsprint Rule (`1px solid #D9D2BF`) wherever you would otherwise reach for a card, a shadow, or a soft outline.
- **Do** keep the Ember Brick footprint under 10% of any screen. Its rarity is what gives it weight on the donate card.
- **Do** vary internal padding. `36px` for permit cells, `48px` for CTA cards, `20px` for inline call-outs. Same padding everywhere reads as monotony.
- **Do** size body type at 17px or larger and respect the 65–75ch line-length cap. The audience is older and this is a public-information site.

### Don't

- **Don't** use side-stripe borders greater than 1px as a colored accent on cards, alerts, or list items. The legacy alert pattern in `index.html` uses a 4px Caution Ochre left edge — treat as a refactor candidate; new alerts use the full-border pattern documented above.
- **Don't** add `box-shadow` to any surface. The system is flat. If a surface needs to read as raised, change its tonal background and add a 1px Newsprint Rule. Glows and drop shadows make this look like a 2014 SaaS template.
- **Don't** use gradient text or `background-clip: text`. Emphasis is achieved with weight (800 vs 400) and italic accent, never with gradients.
- **Don't** use glassmorphism, backdrop-filter blur, or any "frosted" surface. The page is paper, not glass.
- **Don't** add navy, royal blue, or "civic blue" anywhere. The palette is paper, ink, pine, bark, and ember. No blue.
- **Don't** use stock photography of crews silhouetted against sunsets, or any "heroes" rhetoric. The crest does the visual work; the volunteer count (fourteen) does the pride work.
- **Don't** add gradient-mesh hero backgrounds, "Trusted by" logo walls, oversized rounded CTAs, or any element from the SaaS landing playbook. PRODUCT.md is explicit about this.
- **Don't** flip the system to dark mode by default, add neon accents, or import a "modern AI workflow" aesthetic. This is a fire department.
- **Don't** reach for clipart flames, tiled background images, marquee text, or "Welcome to our website" intros. Every visual element is hand-built or it is not on the page.
- **Don't** use em dashes in copy. PRODUCT.md's tone is plain-spoken civic. Commas, colons, semicolons, periods, or parentheses do the work.
- **Don't** add a third typeface. Public Sans + Source Serif 4 italic is the entire system. A condensed display, a humanist supplemental sans, or a "rounded display" face is forbidden.
- **Don't** card the hairline grids (hero meta, FWI conditions, permit-grid). They are tables built from 1px rules on every internal edge. Wrapping them in cards collapses the system's signature.
