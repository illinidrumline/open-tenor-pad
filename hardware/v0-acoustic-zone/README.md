# v0 — Acoustic zone module

A single 12" octagonal gum-rubber practice pad, built to match the measured Evans RealFeel
RF12D. This is the baseline coupon: get this right before scaling to a tenor layout.

## Thickness budget (target ≈1.05–1.15" overall, matching the measured reference)

| Layer | Thickness |
|---|---|
| Fabric skin | ~0.02" |
| Gum rubber | 3/16" (4.8 mm) |
| Adhesive | ~0.005" |
| MDF core | 3/4" (19 mm) |
| Bottom rubber / foam | 1/8" (3.2 mm) |
| **Total** | **≈1.09"** |

Mass cross-check: a 12" octagon of 3/4" MDF is about 1.1 kg, plus gum about 0.40 kg and bottom
about 0.10 kg — roughly 1.6 kg against the measured reference of 1.53 kg. That brackets the core
at 5/8"–3/4"; confirm by weighing the finished build.

## Bill of materials

| Item | Spec | Source |
|---|---|---|
| Gum rubber sheet | natural gum, 40A, 3/16" × 12" × 12", smooth, no backing | industrial rubber supplier (e.g. Kuriyama GF40 tan pure gum, 3/16", 35–45 Duro A) |
| Fabric skin | dark grey, tight weave (nylon oxford / ripstop), 12" × 12" | fabric store |
| Core | MDF, 3/4" × 12" × 12" | big-box |
| Adhesive | solvent contact cement | hardware |
| Insert | M8 × 1.25 tee-nut (4-prong or screw-in) | hardware |
| Bottom | 3/16" recycled rubber sheet or 1/8" closed-cell EVA | hardware / craft |
| Mylar laminate (marching variant) | 0.010"–0.014" sheet | drum shop / plastics |

## Build steps (draft)

1. Cut the 12" octagon from the MDF; ease the edges.
2. Drill and install the M8 tee-nut from the underside, recessed flush.
3. Rough both the MDF and the rubber; apply contact cement to both; let it flash; bond with
   full coverage (no voids — voids become dead spots).
4. Laminate the fabric skin to the gum face (fabric-up) with the same adhesive.
5. Bond the bottom rubber or foam.
6. Weigh, then measure per the protocol below and compare to the reference.

## Acceptance

Run `../docs/realfeel-measurement-protocol.md` on the finished pad and on the reference:

- rebound coefficient within ≈5% of the reference
- contact time inside the 12–18 ms band
- no grid point more than 5% off the mean (no dead spots)

## Open questions carried from the materials doc

- Exact reference durometer and rubber gauge must be measured to close the loop.
- Confirm whether the reference "fabric finish" is a laminated fabric or a fabric-backed rubber sheet.
- Confirm the M8 insert on the 12" variant (Evans marketing and user reports disagree).
