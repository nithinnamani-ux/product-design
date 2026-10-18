# Lumen M6 — Commerce UX Concept (Figma)

A desktop commerce flow for a fictional rangefinder camera brand, built to the same standard as the Nike showcase: real product photography instead of drawn hardware, its own buying process (**Shoot → See → Configure → Commit**), and motion designed around how a mechanical camera actually behaves — a focal-plane shutter firing, a shutter-speed ladder, an exposure dial, ND glass, a long exposure, and a frame coming up in the developing tray.

- **Design file:** https://www.figma.com/design/AqCWo1Hy22Wxl6avyZ8u0X
- **Prototype:** https://www.figma.com/proto/AqCWo1Hy22Wxl6avyZ8u0X?node-id=1-63&scaling=scale-down-width
- **Flow starting point:** C01 Home (node 1:63), flow name "Camera — Build Your Kit"
- **Status:** V3 system "Shutter & Exposure" — COMPLETE in Figma (2026-10-17). It supersedes the "Living Camera" pass (2026-10-16) and the original build's Rangefinder Hunt system: every roll-counter node from that generation was removed in the supersede cleanup. The UX Lab Product Design panel still shows the previous version until the page pass runs.
- **Figma AI used:** none. Every photograph is a real Unsplash/Pexels photograph; the speed/exposure/ND/long-exposure variants are disclosed derivations of those photographs (blur, sharpening, exposure and density grades), never generated imagery.
- **Final read-back (2026-10-17, post-build):** 33 frames, 184 reactions, flow start node 1:63 ("Camera — Build Your Kit"), zero roll-counter nodes, zero filmstrip nodes, no stray top-level nodes.

## The buying process (Shoot → See → Configure → Commit)

1. **Home — The Shutter Moment (C01–C04).** One product (the Lumen M6) and one promise — "Light, let in slowly." The hero fires the camera's own shutter across four poses (curtain closed → first curtain → fully open → captured) and lands on the roll's last frame. Proof points under the hero: 33MP full-frame BSI sensor, coupled rangefinder, mechanical focal-plane shutter, from $2,499.
2. **Explore by Shooting Style (C05) → Shot on Lumen (C06–C09).** Four real photographs (Street, Portrait, Landscape, Night), each with its EXIF line and the reason the M6's bright-line frame suits it. The Night frame carries the Long Exposure piece (below).
3. **Camera Bodies — Gallery (C10).** The bodies gallery, M6 first ($2,499).
4. **Product — Lumen M6, the M6 Viewer (C11–C13M2, C13N1–N3).** One product page, three light instruments around a single hub (full motion map below). Price panel: $2,499 body, kit core M6 + 35mm f/1.4 $799. Buttons on every pose frame: Build your kit → Kit Builder; Trade-in → Trade-In page.
5. **Kit Builder (C17) with Field of View piece (C17F1–F3).** Body, lens, card, strap, protection — the kit builds to $3,735.00. The FoV piece shows 28 / 35 / 50mm framings of one street photograph behind a red hint entry.
6. **Trade-In / Rental Trial (C18).** A $450 trade-in credit (or a 14-day rental trial) — the credit is what the Review maths applies.
7. **Review, Financing & Pay (C19).** $3,735.00 − $450.00 trade-in = $3,285.00 · + $262.80 tax (8%) = **$3,547.80**, or $295.65/mo × 12, no interest, no fees.
8. **Confirmed — The Develop (C20–C22) with the First Print piece (C22P1–P2).** Order **LM-2481**; the exposed frame develops across three poses until frame 14 stands revealed on the contact sheet — then the First Print piece takes it into the tray and out again as a bordered print.

## File map — 33 frames, 1440 wide, one page ("Page 1")

**Row 1 (y=200)** — C01 Home · Shutter Moment Pose 1 — Curtain Closed (1:63, flow start) · C02 Pose 2 — First Curtain (7:109) · C03 Pose 3 — Fully Open (7:143) · C05 Explore (1:87) · C10 Bodies (1:122) · C11 Ladder Pose 1 — 1/15 (1:242) · C12 Ladder Pose 2 — 1/250 (11:42) · C13 M6 Viewer Hub (11:112) · C17 Kit Builder (1:492) · C18 Trade-In (1:601) · C19 Review (1:633) · C20–C22 Develop poses (7:2, 7:46, 1:684)

**Row 2 (y=1560)** — C04 Shutter Moment Pose 4 — Captured (23:12) · C06–C09 gallery (25:2, 25:29, 25:56, 25:83) · C12B Ladder Pose 3 — 1/2000 (31:68) · C12C ExpComp Pose 1 — +2 EV (31:141) · C13M1 ExpComp Pose 2 — 0 EV (33:2) · C13M2 ExpComp Pose 3 — −2 EV (33:75) · C17F1–F3 FoV poses (34:2, 34:85, 34:168)

