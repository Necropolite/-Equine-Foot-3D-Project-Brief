# Equine Foot 3D

This is a concise public summary of an independent 3D equine-foot project I am developing for teaching and visualization.

My background is in software and computing rather than veterinary anatomy. The goal is to build a model whose geometry can be traced back to imaging, published work, or an explicitly documented reconstruction, rather than creating anatomy by eye.

## Project aim

The finished model is intended to allow individual structures to be hidden, isolated, made transparent, sectioned, and labeled in an interactive browser viewer.

The first reference model is expected to include:

- hoof capsule and major external solar/caudal structures;
- P2;
- P3;
- navicular bone;
- digital cushion;
- collateral/ungular cartilages;
- other distal-foot structures where the source data support them.

The first model will be a defined reference configuration, not an “ideal hoof” or a claim that one specimen represents every horse.

## Current technical work

I am using EquiSim (Van Houtte et al., 2021) as a provisional hard-tissue reference because it provides a coherent statistical model of the distal limb rather than unrelated meshes assembled by eye.

I reproduced the zero-principal-component reference and verified the component mapping, source scale, axes, relative placement, and topology for ten components:

- MC3;
- MC2;
- MC4;
- P1;
- both proximal sesamoids;
- P2;
- P3;
- navicular bone;
- hoof capsule.

The source linear units are centimeters. The reconstructed source frame is right-handed; X is approximately dorsal-palmar, Y is proximodistal with positive Y toward the ground, and Z is mediolateral.

This gives the project a reproducible hard-tissue spatial reference. It does not make the model a single measured horse, a complete teaching model, or an “ideal” hoof. EquiSim is population-derived, and I am not publicly redistributing converted EquiSim geometry while the scope of the model-data license remains unresolved.

## Current limiting problem

The main unresolved part of the project is soft tissue, particularly the digital cushion and collateral/ungular cartilages.

The preferred source would be CT and MRI from the same foot with recoverable specimen identity, segmentation history, and registration. That would allow the soft-tissue geometry to remain tied to a coherent spatial frame instead of being fitted from unrelated examples.

## Auburn CT/MRI work

The 2009 Auburn presentation, *Evaluating Soft Tissue Composition of the Equine Palmar Foot with CT, MRI, and 3-D Reconstruction*, lists Adam W. Cooner, D. Ray Wilhite, John T. Hathcock, Pete Ramey, Ivy Ramey, and Debra R. Taylor.

The study used three cadaver forefeet and combined high-resolution CT, MRI, radiography, photography, and Mimics reconstruction. The presentation describes:

- collateral cartilages isolated from CT;
- the digital cushion isolated from MR images;
- an estimated fibrocartilage component derived with a grayscale-mask approach;
- P3 isolated using a bone algorithm;
- CT/MR alignment at the palmar-process foramina;
- volume measurements for P3, collateral cartilage, digital cushion, and estimated fibrocartilage.

For this project, the value of that work is mainly methodological and archival. With only three feet, it should not be treated as population-level evidence. However, preserved DICOM and Mimics projects could provide a coherent example of exactly the soft-tissue structures the current model is missing.

A later Auburn poster, *Predictive Modeling of the Equine Heel* (2013), reports work on thirteen left front Thoroughbred cadaver feet using CT, MRI, ultrasound, radiography, physical measurements, and 3D reconstruction. That raises the possibility that a larger multimodal archive may also have survived.

## Material that would be most useful to recover

In order of value:

1. Original CT and MRI DICOM series with enough naming or metadata to map them to a specific foot.
2. Original Mimics projects, including masks and registration if still preserved.
3. Notes, screenshots, measurements, or project documentation that identify structures and workflow.
4. STL/OBJ exports tied back to a specific specimen and source project.
5. Any later revisions or related projects not represented in the published/poster material.

For each file set, I would want to establish:

- study/project and specimen;
- limb and laterality;
- whether CT and MRI are from the same foot;
- which structures were segmented directly versus estimated/reconstructed;
- how CT/MRI registration was performed and whether the transform survives;
- whether exported meshes were rescaled, rotated, or repositioned later;
- the Mimics version and any linked source folders;
- what private use, modification, rendering, and redistribution are permitted.

## Data handling

If I receive research data, I plan to preserve an untouched source copy before opening, converting, or reorganizing anything.

The working procedure is:

1. preserve original folders and filenames;
2. record source, date received, project/study, specimen mapping, and permission notes;
3. calculate hashes and make a second backup;
4. create working copies for inspection, conversion, or segmentation;
5. keep raw DICOM, Mimics projects, and restricted meshes out of the public repository;
6. record every transform, scale conversion, reconstruction, and cleanup step applied to derivatives.

I am also keeping three geometry categories separate:

- **directly segmented/measured** — derived from known imaging or measurements;
- **registered/reconstructed** — built from credible references and fitted to a known spatial frame;
- **teaching geometry** — deliberately simplified or illustrative.

Anatomical confidence and permission to redistribute are tracked separately.

## Next steps

The next useful work is to:

1. review surviving Auburn material and establish file/specimen provenance;
2. determine whether same-foot CT/MRI registration can be recovered or independently checked;
3. identify which soft-tissue structures can remain directly segmented and which would still require reconstruction;
4. clarify reuse and redistribution terms;
5. only then proceed to production mesh cleanup, additional anatomy, expert review, and the browser viewer.

## References

Van Houtte J, Vandenberghe F, Zheng G, Huysmans T, Sijbers J. *EquiSim: An Open-Source Articulatable Statistical Model of the Equine Distal Limb.* Frontiers in Veterinary Science. 2021;8:623318. DOI: 10.3389/fvets.2021.623318.

Cooner AW, Wilhite DR, Hathcock JT, Ramey P, Ramey I, Taylor DR. *Evaluating Soft Tissue Composition of the Equine Palmar Foot with CT, MRI, and 3-D Reconstruction.* Auburn University research presentation, 2009.

Guidry LN, Taylor DR, Sanders RK, Cole RC, Wilhite DR, DeGraves FJ, Sanders AK, Bowker RM. *Predictive Modeling of the Equine Heel.* Auburn University Summer Scholars research poster, 2013.

Zarucco L, Wisner ER, Swanstrom MD, Stover SM. *Image fusion of computed tomographic and magnetic resonance images for the development of a three-dimensional musculoskeletal model of the equine forelimb.* Veterinary Radiology & Ultrasound. 2006;47(6):553-562. DOI: 10.1111/j.1740-8261.2006.00185.x.

---

This is an independent project by Clint Ramey. This repository contains no raw imaging, Mimics projects, unpublished research files, private correspondence, or restricted 3D data. It does not imply endorsement by Auburn University, Ray Wilhite, Pete Ramey, or any other researcher or institution.
