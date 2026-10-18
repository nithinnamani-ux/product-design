# Skylark — Drone Commerce UX (Concept)

Fictional brand "Skylark", a DJI-style drone store. Built 2026-10-15 with plain `use_figma` canvas scripting only — zero Figma AI. **Motion system rebuilt fresh 2026-10-16 ("WIND & AIR"):** the previous motion system (FIRST TAKEOFF hero, SPIN-UP, GIMBAL + LIVE FEED, ROUTE DRAW, IDLE + PLAN) is SUPERSEDED and removed — its pose frames were deleted or reworked so no old chain remains reachable in the prototype. The new system is built on one language: the drone fights, rides, and reads the air. Process, products, photos, prices and totals are unchanged from the original build; the turntable remains as a content viewer.

- **Figma file:** https://www.figma.com/design/9VixyGJ1BmZYZOttuFwamY
- **fileKey:** `9VixyGJ1BmZYZOttuFwamY`
- **Flow start:** node `2:8` (D01 Home · Hold Pose 1 — Calm Air, Holding), flow name "Skylark — Fly Before You Buy" — re-verified after the rebuild as the page's only flowStartingPoint
- **Format:** desktop-only, 1440 × 1024 frames, page "Desktop Flow"
- **Counts (read back after the rebuild):** 24 frames · 51 reactions (every action type NODE with navigation NAVIGATE, DISSOLVE 0.35s; pose chains on AFTER_TIMEOUT 1.5–1.8s and also click-advanceable; zero dangling destinations)

## Motion doctrine (the point of this concept)

NO INTERCONNECTING. Nothing morphs, transforms, assembles, folds, flies or carries from one item into the next or from screen to screen. All motion is SELF-CONTAINED inside its own screen/frame — the product presents itself in place, inside its own image frame — and screens connect by plain dissolve navigation only. Every pose is a complete readable screen; pose sets live within their own screen and chain by AFTER_TIMEOUT, and are also click-advanceable.

**Balance rule for this design:** the HERO carries the excitement animation (Hold Position against the gusts); the rest of the flow carries purposeful motion design that explains the air (airspeed, obstacle sensing, altitude profile, return-to-home).

## Process — "Fly Before You Buy"

Home → Shop by Mission (Film / Travel / Racing / Inspection) → Compare Flight Specs → Product (in-frame turntable + airspeed ladder + obstacle sense) → Flight Kit → Delivery & Fly-Safe Check (altitude profile) → Review & Pay → Confirmed + First-Flight Plan (return to home). No quiz, no login/verification.

## Frames (node ids)

| Node | Frame |
|---|---|
| 2:8 | D01 Home · Hold Pose 1 — Calm Air, Holding |
| 22:2 | D01 Home · Hold Pose 2 — Gust Front, Leaning In |
| 22:57 | D01 Home · Hold Pose 3 — Gust Peak, Drift Corrected |
| 22:112 | D01 Home · Hold Pose 4 — Holding, Rock Steady |
| 2:170 | D02 Shop by Mission + line-up grid |
| 2:270 | D03 Compare Flight Specs |
| 2:362 | D04 Product · Turntable Pose 1 — Front 0° |
| 2:439 | D04 Product · Turntable Pose 2 — Side 90° |
| 2:516 | D04 Product · Turntable Pose 3 — Top, plan view |
| 2:593 | D04 Product · Turntable Pose 4 — Gimbal tilt, camera down 45° |
| 23:2 | D04 Product · Airspeed Pose 1 — Hover, 0 KM/H |
| 23:79 | D04 Product · Airspeed Pose 2 — Cruise, 36 KM/H |
| 23:156 | D04 Product · Airspeed Pose 3 — Sport, 68 KM/H |
| 23:261 | D04 Product · Sense Pose 1 — Scanning |
| 23:338 | D04 Product · Sense Pose 2 — Obstacle Detected |
| 23:415 | D04 Product · Sense Pose 3 — Avoided, Course Held |
| 2:670 | D05 Flight Kit |
| 2:768 | D06 Delivery & Fly-Safe · Altitude Pose 1 — Climb |
| 23:520 | D06 Delivery & Fly-Safe · Altitude Pose 2 — Cruise 60 M |
| 23:614 | D06 Delivery & Fly-Safe · Altitude Pose 3 — Descent & Land |
| 2:848 | D07 Review & Pay |
| 2:918 | D08 Confirmed · RTH Pose 1 — Return Engaged |
| 23:743 | D08 Confirmed · RTH Pose 2 — 180 M Out |
| 23:814 | D08 Confirmed · RTH Pose 3 — Landed, Home Safe |

