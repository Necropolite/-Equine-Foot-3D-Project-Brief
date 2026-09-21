# Validation Model

## Validation is layered

The project does not use a single "looks right" judgment.

### 1. Source validation

Confirm source identity, specimen/population identity, imaging or measurement method, file provenance, units, orientation, and reuse terms.

### 2. Technical geometry validation

Check transforms, scale, axis orientation, component identity, topology, normals, watertightness where appropriate, and preservation of relative placement.

### 3. Registration validation

For multimodal or reconstructed anatomy:

- identify the registration method;
- verify landmarks or fiducials;
- inspect alignment in more than one plane;
- record residual uncertainty;
- avoid undocumented manual placement.

### 4. Cross-source anatomical validation

Use independent high-quality CT, MRI, anatomic slices, dissections, and published references to check plausibility.

External examples are validation references, not interchangeable geometry.

### 5. Teaching validation

Before a model is described as instruction-ready, teaching-critical anatomical relationships should be reviewed by a qualified domain expert where practical.

## Claims must match evidence

The project should never describe:

- a statistical mean as a single measured horse;
- reconstructed anatomy as directly segmented;
- a three-foot exploratory study as population proof;
- an exported mesh as a source-of-truth object when the source DICOM/project is available;
- a collaborator's willingness to help as institutional endorsement.
