# Data and Provenance

## Why provenance is central

A mesh is not automatically reliable anatomy merely because it looks realistic.

For every anatomical object, the project should be able to answer:

- where did this geometry come from?
- what specimen, population, or statistical model does it represent?
- what imaging or measurement method produced it?
- what units and coordinate system does it use?
- was it transformed after segmentation?
- is it directly measured or reconstructed?
- can it legally be modified and redistributed?

## Evidence classes

### Measured / segmented

Use when geometry is directly derived from source imaging or measured data and the provenance is known.

### Registered / reconstructed

Use when anatomy is rebuilt from credible references and fitted into the spatial frame of a known reference.

### Teaching representation

Use when geometry is intentionally simplified or illustrative.

## Source preservation

Original source data should be kept unchanged.

For acquired research files:

1. preserve original folder structure;
2. do not rename or reorganize the source copy;
3. record source person/institution, date, project, and specimen mapping;
4. compute file hashes;
5. create a second backup;
6. work from derivatives/copies;
7. keep raw/restricted data out of public Git repositories.

## Registration

When CT and MRI are combined, the project needs to know how the two modalities were aligned.

Important questions include:

- same foot or different feet?
- same pose?
- anatomical landmarks or fiducials?
- rigid or non-rigid registration?
- registration preserved in the source project?
- any post-export transformation?

## Reuse status is a separate axis

Anatomical confidence and legal permission are not the same thing.

A dataset may be scientifically excellent but not redistributable. The project records both dimensions separately.
