<!-- SPDX-FileCopyrightText: 2026 Illini Drumline contributors -->
<!-- SPDX-License-Identifier: CERN-OHL-S-2.0 -->

# Hardware

Design files for the Open Tenor Pad.

## v0 — acoustic zone (`v0-acoustic-zone/`)

A single 12" octagonal pad built to match the Evans RealFeel gum-rubber surface. This is the
measurement baseline. Materials and rationale are specified in
[`../docs/materials-decisions.md`](../docs/materials-decisions.md); the reference numbers come from
[`../docs/realfeel-measurement-protocol.md`](../docs/realfeel-measurement-protocol.md).

Planned contents once CAD exists:

- `parts/` — parametric source (FreeCAD `.FCStd`) and STEP exports
- `drawings/` — dimensioned drawings
- `bom.csv` — bill of materials
- `build-notes.md` — assembly and finishing notes

## Conventions

- Units: millimetres.
- Source CAD stays parametric; export STEP for interchange and STL only for print parts.
- Every BOM line must be an orderable, currently-produced part.
