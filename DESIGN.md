---
name: Perfect X Contracting
description: A taped-and-spotted stairwell wall under window light, in the logo's violet and brushed silver.
colors:
  violet: "#6d2ee6"
  violet-press: "#5a20cf"
  violet-hi: "#a678ff"
  form-accent: "#2b6fd6"
  silver: "#c9cbd4"
  silver-lettering: "#dcdee6"
  ground: "#1d1932"
  ground-2: "#262042"
  on-dark: "#efecf7"
  on-dark-soft: "#bdb6d6"
  compound: "#f1efe9"
  wall-board: "#c4beb4"
  ink: "#1d1932"
  ink-soft: "#4a4466"
  line-light: "#cdc8bd"
  control-line: "#8f8899"
  arrow-rest: "#e2ded5"
  chip-checked: "#efe8fd"
  error: "#a3122f"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "min(clamp(2.35rem, 10.4vw, 5.6rem), 12svh)"
    fontWeight: 900
    lineHeight: 0.98
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2rem, 8.4vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 0.98
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(20px, 5.6vw, 28px)"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "-0.01em"
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 20px)"
    fontWeight: 400
    lineHeight: 1.55
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 800
    lineHeight: 1.3
  button:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 800
    lineHeight: 1
  sign-off:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(18px, 5vw, 24px)"
    fontWeight: 900
    letterSpacing: "0.06em"
rounded:
  control: "10px"
  button: "12px"
  surface: "14px"
  circle: "50%"
spacing:
  gutter: "16px"
  gap-sm: "10px"
  gap-md: "14px"
  gap-lg: "18px"
  section-top: "56px"
  section-bottom: "64px"
  column-gap: "56px"
components:
  button-primary:
    backgroundColor: "{colors.violet}"
    textColor: "#ffffff"
    typography: "{typography.button}"
    rounded: "{rounded.button}"
    padding: "0 24px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.violet-press}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.button}"
    rounded: "{rounded.button}"
    padding: "0 24px"
    height: "56px"
  service-row:
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    padding: "10px 0"
    height: "72px"
  service-arrow:
    backgroundColor: "{colors.arrow-rest}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "46px"
  service-arrow-hover:
    backgroundColor: "{colors.violet}"
    textColor: "#ffffff"
  input:
    backgroundColor: "#ffffff"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.control}"
    padding: "12px 14px"
    height: "52px"
  chip:
    backgroundColor: "#ffffff"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "0 16px"
    height: "48px"
  chip-checked:
    backgroundColor: "{colors.chip-checked}"
  more-link:
    textColor: "#ffffff"
    rounded: "{rounded.surface}"
    padding: "18px 20px"
    height: "64px"
  step-number:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.compound}"
    rounded: "{rounded.circle}"
    size: "44px"
  work-figure:
    backgroundColor: "{colors.ground-2}"
    rounded: "{rounded.surface}"
---

# Design System: Perfect X Contracting

## Overview

**Creative North Star: "The Last Sanding Pass"**

The page is a stairwell under construction: dark violet-slate sections are the stairwell in shadow, light sections are sanded joint compound, and the two meet on slow, feathered mud edges instead of straight lines. The logo supplies the only color: violet for action, brushed silver for lettering. The hero wall is a working surface you sand by hand.

Density is phone-first and generous: one column, 56px buttons, 72px service rows, 16px gutters. Hierarchy comes from weight and case alone: heavy uppercase headings over plain sentence-case body, all in the system font stack (a deliberate house choice, not a placeholder). Depth lives in the canvas lighting, not in UI shadows.

**Key Characteristics:**
- Deep violet-slate ground, never black; compound-white light sections.
- Feathered, moving mud edges at every dark/light seam.
- One violet action color; a separate blue used only inside the form.
- System font stack: 900-weight uppercase headings, 400 sentence-case body.
- Flat UI; window light from the top left drives all depth in the wall.

## Colors

Two grounds (shadowed stairwell and sanded compound) with logo violet as the only action color and silver as lettering.

### Primary
- **Logo Violet** (violet): filled buttons, the hovered service arrow, checked chips, selection, focus rings on light sections. Darkened from the logo so white text passes contrast.
- **Pressed Violet** (violet-press): filled-button hover only.
- **Lit Violet** (violet-hi): violet on dark ground: focus rings, the Facebook "more" border and icon, header and footer link hover, the Messenger icon.

### Secondary
- **Estimate Blue** (form-accent): hover and focus border, 3px halo `rgba(43,111,214,.2)` on inputs and chips, and the 3px outline on form buttons. Nowhere outside the form.

### Tertiary
- **Brushed Silver** (silver): outline-button border on dark, closing sign-off text.
- **Headline Silver** (silver-lettering): the hero headline only, echoing the logo's metal caps.

