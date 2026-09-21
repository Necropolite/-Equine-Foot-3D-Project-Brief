# Current Status

## Phase

**Phase 0B — source/data gates before production anatomy**

Detailed Blender production modeling is intentionally deferred until the source and registration questions that matter to the anatomy are resolved.

## Completed

### EquiSim extraction and verification

The project has reproducibly extracted ten named components from the zero-PC EquiSim reference:

1. cannon / MC3
2. MC2
3. MC4
4. long pastern / P1
5. left proximal sesamoid
6. right proximal sesamoid
7. short pastern / P2
8. coffin bone / P3
9. navicular / distal sesamoid
10. hoof capsule

The extraction preserves relative placement, source orientation, component identity, and scale.

### Units and orientation

The verified EquiSim source uses:

- linear coordinates in centimeters;
- angular values in radians;
- a retained right-handed source coordinate frame;
- X approximately sagittal, with dorsal/toe and palmar/heel direction;
- Y proximodistal, positive toward the ground/distal direction;
- Z mediolateral.

### Provenance rules

The project has formalized three evidence classes:

- measured / segmented;
- registered / reconstructed;
- teaching representation.

## Open gates

### Soft tissue

The central technical gap is still high-confidence soft-tissue anatomy, especially:

- digital cushion;
- collateral / ungular cartilages;
- associated caudal-foot structures;
- other structures needed for a complete teaching view.

### EquiSim redistribution

The repository and paper strongly suggest the statistical model was intended as part of the open-source EquiSim release, but the project is not publicly redistributing converted EquiSim geometry until the license scope for model data and derivatives is explicit.

### Auburn legacy assets

Historical Auburn CT/MRI + Mimics reconstruction work is being investigated as a possible same-project source for internal soft-tissue anatomy.

## What would move the project forward most

A well-documented file set containing original imaging plus preserved segmentation/registration state would be substantially more valuable than standalone STL/OBJ files with uncertain provenance.
