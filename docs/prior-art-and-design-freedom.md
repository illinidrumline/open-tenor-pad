<!-- SPDX-FileCopyrightText: 2026 Illini Drumline contributors -->
<!-- SPDX-License-Identifier: CC-BY-4.0 -->

# Prior art and design freedom

This project reverse-engineers a reference practice pad from published measurements and public
patents. This note records what we draw on, what we avoid, and where the boundary sits. It is
engineering provenance, not legal advice.

## What we derive from

| Source | Status | What we take |
|---|---|---|
| US3597520A (1971), drum practice pad | expired | a pure gum rubber surface of uniform thickness, cemented to a hard flat base |
| Published measurements of commercial pads | current products | dimensions, mass, and layer thicknesses for a reference target |
| Industrial material datasheets | public | gum rubber durometer and gauge, adhesive, MDF, recycled rubber |

The 1971 patent is the ancestor of the modern pad: a solid base with a gum rubber striking surface
recessed into it. Its term expired decades ago and its subject matter is free to use.

## What we deliberately avoid

Several later patents are plausibly still in force. We avoid their claimed features so the v0
design stays clear of them:

| Patent | Feature we avoid |
|---|---|
| US9437177B2 | a striking surface whose thickness varies across its area; a raised rim sized so the stick angle matches a 14-inch snare; articulating wings for a three-point snare basket |
| US9245504 | a dodecagon instructional base with a specific stacked pad and neoprene construction |
| US5929354A | a one-piece silicone (VMQ) pad with the claimed compound properties |
| US5932823A | a poured two-part elastomer striking surface in a recessed base |
| US7498499 | a viscoelastic damping layer under a harder striking layer |

v0 is a uniform-thickness gum rubber surface on a flat, unpainted MDF base with a recessed tee-nut.
That is the expired-patent design, not the later ones.

## If we diverge

A future marching-tuned variant that copies a Kevlar/Aramid-Mylar style surface, a raised rim, or a
graded-thickness surface would move into the avoided set. Any such change must be reviewed for
freedom to operate before it is merged, and the review recorded in the pull request.

## Corrections welcome

If any status here is wrong, open a design change issue with a citation.