## Motion map (piece by piece) — "WIND & AIR" system

1. **HOLD POSITION (Home, hero — the excitement piece).** One hero frame, four poses chained by AFTER_TIMEOUT (1.6s) and status-pill clicks; the Mission/Compare CTAs are live on every pose. The Air Pro never takes off — it holds its hover against the weather inside the hero frame. Pose 1: level photo, faint wind streaks, pill "● HOLD POSITION — CALM AIR", telemetry "WIND 12 KM/H · HOLDING POSITION". Pose 2: the photo leans −3° into the gust (photo enlarged 1.3× inside a clipping frame so the lean never spills), streaks build, pill "● GUST FRONT — LEANING INTO THE WIND", telemetry "WIND 21 KM/H · LEANING IN". Pose 3: lean deepens to −5°, eight thick streaks stream past, pill "● GUST PEAK — CORRECTING DRIFT", telemetry "GUST 24 KM/H · DRIFT CORRECTED". Pose 4: level again, streaks fade to a calm three, pill "● HOLDING · ROCK STEADY", telemetry "WIND 12 KM/H · HOLDING · ROCK STEADY". All drawn elements are interface/state elements (wind streaks, telemetry) over the unchanged photo.
2. **TURNTABLE (Product, kept from the original build as a content viewer).** Four photos of the same drone in one viewer frame (front / side / top / gimbal tilt); the dot under the viewer advances the cycle. The last turntable dot now continues into the Airspeed Ladder instead of looping.
3. **AIRSPEED LADDER (Product, new).** In the same viewer, over the fixed front photo, the air itself speeds up across three poses: wind streaks build from two faint lines (HOVER) to six (CRUISE) to nine long fast streaks (SPORT); the viewer chip and a readout pill step "AIRSPEED · 0 KM/H" → "36 KM/H" → "68 KM/H" while a meter bar under the viewer fills (empty → half → full). Poses chain by AFTER_TIMEOUT (1.5s), the readout pill, and the viewer dot; the last pose continues into Obstacle Sense.
4. **OBSTACLE SENSE (Product, new).** Over the viewer's high-angle photo, drawn sensor rings pulse outward from the drone across three poses: one ring ("● SCANNING") → two rings as a red obstacle marker + label appears front-left ("OBSTACLE · 4.2 M AHEAD") → three rings with the marker and label turned teal ("✓ AVOIDED · COURSE HELD"). Chains by AFTER_TIMEOUT (1.6s), the viewer dot, and the obstacle label; the final pose's dot/label returns to Turntable Pose 1.
5. **ALTITUDE PROFILE (Fly-Safe, new — replaces Route Draw in the same card).** The card beside the order summary is now a chart card ("FIRST-FLIGHT ALTITUDE PROFILE · SAT 9:00 AM"): a profile line draws itself across the chart in three poses — climb only (chip "● CLIMB — TAKEOFF TO 60 M") → climb + cruise plateau under a dashed 60 M ceiling line (chip "● CRUISE — HOLDING 60 M") → the full profile with descent (chip "✓ PROFILE SET — DESCENT & LANDING PLANNED"); stage labels TAKEOFF / CRUISE 60 M / DESCENT / LAND light up as the line reaches them. Poses chain by AFTER_TIMEOUT (1.6s); the Continue button advances the piece and, on the final pose, goes to Review & Pay.
6. **RETURN TO HOME (Confirmed, new).** Inside a dark map card overlaid on the Confirmed photo, a drone dot rides a dashed route toward the HOME marker across three poses while the readout counts down: "RETURN TO HOME · 420 M TO GO · BATT 78%" → "180 M TO GO · BATT 74%" → "LANDED · HOME SAFE · BATT 71%"; the photo's status pill steps "● RETURN TO HOME — ENGAGED" → "● RETURNING — 180 M OUT" → "● LANDED — HOME SAFE". The movement lives inside the map card only. Chains by AFTER_TIMEOUT (1.8s) and pill click.
7. **Still screens (by design):** Shop by Mission, Compare Flight Specs (the carried Air Pro row keeps its selected state), Flight Kit tiles, Review & Pay — plain dissolve navigation only.