**Row 3 (y=2920)** — C13N1–N3 ND Filter poses (52:2, 52:80, 52:158) · C09L1–L2 Long Exposure poses (52:246, 52:273) · C22P1–P2 First Print poses (52:309, 52:372)

Full flow wiring: header nav everywhere (logo → Home; Cameras → Bodies; Lenses/Kits → Kit Builder; Trade-In → Trade-In); hero pieces chain by AFTER_TIMEOUT and click; gallery auto-advances C06→C07→C08→C09→C06 at 1.6s and on click; hub entries by precise clicks (viewer inset, dial strip, ND chip); Kit Builder → Review → Confirmed → Home (via C03).

## The V3 motion system — "Shutter & Exposure"

One idea, stated on the hub: **time the light**. Every piece is a real camera control changing one real photograph, in place, inside its own screen — nothing travels between screens, and every chain also advances on click. All transitions DISSOLVE / EASE_OUT / 0.3s.

- **The Shutter Moment (Home hero, 4 poses, 1.3s/1.3s/1.3s/1.6s).** The shutter diagram on the hero fires — curtain closed, first curtain, fully open, captured — the roll counter ticking 12 → 13 → 14 as frame 14 is exposed. The hero's excitement piece: the product demonstrating its own mechanism.
- **Shutter-Speed Ladder (Product, 3 poses, from the hub's viewer inset).** One street photograph at 1/15 (streaked), 1/250 (the untouched original), 1/2000 (frozen) — the exposure dial under the stage tracks the active speed in orange on every pose (readouts: "DIAL · 1/15 · ƒ/2.8 — MOTION STREAKED" etc.).
- **Exposure Compensation (Product, 3 poses, from the hub's dial strip).** The same photograph at +2 EV, 0 EV, −2 EV; the dial's marker and readout (−2 … +2) move with it. The lesson the ladder can't teach: brightness is a choice, not a shutter.
- **ND Filter (Product, 3 poses, from the hub's ND chip — new in the completion pass).** ND2 / ND8 / ND64 glass over the same daylight frame: three disclosed darkened derivations, the filter dial relabelled CLEAR · ND2 · ND8 · ND64, readouts converting the shutter each stop buys (1/250 → 1/125 → 1/30 → 1/4).
- **Long Exposure (Night gallery, 2 poses, from the Night frame's photo or its "HOLD IT OPEN" chip — new).** The Tokyo night frame held open: 8 seconds (trails forming) → 30 seconds (the street paints itself), EXIF chip and counter updating per pose, then back to the gallery frame. Disclosed derivations of the same photograph.
- **Field of View (Kit Builder, 3 poses).** 28 / 35 / 50mm crops of one photograph behind the red hint on the Kit Builder ("COMPARE FIELDS OF VIEW — 28 · 35 · 50 · A FRAME, NOT A FILTER →" — the hint copy now carries the piece's own disclosure line). Each pose states it plainly: "Field of view is a frame, not a filter — choose it before the roll starts."
- **The Develop (Confirmed, 3 poses, 1.0s/0.6s).** The order confirmation develops frame 14: shutter readout → dark exposure frame → the revealed photograph, landing on the contact sheet with all six frames filled.
- **First Print (Confirmed, 2 poses, from the revealed photo or its chip — new).** The revealed frame goes into the tray (the dark variant) and comes out as a bordered print — "● FIRST PRINT — FRAME 14 · YOURS TO KEEP" — the print border drawn as a real white mount around the photograph.

### Completion-pass fixes (2026-10-17, beyond the resume list)

Found by screenshot inspection during the finishing pass and fixed in the same pass:
- **Ladder Pose 2 stage image:** the earlier pass had left the hub's camera-body photograph on the 1/250 pose's stage; it now shows the untouched street photograph its own copy describes (the same original the Exposure Compensation 0 EV pose uses).
- **Dial readout legibility:** the readouts under all nine dial frames (Ladder ×3, Exposure Compensation ×3, ND ×3) rendered in a near-white fill on the white page; darkened to a readable charcoal.
- **Chip widths:** the red stage chips on the Ladder and Exposure Compensation poses wrapped and clipped their labels; widened (300 → 400) so every label sits on one line. The hub's viewer chip was shortened to "THE M6 VIEWER · THREE WAYS" for the same reason.
- **ND dial label colours:** the active stop now carries the orange highlight that matches the dial marker on each ND pose (the clones had inherited the template's 1/250 highlight).

## Motion Design tour (UX Lab panel copy — 12 stops, fresh for V3)

1. **The Shutter Moment** — the hero fires the focal-plane shutter: curtain closed, first curtain, fully open, captured. Four poses, one loop — the camera demonstrating its own mechanism before anything is sold.
2. **The M6 Viewer** — one product page, three light instruments. Click the viewer for the shutter ladder, the dial strip for exposure compensation, the black chip to screw on an ND filter.
3. **Shutter-Speed Ladder · 1/15** — the street streaks. One real photograph at a fifteenth of a second: motion blur you can read.
4. **Shutter-Speed Ladder · 1/250** — the same photograph, untouched. The ladder's middle rung — the moment the way your eye saw it, dial tracked underneath.
5. **Shutter-Speed Ladder · 1/2000** — frozen mid-stride. One disclosed sharpening derivation of the same frame; the streak, stopped.
6. **Exposure Compensation · +2 EV** — the same frame, lifted two stops. Brightness as a choice: the dial rides +2 through 0 to −2 and the photograph never changes hands.
7. **Exposure Compensation · −2 EV** — two stops under, the crossing falls toward silhouette — and the readout under the stage says exactly why.
8. **ND Filter · ND2 → ND64** — glass on the lens. Three disclosed darkened derivations of one daylight frame; every stop of glass buys a slower shutter, 1/250 all the way down to 1/4.
9. **Long Exposure** — click the Night frame and hold it open: 8 seconds of trails, then 30, until the street paints itself. Same photograph, held longer.
10. **Field of View · 28 / 35 / 50** — three framings from one spot on the pavement. A frame, not a filter — every pose says so on its face.
11. **Build Your Kit** — body, lens, card, strap, care: $3,735.00, trade-in −$450, tax $262.80, total $3,547.80 — or $295.65/mo × 12. The numbers never move between screens.
12. **The Develop & First Print** — order LM-2481 develops frame 14 across three poses, then prints it: down into the tray, up again bordered and yours to keep.

## Proof screenshots (this folder)

- `pose-shutter-1..4.png` — the Shutter Moment hero poses (pose-4 = the Captured hub).
- `pose-ladder-1..3.png`, `pose-expcomp-1..3.png` — the two dial pieces (pose-ladder-2 re-shot 2026-10-17 after the stage-image fix).
- `pose-nd-1..3.png`, `pose-hub-nd.png` — the ND Filter poses and the hub with its ND chip (new, 2026-10-17).
- `pose-longexp-1..2.png`, `pose-night-entry.png` — the Long Exposure poses and the Night frame with its entry chip (new, 2026-10-17).
- `pose-print-1..2.png` — the First Print poses (new, 2026-10-17).
- `pose-gallery-clean-1.png` — Street gallery frame after the filmstrip removal (2026-10-17).
- `pose-fov-1..3.png`, `pose-develop-1..3.png` — the Field of View and Develop pieces.
- `home.png`, `explore.png`, `bodies.png`, `product.png`, `kit.png`, `tradein.png`, `review.png`, `confirmed.png` — the main flow at desktop width.
- Older proof files from the Living Camera pass (`pose-roll-*`, `pose-gallery-*`, `pose-hunt-*`) are superseded and may be deleted.

## Source photographs

Real photographs only (Unsplash/Pexels), in `assets/`; derivations are named after the frame they derive from (`photo-street-ladder-15.jpg`, `photo-street-exp-plus2.jpg`, `photo-fov-nd2/nd8/nd64.jpg`, `photo-night-le8/le30.jpg`) and disclosed as derivations in the frame copy or the piece's readout. The M6 body photograph is used consistently for the product everywhere (hero, hub, bodies, kit).

## Numbers (frozen across every pass)

Body $2,499 · 35mm f/1.4 lens $799 · SD card $129 · strap $59 · LumenCare $249 · kit $3,735.00 · trade-in −$450.00 · tax $262.80 (8%) · **total $3,547.80** · financing $295.65/mo × 12 · order **LM-2481**.

## Caveats

- The ND64 stage is a brightness-only derivation — the frame copy describes the light the filter takes and the shutter the dial answers with; it does not claim visible motion streaks in that still.
- The Long Exposure 30-second derivation is deliberately blown out (a real 30 s ƒ/8 exposure of that neon street would be); it reads as light painting, disclosed as a derivation on the piece's frames.
- Present-mode feel of the new chains (ND, Long Exposure, First Print) is verified by wiring read-back and rendered screenshots, not by a human click-through — Nithin's own Present pass is the final check, as with every concept in this series.
- The UX Lab panel still shows the previous "Living Camera" version until the coordinated V3 page pass runs.
