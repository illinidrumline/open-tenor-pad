# RealFeel measurement protocol

Capture the reference numbers that the materials spec currently estimates, so the v0 build can be
tuned to match rather than guessed.

**Reference unit:** Evans RealFeel 12" double-sided (RF12D). A single-sided RF12G is also useful,
since the gum face is shared across the family.

**Conditions:** measure at **21 °C ± 2**. Record ambient temperature and relative humidity with
every dynamic run — natural rubber softens about 3–5 Shore A per 10 °C.

## Equipment

- Digital calipers, 0.01 mm resolution
- Kitchen scale, 1 g resolution or better
- Shore A durometer (optional, about US$25–40)
- Steel ball, 16 mm / about 16.7 g (or a golf ball — record which and be consistent)
- Drop tube, e.g. 300 mm of 20 mm ID PVC, to guide the ball
- Ruler or steel tape
- Smartphone with 240 fps slow-motion video
- Sound level meter, or a calibrated-mic app reading dB(A) at a fixed 300 mm
- Backlight or bright diffuse light for edge photography
- Marker and paper for the dead-spot grid

## Part A — dimensions

| ID | Measurement | Method |
|---|---|---|
| A1 | Diameter across flats | calipers or tape across two parallel octagon flats, 3× |
| A2 | Diameter across corners | 3× |
| A3 | Overall thickness | at centre plus 4 edge points |
| A4 | Layer thicknesses | cross-section silhouette photo against a ruler, backlit |
| A5 | Insert bore depth | calipers or steel rule |
| A6 | Insert thread | M8 × 1.25 thread gauge, or caliper across the crests |
| A7 | Insert inset | protrusion or recess from the underside |
| A8 | Mass | scale |

Notes: A4 is the critical one — it separates fabric, gum, adhesive, core, and bottom. Photograph
both faces with a ruler and a coin for scale, and note any moulded part numbers.

## Part B — material

| ID | Measurement | Method |
|---|---|---|
| B1 | Gum-face durometer | Shore A, 5 spots; record as "through fabric" |
| B2 | Reverse-face durometer | Shore A, 5 spots |
| B3 | Exposed rubber durometer | lift a corner with a thin blade and measure the rubber directly |
| B4 | Surface character | macro photo; woven fabric or bare rubber? |
| B5 | Colour | sample a hex value from a colour-corrected photo |
| B6 | Adhesion | probe the edge; note whether the fabric is laminated or the rubber is fabric-backed |

## Part C — dynamic (the numbers that define feel)

**C1. Rebound coefficient.** Centre the drop tube on a zone. Drop the ball from H = 300 mm, measured
from the pad surface to the bottom of the ball. Film at 240 fps and record the peak rebound height
h, 5 trials. Rebound coefficient e = sqrt(h / H).

**C2. Contact time.** Strike with a drumstick at a repeatable angle — a pendulum jig is better than
freehand. Film at 240 fps; count the frames from first contact to separation; contact time =
frames / 240 seconds. Target band 12–18 ms.

**C3. Loudness.** Strike 10× at a fixed force (metronome or pendulum); record the peak dB(A) at
300 mm.

**C4. Dead-spot map.** Tap a 3×3 grid (centre plus 8 points). Compare rebound and loudness; flag any
point more than 5% off the mean.

**C5. Temperature sensitivity (optional).** Repeat C1 at about 15 °C and about 30 °C to quantify
drift.

## Part D — record sheet

### Reference unit

| ID | Reading 1 | Reading 2 | Reading 3 | Notes |
|---|---|---|---|---|
| A1 diameter across flats | | | | |
| A2 diameter across corners | | | | |
| A3 overall thickness | | | | |
| A4 fabric thickness | | | | |
| A4 gum thickness | | | | |
| A4 core thickness | | | | |
| A4 bottom thickness | | | | |
| A5 insert bore depth | | | | |
| A6 insert thread | | | | |
| A7 insert inset | | | | |
| A8 mass | | | | |
| B1 durometer through fabric | | | | |
| B2 durometer reverse | | | | |
| B3 durometer exposed rubber | | | | |
| C1 rebound height h (mm) | | | | ambient T/RH: |
| C1 rebound coefficient e | | | | |
| C2 contact time (ms) | | | | |
| C3 peak dB(A) | | | | |
| C4 worst grid deviation | | | | location: |

## Part E — coupon comparison

Build 4" coupons that vary one axis at a time: rubber gauge (1/8" / 3/16" / 1/4"), durometer
(40A / 50A), skin (bare / fabric / mylar), core (MDF / ply / polycarbonate). Run C1–C3 on each.

**Pass criterion:** rebound coefficient within about 5% of the reference, and contact time inside
the 12–18 ms band.

## Mapping — what each number decides

| Measurement | Decision it settles |
|---|---|
| A4 fabric thickness | D2 skin spec |
| B3 exposed rubber durometer | D1 durometer |
| A4 gum thickness | D1 gauge |
| A8 mass and A3 | D3 core thickness |
| C1 and C2 | pass or fail for the whole stack |
| C4 | D4 adhesive coverage and core flatness |
