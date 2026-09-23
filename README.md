# Open Tenor Pad

[![License: CERN-OHL-S-2.0](https://img.shields.io/badge/license-CERN--OHL--S--2.0-blue.svg)](LICENSE)
[![Release](https://img.shields.io/github/v/release/illinidrumline/open-tenor-pad.svg?include_prereleases&label=release&color=orange)](https://github.com/illinidrumline/open-tenor-pad/releases)
[![Docs: CC BY 4.0](https://img.shields.io/badge/docs-CC%20BY%204.0-lightgrey.svg)](docs/)
[![Status: design baseline](https://img.shields.io/badge/status-design%20baseline-orange.svg)](CHANGELOG.md)

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
- [Prior art and design freedom](docs/prior-art-and-design-freedom.md) — provenance and patent posture
- [Changelog](CHANGELOG.md) — what changed, and when

## Licensing

| Scope | Licence | Text |
|---|---|---|
| Hardware design files | CERN-OHL-S-2.0 | [LICENSE](LICENSE) |
| Documentation | CC BY 4.0 | [LICENSES/CC-BY-4.0.txt](LICENSES/CC-BY-4.0.txt) |
| Firmware and workflows | MIT | [LICENSES/MIT.txt](LICENSES/MIT.txt) |

No non-commercial or no-derivatives terms. CERN-OHL-S-2.0 is strongly reciprocal: if you distribute
hardware built from these files, you must make the corresponding design files available under the
same licence.

## Project standards

- [Contributing](CONTRIBUTING.md) — how to build, measure, and submit changes
- [Safety](SAFETY.md) — shop and material hazards
- [Trademarks and non-affiliation](TRADEMARK.md) — marks, endorsements, and patents
- [Citation metadata](CITATION.cff)

## Trademarks

This project is not affiliated with Evans, D'Addario, Vic Firth, Offworld Percussion, or the
University of Illinois. Do not distribute hardware bearing the University of Illinois Block I,
the "Illinois" wordmark, or Illini Drumline marks without approval from the UIUC Trademark and
Licensing Office (licensing@illinois.edu). Distributed physical goods bearing university marks
are merchandise. See [TRADEMARK.md](TRADEMARK.md).
