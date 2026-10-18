# PlayStation 5 Commerce UX — Concept (Not affiliated with Sony)

Slot 2 of the UX Lab Product Design series — replaces the fictional "Nova Play" console.
The concept/process were kept; the hardware is now the ACTUAL PlayStation 5 and DualSense,
shown with real product photography throughout. Zero Figma AI — plain `use_figma` canvas
scripting only. The Nova Play file was not modified.

**Figma file:** https://www.figma.com/design/wZptwo99BVE4M39qXEgcER
**File key:** `wZptwo99BVE4M39qXEgcER`
**Page:** "PS5 — Launch Day"
**Flow start:** node `2:107` — "P01 Home · Boot 1 — STANDBY", flow name "PS5 — Launch Day"
**Totals read back after wiring:** 27 frames / 78 reactions (NODE actions, DISSOLVE transitions,
AFTER_TIMEOUT pose chains + click-advance on pose frames; read back after the V3 rebuild —
27 frames / 78 reactions / flow start `2:107` confirmed. A final extra read-back attempt was
blocked by the Figma MCP seat rate limit; the edits after that read-back touched no
reaction-bearing nodes — only overlay panels, 4 haptic-ring ellipses and caption texts were
removed/moved — so the counts stand as read.)
**Format:** desktop 1440 × 1024 per frame, premium dark launch-stage storefront
(deep black-blue, white hardware). Disclaimer in the footer of every screen:
"Concept experience — not affiliated with Sony Interactive Entertainment."

## Process — "PS5 Launch Day"
Home (Launch Reveal) → Choose Your Console → PS5 Product (turntable + DualSense FEEL) →
Build Your Launch Library (pick 3) → Gear Up → Trade In Your PS4 → Delivery or Pickup →
Review & Pay → Confirmed + Install Queue. Order number: **PS5-2481**.

## Carried build — identical on Library summary, Gear summary, Review, Confirmed, Pay label
| Item | Price |
|---|---|
| PlayStation 5 Console — Disc Edition (1TB) | $649.99 |
| Marvel's Spider-Man 2 (PS5) | $69.99 |
| Astro Bot (PS5) | $59.99 |
| Helldivers 2 (PS5) | $39.99 |
| DualSense Wireless Controller — White (extra) | $74.00 |
| DualSense Charging Station | $29.00 |
| **Merchandise subtotal** | **$922.96** |
| Trade-in credit — PlayStation 4 (concept valuation) | −$100.00 |
| Tax (8%) | $65.84 |
| **TOTAL** | **$888.80** |

Arithmetic, verified twice:
- Games: 69.99 + 59.99 + 39.99 = 169.97. Gear: 74.00 + 29.00 = 103.00.
- Subtotal: 649.99 + 169.97 + 103.00 = **922.96** ✓
- After trade-in: 922.96 − 100.00 = 822.96. Tax: 822.96 × 0.08 = 65.8368 → **$65.84** ✓
- Total: 822.96 + 65.84 = **$888.80** ✓ — Pay label reads "Pay $888.80"; Confirmed reads "Paid $888.80".
- Running bag totals shown in nav: Editions/Product $649.99 → Library $819.96 (649.99+169.97) →
  Gear $922.96 → Trade/Delivery $822.96 → Review $888.80.

## Price sources (checked 2026-10-15/16)
- PS5 Disc **$649.99** / PS5 Digital **$599.99** / PS5 Pro $899.99 — PlayStation.Blog "New Price
  Changes for PS5, PS5 Pro, and PlayStation Portal" (effective April 2, 2026, current US RRP);
  corroborated by Target's current listings ($649.99 / $599.99).
- DualSense (White) **$74.00**, DualSense Charging Station **$29.00**, DualSense Edge **$199.00**,
  PULSE Elite **$149.00** — PlayStation Direct US (direct.playstation.com, current listings;
  retailers show .99 equivalents, e.g. Edge $199.99, PULSE Elite $149.99).
- Games: Spider-Man 2 **$69.99** (PlayStation Store base price), Astro Bot **$59.99**,
  Helldivers 2 **$39.99** (PlayStation.com product data: 39.99 USD), God of War Ragnarök $69.99,
  Gran Turismo 7 $69.99.
- WD_BLACK SN850X shown as "from $269.99" (1TB heatsink SKU, Best Buy listing, May–Oct 2026);
  the SSD is a browse/detail item only and is NOT in the carried total (2026 SSD prices are volatile).
- PS4 trade-in −$100.00 is a labeled **concept valuation** (retailer values vary by condition);
  the screen and footer both say so.

