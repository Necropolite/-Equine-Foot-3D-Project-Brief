# Validation approach

The project uses several checks rather than a single visual judgment.

## 1. Source check

Before using geometry, establish:

- source project or publication;
- specimen/population;
- imaging or measurement method;
- units and orientation;
- file provenance;
- reuse terms.

## 2. Geometry check

For imported or converted meshes, check:

- scale;
- transforms;
- axis orientation;
- component identity;
- normals/winding;
- topology;
- preservation of relative placement.

## 3. Registration check

When CT and MRI or separately reconstructed structures are combined:

- identify the registration method;
- inspect the anatomical landmarks or fiducials used;
- check alignment in more than one plane;
- preserve the transform where possible;
- record any residual uncertainty.

## 4. Anatomical cross-check

Independent CT, MRI, anatomic sections, dissections, and published references are used to test plausibility.

Those sources are cross-checks unless their geometry is explicitly incorporated under a documented reconstruction method.

## 5. Domain review

Before a model is treated as teaching-ready, I want the relationships that matter most for instruction reviewed by someone with the relevant anatomy/hoof expertise.

## Claim discipline

A few rules I am using throughout the project:

- a statistical mean is not a single specimen;
- a reconstructed structure is not a direct segmentation;
- a three-foot exploratory project is not population proof;
- a clean mesh is not automatically a trustworthy source;
- willingness to share data is not the same as permission to publish it.
