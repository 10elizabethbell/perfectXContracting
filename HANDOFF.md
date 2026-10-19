# Perfect X Contracting — handoff at ~60%

**Live:** https://10elizabethbell.github.io/perfectXContracting/ · **Repo:** https://github.com/10elizabethbell/perfectXContracting · **Built:** 2026-10-19 from Muse brief of 2026-10-19 (Essex County Contractor Referrals group, project-showcase video post)

## What's built
- One page, phone first: header (PX mark from their logo + "Perfect X / Contracting", **Message us** top-right in place of a phone number), hero "Perfect walls, every floor." (silver) with their own promise wording ("precision and care", "start to finish") and two buttons (Get a free estimate → form, See our work → stairwell).
- **Signature element: sand the seams.** A drywall wall drawn like the one in their video: grey board, a taped horizontal joint and a butt joint, rows of screw spots, every coat edge lit by window light from the top left so the knife ridges show. A violet sanding sponge (the logo's X violet) sands along the joints by itself; any finger or mouse takes it. Sanding erases the ridges back to the flat, feathered finish, and compound dust puffs off the sponge, drifts, glows in the window light and gets pushed by the pointer. The coat creeps back slowly (`REGROW` 0.0045, Above All's tuning). After ~1400px of dragging the hint says "Ready for paint." Drag works up, down and sideways on phones without scrolling the page. Tunables at the top of the wall IIFE (`SPONGE_W/H`, `SAND`, `REGROW`, `DUST_MAX_*`, `AUTO_SPEED`, `IDLE_MS`, `REWARD_PX`).
- Feathered mud edges (two-layer, slowly moving) join every dark and light section; paused off screen.
- What we do (Drywall installation / Taping & finishing / Repairs rows; each pre-ticks that service in the form), Four stories of stairwell (8 s clip from their video, tap to pause, + four stills; they climb like treads on phones and desktop) with the big "Click to see more of our work." Facebook link, Free estimate ("Serving Vermont. We reply on Messenger.", the three how-it-works steps, then the form), closing logo with their sign-off "Quality work. Reliable service.", footer with Facebook and Messenger.
- **Contact wiring:** the form composes a message (name, town, services, job, when), shows it, tries to copy it, and gives an **Open Messenger** button (`https://m.me/61595304966148`, checked: redirects to a Messenger thread). Messenger links can't pre-fill text, so the visitor pastes it; if copy is blocked (Facebook's in-app browser), the note says press-and-hold to copy.
- **When a phone number arrives:** set `CONTACT.PHONE` at the top of the first `<script>`. The top-right link becomes the number (`tel:`), and the form becomes "Text us this request" and opens an `sms:` with the message pre-filled. Add the number to the footer by hand.
- Favicon / home-screen icon from the PX mark; og:image 1200×630 (logo, headline, stairwell still).

## Assumptions I made
- **"We" voice, a crew:** from "Message us" in their caption. Change to "I" if it's one person.
- **Name styling:** "Perfect X Contracting" (from the logo's lettering). The Facebook page writes "Perfect x contracting"; Muse said keep theirs until confirmed. The logo is the stronger signal, but ask.
- **Colors:** violet #6d2ee6 (darkened from the logo's violet so white button text passes contrast) and brushed silver from the logo; deep violet-slate ground #1d1932 instead of the logo's black; joint-compound white #f1efe9 for light sections.
- **Headline** "Perfect walls, every floor." is mine (name + the four-story job). **Promise** line reuses their words. Step 3 adds "the same care we put into four floors of stairwell" to their caption. Form hover/focus accent is a cool blue (#2b6fd6) so it stands apart from the violet buttons.
- **Audience:** homeowners and builders/GCs (the job is a commercial stairwell posted to a contractor group). Not treated as a 40+ audience, so the motion is on.

## Placeholders and gaps
- **No phone number anywhere** (biggest gap). Top-right holds "Message us" (Messenger) instead. See the `PHONE` switch above.
- **No email** → no footer email (rule: footer only, never invented).
- **Area is only "Vermont"**; no towns listed.
- **Photos:** all imagery is frames from one 77 s phone video, so stills are soft (720×1280 source). Real photos of finished, painted walls would be a big upgrade. One frame I skipped: the capped-window close-up at 65 s shows a rough, unfinished exterior edge.
- No reviews, prices, hours, licensing or insurance on the page (none published).
- Logo is the 720px Facebook profile image keyed off its black background; a vector/PNG original would sharpen the closing logo and favicon.

## Questions for the owner
- Phone number, and do you take texts? An email for the footer?
- Which towns or counties do you cover?
- Your first name (and is it "Perfect X" or "Perfect x")?
- Photos of finished jobs, especially before/after repairs?
- Do you do ceilings, texture, painting, or commercial only?
- Licensed/insured, if you want it said?

## Ideas not built (yours to pick)
- **Runner-up world:** the stairwell itself — four floors as stacked landings you scroll up through, with daylight from the capped windows moving across finished walls as you climb.
- Other worlds considered: a violet laser level throwing a crossed X across the wall; a taping knife pulling mud over the joints (skipped: Green Mountain Renovations, same day, same group, uses it); raking work-light inspection.
- A paint roller pass as the "Ready for paint." reward (roller nap, wet edge, fades back after ~3 s).
- A puff of compound dust when a service chip is ticked (Sunny Side's splash precedent).
- Before/after slider once real before/after pairs exist (spotted vs. painted).
- Self-hosted wide heavy display face matching the logo's lettering (craft floor wants it; house style says system stack, so I didn't).

## Review notes
- Impeccable: ran the finish reviewer plus critique, audit, polish, harden, clarify, adapt, optimize, animate, typeset, layout, colorize, delight, distill, bolder, quieter and overdrive (live and onboard skipped). No concept roll (unattended build; the world was chosen from the trade).
- Applied: smaller flush screw spots, knife-wobbled coat edges and deeper ridges (the first pass read as pinstripes and marshmallows), gradient-feathered dividers (were a grey ribbon), stronger window light, silver headline, `we` promise, wall height capped so the hint lands on a 360×640 first screen, How it works merged into Free estimate (killed desktop dead space), only one filled button after composing, clip pausable by tap (controls under reduced motion), form borders at 3:1, chip label matches the service row, logo re-exported at 720px, `<main>` around everything, pre-feathered eraser sprite instead of a per-stroke blur, sponge size resets on resize, iOS select height, landscape-phone hero fit.
- Not applied: rewording "Click to see more of our work." (your wording); trust signals (none exist); a sticky or bottom CTA; dropping the motion.
- Detector: ignores recorded in `.impeccable/config.json` (system stack flagged as Roboto, 31-char caps sign-off, list hairline). `flat-type-hierarchy` fixed by collapsing UI text to one 17px step (20px for lead lines). Detector now reports nothing.
- Checks run (Playwright, Chromium + WebKit at 360×640, 390×760, 430×900, 844×390, 1440×900): no sideways overflow, all tap targets ≥44px, inputs ≥16px, CTA in the first screen, touch drag sands in every direction without scrolling the page, motion advancing, form errors and the Messenger message correct, no JS errors.

## Not verified
- Real-device touch on iOS/Android (Chromium touch emulation and WebKit synthetic touch pointers passed: drag sands in all directions, page doesn't scroll).
- Messenger handoff inside Facebook's in-app browser on a real phone (redirect checked with curl only), and whether clipboard copy works there.
- Frame rate on older phones (canvas capped at 1.5x on phones, ≤520 dust motes).
