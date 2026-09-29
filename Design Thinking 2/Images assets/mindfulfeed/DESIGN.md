---
name: MindfulFeed
colors:
  surface: '#fbf9f2'
  surface-dim: '#dcdad3'
  surface-bright: '#fbf9f2'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f4ed'
  surface-container: '#f0eee7'
  surface-container-high: '#eae8e1'
  surface-container-highest: '#e4e2dc'
  on-surface: '#1b1c18'
  on-surface-variant: '#424843'
  inverse-surface: '#30312c'
  inverse-on-surface: '#f3f1ea'
  outline: '#727972'
  outline-variant: '#c2c8c1'
  surface-tint: '#476550'
  primary: '#213f2c'
  on-primary: '#ffffff'
  primary-container: '#385642'
  on-primary-container: '#a8cab1'
  inverse-primary: '#adcfb5'
  secondary: '#446651'
  on-secondary: '#ffffff'
  secondary-container: '#c3e9cf'
  on-secondary-container: '#496a55'
  tertiary: '#2b3b40'
  on-tertiary: '#ffffff'
  tertiary-container: '#425257'
  on-tertiary-container: '#b3c5ca'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#c8ebd0'
  primary-fixed-dim: '#adcfb5'
  on-primary-fixed: '#032111'
  on-primary-fixed-variant: '#2f4d3a'
  secondary-fixed: '#c6ebd1'
  secondary-fixed-dim: '#abcfb6'
  on-secondary-fixed: '#002111'
  on-secondary-fixed-variant: '#2d4d3a'
  tertiary-fixed: '#d4e6eb'
  tertiary-fixed-dim: '#b8cacf'
  on-tertiary-fixed: '#0d1e22'
  on-tertiary-fixed-variant: '#39494e'
  background: '#fbf9f2'
  on-background: '#1b1c18'
  surface-variant: '#e4e2dc'
typography:
  display-lg:
    fontFamily: Newsreader
    fontSize: 40px
    fontWeight: '400'
    lineHeight: 48px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Newsreader
    fontSize: 32px
    fontWeight: '400'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Newsreader
    fontSize: 28px
    fontWeight: '400'
    lineHeight: 36px
  headline-md:
    fontFamily: Newsreader
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
  headline-sm:
    fontFamily: Newsreader
    fontSize: 20px
    fontWeight: '500'
    lineHeight: 28px
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-lg:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-md:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Manrope
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 14px
    letterSpacing: 0.03em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  space-xxs: 0.25rem
  space-xs: 0.5rem
  space-sm: 0.75rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
  space-2xl: 3rem
  space-3xl: 4rem
  gutter-mobile: 1rem
  gutter-tablet: 1.5rem
  gutter-desktop: 2rem
  margin-mobile: 1.25rem
  margin-tablet: 2rem
  margin-desktop: auto
  container-max-width: 42rem
---

## Brand & Style

This design system embodies an intentional, tranquil, and restorative digital sanctuary. Built to counter behavioral dark patterns, algorithmic slot machines, and dopamine loops, its aesthetic foundation combines Scandinavian minimalism with tactile, organic calm. 

The emotional signature is grounded, unhurried, and respectful. Interfaces do not compete for attention or manufacture urgency; instead, they act as clear glass vessels for meaningful human exchange and personal reflection. Equal visual weight across opposing actions (e.g., leave vs. stay, mute vs. consume) ensures human agency remains uncompromised. Surfaces feel breathable, silent, and natural, fostering emotional balance and continuous cognitive ease.

## Colors

The color architecture is deliberately low-stimulation, removing saturated reds, neon highlights, and high-contrast electric blues that fuel compulsive engagement.

- **Primary (`#385642` - Muted Deep Forest):** Evokes steady grounding and intention. Used for primary focus elements, intentional affirmations, and active states.
- **Secondary (`#7B9E87` - Soft Sage):** Adds gentle organic warmth. Used for supportive indicators, subtle progress markers, and secondary interactive accents.
- **Tertiary (`#6C7D82` - Warm Slate):** A balanced, mineral tone that manages utility states, meta labels, and non-demanding informational glyphs.
- **Neutral (`#F4F2EB` - Gentle Oat / Stone):** Replaces harsh stark whites with a tactile, paper-like background that reduces ocular strain during sustained reading.

### Functional Tones
- **Subtle Surface Container:** `#EBE8DE` (for nested content grouping without heavy borders).
- **Text & High Contrast:** `#202621` (soft charcoal rather than pure black, reducing optical vibration).
- **Gentle Caution / Notice:** `#9C7F60` (warm earthenware tone to communicate changes or deletions without adrenaline-inducing amber/red alerts).

