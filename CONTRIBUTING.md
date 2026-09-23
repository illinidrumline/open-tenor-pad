<!-- SPDX-FileCopyrightText: 2026 Illini Drumline contributors -->
<!-- SPDX-License-Identifier: CC-BY-4.0 -->

# Contributing

Thanks for helping build an open tenor practice pad. This project is measurement-driven: claims
about feel, rebound, or durability are only accepted with numbers attached.

## Ways to contribute

- **Build and report.** Build a v0 zone and open a build report issue.
- **Measure.** Run the [measurement protocol](docs/realfeel-measurement-protocol.md) on a reference
  pad or a coupon and submit the data.
- **Source and substitute.** Find cheaper or more available materials that still meet the spec.
- **Design.** Improve the CAD, tolerances, or geometry.
- **Document.** Fix errors, tighten wording, add diagrams.

## Ground rules

1. **Numbers beat opinions.** Any change to a materials decision needs test data or a cited source.
2. **One variable at a time.** Coupon tests change a single axis: gauge, durometer, skin, or core.
3. **State your conditions.** Temperature, humidity, tooling, and method belong in every result.
4. **No university marks.** Do not add University of Illinois, Block I, "Illinois", or Illini
   Drumline marks to hardware, documentation, or images. See [TRADEMARK.md](TRADEMARK.md).
5. **Safety first.** Read [SAFETY.md](SAFETY.md) before posting build instructions involving dust,
   solvents, or power tools.

## Licensing of contributions

By contributing, you agree to license your work under the licence that covers the files you touch:

| Area | Licence |
|---|---|
| Hardware design files (`hardware/`) | CERN-OHL-S-2.0 |
| Documentation (`docs/`, readme files) | CC BY 4.0 |
| Firmware and workflows (`firmware/`, `.github/workflows/`) | MIT |

Sign off every commit with the [Developer Certificate of Origin](https://developercertificate.org/):

```text
git commit -s -m "Add flange tolerance note"
```

The `Signed-off-by:` line certifies that you wrote the change or otherwise have the right to submit
it under the licence above.

## Design conventions

- **Units:** millimetres in all CAD and drawings. Imperial in parentheses only for reference.
- **CAD:** parametric source (FreeCAD or OpenSCAD) plus exported STEP and STL. One part per file.
- **Naming:** `part-rev.step`, `part-rev.stl`, `drawing-part-rev.pdf`.
- **BOM:** one CSV line per orderable item, with spec, quantity, and a source.
- **Drawings:** dimensioned PDFs for anything that gets cut or drilled.

## Pull requests

- Keep each pull request to one concern.
- Reference the issue or measurement that motivates the change.
- Update [`CHANGELOG.md`](CHANGELOG.md) under `[Unreleased]`.
- Confirm each item in the pull request template.
