# Intro C6 — Private Pilot Ground School: FAA Written Test Prep (course tracker)

Course spec, status, and checklist. Delivered guide: [index.html](index.html).
Specialization: [../intro.md](../intro.md) · Master plan: [../../PLAN.md](../../PLAN.md).

> **Educational only — not flight instruction.** This is exam-prep familiarization for the FAA Private Pilot Airplane (PAR) knowledge test. It is NOT a substitute for training with a Certificated Flight Instructor (CFI), does not by itself qualify anyone to fly, and regulations/procedures change — always verify against the current FARs/AIM and FAA-approved test prep before a real checkride or flight.

## At a glance
- **Level:** intro (Wings) · **Length:** 10 weeks / 10 lectures
- **Prereq:** none — high-school physics/algebra helpful
- **Software:** SkyVector (free sectional charts), a free E6-B flight-computer app or manual wheel, aviationweather.gov (free METAR/TAF). Setup covered in L1 (Week-1 setup).
- **Grading:** Quiz 30 · Project 30 · Final 30 · Discussion 10
- **Project:** Cross-country flight-plan package — real route on SkyVector, nav log (headings/times/fuel via E6-B), live METAR/TAF go/no-go writeup, personal "Must-Know Tables" reference; due Wk 10
- **Discussions:** weeks 3 / 6 / **10** (C1–C5 use 3/6/9; C6 shifts the third to Week 10 because the hazardous-attitudes content it discusses is taught in L10)
- **Final:** comprehensive, no midterm, **60 questions matching the real FAA knowledge test** — **LIVE** at `exam/final-exam.html`

## Source material
Built from the user-supplied `FAA_Private_Pilot_Written_Study_Guide.md` (conversation notes + proposed 8-module structure), remapped into the Academy's fixed 10-lecture course shape. All 8 modules are represented; Human Factors/ADM (flagged "still to cover" in the source notes) was added as its own lecture.

## Per-lecture status
| Wk | Lecture | Built | Quiz | Notes |
|----|---------|-------|------|-------|
| 1 | Foundations & Test Strategy | ✅ BUILT | ✅ | Test format, ACS mapping, study resources, test-taking strategy; Project: SkyVector/E6-B setup |
| 2 | Regulations — Part 61/91 & Right-of-Way | ✅ BUILT | ✅ | Currency, right-of-way hierarchy, converging/head-on/overtaking/landing diagrams, distress signals |
| 3 | Airspace, Special-Use & ADS-B | ✅ BUILT | ✅ | **Discussion 1** — wedding-cake airspace diagram, VFR minimums table, sectional-chart practice |
| 4 | Aircraft Systems & Instruments | ✅ BUILT | ✅ | Six-pack, pitot-static, ANDS/UNOS deep dive, glass cockpit |
| 5 | Weather Theory | ✅ BUILT | ✅ | Air masses, fronts, clouds, icing, fog, turbulence |
| 6 | Weather Services & Go/No-Go | ✅ BUILT | ✅ | **Discussion 2** — METAR/TAF decode, personal minimums |
| 7 | Aerodynamics & Flight Principles | ✅ BUILT | ✅ | Four forces, lift, AoA/stall, load factor, drag curve, ground effect — **Project checkpoint** |
| 8 | Navigation | ✅ BUILT | ✅ | Sectional symbology, wind triangle, VOR/GPS, lost procedures |
| 9 | Performance & Weight-and-Balance | ✅ BUILT | ✅ | Density altitude, performance charts, CG envelope — **Project checkpoint** |
| 10 | Human Factors/ADM + High-Yield Review + Capstone | ✅ BUILT | ✅ | **Discussion 3** — IMSAFE/PAVE, illusions, full review; **Project due** |

> **Build status:** complete — course page, L1–L10, final exam, and Intro landing card all live. QC pass (SVG render + MCQ re-solve + live fact-check) done 2026-08-07.

