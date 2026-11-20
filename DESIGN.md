---
name: Side A
description: An ink-dark coffee and listening identity with the structure of a catalog sleeve.
colors:
  ink: "#171719"
  paper: "#faf8f3"
  muted: "#b9b7b1"
  accent: "#b8d88a"
  rule: "#454547"
  track-hover: "#232a21"
typography:
  display:
    fontFamily: '"Barlow Condensed", "Arial Narrow", sans-serif'
    fontSize: "clamp(4rem, 7.1vw, 6rem)"
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: "-0.025em"
  headline:
    fontFamily: '"Barlow Condensed", "Arial Narrow", sans-serif'
    fontSize: "clamp(2.75rem, 4.7vw, 4.75rem)"
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: "-0.025em"
  title:
    fontFamily: "Arial, Helvetica, sans-serif"
    fontSize: "1.3rem"
    fontWeight: 400
    lineHeight: 1.6
  body:
    fontFamily: "Arial, Helvetica, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Arial, Helvetica, sans-serif"
    fontSize: "0.75rem"
    fontWeight: 400
    lineHeight: 1.6
  action:
    fontFamily: "Arial, Helvetica, sans-serif"
    fontSize: "0.9rem"
    fontWeight: 700
    lineHeight: 1.6
rounded:
  square: "0"
  record: "50%"
spacing:
  half: "0.5rem"
  three-quarter: "0.75rem"
  one: "1rem"
  one-quarter: "1.25rem"
  one-half: "1.5rem"
  two: "2rem"
  three: "3rem"
  four: "4rem"
  gutter: "clamp(1.25rem, 4vw, 4rem)"
components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.ink}"
    typography: "{typography.action}"
    rounded: "{rounded.square}"
    padding: "0.85rem 1.25rem"
  button-primary-hover:
    backgroundColor: "{colors.paper}"
  navigation-link:
    textColor: "{colors.paper}"
    padding: "0.75rem 0"
  sleeve-note:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.ink}"
    rounded: "{rounded.square}"
    padding: "2rem"
  menu-row:
    textColor: "{colors.paper}"
    padding: "1.35rem 0.75rem"
  menu-row-hover:
    backgroundColor: "{colors.track-hover}"
  disclosure-summary:
    textColor: "{colors.paper}"
    padding: "1.2rem 0"
---

# Design System: Side A

## Overview

**Creative North Star: "The catalog sleeve"**

Side A pairs an ink-dark listening-room identity with direct coffee photography. Condensed display lettering, fine rules, and aligned catalog entries establish the structure; muted green marks emphasis without turning the page into a field of floating cards.

The surface is flat and deliberate. Photographs supply real-world depth, while a simple concentric record mark supplies geometry rather than simulated vinyl texture. Spacious section breaks contrast with compact labels and menu rows.

**Key Characteristics:**
- Ink-dark ground, chalk text, and muted-green emphasis.
- Condensed display lettering with plain, readable supporting text.
- Fine rules, squared controls, and aligned catalog rows.
- Real photography and restrained geometric record imagery.

## Colors

The palette combines near-neutral ink and chalk with a soft green accent; the frontmatter owns exact color values.

### Primary
- **Muted green / accent:** primary action fill, selected headline phrase, record-note panel, track identifiers, and keyboard focus.
- **Track hover:** subdued green-dark feedback on informational menu rows.

### Neutral
- **Matte ink:** the page ground and text on green-filled surfaces.
- **Chalk / paper:** primary text and the primary action's hover fill.
- **Muted neutral:** supporting copy, captions, and explanatory metadata.
- **Fine rule:** section boundaries, list dividers, and disclosure separators.

### Named Rules
**The Green Signal Rule.** Green identifies emphasis, action, and catalog annotations; supporting copy remains muted.

## Typography

**Display Font:** self-hosted Barlow Condensed Semibold, with Arial Narrow and sans-serif fallbacks.
**Body Font:** Arial, Helvetica, sans-serif. There is no separate monospace voice.

**Character:** tightly set condensed capitals carry the identity; ordinary sans-serif prose carries explanations without competing with the display.