**Superseded system (removed 2026-10-16, do not restore):** FIRST TAKEOFF hero (frames 2:62, 2:116, 13:2 — deleted; 2:8 reworked into Hold Pose 1), SPIN-UP (14:2, 14:79, 14:156 — deleted), GIMBAL + LIVE FEED (14:233, 14:310 — deleted), ROUTE DRAW (14:441, 14:535 — deleted; 2:768's map card reworked into the Altitude Profile chart card), IDLE + PLAN (14:649 — deleted; 2:918 reworked into RTH Pose 1). No takeoff/liftoff, rotor spin-up readouts, gimbal pitch, route drawing, or idle blur remain anywhere in the prototype.

## Carried product & totals (identical on Kit, Review, Confirmed and the Pay label)

- Skylark Air Pro — **$999.00**
- Extra Flight Batteries × 2 @ $99.00 — **$198.00** (Flight Kit)
- Skylark Care Refresh — **$99.00** (Flight Kit)
- Subtotal **$1,296.00** · Tax (8%) **$103.68** · **TOTAL $1,399.68**
- Pay button label: "Pay $1,399.68". Arithmetic checked twice: 999 + 198 + 99 = 1,296; 1,296 × 0.08 = 103.68; 1,296 + 103.68 = 1,399.68.
- Also shown on the Kit screen but NOT added (totals unaffected): ND Filter Set $79.00, Spare Propellers $19.00. Express delivery $24.00 shown on Fly-Safe as not selected.
- Delivery: Fri, Oct 23, 2026 (standard, free). First flight in the plan: Sat, Oct 24, 2026, 9:00 AM.

## Grid (D02 line-up)

| Product | Price | Photo |
|---|---|---|
| Skylark Air Pro (carried) | $999 | forest hover, front |
| Skylark Mini | $449 | compact folding close-up |
| Skylark Cine | $1,899 | large pro rig on the ground |
| Skylark Racer X | $749 | grey sport close-up |
| Skylark Inspect | $2,499 | field front view |
| Fly More Kits tile | from $19 | sunset field lifestyle |

## Images — sources & verification

All photos are free stock (Unsplash/Pexels), downloaded locally to `img/` and visually verified by the builder from contact sheets (`contact1–3.jpg`) before placement; Figma fills were set from the uploaded assets by hash. Every product photo is a generic white/grey quadcopter with **no legible third-party brand logo**. Rejected during screening: a front shot with "MAVIC MINI" legible on the arm (third-party branding), plus non-drone results. Sources: Unsplash photo IDs 1473968512647 (Air Pro hero), 1507582020474 (Inspection mission), 1487887235947 (gimbal close-up), 1508614589041 (Mini), 1508444845599 (Travel mission), 1521405924368 (Inspect grid); Pexels photo IDs 1034812 (side view), 744366 (Cine), 442589 (Fly More tile), 724921 (Racer X), 343238 (front view). Accessory tiles on the Kit screen (battery with in-place charge bars, ND filters, propellers, Care Refresh) are drawn vector elements by design — the charge state is the motion, so it is drawn, not photographed. The same applies to the WIND & AIR system's drawn UI elements: wind-streak lines, telemetry/readout pills, the airspeed meter, sensor rings and obstacle markers, the altitude chart (profile line, ceiling line, stage labels), and the RTH map card — all interface/state elements drawn over or beside the unchanged photos.

## Motion Design tour captions (for the UX Lab page tour) — WIND & AIR, written fresh for this system

1. HOLD POSITION · 1 — Calm air. The Air Pro hovers level inside the hero frame; its telemetry reads WIND 12 KM/H · HOLDING POSITION.
2. HOLD POSITION · 2 — A gust front arrives: wind streaks stream past the photo and the Air Pro leans into the wind — still holding its spot.
3. HOLD POSITION · 3 — Gust peak, 24 KM/H. The lean deepens, the streaks thicken, the telemetry answers: DRIFT CORRECTED.
4. HOLD POSITION · 4 — The air settles and the Air Pro sits rock-steady again. The hero never took off — holding position was the show.
5. Shop by Mission: every drone rests in its own card at its own state; moving between them is plain navigation — nothing carries over.
6. Compare Flight Specs: three spec sheets side by side, each drone pictured in its own frame. The specs do the persuading; the carried Air Pro row stays selected.
7. TURNTABLE — The product viewer turns the Air Pro inside its frame: front, side, top, then the gimbal-tilt view. One tap per dot.
8. AIRSPEED LADDER — In the same viewer the air itself speeds up around the fixed photo: the readout steps 0 → 36 → 68 KM/H, the meter fills, and the wind streaks build to SPORT.
9. OBSTACLE SENSE — Sensor rings pulse out from the Air Pro; an obstacle marker appears front-left at 4.2 M, gets sensed, and turns teal — AVOIDED · COURSE HELD, all in place.
10. Flight Kit: every accessory presents itself in its own tile — the battery tile fills its own charge bars to 100% in place.
11. ALTITUDE PROFILE — On the Fly-Safe screen the first flight's climb draws itself across the chart card: TAKEOFF → CRUISE 60 M → DESCENT → LAND — the profile is set before you pay.
12. RETURN TO HOME — Confirmed: inside the map card on the photo, the Air Pro's dot rides the dashed route home — 420 M → 180 M → LANDED · HOME SAFE — while the battery readout ticks down.

## Proof screenshots (this folder)

New for the WIND & AIR rebuild (exported 2026-10-16, byte sizes verified on disk — all real 1440×1024 PNGs, none empty):
pose-hold-1.png (786,123 B) · pose-hold-2.png (778,913 B) · pose-hold-3.png (780,869 B) · pose-hold-4.png (715,255 B) · pose-airspeed-1.png (686,641 B) · pose-airspeed-2.png (684,147 B) · pose-airspeed-3.png (679,740 B) · pose-sense-1.png (525,740 B) · pose-sense-2.png (526,154 B) · pose-sense-3.png (534,048 B) · pose-altitude-1.png (128,920 B) · pose-altitude-2.png (128,893 B) · pose-altitude-3.png (130,681 B) · pose-rth-1.png (376,990 B) · pose-rth-2.png (377,290 B) · pose-rth-3.png (376,182 B) · refreshed home.png (= pose-hold-1) · product.png (= pose-airspeed-1) · fly-safe.png (= pose-altitude-3) · confirmed.png (= pose-rth-3)

From earlier builds (unchanged frames): missions.png · compare.png · pose-turntable-1.png · pose-turntable-2.png · pose-turntable-3.png · pose-turntable-4-gimbal.png · kit.png · review.png. Superseded-system exports kept on disk for history only: pose-takeoff-1/2/3/4.png · pose-spinup-1/2/3.png · pose-gimbal-1/2.png · pose-route-1/2/3.png · pose-idle-1/2.png · pose-hover-1/2/3.png — the frames they show no longer exist in the prototype.

The builder visually inspected the full Hold Position sequence (poses 1–4), Airspeed poses 2 and 3, Obstacle Sense pose 2, Altitude Profile pose 3, and RTH poses 1 and 3 from these exports; two inspection fixes were applied and re-exported (hero lean rebuilt on a clipping frame after imageTransform rotation left white corners; airspeed meter moved off the viewer's caption text).

## Caveats

- All prices, specs, ratings, dates, the FAA registration string and the order number are assigned concept figures.
- The turntable's "Top" pose uses the highest-angle logo-free photo available among the free sources screened (a high front three-quarter view), not a true 90° overhead shot — no logo-free true top-down product photo was found.
- The hero lean in Hold Poses 2–3 is conveyed by the real photo enlarged 1.3× and rotated (−3° / −5°) inside a clipping frame matched to the hero photo's rect and corner radius, plus the drawn wind streaks, status pills, and telemetry readouts; the underlying photo is a real airborne shot in all four poses. (An earlier pass used imageTransform rotation on the fill, which sheared the image and left white corners; the clipping-frame build replaced it and was re-verified from exports.)
- The RTH map card and the altitude chart are drawn interface elements (streets, route dash, profile line, ceiling line), not real map or flight data; the RTH dashed route renders slightly high inside its card — a minor cosmetic, the dot/readout carry the state.
- The hero body copy ("The Air Pro lifts off right here… Watch it hover — then decide.") is frozen screen content from the original build and was not rewritten for the new system; it still reads correctly for a hover-hold hero.
- Present-mode feel is unverified until Nithin's real click-through — pose chains ride on AFTER_TIMEOUT firing, though every pose is a complete readable screen and each set is click-advanceable if a timeout stalls.
- Minor cosmetics: the step-bar connector lines sit tight against the longer step labels (pre-existing).