## Course-level checklist
- [x] 10 lectures built — **10/10**; titles + topics match the course page syllabus
- [x] Hands-on project defined (cross-country flight-plan package, all-free tools)
- [x] Project milestones include Week-1 tool-setup step
- [x] 3 discussions at wk 3/6/10 with the interactive component (in L3/L6/L10)
- [x] **SVG render + legibility pass** — all figures rasterized and visually inspected; 14 defects fixed in the original 19 (see As-built decisions)
- [x] **Figure expansion (2026-08-08)** — **+30 new diagrams, 19 → 49**, targeting the topics that were still table-or-prose only (see As-built decisions)
- [x] **Independent MCQ re-solve** — all 68 lecture-quiz + 60 exam questions re-solved from FAA sources; 1 wrong answer found and fixed (Va), answer-position balance preserved
- [x] **Live fact-check** of the highest-stakes citations against eCFR/Cornell + the FAA Airman Knowledge Testing Matrix; 1 stale number found and fixed (test allotted time)
- [x] Final exam built — separate page `exam/final-exam.html`, **60 interactive MCQs**, answer distribution verified 15/15/15/15 A–D (matches real FAA test length/pass threshold, not the usual 25)
- [x] Grading applied (30/30/30/10)
- [x] Prereq line on course page
- [x] Course page built (meta · grading bar · syllabus · project · discussions · final)
- [x] Disclaimer line on course page (not flight instruction / not a CFI substitute / verify current regs)
- [x] AI-disclosure footer present
- [x] Linked from Intro landing page

## As-built decisions
- Accent palette **#0ea5e9 / #38bdf8** (sky blue — aviation, distinct from the other five Intro courses).
- Heavy use of inline SVG diagrams per the user's explicit request — right-of-way scenarios, four forces on a wing, airfoil lift, AoA/stall curve, drag-vs-speed curve, wedding-cake airspace, pitot-static system, ANDS/UNOS compass errors, front cross-sections, METAR decode, wind triangle, VOR compass rose, CG envelope, IMSAFE/PAVE.
- Final exam sized to **60 questions / 70% pass** to mirror the real FAA knowledge test, rather than the Academy's usual 25-question default.
- No external school/vendor names used (e.g. "Gleim/King/Sheppard Air" from the source notes generalized to "a commercial test-prep provider").
- Numbers/regulations (14 CFR 61/91, 91.113 right-of-way order, 91.215 transponder, VFR minimums table) cross-checked against current knowledge as of 2026; flagged in-content to verify against the current FAR/AIM before a real checkride, since regulations are amended periodically.
- **QC pass (2026-08-07) — SVG render + visual inspection.** All 19 inline figures rasterized and inspected. Note: `academy/tools/render-figures.js` could not run (Node is not installed on this machine); figures were extracted with a Python script and rasterized via macOS `qlmanage` (Quick Look → WebKit), which renders SVG faithfully for geometry/clipping purposes but substitutes a serif fallback font. **14 defects found and fixed:**
  - *L02 fig2 (right-of-way panels)* — `<defs>` block sat **outside** the `<svg>`, so `url(#a1)`/`url(#a2)` never resolved and **no arrowheads rendered at all**; all four panel captions overflowed the viewBox; the Overtaking panel drew the overtaker's arrow pointing backwards with both aircraft on one overlapping line; the Landing panel drew both aircraft diverging from a single point on the runway rather than two aircraft on final. Panel rebuilt: defs moved inside, captions split to two lines, both geometries redrawn.
  - *L02 fig1* — row-5 label ("Powered parachute / weight-shift-control") overflowed its box on both sides; pyramid widened and font reduced.
  - *L03 fig1 (wedding cake)* — **Class B and Class C tiers were drawn upside-down** (narrow tier on top of a wider one), contradicting the figure's own "inverted wedding cake" aria-label; rebuilt as narrow surface core + wider shelves above. "Class E" label was clipped off the right edge; relocated.
  - *L04 fig1* — legend row overlapped the bottom of the TC/HI instrument circles. *L04 fig2 (pitot-static)* — connector lines ran straight through the "Pitot tube"/"Static port" labels, the VSI circle overlapped the ALT circle, the VSI static line dead-ended inside the ALT, the ASI had no static connection despite its "ram vs static" label, and a stray `r="0"` circle was dead code. Relaid out. *L04 fig3/fig4 (ANDS/UNOS)* — caption text at y=192 in a viewBox only 190 tall, i.e. **clipped below the canvas**; viewBox extended.
  - *L05 fig1 (fronts)* — **the cold front's slope was drawn backwards**, showing cold air overhanging warm air (physically impossible) instead of wedging under it; slope reversed and frontal pips repositioned. Both panel captions were clipped at the edges *and* collided with each other in the middle; air-mass labels were struck through by the frontal lines. Relaid out.
  - *L07 fig2 (airfoil)* — the Net Lift arrow passed straight through the word "LOWER"; "Air deflected down (Newton)" was clipped off the right edge.
  - *L07 fig4 (drag curve)* — **the most serious figure defect: the total-drag curve was drawn as an inverted U (a maximum), with the green "L/D-max speed" marker sitting at the curve's peak** — the exact opposite of the point the figure exists to make, and contradicting its own aria-label ("U-shaped curve with its minimum"). It also dipped *below* the parasite-drag curve at high speed, impossible for a sum. Rebuilt so the two component curves are mirror images and the total curve is their **exact algebraic sum** (control points summed, since both share an x-parameterization), giving a true U with its minimum precisely at the induced = parasite crossing; that crossing is now marked too.
  - *L08 fig1 (wind triangle)* — **the wind vector was drawn reversed** (pointing from the destination back to the air-vector tip), breaking the vector addition the figure teaches; direction flipped. The "True Course" label was struck through by both the course line and the wind arrow, and the "True Heading" label ran off the right edge. *L08 fig2 (VOR)* — the radial line carried both a `marker-end` and a hand-drawn `<polygon>`, rendering a doubled arrowhead; caption overran the right edge.
  - *L09 fig1 (CG envelope)* — **the envelope's top-left vertex poked above its own "Max gross weight" line**, and the envelope *widened* toward the top, contradicting both the figcaption and the aria-label ("narrows near maximum gross weight"). Rebuilt as a trapezoid capped exactly on the max-gross line and narrowing upward; the "Loaded point" label no longer straddles the boundary.
