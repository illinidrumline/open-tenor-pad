# Materials decisions

Goal: build a practice pad that feels as close as possible to the Evans RealFeel. This document
records the reference measurements, the physical model of what controls feel, and the material
decisions that follow from them.

Confidence labels: **measured** (tape/scale on a real unit), **published** (manufacturer or patent),
**inferred** (derived from analogous materials), **verify** (sources disagree).

## 1. The target, quantified

From a ruler-and-scale teardown of a reference unit plus Evans' own product copy:

| Property | Evans RealFeel RF12D (12", double-sided) | Confidence |
|---|---|---|
| Playing diameter | 12.00" edge-to-edge | measured |
| Overall thickness | ≈1.05–1.15" ("a little over 1 inch") | measured |
| Mass | 1.53 kg (3 lb 10 oz) | measured |
| Core | unfinished pressed wood (MDF/HDF), rough, octagonal, unpainted | measured + 2 sources |
| Gum face | natural gum rubber plus a **dark grey fabric finish**, textured | published (Evans) |
| Reverse face | porous pressed / recycled rubber (harder, higher rebound) | measured |
| Mount | M8 × 1.25 threaded insert (tee-nut) in the base | reported ×2 — **verify** |
| Rebound character | "medium, controlled" | reviewer rubric |

The most important finding: **the grey surface is not bare rubber — it is gum rubber with a grey
fabric skin laminated on top.** That skin is a real design element. It resists stick scuffs and it
tames the rebound, which is why the RealFeel reads "controlled" rather than "bouncy".

## 2. The feel model

A stick sees the pad as one spring-damper. Stiffness comes from rubber durometer, thickness, bond
quality, and core rigidity; damping comes from rubber hysteresis and the skin.

| Change | Effect on feel |
|---|---|
| Durometer up | crisper, louder, more articulate, more rebound, shorter contact time |
| Rubber thickness up (on a rigid core) | more absorption, quieter, less rebound, softer |
| Fabric or mylar skin | more articulation and attack, protects the rubber, slightly tames rebound |
| Core stiffness/mass up (MDF to polycarbonate) | more rebound, less energy loss |
| Bond voids or partial glue | dead spots — adhesive coverage is a spec |
| Temperature up | rubber softens about 3–5 Shore A per 10 °C, so rate at 21 °C |

Published anchor points: **40 Shore A** is the most-repeated "correct" durometer (MadPad calls it
"the most desirable and most commonly used"; patents US3597520, US5929354, and US9245504 all land at
40). Patent thicknesses run 3/16" to 3/8". The composite rebound target band is a **12–18 ms**
contact/rebound time.

## 3. Decisions

| # | Parameter | Decision | Rationale | Alternatives held in reserve |
|---|---|---|---|---|
| D1 | Playing rubber | natural gum rubber, 40 ± 5 Shore A, 3/16" (4.8 mm) | most-cited authentic spec (MadPad 40A at 1/4"; patents at 40; retail gum sheet is universally 40A) | 1/8" (snappier), 1/4" (quieter); 50A/60A to bracket; TPE only if thermal/UV stability outweighs authenticity |
| D2 | Surface skin | dark grey, tightly-woven nylon/polyester fabric, laminated fabric-up | reproduces Evans' "dark grey fabric finish", the reason the reference feels controlled | bare gum; mylar laminate for the marching variant |
| D3 | Core | MDF (or HDF) 3/4", 12" octagon, unpainted, eased edges | measured match; cheap, stiff, warp-resistant, absorbs vibration like the original | 5/8" MDF; Baltic-birch ply (lighter, more resonant); polycarbonate (the dense-base approach MadPad uses) |
| D4 | Adhesive | solvent contact cement, full-surface coverage | matches the documented "strong rubber cement"; full coverage avoids voids | 3M Hi-Strength 90 spray; epoxy rejected (too stiff, brittle under impact) |
| D5 | Mount | M8 × 1.25 tee-nut, recessed flush in the underside | matches the reference and every cymbal stand | — |
| D6 | Reverse face | 3/16" medium-density recycled rubber (double-sided build) or non-slip EVA foam (single-sided) | matches the measured "porous pressed/recycled rubber" reverse | foam only |
| D7 | Geometry | 12" octagon for the clone; 6-zone playable-area layout for the tenor pad (later) | an octagon drops into a snare basket, like the reference | round |
| D8 | Marking | none, or a printed label with no university mark | distributing a pad bearing Block I, "Illinois", or the flamingo is merchandise and needs UIUC Trademark and Licensing approval | — |

