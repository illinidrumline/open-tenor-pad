# Open Tenor Pad

Open-source hardware for a marching tenor practice pad: a documented, buildable, sensor-ready
practice surface designed to feel as close as possible to the real thing.

**Status:** v0 — acoustic zone module in design. The first milestone is a single 12" pad built to
match the Evans RealFeel gum-rubber surface, measured against a reference unit rather than guessed.

## Why

Marching tenors are the loudest and least practice-friendly instrument in the band. Commercial
tenor pads exist, but there is no open, documented, printable, sensor-ready tenor-layout pad —
the geometry, materials, and feel are trade secrets. This project reverse-engineers the reference
pads, publishes the numbers, and builds up from a single zone to a full electronic line.

## Roadmap

| Stage | Deliverable |
|---|---|
| v0 | One acoustic zone: a 12" RealFeel-style gum-rubber pad measured against a reference unit |
| v1 | Tenor layout: multi-zone acoustic pad on a shared base, correct playable-area spacing |
| v2 | Electronic tier: piezo per zone plus rim, ESP32-S3 / Teensy 4.x, edrumulus-class firmware |
| v3 | Host software: per-strike capture, sweep-evenness scoring, adaptive drills |
| v4 | Ensemble: multi-pad line, group practice tooling |

## Layout

- `docs/` — material decisions, measurement protocols, design notes
- `hardware/` — design files, BOMs, drawings, build instructions
- `firmware/` — sensor firmware (planned)

## Docs

- [Materials decisions](docs/materials-decisions.md) — what we build the pad from, and why
- [RealFeel measurement protocol](docs/realfeel-measurement-protocol.md) — how to capture the reference numbers

## Licensing (proposed, pending confirmation)

| Scope | License |
|---|---|
| Hardware design files | CERN-OHL-S-2.0 |
| Documentation | CC BY 4.0 |
| Firmware | MIT |

No non-commercial or no-derivatives terms.

## Trademarks

This project is not affiliated with Evans, D'Addario, Vic Firth, Offworld Percussion, or the
University of Illinois. Do not distribute hardware bearing the University of Illinois Block I,
the "Illinois" wordmark, or Illini Drumline marks without approval from the UIUC Trademark and
Licensing Office (licensing@illinois.edu). Distributed physical goods bearing university marks
are merchandise.
