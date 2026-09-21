# Current technical status

## EquiSim reference extraction

I have completed a local reproduction of the EquiSim zero-PC reference.

The workflow reconstructs ten named components while retaining the source coordinate system and relative placement:

| Component | EquiSim name |
| --- | --- |
| Third metacarpal | `cannon` |
| Second metacarpal | `mc2` |
| Fourth metacarpal | `mc4` |
| P1 | `longpastern` |
| Proximal sesamoid | `sesamoidleft` |
| Proximal sesamoid | `sesamoidright` |
| P2 | `shortpastern` |
| P3 | `coffin` |
| Navicular bone | `navicular` |
| Hoof capsule | `hoofcapsule` |

The source linear units are centimeters. The source frame is right-handed; in the reconstructed reference, X is roughly dorsal-palmar, Y is proximodistal with positive Y toward the ground, and Z is mediolateral.

I have also checked the extracted meshes for component identity, placement, topology, and plausible scale.

## What this does and does not establish

This gives the project a reproducible hard-tissue reference.

It does **not** establish:

- a specimen-specific foot;
- a complete soft-tissue model;
- an "ideal" hoof;
- permission to redistribute converted EquiSim geometry.

The statistical reference is population-derived, not a single measured horse.

## Soft-tissue work

The structures I most need to resolve next are:

- digital cushion;
- collateral/ungular cartilages;
- DDFT/navicular-region relationships where the source material supports them;
- additional caudal-foot structures needed for teaching.

The preferred source is a same-foot multimodal dataset in which CT and MRI registration can be recovered or checked.

## Data rights

I am using EquiSim-derived geometry only in private/local development until I have a clear answer on whether the repository's MIT license was intended to cover the statistical model data and converted derivatives.

The same rule will apply to any Auburn material: anatomical usefulness and permission to redistribute are separate questions.

## Next technical milestone

The next meaningful milestone is not more mesh cleanup. It is establishing a soft-tissue source with known specimen identity, modality, segmentation history, registration, and reuse terms.
