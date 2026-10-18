# Volt Cycles — E-Bike Commerce UX (Concept)

Product-design concept for Nithin's UX Lab Product Design series. Fictional brand
"Volt Cycles" — a VanMoof/Cowboy-style e-bike store. Built with plain `use_figma`
canvas scripting only. **Zero Figma AI used.**

## Figma file

- **Name:** E-Bike Commerce UX — Concept
- **URL:** https://www.figma.com/design/RZrxDgR3zY1J0PlWWXNjc4
- **fileKey:** `RZrxDgR3zY1J0PlWWXNjc4`
- **Page:** "Volt Cycles — Test Ride First" (`0:1`)
- **Flow start:** node `3:2` — re-verified after the motion upgrade
  (`flowStartingPoints = [{nodeId: "3:2"}]`).
- **Prototype:** https://www.figma.com/proto/RZrxDgR3zY1J0PlWWXNjc4?node-id=3-2
- Desktop only, all frames 1440 × 1024, one page.
- **Build state after the NIGHT RIDE & CADENCE rebuild (2026-10-16), read back
  from the file: 25 frames, 77 reactions** (19 AFTER_TIMEOUT + 58 ON_CLICK, all
  NODE actions, DISSOLVE navigation, zero dangling destinations). The previous
  "RIDE OUT" system (76 reactions) is superseded — see the motion section.

## ⚠ One deliberate deviation from the brief — read first

The brief named the carried colour **Matte Sage**. The carried bike is labelled
**Matte Black** in the build. Reason: after visually verifying 30+ candidate
photos, the only sage-green studio bike available (Tenways CGO600 Pro, Avocado
Green) carries a clearly legible "TENWAYS" wordmark on the top tube in zoom
crops. The standing rule for this series — a photo whose brand logo doesn't
match its label is rejected (the Puma shoe and Bezzera machine precedents) —
won over the colour name. No logos were retouched out of any photo.
"Matte Sage" still exists in the build as a selectable colour swatch/tile on
Product and Build Yours; the photographed, carried configuration is Matte Black.
If Nithin prefers, swapping the label back is a copy-only change once a
logo-free sage photo exists. **Page copy must keep saying Matte Black.**

## Frames (25) with node ids

Main row (y = 0), in flow order:

| # | Frame | Node id | Notes |
|---|-------|---------|-------|
| 1 | S1 Home · Night Ride 1 — Daylight | `3:2` | Flow start. Hero pose 1/3 |
| 4 | S2 Book a Test Ride | `3:146` | Studio + day/time selection; entry link to Lock & Go |
| 5 | S3 Find Your Fit | `3:230` | Height → frame size |
| 6 | S4 Shop Bikes | `8:2` | Browse grid (hero screen) |
| 7 | S5 Product · Turntable 1 | `5:98` | Front three-quarter (hero screen); entry link to Cadence |
| 8 | S5 Product · Turntable 2 | `5:175` | Side profile; entry link to Cadence |
| 9 | S5 Product · Turntable 3 | `5:252` | Rear three-quarter; entry link to Cadence |
| 10 | S6 Build Yours | `5:329` | Colour, battery, accessories + summary; entry link to the Range Ring piece |
| 11 | S7 Delivery & Assembly Scheduling | `6:2` | Address + day/window |
| 12 | S8 Review & Pay | `6:95` | Itemised review + payment |
| 13 | S9 Confirmed · First Ride Lit 1 — Route Dark | `6:175` | Confirmation + route map; First Ride Lit pose 1/3 |

Motion row (y = 1224) — each frame belongs to exactly one standalone piece and
is reached from that piece's home screen:

