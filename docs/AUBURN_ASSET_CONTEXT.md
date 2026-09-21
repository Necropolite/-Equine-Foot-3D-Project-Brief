# Auburn data context

## 2009 CT/MRI reconstruction project

The 2009 Auburn presentation, *Evaluating Soft Tissue Composition of the Equine Palmar Foot with CT, MRI, and 3-D Reconstruction*, lists Adam W. Cooner, D. Ray Wilhite, John T. Hathcock, Pete Ramey, Ivy Ramey, and Debra R. Taylor.

The study used three cadaver forefeet. The presentation describes:

- photographs and lateral radiographs;
- high-resolution CT;
- MRI;
- manual isolation of collateral cartilages from CT;
- digital-cushion segmentation from MR images;
- an estimated fibrocartilage component derived with a grayscale-mask approach;
- P3 isolation using a bone algorithm;
- 3D reconstruction in Mimics;
- CT/MR alignment at the palmar-process foramina.

Volumes were reported for P3, collateral cartilage, digital cushion, and estimated digital-cushion fibrocartilage.

The presentation is useful to this project mainly because it documents a multimodal reconstruction workflow. With only three feet, it should not be treated as population-level evidence.

## 2013 predictive-heel project

The later Auburn poster, *Predictive Modeling of the Equine Heel*, reports work on thirteen left front Thoroughbred cadaver feet.

The study used CT, MRI, ultrasound, radiography, physical measurements, and 3D reconstruction. The poster describes reconstructed digital cushion, collateral cartilages, and P2, among other measurements.

For this project, that raises the possibility that a larger set of multimodal source data or Mimics projects may have existed beyond the original three-foot pilot.

## What would be most useful to recover

In order of value for this project:

1. original CT and MRI DICOM series with specimen mapping;
2. original Mimics project files;
3. mask/segmentation labels and registration state;
4. notes or measurements that identify structures and methodology;
5. STL/OBJ exports tied back to a specific project and specimen.

The original project files matter because they may retain information that an STL/OBJ export does not: source series, masks, labels, measurements, and registration.

## Questions I would want to answer for each surviving project

- Which study did this file set belong to?
- Which specimen and limb?
- Are the CT and MRI series from the same foot?
- Which structures were directly segmented?
- Which were estimated or reconstructed?
- How was CT/MRI registration performed?
- Is the registration still preserved in the Mimics project?
- Were any meshes rescaled or repositioned after export?
- What Mimics version created the project?
- What use, modification, and redistribution are permitted?

The goal is to preserve enough context that the files can be used correctly rather than simply imported because they are available.