## Grid / non-carried items and prices
Editions: PS5 Pro $899.99 · DualSense Edge $199.00 · PULSE Elite $149.00 · Games from $39.99.
Bundles strip: Console + Spider-Man 2 $719.98 · Console + DualSense Edge $849.98.
Gear: PULSE Elite $149.00 (not added) · WD_BLACK SN850X from $269.99 (not added).
Library bench: God of War Ragnarök $69.99 · Gran Turismo 7 $69.99 (unselected).

## Frames (27) and node ids — V3 "Boot & Light States" names
Home / Hero Boot: P01 `2:107` Boot 1 — STANDBY · P02 `2:72` Boot 2 — POWER PRESS / LED CHASE ·
P03 `2:37` Boot 3 — BOOT / STRIP FULL WHITE · P04 `2:2` Boot 4 — READY / PLAYER BLUE
Editions Light Check: P05 `3:2` Disc / White Light · P06 `3:59` Digital / Blue Light
Console Light Tour: P07 `3:116` FRONT / STRIP FULL · P08 `3:157` ANGLE / STRIP CHASE ·
P09 `3:198` REAR / PORTS LIT · P10 `3:239` ON YOUR SHELF / AMBIENT
DualSense Light Bar: P11 `3:280` PLAYER BLUE · P12 `3:319` PULSE WAVE · P13 `3:361` TRIGGER GLOW
Library Light Match: P14 `4:2` Spider-Man 2 / Red · P15 `4:61` Astro Bot / Cyan ·
P16 `4:120` Helldivers 2 / Orange
Gear Charge Gauge: P17 `5:2` 24% · P18 `5:73` 68% · P19 `5:146` 100% READY
Trade-In Light Transfer: P20 `5:346` 0% · P21 `5:381` 50% · P22 `5:416` 100% / Credit In
P23 `5:451` Delivery or Pickup (Delivery Light panel) · P24 `5:484` Review & Pay (All Lights Green panel)
Confirmed Install Light-Fill: P25 `5:546` Igniting · P26 `5:584` Filling · P27 `5:623` ALL READY

## Motion design — V3 "BOOT & LIGHT STATES" (current, built 2026-10-16)
**SUPERSEDED:** the V2 "Launch Reveal" system (Lights Down → First Light → Push In hero,
turntable, FEEL haptic rings, dock photo states, trade-in dim chain, install chain). Its hero
shade/sweep overlays and pose captions were removed, its 4 haptic-ring ellipses on the FEEL
pulse frame were deleted, and every pose frame was renamed and reworked into the system below.
No old chain remains: the prototype wiring (destinations, AFTER_TIMEOUT + click-advance,
NODE/DISSOLVE) is unchanged in shape, but every pose now reads as a light state, not a reveal.

**The language:** the console and controller live by their lights. The hardware never moves —
every frame carries a "BOOT & LIGHT STATES" readout panel (full-width on most screens, a slim
strip on Editions and Library where the bottom summary bar owns the space) with an 8-segment
LED strip that lights segment by segment, a big state line, and a readout. All pieces are
self-contained in their own frame, self-playing (AFTER_TIMEOUT) and click-advanceable; screens
connect by plain NODE/DISSOLVE navigation only. Balance: the HERO boot carries the launch
excitement; the wider flow's pieces explain the product through its lights.

**The pieces:**
- **Hero Boot Sequence (P01–P04):** STANDBY (amber glow only, 1/8 segments) → POWER PRESS
  (LED strip chase, 4/8 white) → BOOT (strip full white, 8/8, light bar answering) → READY
  (player blue, 8/8, store live). No camera push-in — the light tells the story in place.
- **Edition Light Check (P05–P06):** Disc answers in white light, Digital in blue; slim strip
  in the left column so the build bar and launch grid stay fully readable.
- **Console Light Tour (P07–P10):** the same four real photographs, re-read as light states —
  FRONT strip full · ANGLE chase runs the fin · REAR every port lit · ON YOUR SHELF ambient blue.
- **DualSense Light Bar (P11–P13):** PLAYER BLUE steady → PULSE WAVE rolls across → TRIGGER
  GLOW with L2/R2 lit — on the same real controller photo; the old haptic rings are gone.
- **Library — The Light Bar Matches the Game (P14–P16):** a slim light strip under the gameplay
  panel takes each anchor game's colour — Spider-Man red, Astro cyan, Helldivers orange —
  with a MATCH readout, cycling in place with the selection states.