| # | Frame | Node id | Piece |
|---|-------|---------|-------|
| 14 | S1 Home · Night Ride 2 — Dusk · Beam Low | `26:2` | Night Ride pose 2/3 |
| 15 | S1 Home · Night Ride 3 — Beam High | `26:46` | Night Ride pose 3/3 |
| 16 | S5 Product · Cadence 1 — At Rest | `26:90` | Cadence pose 1/4 |
| 17 | S5 Product · Cadence 2 — 60 RPM | `26:168` | Cadence pose 2/4 |
| 18 | S5 Product · Cadence 3 — 85 RPM | `26:246` | Cadence pose 3/4 |
| 19 | S5 Product · Cadence 4 — Rhythm Held | `26:324` | Cadence pose 4/4 |
| 20 | S6 Build · Range Ring 1 — City 90 KM | `26:402` | Range Ring pose 1/3 |
| 21 | S6 Build · Range Ring 2 — Stepping Up | `26:506` | Range Ring pose 2/3 |
| 22 | S6 Build · Range Ring 3 — Touring 120 KM | `26:610` | Range Ring pose 3/3 |
| 23 | S2 Test Ride · Lock & Go 1 — Locked | `26:714` | Lock & Go pose 1/3 |
| 24 | S2 Test Ride · Lock & Go 2 — Unlocking | `26:799` | Lock & Go pose 2/3 |
| 25 | S2 Test Ride · Lock & Go 3 — Unlocked | `26:884` | Lock & Go pose 3/3 |
| — | S9 Confirmed · First Ride Lit 2 — Lighting Up | `26:969` | First Ride Lit pose 2/3 |
| — | S9 Confirmed · First Ride Lit 3 — Route Lit | `26:1045` | First Ride Lit pose 3/3 |

(The two First Ride Lit poses bring the motion row to 14 frames; total file
frames = 11 base + 14 motion = 25.)

## Process — "Test Ride First" (unchanged by the upgrade)

Home → **Book a Test Ride** (studio location + day + time slot) → **Find Your
Fit** (rider height 178 cm → Volt One Size M/L, saddle 86 cm) → **Shop Bikes** →
**Product** (in-frame 360° turntable) → **Build Yours** (colour, battery range,
accessories) → **Delivery & Assembly Scheduling** (Sat Oct 24, 9–11 AM, mechanic
assembles at the door) → **Review & Pay** → **Confirmed + First-Ride Route**
(Riverside Loop, 12.4 km). An 8-step progress stepper runs across S2–S9.

## Carried product & money (exactly as shown, unchanged)

