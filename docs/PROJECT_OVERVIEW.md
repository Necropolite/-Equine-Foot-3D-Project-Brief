# Project overview

## What I am building

The project is an interactive 3D model of the equine foot for teaching and visualization.

The useful part of a model like this is not simply the ability to render a hoof. It is the ability to expose the relationships among the hoof capsule, distal phalanx, navicular bone, digital cushion, collateral/ungular cartilages, and the external structures of the solar and caudal foot.

The planned viewer should allow a user to isolate structures, change transparency, use section/cutaway views, and inspect labeled anatomical landmarks.

## Why the source data matters

A 3D model can look convincing while still being anatomically wrong. Two accurate meshes from different horses can become misleading if they are scaled or placed together without a defensible registration.

For that reason, I am trying to avoid building the first reference foot by collecting unrelated meshes and aligning them by eye.

The preferred order is:

1. use a coherent specimen or registered dataset where possible;
2. preserve the original scale, orientation, and coordinate relationships;
3. reconstruct missing structures only when necessary;
4. document exactly which structures are direct segmentations and which are not.

## Reference configuration

The first model will represent a defined reference configuration. I do not intend to label it an "ideal hoof" or imply that one specimen or statistical mean represents every horse.

If later versions show different heel development, hoof-capsule configuration, laminitic change, or rehabilitation stages, those will be separate comparison models rather than silent changes to the reference anatomy.

## Current hard-tissue reference

I have reproduced the zero-PC reference from EquiSim and verified its scale, axes, component identities, and relative placement.

The extracted reference contains:

- MC3, MC2, and MC4;
- P1;
- both proximal sesamoids;
- P2;
- P3;
- navicular bone;
- hoof capsule.

For this project, the most important pieces are P2, P3, navicular, and the hoof capsule. EquiSim is useful as a hard-tissue spatial framework, but it does not provide the soft-tissue anatomy required for the finished teaching model.

## Current limiting problem

The main technical question is how to obtain or reconstruct the digital cushion, collateral/ungular cartilages, and related caudal-foot structures without losing spatial coherence.

That is why preserved same-foot CT/MRI data and original segmentation projects are particularly valuable.