## 4. Thickness budget

| Layer | Thickness |
|---|---|
| Fabric skin (D2) | ~0.02" |
| Gum rubber (D1) | 0.1875" |
| Adhesive (D4) | ~0.005" |
| MDF core (D3) | 0.75" |
| Bottom rubber / foam (D6) | 0.125" |
| **Total** | **≈1.09"** |

Cross-checks against the measured ≈1.1". Mass: a 12" octagon of 3/4" MDF is about 1.1 kg, plus gum
about 0.40 kg and bottom about 0.10 kg, roughly 1.6 kg against the measured 1.53 kg, which brackets
the core at 5/8"–3/4". Lean 3/4" and confirm by weighing the build.

## 5. Bill of materials (v0)

| Item | Spec | Source |
|---|---|---|
| Gum rubber sheet | natural gum, 40A, 3/16" (4.8 mm), 12" × 12", tan or grey, smooth, no backing | industrial rubber supplier (Kuriyama GF40 tan pure gum is 3/16", 35–45 Duro A) |
| Fabric skin | dark grey, tight weave (nylon oxford / ripstop), 12" × 12" | fabric store |
| Core | MDF, 3/4" × 12" × 12" | big-box |
| Adhesive | solvent contact cement | hardware |
| Insert | M8 × 1.25 tee-nut | hardware |
| Bottom | 3/16" recycled rubber sheet or 1/8" closed-cell EVA | hardware / craft |
| Mylar (marching variant) | 0.010"–0.014" sheet | drum shop / plastics |

## 6. How we prove "as close as possible"

Buy one reference RF12D and build 4" coupons that vary one axis at a time: rubber gauge (1/8" /
3/16" / 1/4"), durometer (40A / 50A), skin (bare / fabric / mylar), and core (MDF / ply /
polycarbonate). Run the dynamic tests in the measurement protocol on each coupon. The pass
criterion is a rebound coefficient within about 5% of the reference and a contact time inside the
12–18 ms band. The winner is then built at 12".

## 7. Open items

- Exact reference durometer and rubber gauge are not published anywhere; measure the reference
  (see the protocol) to close the loop.
- Confirm whether the reference "fabric finish" is a laminated fabric or a fabric-backed rubber
  sheet; the two need different sourcing.
- Confirm the M8 insert on the 12" variant: Evans' marketing copy calls the 12" pad "not mountable",
  while at least two reviews document the tee-nut in the Masonite base.
- **Strategic fork:** the RealFeel is a snare substitute and reviewers call it too soft for
  marching. A marching tenor pad's true target is a high-tension Kevlar/Aramid-Mylar head, which is
  the Offworld DarkMatter direction (harder, *less* rebound, articulate), not gum rubber. v0 clones
  the RealFeel to get a measured baseline; decide later whether v1 diverges toward the marching feel.

## Sources

- Evans RealFeel product copy (D'Addario); Drumsilent practice-pad teardown by Luke Petterson
  (ruler and scale measurements).
- US3597520A (Andrews), US4179974 (Trankle), US5929354A, US5932823A, US7498499, US9245504,
  US9437177B2.
- MadPad product description (rubber thickness and durometer, polycarbonate base).
- Offworld Percussion DarkMatter / Invader V3 product descriptions.
- Retail pure gum rubber sheet listings (40A, 1/16"–3/16"); Kuriyama GF40 data sheet.