- **Gear — Charge Gauge (P17–P19):** the gauge fills 24% → 68% → 100% READY with a big
  percentage readout, panel seated between the dock/SSD boxes and the summary bar.
- **Trade-In — Light Transfer (P20–P22):** the PS4's light moves over to the PS5 — 0% (PS4
  still lit) → 50% (half moved) → 100% (light out, −$100.00 credit in). Replaces the dim chain.
- **Delivery Light (P23) / All Lights Green (P24):** single-state readouts — route light in
  transit; at Review every segment green, "PAY $888.80".
- **Confirmed — Install Light-Fill (P25–P27):** each game's cover card gets a light bar in its
  own colour (red/cyan/orange) that fills across poses — Igniting (Spider-Man started) →
  Filling (Spider-Man READY, Astro 50%, Helldivers started) → ALL READY · PLAY.

### The 12 tour captions (V3)
1. **Standby** — launch day, powered down: one amber segment glows and the whole store holds its breath.
2. **Power Press** — a thumb on the power button and the LED strip chases alight, segment by segment.
3. **Boot** — the strip hits full white and the DualSense light bar answers from the dock.
4. **Ready** — player blue. Booted, signed in, store live — the light says go.
5. **Edition Light Check** — Disc answers in white, Digital in blue; the drive is the only difference and the light knows it.
6. **Console Light Tour** — front, angle, rear, shelf: four real photographs, four light states, zero camera tricks.
7. **Light Bar · Player Blue** — the DualSense sits steady in player blue, the colour of player one.
8. **Light Bar · Pulse Wave** — a pulse rolls the length of the bar; the controller feels alive in place.
9. **Light Bar · Trigger Glow** — L2 and R2 light up as the read shifts to the adaptive triggers.
10. **The Light Bar Matches the Game** — Spider-Man red, Astro cyan, Helldivers orange: pick a game and the bar wears its colours.
11. **Charge Gauge** — 24, 68, 100: the dock reports charge as a filling light gauge, ending in a steady READY.
12. **Light Transfer → Install Light-Fill** — the PS4's light moves over and the credit lands; after Pay $888.80, three light bars fill game by game to ALL READY.

### V3 proof screenshots (`~/workspace/product-design-concepts/ps5/shots/`, all byte-verified non-empty)
`v3_boot1_standby.png` (248,965 B) · `v3_boot2_chase.png` (300,736 B) · `v3_boot3_boot.png`
(361,895 B) · `v3_boot4_ready.png` (304,729 B) · `v3_editions_disc.png` (372,492 B) ·
`v3_editions_digital.png` (325,140 B) · `v3_lighttour_rear.png` (339,686 B) ·
`v3_lightbar_pulse.png` (750,757 B) · `v3_library_red.png` (612,479 B) · `v3_library_cyan.png`
(547,319 B) · `v3_library_orange.png` (552,536 B) · `v3_gear_24.png` (211,648 B) ·
`v3_gear_68.png` (307,378 B) · `v3_gear_100.png` (308,663 B) · `v3_trade_50.png` (333,876 B) ·
`v3_install1.png` (165,624 B) · `v3_install_ready.png` (162,357 B) · `v3_review_green.png`
(134,183 B). Visually inspected: all four hero frames, Editions, Light Tour rear, Light Bar
pulse (rings confirmed gone), Library red, Gear 68%, Trade 50%, Review, Install READY —
panels cover no prices, totals, or CTAs on any inspected frame.

## Image-source map (every image visually verified by contact sheet before use)
Verification method: all candidates were downloaded, assembled into contact sheets, and
eyeballed against their labels; anything that did not read as the real product was dropped
(e.g. a PS4 "KEEP CALM" poster, blue-plate console shots). In-Figma screenshots of the hero,
editions, product, FEEL, library, gear, trade-in, delivery, review and confirmed screens were
inspected again after the build.

