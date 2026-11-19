---
name: Dr. A.M. — Dentistry
description: A one-practitioner dental portfolio in a dark editorial room with one signal-red voice.
colors:
  ink: "#0d0607"
  ink-raised: "#180a0c"
  signal-red: "#ff2b1a"
  signal-red-deep: "#c2170c"
  paper: "#f3e8e2"
  paper-shade: "#e6d6cf"
  muted-on-dark: "rgba(243,232,226,0.74)"
  rule-on-dark: "rgba(243,232,226,0.22)"
typography:
  display:
    fontFamily: "Archivo, Arial, sans-serif"
    fontSize: "clamp(3rem, 8.2vw, 8.5rem)"
    fontWeight: 700
    lineHeight: 0.88
    letterSpacing: "-0.065em"
  body:
    fontFamily: "Manrope, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Manrope, Arial, sans-serif"
    fontSize: "12px"
    fontWeight: 500
    letterSpacing: "0.03em"
rounded:
  pill: "999px"
  float: "14px"
spacing:
  gutter: "clamp(20px, 4.2vw, 64px)"
  section: "clamp(90px, 13vw, 190px)"
components:
  button-primary:
    backgroundColor: "{colors.signal-red-deep}"
    textColor: "#ffffff"
    rounded: "{rounded.pill}"
    padding: "clamp(16px, 2.2vw, 26px) clamp(26px, 4vw, 54px)"
  button-primary-hover:
    backgroundColor: "#a5140a"
    textColor: "#ffffff"
    rounded: "{rounded.pill}"
    padding: "clamp(16px, 2.2vw, 26px) clamp(26px, 4vw, 54px)"
  nav-link:
    textColor: "{colors.paper}"
    typography: "label"
    padding: "3px 0"
---

# Design System: Dr. A.M. — Dentistry

## Overview

**Creative North Star: "The Quiet Red Studio"**

A dark room with one red light. The visual language borrows from a solo designer's portfolio rather than a clinic brochure: oversized lettering, hairline rules, generous black space, and a single saturated accent that appears only where the eye should land. The person using this system should feel that one person made the work on the page and that nothing here is there to sell them something they did not ask for.

Density is deliberately uneven. A few large, quiet passages alternate with a dense work grid and a red testimonial field. Motion carries the sequence: the page reveals itself line by line, shifts from dark to paper to red, and settles on one action. The category opposite refused here is the bright, card-based multi-dentist site with a team grid and a booking form.

**Key Characteristics:**
- Near-black aubergine ground with one signal-red voice
- Display type that fills the measure and body copy that stays small and calm
- Image-led work grid with type revealed on hover
- One repeated action: the WhatsApp appointment button

## Colors

### Primary
- **Signal Red** (#ff2b1a): The only saturated voice. Reserved for key words in headlines, the hero field, the testimonial ground, and active states.

### Secondary
- **Signal Red Deep** (#c2170c): The darker red used behind white button text so it meets contrast requirements. The bright red is type and field; the deep red is interactive surface.

### Neutral
- **Ink** (#0d0607): The primary ground.
- **Ink Raised** (#180a0c): Image frames and recessed panels.
- **Paper** (#f3e8e2): Text on dark, and the full ground of the about section.
- **Paper Shade** (#e6d6cf): Secondary paper surfaces.

### Named Rules
**The One Voice Rule.** Signal Red is the only chromatic accent. No second hue enters the system; secondary text is tinted from the ground's own hue rather than greyscaled.

**The Contrast Rule.** White text never sits on bright Signal Red. Interactive red surfaces use Signal Red Deep (#c2170c) or darker.

## Typography

**Display Font:** Archivo (fallback Arial)
**Body Font:** Manrope (fallback Arial)
**Label Font:** Manrope

**Character:** Archivo is compressed and tightly tracked for the large lines; Manrope stays neutral and small for everything functional. The pairing puts all expression into scale and spacing rather than into two competing typefaces.

### Hierarchy
- **Display** (700, `clamp(3rem, 8.2vw, 8.5rem)`, 0.88 line height, -0.065em): Hero and section statements.
- **Work Title** (800, `clamp(2.4rem, 7.5vw, 7rem)`, 0.82 line height, uppercase): Revealed over project imagery on hover.
- **Body** (400, 15px to 25px, 1.55 line height, 62ch max): About copy and section descriptions.
- **Label** (500, 12px, 0.03em): Navigation, captions, metadata.

### Named Rules
**The Type Leads Rule.** A section opens with its statement at display scale. No eyebrow or kicker precedes it; the heading carries its own weight.

## Layout

A twelve-column grid with a fluid gutter of `clamp(20px, 4.2vw, 64px)`. Section padding is `clamp(90px, 13vw, 190px)`. On desktop the work grid uses alternating six-column items with the even column dropped; below 900px every item becomes full width and the drop disappears. The about copy moves from columns 4–8 to full width. Approach rows use a 1 / 4 / 5 column split for number, title, and description, collapsing to a stacked two-column layout on phones.

The first viewport is a single display statement anchored to the bottom, with one supporting sentence and a scroll cue. A red field rises from below as the hero leaves the viewport.

## Elevation & Depth

The system is flat. Depth comes from tonal layering (Ink against Ink Raised, Paper against Paper Shade) and from the single contact bar's diffuse shadow (`0 18px 48px -24px rgba(0,0,0,0.85)`). No zero-blur offset shadows are used.

### Shadow Vocabulary
- **Floating contact bar** (`0 18px 48px -24px rgba(0,0,0,0.85)`): Lifts the single persistent action off the page.

## Shapes

Most surfaces are square-edged. The only rounded forms are the pill buttons (`999px`) and the floating contact bar on phones (`14px`). A slow-drifting SVG wave forms the upper and lower edges of the red testimonial field; it is the one organic contour in the system.

## Components

### Buttons
- **Shape:** Fully rounded pill (999px).
- **Primary:** Signal Red Deep background, white text, `clamp(16px, 2.2vw, 26px)` by `clamp(26px, 4vw, 54px)` padding, Archivo 700.
- **Hover / Focus:** Background darkens to #a5140a; the large CTA also lifts 5px and its arrow shifts up and right. Focus uses a 2px Signal Red outline at 4px offset.

### Navigation
- Fixed top bar, 12px Manrope links with an underline that wipes in from the left on hover. The bar's colour inverts over the Paper and Signal Red sections. On phones only the name mark and the WhatsApp button remain.

### Work Item
- Four-column-image grid cell with a square frame. Image is desaturated and tinted red at render time. On hover the image zooms to 1.075 and a large uppercase Archivo title slides up from the bottom edge.

### Testimonial Field
- A full-width Signal Red panel bounded by drifting SVG waves, with one large pull quote and a source line.

### Floating Contact Bar
- A fixed Paper pill near the bottom centre with a deep-red WhatsApp button. It retracts when the contact section enters the viewport. On phones it becomes a full-width rounded bar.

## Do's and Don'ts

### Do:
- **Do** keep Signal Red rare and structural: a word, a field, or an action.
- **Do** use deep red behind white text.
- **Do** reveal content with masked lines and short staggered delays, and keep everything visible when reduced motion is requested.
- **Do** keep the WhatsApp button as the only conversion action.

### Don't:
- **Don't** add a second accent colour or a gradient background.
- **Don't** introduce a booking form, a team grid, or facility cards.
- **Don't** put an eyebrow above a heading or number the sections.
- **Don't** use the bright Signal Red as a white-text button surface.