### Neutral
- **Stairwell Shadow** (ground): page ground, dark sections, theme-color. Also used as `ink` text on light sections.
- **Deep Landing** (ground-2): placeholder behind work photos and video.
- **Chalk Violet** (on-dark) / **Dusk Violet** (on-dark-soft): text and secondary text on dark (promise line, lockup subline, footer).
- **Sanded Compound** (compound): light section ground, step-number text.
- **Wall Board** (wall-board): the hero wall's board grey, CSS fallback under the canvas.
- **Muted Ink** (ink-soft): secondary text on light (step body, "optional", service area line).
- **Compound Rule** (line-light): hairline between service rows, composed-message border.
- **Control Line** (control-line): 2px border on inputs, chips, chip check box, outline button inside the form.
- **Arrow Rest** (arrow-rest): service arrow circle at rest. **Chip Tint** (chip-checked): checked chip fill.
- **Error Red** (error): inline error text and failed-field border.

### Named Rules
**The Never-Black Rule.** The darkest surface is Stairwell Shadow (violet-slate). No #000 or near-black grounds.

**The Two Accents Rule.** Violet means "act" (fill, arrow, checked). Blue means "you are here in the form" (hover/focus). Never swap them, and never use violet as the form's hover color.

**The Hover-Only Accent Rule.** Arrows and links sit neutral at rest and take the accent on hover or focus.

## Typography

**Display Font:** system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif)
**Body Font:** same stack

**Character:** Heavy, tight uppercase headings that read like the logo's block caps, over relaxed sentence-case body. One family; weight (400 / 800 / 900) and case do all the work.

### Hierarchy
- **Display** (900, uppercase, capped at 12svh so it fits the first phone screen): hero headline only, in Headline Silver, `text-wrap: balance`.
- **Headline** (900, uppercase): section headings ("What we do", "Free estimate").
- **Title** (800, sentence case): service rows; the "more" link (18 to 22px) and step titles (20px) sit at the same weight.
- **Lead** (400, 17 to 20px, max 34ch): the hero promise, in Dusk Violet.
- **Body** (400, 17px/1.55): all running text and form input text. Never below 16px.
- **Label** (800, 17px): field labels, legend, "Message us" header link. "(optional)" drops to 500 in Muted Ink.
- **Button** (800, 17px/1).
- **Sign-off** (900, uppercase, 0.06em tracking): the closing "Quality work. Reliable service." in silver. The lockup's "CONTRACTING" (11px, 0.24em, uppercase) is the only other tracked caps.

### Named Rules
**The Caps-Are-Lettering Rule.** Uppercase belongs to headings, the brand lockup and the sign-off, which mirror the logo. Body, labels, buttons and service names stay sentence case.

## Layout

Phone-first single column inside a 1180px max container with 16px gutters. Sections run 56px top / 64px bottom; the heading-to-content gap is 24px. Gaps step 10 / 14 / 18px.

- **Hero:** fills `100svh` on phones: header, copy, buttons, then the wall takes the remaining height (min `clamp(200px, 34svh, 300px)`). At 600px the two buttons sit side by side. At 1024px the hero splits into copy | wall columns (1fr / 1.05fr), wall bleeding to the right edge.
- **Landscape phones** (min-width 600px and max-height 520px): hero padding and margins tighten.
- **Desktop splits** (1024px): services and estimate become 5fr / 7fr grids with a 56px gap.
- **Stairwell gallery:** see Components. It is the page's one deliberately staggered layout.

**The Thumb Rule.** Every tap target is 44px or taller; primary buttons are 56px and full width on phones.

## Elevation & Depth

The UI is flat. Buttons, inputs, rows and panels carry no shadow; state is shown with fill, border and focus rings. The work photos are the only lifted elements (`0 14px 30px -14px rgba(0,0,0,.6)`), so they read as panels standing off the dark ground.

Real depth is drawn in the hero wall canvas: board grain, feathered compound, knife-lap ridges, and screw spots lit by raking light, plus a warm light gradient across the wall and dust that glows inside the light beam.