- **Volt One** city e-bike — **Matte Black** (see deviation note), Size M/L — **$2,899.00**
- Build adds: Rear rack **$89.00** + Smart lock **$129.00**
- Subtotal **$3,117.00** · Tax (8%) **$249.36** · Delivery & assembly **FREE**
- **TOTAL $3,366.36** — identical on Build Yours (summary + header pill),
  Scheduling (summary strip + header pill), Review & Pay (total row + header
  pill), and the **"Pay $3,366.36"** button label. Confirmed references the
  same order (#VC-2481).
- Arithmetic: 2,899 + 89 + 129 = 3,117; 3,117 × 0.08 = 249.36; total 3,366.36. ✓

## Shop grid

| Card | Price | Photo |
|------|-------|-------|
| Volt One (carried, "YOUR FIT" badge) | $2,899 | Front three-quarter studio |
| Volt One Step-Through | $2,799 | Mint step-through |
| Volt Cargo | $3,499 | Longtail cargo, outdoors |
| Volt Fold | $2,499 | Black folding bike |
| Volt Sport | $3,299 | Rider on e-MTB, trail |
| Parts & Accessories tile | From $49 | Battery cell-pack close-up |

## Motion design — "NIGHT RIDE & CADENCE" (current system, built 2026-10-16)

**SUPERSEDED:** the previous "RIDE OUT" system (display wake/rolling hero,
Assist ladder, Charge bar, Test Ride street preview, self-ticking checklist)
was removed at Nithin's direction ("redo fresh"). All 14 of its pose frames
were deleted, its furniture was stripped from the base screens (hero display
panel, spoke-rings, crank dot, Confirmed checklist card), and no old chain
remains reachable in the prototype.

The new language is **light after dark, and the rhythm of pedalling**. The
doctrine is unchanged: **no cross-screen animation anywhere** — no element
morphs, travels, or continues between screens. Screens connect by plain
DISSOLVE navigation only. Every piece is self-contained inside its own
screen, self-plays on AFTER_TIMEOUT, and can also be advanced by clicking
its photo/panel. The hero carries launch-style excitement; the flow pieces
explain the product. The Product turntable is kept as a content viewer
(unchanged: `5:98` → `5:175` → `5:252` → loop, 1.5 s, DISSOLVE).

### Piece 1 — HOME hero "NIGHT RIDE" (3 poses: `3:2` → `26:2` → `26:46` → loop)

The hero photo's world goes to dusk **in place** — the bike never moves.
Drawn interface elements only: a dark overlay over the same photo, a beam
cone from the headlight, a lit pool on the ground, light glows, and the
handlebar-display panel returning as a glowing night readout:

1. **Daylight** (`3:2`, flow start) — no overlay, no panel; chip
   "NIGHT RIDE · DAYLIGHT · LIGHTS OFF · 1/3".
2. **Dusk · Beam Low** — dim overlay (opacity 0.42) over the photo; beam cone
   appears at low strength, a small lit pool forms on the ground ahead of
   the front wheel, headlight and rear-light glows on; display panel glows
   "LOW BEAM · AUTO · DUSK SENSOR"; chip "NIGHT RIDE · DUSK · BEAM LOW · 2/3".
3. **Beam High** — dim deepens (0.58), the cone widens and brightens, the
   pool grows, glows strengthen; panel reads "HIGH BEAM"; chip
   "NIGHT RIDE · BEAM HIGH · SEE & BE SEEN · 3/3".

Timing: 1.6 s / 1.6 s, then a 2.6 s hold before looping. Clicking the hero
photo advances. Both Home CTAs work in every pose.

### Piece 2 — PRODUCT "CADENCE" (4 poses: `26:90` → `26:168` → `26:246` → `26:324` → loop)

Clones of the side-profile product screen, entered from all three turntable
poses via "Feel the cadence →". Over the photo, a drawn amber crank arm
cycles through pedal positions (200° → 290° → 20° → 110°) around a ring at
the crank, while a dark readout panel steps the cadence:

- **At Rest** — 0 RPM · PEDALS STILL.
- **60 RPM** — A RELAXED CITY RHYTHM · THE MOTOR MATCHES YOU (1.4 s).
- **85 RPM** — CRUISING RHYTHM (1.2 s, the chain quickens with the cadence).
- **Rhythm Held** — 85 RPM, crank advanced another quarter-turn (1.0 s in,
  2.2 s hold, loops).

The view chip re-reads "CADENCE · n/4 · FIND YOUR RHYTHM"; clicking the
photo advances; "← Back to the 360° view" returns to the turntable;
"Build yours" and "Book a test ride" still work in every pose.

### Piece 3 — BUILD "RANGE RING" (3 poses: `26:402` → `26:506` → `26:610` → loop)

Clones of Build Yours with a range panel added below the accessories row,
entered from the original Build screen via "Watch the range ring fill →".
A big donut gauge (arc fill) is the piece — it fills and re-reads in place
as the battery choice steps up; the matching battery tile gains a selection
outline per pose:

- **City 90 KM** — ring at 75%, CITY BATTERY · STANDARD RANGE.
- **Stepping Up** — ring at 88%, readout 105 KM, TOURING BATTERY.
- **Touring 120 KM** — ring full (100%), TOURING BATTERY · EXTENDED RANGE.

1.5 s / 1.5 s, 2.4 s hold on full, loops; clicking the panel advances. The
build summary and the $3,366.36 total stay untouched on screen in every
pose. (Ring figures follow the screen's own frozen battery copy — City
90 km included, Touring 120 km — rather than introducing new numbers.)

### Piece 4 — TEST RIDE "LOCK & GO" (3 poses: `26:714` → `26:799` → `26:884` → back to `3:146`)

Clones of Book a Test Ride with a lock panel added under the ride note,
entered from the original screen via "Unlock it with your phone →". The
panel carries the Matte Black Volt One photo (same hero photograph) with a
drawn frame-lock glyph at the rear wheel; amber pulse rings breathe outward
from the lock as the states step, beside a phone-key chip:

1. **Locked** — one faint ring; "LOCKED · TAP TO UNLOCK · YOUR PHONE IS THE
   KEY"; chip "PHONE KEY · STANDING BY".
2. **Unlocking…** — two rings; "PULSE SENT · TALKING TO THE FRAME LOCK";
   chip "PHONE KEY · SENDING PULSE".
3. **Unlocked** — three bright rings; "READY TO RIDE · KEY STAYS IN YOUR
   POCKET"; chip "PHONE KEY · CONNECTED ✓".

1.5 s / 1.5 s, 2.6 s hold on Unlocked, then the chain returns to the
booking screen. Clicking the panel advances.

### Piece 5 — CONFIRMED "FIRST RIDE, LIT" (3 poses: `6:175` → `26:969` → `26:1045` → loop)

The original Confirmed screen is pose 1. Inside the route map card, the
Riverside Loop route line lights segment by segment (amber) across the
poses; a dark status pill inside the map carries the readout:

1. **Route Dark** — all five segments muted; "ROUTE DARK · 0.0 KM LIT".
2. **Lighting Up** — the first three segments lit; "ROUTE LIT · 6.2 KM ·
   LIGHTING UP".
3. **Route Lit** — the full loop glows, the end dot glows, and a
   "HEADLIGHT · AUTO ON" chip appears on the confirmed photo;
   "ROUTE LIT · 12.4 KM · READY".

1.5 s / 1.5 s, 2.6 s hold on the lit loop, loops; clicking the route card
advances. The order number (#VC-2481) and all confirmation content are
unchanged.

**Reactions read back after the rebuild: 77 total** — 58 ON_CLICK (all NODE,
DISSOLVE 0.5 s) + 19 AFTER_TIMEOUT pose advances across the pieces (incl.
the kept turntable). Read-back confirmed zero dangling destinations and
`flowStartingPoints = [{nodeId: "3:2"}]`.

## Motion Design tour captions (for the UX Lab page) — 12 · NIGHT RIDE & CADENCE

1. Night Ride starts in daylight: the Matte Black Volt One in the hero, lights off, the city bright around it.
2. Then dusk falls in place — the same photo dims, the headlight wakes, and a low beam pools on the ground ahead of the front wheel.
3. Beam high: the cone widens, the pool grows, the rear light glows red, and the handlebar display lights up in the dark — SEE & BE SEEN.
4. The walkthrough starts where Volt does: Book a Test Ride — a studio, a day, and a 10:30 slot, free for 45 minutes.
5. On the booking screen, Lock & Go: one faint pulse ring around the frame lock — LOCKED, and your phone is the key.
6. Tap, and the rings breathe outward — pulse sent, talking to the lock — until the panel reads UNLOCKED · READY TO RIDE, key still in your pocket.
7. On Product, the same Matte Black Volt One turns in place — front three-quarter, side profile, rear three-quarter — without ever leaving its frame.
8. Cadence begins at rest over the side profile: crank still, readout at 0 RPM, one beat from turning.
9. 60 RPM — a relaxed city rhythm. The drawn crank arm steps a quarter-turn per beat and the motor matches you.
10. 85 RPM, and the chain itself quickens — the poses arrive faster as the rhythm rises, then hold at the Volt One sweet spot.
11. On Build Yours, the Range Ring fills as the battery steps up: 90 KM of City range at three-quarters, then the full circle — Touring, 120 KM, extended range.
12. Confirmed ends the story lit: inside the route card, the Riverside Loop lights segment by segment until all 12.4 KM glow — ROUTE LIT · READY, headlight on auto.

## Images — sources & verification

Method: every candidate photo was downloaded, assembled into contact sheets,
and visually inspected (with zoom crops on any suspect frame text) before use.
Finals live in `assets/`; candidates and inspection sheets in `assets-src/`.

Used (9 photos, uploaded to the file):

| Build asset | Used for | Source | Verification |
|---|---|---|---|
| `assets/hero.jpg` | Home hero; Product turntable pose 2 (side) | `assets-src/u4.jpg` (Unsplash batch) | Zoom-inspected: matte-black minimalist city bike, **no legible branding** at any zoom |
| `assets/one-front.jpg` | Product pose 1; Shop Volt One card; Review thumb | https://outdoorgearlab.b-cdn.net/photos/25/97/381195_26656_XXL.jpg | Same bike model as hero (extended top tube, head plate, pale seat-cluster stripe), front three-quarter, no text |
| `assets/one-rear.jpg` | Product pose 3; Confirmed still | https://bikes-world.com/wp-content/uploads/2025/01/d1920_pdp_sdark_header_00_0.jpg | Same bike model, rear three-quarter, no text |
| `assets/step.jpg` | Volt One Step-Through card | `assets-src/c3.jpg` (image-search batch) | Mint step-through matches label; tiny down-tube model text is sub-legible at card size (disclosed) |
| `assets/cargo.jpg` | Volt Cargo card | `assets-src/c6.webp` (image-search batch) | Longtail cargo matches label; small "HAUL" seat-tube model text sub-legible at card size (disclosed) |
| `assets/fold.jpg` | Volt Fold card | `assets-src/c8.jpg` (image-search batch) | Black folding bike matches label; only tiny component text (crank/tyre) |
| `assets/sport.jpg` | Volt Sport card | `assets-src/c10.jpg` (image-search batch) | Rider on e-MTB matches "Sport" label |
| `assets/battery.jpg` | Accessories tile; Spare Battery tile | `assets-src/c13.webp` (image-search batch) | Battery cell-pack close-up, no branding |
| `assets/test-ride-street.jpg` | Test Ride preview card in the superseded RIDE OUT system — **no longer placed in the file** after the Night Ride & Cadence rebuild (the Lock & Go panel reuses the hero photograph instead) | Pexels photo 20409358 — https://images.pexels.com/photos/20409358 (page: pexels.com photo 20409358, "man riding electric bike"); downloaded at 1600×1067; Figma imageHash `60e8021dd595224e157ef6b52d0ed4add0a617dc` | Motion-blurred city street, rider on a grey city e-bike. Zoom-cropped at the frame before acceptance: **no legible wordmark anywhere on the bike** (down tube clean; the rider's t-shirt graphic is not bike branding and reads as no text) |

Note: exact page URLs for the six batch-sourced photos were not retained from
the original sourcing pass; local source files are listed instead. The two
URLs above are verbatim from the original build session's downloads.

Rejected after visual inspection (legible third-party branding): a studio bike
with "HAVEN BICYCLES" embossed on the battery; an "ENVO" down-tube logo;
"HIMIWAY" down-tube bikes; Lime share bikes; a "cake" branded bike; the sage
Tenways CGO600 Pro set ("TENWAYS" wordmark legible in zooms on all angles —
see deviation note); a "VELO"-branded white bike; a Cowboy C4 studio shot
with a faintly legible "COWBOY" top-tube wordmark. **Added by the upgrade
pass:** Pexels photo 15021623 (rider on a white step-through e-bike past a
teal wall) — rejected because a tight crop of the down tube reads "EVELO".

An attempt in the original build to generate the hero wheel-spin by rotating
the photo's wheel regions in PIL was made and rejected: the fork and
background inside the rotation discs moved visibly. The shipped loop uses
drawn spoke-rings over the unmodified photo instead; the upgrade's blur discs
are likewise drawn UI over the photo, never edits to the photo itself.

## Proof screenshots (this folder)

**Night Ride & Cadence poses — EXPORTED and visually inspected 2026-10-17**
(the 2026-10-16 export was blocked by the Figma MCP tool-call limit; the
limit had reset by the finishing pass): `pose-nightride-1/2/3.png` (hero
sequence), `pose-cadence-2/3.png`, `pose-rangering-1/3.png`,
`pose-lockgo-1/3.png`, `pose-firstlit-1/3.png`, plus refreshed `home.png`
(= Night Ride pose 1) and `confirmed.png` (= First Ride Lit pose 1). All
files byte-verified non-empty and read visually. Placement defects found in
that inspection and fixed in the same pass (re-rendered and re-inspected):

- **Beam cones (poses 2/3):** the authored cone vectors sat at the frame
  origin (a giant triangle in the page's top-left corner). Rebuilt as
  wedges thrown from the headlight (centre 1288, 322) down to the lit pool;
  the lit pools, which spilled past the photo's right edge, were moved
  fully inside the hero photo.
- **Lock & Go rings (all 3 poses):** the pulse rings and lock glyph centred
  mid-bike over the crank; shifted (−84, +8) so they centre on the rear
  wheel / seat-stay — where the frame lock lives.
- **First Ride Lit pose 3:** the added "HEADLIGHT · AUTO ON" chip sat
  exactly on top of the base screen's display chip; now stacked 8 px below
  it.
- Verified clean with no changes needed: Cadence crank ring/arm (centred on
  the bottom bracket), Range Ring donut and readouts, First Ride Lit route
  segments, all chips and totals ($3,366.36).

Superseded RIDE OUT system poses (kept on disk as history; the frames no
longer exist in the file): `pose-rideout-1/2/3/4.png`, `pose-assist-1/2/3.png`,
`pose-charge-1/2/3.png`, `pose-testride-1/2/3.png`, `pose-ready-1/2/3.png`.
Unchanged from the original build: `test-ride.png` · `fit.png` · `shop.png` ·
`pose-turntable-1/2/3.png` · `build.png` · `scheduling.png` · `review.png` ·
`product.png` (still accurate except its entry link now reads
"Feel the cadence →").

## Caveats

- Present-mode feel is unverified until Nithin's real click-through — the
  loops ride on AFTER_TIMEOUT; every pose is a complete readable screen if a
  timer stalls.
- **The Night Ride & Cadence poses were visually inspected on 2026-10-17**
  (rendered screenshots, this folder) after the MCP limit reset; the
  placement defects that inspection found (beam cones at the frame origin,
  pools spilling off the photo, Lock & Go rings centred mid-bike, an
  overlapping chip on First Ride Lit pose 3) were fixed and re-inspected —
  see Proof screenshots. Final read-back after the fixes: **25 frames, 77
  reactions, flow start 3:2, zero dangling destinations.**
- The Night Ride display panel is a drawn UI state floating at the cockpit
  of the hero photo (a magnified-display treatment, as in the sibling
  builds) — it covers part of the wall/top-tube area beside the handlebar,
  not the bike's own display (the photo's cockpit is small at this framing).
- Cadence figures (60/85 RPM) and the Range Ring's intermediate 105 KM
  readout are concept figures; the ring's endpoints (City 90 KM, Touring
  120 KM) are the screen's own frozen battery copy.
- Prices, ratings (4.9 · 1,284 reviews), dates, addresses, and the order
  number are assigned concept figures, labelled as such in every frame's
  footer.
- Mixed locales by concept design: Berlin test-ride studios (per the brief's
  VanMoof-style setting) and a Brooklyn delivery address; copy is a concept
  draft, not localised.
- Only the Volt One card on Shop is wired (it is the carried product); other
  cards and the header nav are display elements, as in the rest of the series.