- **QC pass (2026-08-07) — independent MCQ re-solve.** All **68 lecture-quiz + 60 final-exam questions** re-solved from FAA sources without reference to the marked key. **1 wrong answer found**, appearing in both banks: **maneuvering speed (Va) had the stall/overstress relationship inverted.** L07 Q6 option B and the exam's Q37 option A both read "the speed *above* which the wing will stall before the airframe is overstressed"; correct is *at or below* Va the wing stalls first, and *above* Va an abrupt full control input can overstress the airframe first. The same inversion had propagated into L07's §7.4 body paragraph and its key-takeaways bullet — all four sites corrected. Everything else verified correct. **Answer-position balance preserved** (fixes reworded option *text* in place, never moved the key): exam still 15/15/15/15 A–D; no lecture quiz clusters a letter above 2.
- **QC pass (2026-08-07) — worked-example arithmetic.** All three spot-checked and correct: L07 load factor (60° bank → 2G; 50 × √2 ≈ 71 KIAS), L08 wind triangle (TC 090°/TAS 100/wind 360°@20 → WCA 11.5°, TH ≈ 078°, GS = √(100²−20²) ≈ 98 kt), L09 weight-and-balance (moments 60,000 + 12,580 + 12,410 + 8,640 = 93,630; 2,190 lb; CG 42.75″). L09's density-altitude rule of thumb (120 ft/°C) and its "sea-level airport at 100°F ≈ 2,500 ft" analogy also check out (≈2,740 ft).
- **FULL QC PASS (2026-08-08) — figures rasterised, all 128 MCQs re-solved, prose + live sources re-verified.**
  Prompted by noticing that the +30 figures added earlier that day had been validated only by the *estimator*
  (overflow checker + structural validation), never rasterised and looked at — the check that catches wrong
  geometry and figures contradicting their own captions. Coverage this pass: **49/49 figures rendered and
  inspected**, **128/128 MCQs independently re-solved**, all 6 worked examples recomputed, all 13 CFR citations
  checked, 5 high-stakes numbers verified against live sources. **6 figure defects found, 0 wrong answer keys.**
  - **L09 fig4 (weight & balance) — the worked example did not add up.** Its five rows
    (1,400×36 + 340×37 + 240×48 + 170×73 + 40×95) sum to **90,710 in-lb**, but the figure printed
    `total 2,190  93,630` and `93,630 ÷ 2,190 = 42.75″` — **off by 2,920 in-lb / 1.33 inches, with a printed
    division that was arithmetically false.** *Root cause:* the +30 expansion built a new 5-row table (adding a
    baggage station) but carried over the TOTALS from the lecture's prose worked example, which uses different
    line items (1,500×40 + 340×37 + 170×73 + 180×48 = 93,630 / 2,190 = 42.75″ — that one is correct and was left
    untouched). Both weights happen to total 2,190 lb, which is what let the mismatch hide. Corrected to
    90,710 / **41.42″**, CG marker moved 159→154 px, aria-label updated. *This is also why the round-1 note above
    is misleading: the marker had been aligned to a CG that was never the right answer for that table.*
  - **L09 fig1 (density altitude) — cool-day figure didn't use the rule the figure itself teaches.** Field elev
    3,000′, ISA = 9 °C. Hot day +35 °C → 3,000 + 120(26) = 6,120 ≈ "6,000′" ✓, but cool day +5 °C → 3,000 + 120(−4)
    = **2,520′**, printed as "2,200′". A student applying the 120 ft/°C rule gets a different answer than the
    figure. Corrected to 2,500′.
  - **L08 fig5 (VOR indicator) — orphaned sentence fragment.** "The VOR is heading-independent — it shows where
    the COURSE is," sat inside the green box at x=381, while its own tail "not which way the airplane is pointed."
    was rendered at **x=110** under the *left* dial panel, wedged between the Reverse-sensing box's two lines —
    a non-sequitur in both places. Green box line made self-contained; orphan deleted.
  - **L06 fig1 (METAR decode) — text collision.** "Altimeter 30.02 in Hg" (→x≈199) ran into "Remarks: automated
    station, sea-level pressure" (x≈190→), rendering as "in H(R)emarks". Remarks label split onto two lines.
  - **L03 fig3 (special-use airspace) — truncated text.** The Prohibited card read `e.g. P-56, the` and stopped
    mid-sentence. Now "e.g. P-56 — Washington DC" on two lines.
  - **L05 fig3 (icing) — overlap.** Sub-labels "large droplets freeze slowly" / "small droplets freeze on contact"
    were drawn on top of the airfoil outlines; both pairs lifted clear.
  - **MCQ re-solve: 68 lecture + 60 exam = 128/128, zero wrong keys** (the 38 exam stems reworded the same day were
    re-solved as part of that; 2 wording defects in the *new* stems were caught and fixed — "the wing breaks" →
    "the wing stalls", and an "unheated ports are unavailable" clause → "the alternate static source is inoperative").
  - **Worked examples recomputed, all correct:** L02 converging right-of-way, L04 blocked-pitot diagnosis, L05 cloud
    read, L07 50 × √2 ≈ 71 KIAS, L08 wind triangle (WCA = asin 20/100 = 11.5°, GS = √(100²−20²) = 98 kt), L09 prose W&B.
  - **Live-source checks (Cornell LII + FAA testing matrix), all confirmed:** §91.211 oxygen (12,500/>30 min ·
    14,000 always · 15,000 all occupants), §91.117 speeds (250 KIAS <10,000 MSL; 200 under a Class B shelf and in
    Class C/D surface areas), §91.215(b) Mode C (all four provisions incl. the 30 NM veil), §91.155 VFR minimums
    (every row of the L03 table), and the PAR knowledge-test spec (**60 questions · 2.0 h · 70% = 42/60**).
  - **Method note:** `qlmanage -t` sizes its canvas to the *content* bounding box, not the viewBox, so it silently
    hides clipping. Every figure was re-rendered with a dashed `<rect>` injected at the viewBox bounds — anything
    crossing that frame is clipped in a real browser. Without that frame this pass would have missed the class of
    defect it was run to find.

