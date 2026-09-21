# Equine Foot 3D

This repository is a short technical summary of an independent 3D equine-foot project I am developing for teaching and visualization.

My background is in software and computing rather than veterinary anatomy. The point of the project is not to invent anatomy, but to build a model whose geometry can be traced back to imaging, published work, or an explicitly documented reconstruction.

## Project aim

The end product is intended to be an interactive 3D foot in which structures can be isolated, hidden, made transparent, sectioned, and labeled. The first useful version would include the hoof capsule, P2, P3, navicular bone, digital cushion, collateral/ungular cartilages, and the main external structures of the solar and caudal foot.

The model will ultimately be exported for browser viewing so that it does not depend on Blender or specialist software.

## Current work

I have been using EquiSim as a provisional hard-tissue reference because it provides a coherent statistical model of the distal limb rather than unrelated meshes assembled by eye. I reproduced the zero-PC reference and verified the component mapping, scale, source axes, and relative placement for ten components, including P2, P3, navicular bone, and the hoof capsule.

I am not treating that model as a single measured horse. It is a population-derived statistical reference, and I am not redistributing converted EquiSim geometry while the scope of the data license remains unclear.

The main unresolved part of the project is soft tissue. In particular, I need a defensible source for the digital cushion and collateral/ungular cartilages, ideally from CT and MRI belonging to the same foot and retained in a common coordinate system.

## Auburn work

The 2009 Auburn CT/MRI reconstruction project is especially relevant because it used Mimics to reconstruct P3, collateral cartilages, and the digital cushion, with the CT and MR datasets aligned at the palmar-process foramina.

A later 2013 Auburn project used CT, MRI, ultrasound, radiography, and physical measurements in thirteen left front Thoroughbred cadaver feet and also produced 3D reconstructions of heel structures.

For this project, the most useful surviving material would be original DICOM data and Mimics projects with enough provenance to determine which specimen, modality, segmentation, and registration each file belongs to. STL/OBJ exports are useful as well, but the source projects are more informative if they still preserve masks, labels, measurements, or registration.

See [Auburn data context](docs/AUBURN_ASSET_CONTEXT.md).

## How I am handling uncertainty

I am keeping three categories separate:

- **directly segmented/measured** — geometry derived from known source imaging or measurements;
- **registered/reconstructed** — geometry built from references and fitted into a known spatial frame;
- **teaching geometry** — deliberately simplified or illustrative material.

I also keep anatomical confidence separate from reuse permission. A dataset may be excellent scientifically and still not be something I am allowed to publish.

## Repository contents

- [Project overview](docs/PROJECT_OVERVIEW.md)
- [Current technical status](docs/CURRENT_STATUS.md)
- [Anatomy in scope](docs/ANATOMY_SCOPE.md)
- [Data handling and provenance](docs/DATA_AND_PROVENANCE.md)
- [Auburn data context](docs/AUBURN_ASSET_CONTEXT.md)
- [Validation approach](docs/VALIDATION_MODEL.md)
- [Development roadmap](docs/ROADMAP.md)
- [References](CITATIONS.md)

This public repository intentionally contains no raw imaging, Mimics projects, unpublished research files, private correspondence, or restricted 3D data.

— Clint Ramey
