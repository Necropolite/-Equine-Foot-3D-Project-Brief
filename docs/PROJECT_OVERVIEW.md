# Project Overview

## Problem

Interactive equine-foot models are useful for teaching, but a visually convincing model can still be anatomically misleading if its structures come from unrelated sources, are placed by eye, or are presented without provenance.

This project treats source quality and spatial coherence as first-class requirements.

## Intended model

The finished model should support:

- hoof capsule and wall;
- sole, frog, sulci, bars, and heels;
- white-line / lamellar region;
- P3 / coffin bone;
- P2 / short pastern where useful for orientation;
- navicular / distal sesamoid;
- digital cushion;
- collateral / ungular cartilages;
- other caudal-foot structures where source material supports them;
- labeled structures and landmarks;
- visibility/isolation controls;
- transparency and section/cutaway views;
- GLB export and browser viewing.

## What the first model is

The first model is a **defined reference configuration**.

It is not intended to be described as:

- the ideal hoof;
- the universal hoof;
- a statistically average hoof unless the underlying dataset supports that exact claim;
- a specimen-specific multimodal reconstruction unless all relevant anatomy genuinely comes from one registered specimen.

## Method

1. identify the strongest available source for each structure;
2. preserve source coordinate systems and units;
3. keep structures as separate 3D objects;
4. register them into one coherent spatial frame;
5. document which geometry is measured, reconstructed, or illustrative;
6. validate relationships against independent references;
7. keep legal/reuse status separate from anatomical confidence;
8. seek subject-matter review before calling teaching-critical anatomy validated.

## Current technical backbone

EquiSim has been technically verified as a useful hard-anatomy spatial framework. It contains a population-derived statistical model of the equine distal limb and provides ten extracted components in the project's verified reference workflow.

EquiSim does not provide the soft-tissue detail required for the final teaching model, which is why multimodal CT/MRI sources remain important.