- **CLOSE-OUT PASS (2026-08-08) — prose read end-to-end, packaging cross-checked, pages functionally verified.**
  The three gaps the full-QC pass had explicitly left open, now closed. **4 further defects found and fixed.**
  - **Prose: all 10 lecture bodies read end-to-end (~16,300 words), not sampled.** Two findings:
    - **L10's high-yield review table repeated the "VFR minimums loosen as control loosens" slogan that L03
      explicitly debunks.** Round 2 (2026-08-07) corrected the slogan in L03's body but missed its restatement in
      the Week-10 cram table — which is precisely what a student revises from the night before. The table now
      carries both tested traps: Class B is *clear of clouds* (the loosest cloud rule, not the strictest), and
      crossing 10,000 ft MSL tightens everything to 5 SM / 1,000-1,000-1.
    - **L04's blocked-pitot worked example was muddled**: "trapped pressure in the pitot line behaves like the
      ambient static pressure" is not what happens. Rewritten — the trapped pressure stays *constant* while ambient
      static falls, so the difference grows; that is why the ASI acts like an altimeter.
    Everything else verified correct: all 6 worked examples, the L06 prose TAF (valid 1218/1324 with every change
    group inside the window), the L09 "sea-level at 100 °F ≈ 2,500 ft DA" analogy (≈2,740 actual), L05's
    icing/fog/turbulence scales, L10's §91.211 and §91.17 numbers, and L03's full §91.155 Class G rows.
  - **L01 fig1 — the certification path was factually wrong.** It drew "Oral exam" and "Checkride" as two separate
    stages. The oral *is* the ground portion of the practical test, not an event preceding it. Relabelled to
    "Checkride: oral" → "Checkride: flight → certificate"; aria-label updated.
  - **index.html vs the lectures — project badges drifted.** The project-milestone list credits checkpoints in
    Wk 1/3/7/8/9/10, but the weekly syllabus badged only 1/7/9/10. **Weeks 3 (route locked in) and 8 (nav log
    built) were missing their "Project: checkpoint" pill** — Week 8 being the project's single largest component.
    Both added; badges and milestone list now agree. Weeks, discussion placement (3/6/10), discussion prompts,
    quiz counts (all within the advertised 5–10) and the 30/30/30/10 grading split all verified consistent.
  - **Functional verification (no headless browser on this machine — no Chrome/node/playwright).** Substitutes used,
    all passing:
    - **The real `gradeExam()` was extracted verbatim and executed under `jsc` (JavaScriptCore) against the real
      60 `data-correct` values** with a minimal DOM shim: 60/60 → 100% pass · **42/60 → 70%, marked PASS (boundary
      is inclusive, matching the FAA)** · 41/60 → 68% fail · 0/60 → fail.
    - The discussion widget and progress bar were executed the same way: localStorage save under `ppg-discN`,
      the reload-restore path, model-answer toggle, and the ChatGPT deep-link copying the student's own answer.
    - Every `getElementById`/`querySelector` in every inline script resolves, and every id passed literally into an
      inline handler (`saveDisc('disc2')`, `toggleModel('disc2-model')`, …) exists. L03/L06/L10 correctly reference
      their own disc1/disc2/disc3 — no copy-paste cross-wiring.
    - **`qlmanage -t` renders HTML through WebKit**, so the course index, the exam, and a lecture were rendered as
      real browser output and inspected: dark theme, grading bar proportions, stat cards, figure-in-context layout
      and the reworded exam Q1 all display correctly.

