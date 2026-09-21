# Equine Foot 3D — Project Brief

A source-grounded 3D teaching model of the equine foot.

This repository is the **shareable collaborator-facing brief** for a larger private working project. It is meant to let anatomists, imaging researchers, hoof-care educators, and technical collaborators understand the project quickly without exposing restricted source data or internal scratch work.

## The goal

Build an interactive equine-foot model that can:

- show, hide, isolate, and make anatomical structures transparent;
- preserve anatomically coherent spatial relationships;
- distinguish directly measured anatomy from reconstructed teaching geometry;
- support cutaways, labels, and comparison views;
- eventually export to GLB and run in a browser without requiring Blender.

## Core modeling rule

The model should not be assembled by taking unrelated structures from different horses and forcing them together.

Whenever possible, the project prefers one coherent specimen or registered dataset. If a structure must be reconstructed from external references, that uncertainty remains explicit.

## Geometry confidence classes

Every anatomical object is classified as one of:

1. **measured / segmented** — directly derived from source imaging or a measured dataset;
2. **registered / reconstructed** — rebuilt from credible references and fitted into a known spatial frame;
3. **teaching representation** — intentionally illustrative and not claimed to be specimen-measured.

## Current status

The project has:

- completed a Phase 0 source/dataset audit;
- verified a population-derived hard-anatomy reference from EquiSim;
- preserved ten named hard-anatomy components in a coherent coordinate system;
- documented units, orientation, transforms, topology, and provenance;
- identified soft-tissue anatomy as the main remaining data gap;
- identified historical Auburn CT/MRI + Mimics reconstruction work as a particularly valuable potential source.

No production teaching model has been declared anatomically validated yet.

## Why the Auburn work matters

Historical Auburn work reconstructed structures including P3, the digital cushion, and collateral/ungular cartilages using CT, MRI, and Mimics. CT and MR datasets were aligned using anatomical landmarks.

If original source imaging and segmentation projects can be recovered with clear provenance, they may provide exactly the kind of coherent soft-tissue evidence this project is designed around.

See [Auburn Asset Context](docs/AUBURN_ASSET_CONTEXT.md).

## What is intentionally not in this repository

This public brief does **not** contain:

- raw DICOM;
- Mimics project files;
- unpublished institutional data;
- restricted or unlicensed meshes;
- private correspondence;
- EquiSim-derived geometry pending license clarification;
- learner/patient/specimen identifiers;
- speculative anatomy presented as established.

## Important project framing

This is an independent hobby/research-development project by Clint Ramey.

Pete Ramey is not currently developing the project, and this repository does not imply endorsement by Pete Ramey, Auburn University, Ray Wilhite, or any other institution or researcher.

## Start here

- [Project Overview](docs/PROJECT_OVERVIEW.md)
- [Current Status](docs/CURRENT_STATUS.md)
- [Anatomy Scope](docs/ANATOMY_SCOPE.md)
- [Data and Provenance](docs/DATA_AND_PROVENANCE.md)
- [Auburn Asset Context](docs/AUBURN_ASSET_CONTEXT.md)
- [Validation Model](docs/VALIDATION_MODEL.md)
- [Roadmap](docs/ROADMAP.md)
- [Citations](CITATIONS.md)