**The Window-Light Rule.** Light comes from the top left. Highlights go up-left, shadows down-right (ridges, spots, the sponge's drop shadow `rgba(40,26,70,.38)` offset 5/7px). Anything new drawn in the wall follows the same light.

## Shapes

Gently rounded and consistent: 10px for form controls, 12px for buttons and the composed-message panel, 14px for photo figures and the Facebook "more" block. Circles for the service arrow (46px) and step numbers (44px). The sponge is a 10px-radius rounded block.

**The Mud Edge Rule.** Dark and light sections never meet on a straight line. Each seam is a 44px SVG with two layers: a gradient feather (opacity 0, .35, .7) at baseline 12 and a solid fill at baseline 25. Each follows three layered sine waves (`SPEED` 0.0016, `AMP` 7), pauses off screen, and holds still under reduced motion. Set `data-from` / `data-to` to the two grounds.

## Components

### Buttons
Solid, chunky, the same pair everywhere.
- **Shape:** 12px radius, 56px min height, 2px border, 24px side padding.
- **Primary (fill):** violet fill and border, white text. Hover: pressed violet. One filled button per view; after the form composes its message, "Write my message" swaps to outline so "Open Messenger" is the only fill.
- **Outline:** transparent with a silver border on dark, on-dark text; hover turns the border lit violet and the text white. Inside the form it uses Control Line and ink.
- **Focus:** 3px lit-violet outline, 3px offset (violet on light sections). Form buttons get a 3px Estimate Blue outline on hover and focus.
- Transitions: 0.18s on background, border and color.

### Header lockup
PX mark (52px wide) + "PERFECT X" (900, 17px, uppercase) over "CONTRACTING" (11px, 0.24em, Dusk Violet). Contact top-right: the Messenger icon in lit violet + "Message us" (800, 17px), which turns lit violet on hover. When `CONTACT.PHONE` is set, it becomes the formatted number as a `tel:` link.

### Service rows
Full-width links between Compound Rule hairlines, 72px min height, title type, with a 46px arrow circle on the right.
- **Rest:** Arrow Rest circle, ink arrow.
- **Hover:** only the arrow changes (violet fill, white arrow). The row never gets a background, border or ring.
- **Focus:** the arrow fills violet and gets a 3px violet ring at 3px offset; the row's own outline is removed.
- Clicking a row pre-ticks the matching chip in the form.

### Stairwell gallery (signature)
Photos climb like stair treads. **Phone:** 2 columns with a 12px gap; the 4:5 video clip spans both, then 3:4 stills with every even still dropped 28px. **Desktop (1024px):** 5 columns at 9:14, bottom-aligned, each still raised 36px more than the last (0 to 144px), with 150px top margin to make room. Figures: 14px radius, Deep Landing behind, the photo shadow. The video plays only while on screen and pauses on tap. No captions.

### Facebook "more" block
Directly under the gallery: 2px lit-violet border, 14px radius, `rgba(166,120,255,.12)` tint (`.24` on hover), white title-weight text, 28px Facebook glyph in lit violet on the right. 64px min height, max 520px wide on desktop.

### Inputs / Fields
- **Style:** white field, 2px Control Line border, 10px radius, 52px min height (textarea 120px), 17px body text. The select uses a custom ink chevron.
- **Hover and focus:** Estimate Blue border + 3px blue halo, no outline. Transition 0.15s.
- **Error:** Error Red border and a plain-language message below (700, 17px), shown only after a submit attempt.

### Chips (form only)
Checkbox labels: white, 2px Control Line border, 10px radius, 48px tall, with an 18px rounded box before the text. Hover and focus use the blue border and halo. Checked: violet border, Chip Tint fill, violet box with a white tick. Used only for real choices inside the form, never for static labels.

### How-it-works steps
A numbered list: 44px ink circle with a compound numeral (900), a 20px/800 title and a Muted Ink line below.

### Composed message
White panel, 12px radius, 2px Compound Rule border, 18px padding. Holds a `user-select: all` pre (500, 17px), a note and the "Open Messenger" button.

### Hero wall (signature)
Three stacked canvases (base, rough coat, effects) on a Wall Board ground, with `touch-action: none` so a drag sands in every direction. Tunables at the top of the wall IIFE: `SPONGE_W/H` 74x44 phone, 96x56 desktop; `SAND` 0.34; `REGROW` 0.0045; `DUST_MAX_PHONE` 520 / `DUST_MAX_DESK` 1300; `AUTO_SPEED` 1; `IDLE_MS` 2200; `REWARD_PX` 1400. DPR is capped at 1.5 on phones. The hint sits bottom-left in ink with a compound glow behind it, so it stays readable over the canvas.

### Close and footer
After the last mud edge: the full logo (`min(240px, 64vw)`) centred with the sign-off in silver. The footer sits on the ground with a `rgba(255,255,255,.1)` top rule, 15px Dusk Violet text, and Facebook and Messenger links (700, on-dark, 44px tall) that turn lit violet on hover. Bottom padding adds the safe-area inset.

## Do's and Don'ts

### Do:
- **Do** join every dark/light section with a mud edge (Mud Edge Rule).
- **Do** keep violet for action and Estimate Blue for form hover/focus only (Two Accents Rule).
- **Do** change only the arrow on service-row hover and focus.
- **Do** light anything drawn in the wall from the top left (Window-Light Rule).
- **Do** run new motion through the shared `Loop` (one rAF, paused off screen, still under reduced motion), with tunables as named constants at the top of its IIFE.
- **Do** keep the system font stack; build hierarchy with weight (400/800/900) and case.

### Don't:
- **Don't** use black or near-black grounds; Stairwell Shadow is the floor.
- **Don't** add thin highlight lines or sheens to UI surfaces or photos. The white ridge highlights inside the wall canvas are the material under raking light, not decoration, and stay.
- **Don't** give buttons, rows or inputs shadows; only work photos are lifted.
- **Don't** style non-interactive labels as chips. Chip styling means a real form checkbox.
- **Don't** put captions under the gallery photos or an intro line above them.