- **QC round 2 (2026-08-07) — external cross-check review.** A second reviewer re-solved the banks independently and audited packaging; it confirmed 0 remaining wrong answers (including that the Va fix reads correctly) and found no new figure defects, but caught **five things the first pass missed**, all now fixed:
  - **Three stale "2 h 30 m" strings survived the allotted-time fix** — the L01 `.eq` callout, the L01 "what you learned" recap, and L10's capstone checklist ("finish in under 2h30m"). *Root cause: the first pass grepped for `2 hours 30` / `150 minutes` / `2.5 hour` and never matched the `2 h 30 m` / `2h30m` spellings.* Now corrected to 2 h / 120 min, with the April-2023 change noted in the callout. Lesson for future numeric sweeps: grep a loose regex (`2 ?h ?30|2h30`), not literal spellings.
  - **Discussion 3 week number was inconsistent** — the course page said "wk 3 / 6 / 9" and L10's heading hedged "Week 9/10", but the discussion physically lives in L10 and L09 has none. Aligned everything to **3 / 6 / 10**. Note this is a deliberate deviation from C1–C5, which all put Discussion 3 in L09; C6 shifts it because the hazardous-attitudes content being discussed is taught in L10.
  - **Class G VFR minimums table was incomplete** — it listed only "G, day, below 1,200 ft AGL". Expanded to the full §91.155 airplane table (G night ≤1,200 AGL; G >1,200 AGL day/night; G ≥10,000 MSL), plus a note that Class G is the only class with different day/night numbers and that 1 SM clear-of-clouds is legal *only* in daytime Class G at or below 1,200 AGL.
  - **"Minimums loosen as airspace gets less controlled" was an over-broad slogan** — Class B is *clear of clouds* (looser than C/D/E), and crossing 10,000 ft MSL tightens rather than loosens. Both exceptions now stated explicitly in §3.2 and the takeaways.
  - **Project milestones on the course page contradicted the lectures** — index.html claimed "Wk 7: nav log drafted", but L07's checkpoint only asks for a planned cruise airspeed and L08 is where the nav log is actually built. Milestones corrected to Wk 7 = cruise airspeed, Wk 8 = nav log, and a missing Wk 3 route-lock milestone added.