### Hierarchy
- **Display:** the frontmatter display role governs the wide layout. At widths up to 900px it uses `clamp(3.75rem, 7.4vw, 6rem)`; up to 640px it uses `clamp(3.8rem, 14vw, 5.5rem)`.
- **Headline:** the frontmatter headline role governs major sections. The compact explanatory heading uses `clamp(2.5rem, 3.3vw, 3.25rem)`.
- **Title:** menu names use the title role, reduced to `1.2rem` on mobile. The sleeve-note title is bold at `1.05rem`.
- **Body:** the base role inherits the browser's root size. Actual supporting copy ranges from `0.875rem` to `1.1rem`; general paragraph measure is capped at `65ch`, with shorter local measures.
- **Label:** metadata uses the label role, with tracking of `0.06em` to `0.12em` where present. Track IDs, the interlude, and the hero note use `0.8rem`.
- **Action:** the filled action is bold; navigation and text links use the same size at normal weight.

### Named Rules
**The Two Voices Rule.** Use condensed lettering for identity and headings; keep explanatory copy and functional labels in the body face.

## Layout

The centered shell caps at 1600px with the fluid gutter token. Wide layouts pair columns rather than nesting cards. Major sections use generous vertical spacing; component groups use the smaller spacing steps.

At 900px and below, column gaps narrow, the masthead descriptor disappears, and secondary menu annotations are hidden. At 640px and below, the main sections become one column, navigation wraps, and the footer reorganizes. Mobile section spacing is generally 4rem, with 2rem component gaps. At 1440px and above, the hero gains additional vertical space.

Images occupy explicit frames with cover cropping. The mobile coffee image uses a 1.12 aspect ratio; the room image uses 1.1 on desktop and 1.3 on mobile. Do not stretch source photographs.

## Elevation & Depth

There are no box shadows or elevated cards. Tonal separation, thin rules, photographic depth, and generous space distinguish regions.

### Named Rules
**The Flat Sleeve Rule.** Separate content through rules, space, and flat tone rather than floating-card shadows.

## Shapes

Controls and colored panels are square. Rules are 1px. The record emblem uses concentric circular outlines; it is a geometric mark, not an imitation material. Icons are consistent inline SVG linework, normally 24px with a 1.5 stroke.

## Components

### Primary action
A filled, square in-page anchor pairs a plain action label with an arrow. It has a minimum height of 56px, a 3rem internal gap, and the frontmatter padding. Hover changes green to chalk. Keyboard focus uses a 3px green outline with a 6px offset.

### Navigation and text links
Navigation is unboxed, aligned to the right on desktop, and full-width wrapping on mobile. Navigation links retain a 44px minimum height; mobile vertical padding is reduced to 0.25rem. Hover turns links green. Supporting text links keep their underline with a 0.3em offset; all links share the visible focus treatment.

### Sleeve note
A single green information panel uses the frontmatter padding, reduced to 1.5rem on mobile. The record emblem is 100px across on desktop and 72px on mobile, where it floats beside the text. It is not an interactive card.

### Catalog menu
A semantic description list pairs A/B track identifiers with drink names, descriptions, and optional annotations. Rows are separated by thin rules; hover shifts the background over 0.18s ease-out. Mobile rows lose horizontal padding. Rows are informational and must not be added to the tab order.

### Native disclosures
Native details and summary elements provide expansion without JavaScript. Summary rows are at least 72px tall. The plus icon rotates 45 degrees when open; answer text appears below in muted color. Inline answer links retain underline and focus treatment.

### Motion and browser surfaces
One photo arrival lasts 0.8s with `cubic-bezier(.16, 1, .3, 1)`, moving from a visible 12px offset and reduced saturation to its resting state. Reduced-motion preferences disable animation, transitions, and smooth scrolling. Selection uses green with ink text; scrollbar colors use green and ink. There are no input fields, loading states, or checkout components to document.

## Do's and Don'ts

### Do:
- **Do** use the Green Signal Rule for emphasis and interaction.
- **Do** retain condensed headings, plain supporting text, and clear keyboard focus.
- **Do** use real photographs with intentional cover crops and truthful captions.
- **Do** keep catalog rows informational and disclosures natively operable.

### Don't:
- **Don't** replace the Flat Sleeve Rule with a floating-card scaffold.
- **Don't** simulate vinyl, embossing, or other physical materials with decorative effects.
- **Don't** introduce an unrelated display face or a monospace costume.
- **Don't** use labels above headings as decorative eyebrows.