| Use | Real product shown | Source |
|---|---|---|
| Hero + Product FRONT + Review/Confirmed thumb | PS5 (disc) + DualSense on dock, transparent bg | Wikimedia Commons — "PlayStation 5 and DualSense with transparent background.png" |
| Product ANGLE + Editions Disc preview + Delivery pickup | PS5 three-quarter | Wikimedia Commons — "Black and white Playstation 5 base edition with controller.png" |
| Product REAR | PS5 rear three-quarter | Wikimedia Commons — "Playstation 5.jpg" |
| Product ON YOUR SHELF | PS5 + DualSense in a living room | Wikimedia Commons — "PlayStation 5 and DualSense (2).jpg" |
| Editions Digital preview | PS5 Digital Edition + DualSense | Wikimedia Commons — "PS5DigitalEdition.png" |
| Gear charge poses (docked state) | PS5 on DualSense charging dock, 2 controllers | Wikimedia Commons — "PlayStation 5 and DualSense (cropped).jpg" |
| FEEL piece (all 3 poses) | DualSense (White), front | Wikimedia Commons — "KontrolerDualSense.jpg" |
| Gear tile / Review thumb | DualSense (White), angled | Wikimedia Commons — "Playstation DualSense Controller.png" |
| Editions grid | DualSense Edge | Wikimedia Commons — "DualSense Edge Controller.jpg" |
| Charging Station (empty dock) | DualSense Charging Station | PlayStation Direct CDN (media.direct.playstation.com) |
| Delivery lifestyle | Living room with PS5 + TV | PlayStation Direct CDN |
| PULSE Elite | PULSE Elite headset | PlayStation Direct CDN |
| (asset, unused in final frames) | Hands holding DualSense; DualSense Chroma Pearl / Cobalt Blue; DualSense macro detail | PlayStation Direct CDN / Wikimedia Commons |
| Trade-In (all 3 poses) | PlayStation 4 + DualShock 4 | Wikimedia Commons — "Sony-PlayStation-4-PS4-wDualShock-4.jpg" |
| SSD tile + detail piece | WD_BLACK SN850X (front) | Wikimedia Commons — "Western Digital SN850X NVME solid state drive 8TB front side.jpg" |
| Game covers ×5 | Spider-Man 2, Astro Bot, Helldivers 2, God of War Ragnarök, Gran Turismo 7 key art | Wikipedia (en) article cover-art files |
| IN GAME panels ×3 | Real gameplay stills: Spider-Man 2, Astro Bot, Helldivers 2 | Wikipedia (en) gameplay screenshot files |

Local copies: `~/workspace/product-design-concepts/ps5/assets/` · Proof screenshots (all 27 frames):
`~/workspace/product-design-concepts/ps5/shots/`

## V3 caveats (plain)
- **Panel placement varies by layout:** full-width readout panels on Hero, Product, FEEL, Gear,
  Trade, Delivery, Review and Confirmed; slim light strips on Editions (left column) and
  Library (under the gameplay panel) because those screens' bottom summary bars and grids own
  the full-width space — no frozen content is covered on any visually inspected frame.
- **Base-screen copy still names some old piece labels** in a few body lines (e.g. the FEEL
  right-rail tabs "Haptic Feedback / Adaptive Triggers", the Trade-In sub-line "powers down in
  place", the Gear "THE DOCK, LIVE" heading): screen content is frozen per the brief, so only
  motion captions, chips, frame names and overlays were reworked.
- **Final read-back:** the last successful full read-back (27 frames / 78 reactions / flow
  `2:107`) was taken right after the V3 panels were wired; one further read-back attempt hit
  the Figma MCP Full-seat rate limit. Post-read-back edits removed/moved only overlay, ellipse
  and caption nodes — no reaction-bearing node was touched. Present-mode click-through by
  Nithin remains the final proof, as always.

## Caveats (plain)
- **Digital Edition note:** the Editions preview crossfades Disc ↔ Digital, but the carried build
  stays Disc (both poses' Continue leads to the Disc product build); the screen states this in copy.
- **SSD photo:** the real SN850X photograph shows the 8TB unit; the tile sells the 1TB/2TB heatsink
  SKUs ("from $269.99"). The drive shown is the non-heatsink front — the heatsink claim is a callout,
  and no insertion animation was faked, per the brief.
- **Gameplay stills are low-resolution** (421×237 Wikipedia files) shown inside the IN GAME panel;
  they are real gameplay frames but will look soft at full size.
- **Charging sequence:** empty dock is Sony's official product shot; the docked states use a real
  photo of controllers on the dock (with the console) plus UI state dots — there is no official
  frame-by-frame charge sequence, so states are photo + UI, as the brief allowed.
- **Library IN GAME panel** cycles gameplay from all three selected games (one real still each),
  not multiple stills from a single game.
- **Trade-in credit** is a concept valuation (−$100), labeled as such on screen and in the footer.
- **Hero lighting poses** share one real photograph; the lighting change is done with in-frame
  shade overlays, a light sweep and the glowing LED/light-bar elements, plus a crop push-in —
  the product never leaves its frame.
- **Screenshot-export artifact:** the MCP screenshot exports intermittently ghost the Home stat
  chips into other frames' exports; frame metadata and text probes confirm the frames themselves
  are clean. Present-mode click-through by Nithin remains the final test, as always.