- **⚠️ Open item — final-exam stems clone the lecture quizzes (logged 2026-08-07, P3).** 34 of the 60 exam items (12 *exact* stems + 22 near-duplicates) restate a lecture-quiz question. Measuring the other five Intro courses put this in perspective: **C1–C5 sit at 0–12% overlap (one exact clone across all five combined); C6 is at 56%.** So this is a C6 authoring defect, not a house style — the initial "accepted limitation" framing understated it. Probable cause: C1–C5 exams were authored by a separate per-course agent with no sight of the lecture quizzes, while C6 was built in one session with all 68 quiz items in context. **Not fixed yet** — rewording ~20–25 stems is a 1–2 h job that risks re-introducing errors into a bank now verified 100% correct, so it needs its own re-solve + verification pass. Tracked in [../../TODO.md](../../TODO.md) under Deferred QC. As it stands the final works well as a *comprehensive review retest*, just not as an independent test of transfer.
- **QC pass (2026-08-07) — live fact-check.** Verified against live sources (eCFR blocked; used Cornell LII for the CFR, plus the FAA Airman Knowledge Testing Matrix PDF parsed directly). Confirmed correct as-written: **91.113** right-of-way order and the head-on/overtaking/landing rules; **91.17** (8 hours / 0.04 BAC); **61.57** day currency (3 takeoffs + landings / 90 days, not necessarily full-stop) vs. night currency (3 to a **full stop**, 1 hr after sunset – 1 hr before sunrise); the **91.155 VFR minimums table** (all four rows match exactly); 60 questions and the 70% pass line. **1 stale number found and fixed:** the PAR knowledge test's allotted time is **2.0 hours, not 2.5** — the FAA reduced it effective **April 24, 2023**. L01 said "2 hours 30 minutes" in its body text and Q1 explanation, and Q6 asked the per-question time budget with "About 2.5 minutes" keyed correct (150 ÷ 60). Corrected to 2 hours / "About 2 minutes" (120 ÷ 60), keeping Q6's answer at position B; added an in-content note about the 2023 change and the FAA's unscored "validation" questions (the listed 60 is the *scored* count).
- **Answer-position rebalance (2026-08-07):** initial authoring skewed all 68 lecture-quiz correct answers onto B/C (45×B, 22×C, 1×D, 0×A) — a real defect caught by a post-build distribution check. Fixed with a script (`rebalance_quizzes.py`, run from scratch dir) that cycles each file's correct answers across A→D and swaps option text (+ updates the explanation's answer letter) to match; verified no lecture quiz now clusters a letter above 2/6–2/8. The 60-Q final was authored pre-balanced (15/15/15/15 A–D) and needed no fix.

