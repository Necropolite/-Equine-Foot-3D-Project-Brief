# Data handling and provenance

For this project, a mesh is useful only if I can explain where it came from and what happened to it before it reached the final model.

## Minimum record for a source asset

For each imaging series, Mimics project, or exported mesh, I want to record:

- study/project;
- specimen or population;
- limb and laterality;
- source modality;
- units;
- source orientation;
- segmentation method, where known;
- registration method, where applicable;
- any later transforms or rescaling;
- who supplied or created the file;
- what use and redistribution are permitted.

## Working categories

### Directly segmented/measured

Used for geometry derived from known imaging or measured data.

Example: a digital-cushion mask segmented from a specific MRI series.

### Registered/reconstructed

Used for geometry reconstructed from other references and fitted to a known spatial framework.

This may still be good teaching anatomy, but it should not be described as a direct segmentation from the reference specimen.

### Teaching geometry

Used for deliberately simplified or illustrative structures.

## Original-file preservation

If I receive research data, I plan to keep an untouched source copy before opening, converting, or reorganizing anything.

The intake process is:

1. preserve the directory structure;
2. record who supplied the data and when;
3. calculate file hashes;
4. make a second backup;
5. create working copies for conversion or segmentation;
6. keep raw or restricted data outside the public Git repository.

This is especially important for older Mimics projects because saving them in a newer version may alter the only surviving copy.

## CT/MRI registration

For multimodal anatomy, "same foot" is necessary but not enough. I also need to know how the CT and MRI volumes were aligned.

Useful information includes:

- which dataset was treated as the reference;
- whether registration was rigid or deformable;
- landmarks or fiducials used;
- whether a transform is preserved in the project;
- whether exported objects still share that coordinate system;
- whether any meshes were moved manually after export.

## Permission record

I will keep permission/reuse status separate from anatomical confidence.

For example, a high-quality Mimics project may be excellent for private study but still require separate approval before its source data or derived meshes can be placed in a public viewer.