## Typography

The pairing marries the contemplative, editorial pace of **Newsreader** for titles with the clean, structural clarity of **Manrope** for reading and interface labels.

- **Newsreader** establishes an unhurried, book-like environment. Headlines invite reflection rather than urgency.
- **Manrope** delivers high legibility at micro and macro scales, avoiding mechanical rigidity while remaining neutral and open.
- Tracking is generous and vertical rhythm prioritizes spacious line-heights to eliminate cognitive fatigue and reduce rapid visual scanning.

## Layout & Spacing

The layout is built around a single-column, centered reading column (`container-max-width: 42rem`) that prevents excessive eye motion and maintains peaceful vertical flow.

- **Grid Discipline:** A focused 4-column layout on mobile scales to 8 columns on tablet and a centered, restricted column on desktop. Elements do not compete horizontally; spacing prioritizes vertical breathing room.
- **Rhythm:** Spacing follows an 8pt base scale. Ample margins around content cards prevent crowding and give every thought room to breathe before moving to the next item.
- **Feed Pagination:** Infinite scroll is explicitly avoided. Spacing between feed segments ends in deliberate "session completion" checkpoints.

## Elevation & Depth

To avoid overstimulation and illusory depth tricks that simulate physical micro-rewards, this system relies on **tonal surface stacking** rather than heavy drop shadows.

- **Base Layer (`#F4F2EB`):** The master canvas.
- **Elevated Surfaces (`#EBE8DE`):** Secondary cards, sheets, and modular drawers sit on this subtle tone.
- **Soft Ambient Separation:** When elevation is critical for overlays or modals, a diffuse, low-opacity natural shadow tinted with forest slate is applied:
  `0 4px 24px -2px rgba(56, 86, 66, 0.06), 0 1px 3px 0 rgba(56, 86, 66, 0.04)`
- **Low-Contrast Outlines:** Interactive borders use an understated edge (`rgba(56, 86, 66, 0.12)`) without high-contrast hard outlines.

## Shapes

Shapes utilize a natural, pebble-like curvature (`roundedness: 2`, where base radius is `0.5rem`, reaching `1rem` on container cards and `1.5rem` on prominent focal items).

- Standard interactive components (buttons, input fields) share consistent `0.75rem` - `1rem` corner radii.
- Sheet dialogs and feed modules feature soft `1.5rem` top radii, creating organic, human-friendly contours that feel non-hostile and approachable.

## Components

### Buttons & Intentional Symmetry
- **Balanced Weights:** Primary affirmative actions ("Continue", "Reflect") and autonomy-preserving dismissals ("Step Away", "Done for Now") feature equal visual footprint. Neither is penalized with tiny low-contrast links or hidden gestures.
- **Surface:** Solid `#385642` with `#F4F2EB` text for affirmative; solid `#EBE8DE` with `#202621` text for neutral departure.
- **Height & Padding:** Minimum tap target of 48px height with 20px horizontal padding to ensure comfortable, intentional input.

### Feed Cards & Content Containers
- **Visual Hygiene:** Cards employ `#EBE8DE` backgrounds with no heavy borders.
- **Absence of Metrics:** Cards strictly prohibit public like counts, virality scores, or notification badges. Author information and date stamps share equalized, muted typographic hierarchy (`label-md`).

### Chips & Filters
- **Intentional Selection:** Toggleable chips are muted slate (`#6C7D82` at 12% opacity) in an inactive state, transitioning smoothly to `#7B9E87` with high-contrast text when active.
- **No Infinite Suggestions:** Chips are limited to fixed, user-curated categories rather than unending algorithmic recommendation tags.

### Inputs & Text Areas
- **Focus States:** Focused fields softly shift border tone to `#7B9E87` with an ambient ring `0 0 0 3px rgba(123, 158, 135, 0.25)`.
- **Placeholder Language:** Quiet and welcoming rather than demanding (e.g., *"What is on your mind?"* instead of *"Share your reaction now!"*).

### Checkboxes & Radios
- **Design:** Geometric precision softened with 4px radii for checkboxes and pure circles for radios.
- **Feedback:** Transitions are smooth (250ms ease-out) without bouncy micro-animations that gamify interaction.

### Session Boundary Indicators ("Well Done" Pauses)
- A dedicated layout component that marks the completion of a batch of updates.
- Styled as an unadorned, centered message rendered in `headline-sm` with a calm prompt allowing the user to seamlessly close the application.