- **Figure expansion (2026-08-08) — 19 → 49 inline SVGs (+30).** Driven by a review that the course was strong where geometry *is* the concept (right-of-way, airspace cake, wind triangle, drag curve) but thin exactly where the content was a **table to memorise**, a **cause→effect chain**, or a **decision flow**. All 30 were hand-authored to match the existing conventions (same palette, `role="img"` + `aria-label` + `<figcaption>`, viewBox ~460–600 wide).

  | Lecture | Added |
  |---|---|
  | L01 | written→oral→checkride pipeline with the ACS as a shared spine |
  | L02 | Part 61-vs-91 jurisdiction split · day/night currency clocks · emergency toolkit (Mayday/Pan-Pan, 7700/7600/7500/1200, aviate-navigate-communicate, Part 830) |
  | L03 | **VFR cloud-clearance bubbles drawn to scale** (B / C-D-E<10k / E≥10k / G day) · special-use legend with a "can I go?" verdict per symbol · Mode C veil + ADS-B plan view |
  | L04 | pitot/static blockage failure matrix · carburettor-venturi icing cutaway |
  | L05 | cloud-family ladder + stable-vs-unstable parcel paths · clear-vs-rime ice on the same wing · CB cross-section with the 20 NM ring · four fog mechanisms |
  | L06 | annotated TAF with an FM/TEMPO/PROB30 **timeline** · weather-product decision map · legal-vs-personal minimums ladder |
  | L07 | **bank→load-factor→√n stall speed + the V<sub>A</sub> fence** · flap camber before/after · ground-effect vortices |
  | L08 | sectional symbology cheat sheet · **TC→TH→MH→CH pipeline** · CDI/TO-FROM instrument face · three-Cs flow + diversion sketch |
  | L09 | density altitude (cool vs hot day, same field) · annotated 5-step POH chart read · **moment-arm seesaw** · forward-vs-aft CG behaviour |
  | L10 | hypoxia types + §91.211 oxygen altitudes · PAVE four-quadrant card · five hazardous attitudes paired with their antidotes |

  **Method / verification.** Same rasterise-and-look loop as the original QC pass (Python extraction → macOS `qlmanage`, since Node still isn't installed here). Added an **automated text-overflow checker** that estimates every `<text>` element's rendered width from its font-size, anchor and content and flags anything crossing the viewBox — it catches the clipping class of bug across all 49 figures in one pass, which is what most of the original 14 defects were. Defects found and fixed during this build: **8** — L03 Mode-C radius line crossing the "Class B" label; L04 carb-ice fuel-spray labels colliding with the venturi wall; L05 "keeps rising" and icing captions overflowing the right edge; L05 thunderstorm 20 NM ring drawn as two arcs that read as a lens and collided with the gust-front text (replaced with a single ellipse); L07 flap approach-path lines drawn through their own captions; L09 moment table overlapping the aircraft profile (and the CG marker repositioned so the drawing agrees with the arithmetic — **but see the 2026-08-08 full-QC entry below: the arithmetic it was aligned to was itself wrong**); plus 2 pre-existing marginal captions in L01/L03 tightened. Final state: **overflow checker clean, 0 structural issues** (svg/figure/figcaption/section/details balanced, no unresolved `url(#…)`, no `<defs>` outside its `<svg>`, every figure has `role="img"` + `aria-label` + a `<figcaption>`).
