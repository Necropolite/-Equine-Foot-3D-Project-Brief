# Development roadmap

## 1. Establish the reference data

Current work.

- keep the verified EquiSim hard-tissue extraction reproducible;
- resolve the reuse status of EquiSim model data;
- identify the best available soft-tissue source;
- recover same-foot CT/MRI and original segmentation projects where possible;
- document specimen identity, units, orientation, registration, and reuse terms.

## 2. Build the first anatomical dataset

- preserve original source files;
- create a specimen/project manifest;
- import or segment the required structures;
- verify coordinate relationships;
- classify each object as directly segmented, reconstructed, or teaching geometry.

## 3. Produce teaching geometry

- clean meshes only after the source relationships are established;
- add external structures that are not available directly from imaging;
- retain separate anatomical objects;
- preserve a record of every transform and reconstruction decision.

## 4. Review

- inspect technical alignment and topology;
- cross-check anatomy against independent sources;
- obtain domain review of teaching-critical relationships;
- revise before freezing the first reference version.

## 5. Build the viewer

- structured GLB export;
- browser-based viewing;
- labels;
- show/hide/isolate controls;
- transparency;
- section/cutaway tools;
- later, measurements and comparison views if they are useful.

## 6. Add comparison models

Only after the reference foot is stable.

Possible later work includes different caudal-foot development, hoof-capsule configurations, laminitic changes, and rehabilitation-stage comparisons. Those should remain explicitly separate from the reference model.
