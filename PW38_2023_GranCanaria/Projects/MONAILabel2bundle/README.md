Back to [Projects List](../../README.md#ProjectsList)

# Conversion of MONAI Label trained network into a MONAI bundle

## Key Investigators

- Deepa Krishnaswamy (Brigham and Women's Hospital, USA)
- Cosmin Ciausu (Brigham and Women's Hospital, USA)
- Nazim Haouchine (Brigham and Women's Hospital, USA)
- Andres Diaz-Pinto (NVIDIA, USA)
- Jesse Tetreault (NVIDIA, USA)
- Roya Hajavi (Brigham and Women's Hospital, USA)
- Stephen Aylward (Kitware, USA)
- Steve Pieper (Isomics Inc, USA)
- Andrey Fedorov (Brigham and Women's Hospital, USA)

# Project Description

MONAI Label has become a very popular tool in the NA-MIC community for developing new trained models and incorporating expert feedback into the training process.

Unfortunately, it is currently not straightforward to take the models trained using MONAI Label and apply them in batch mode.

MONAI supports bundles, which are designed for batch mode processing, but the process of converting MONAI Label trained networks into MONAI bundle representation is not well understood and (per MONAI experts) currently requires support from MONAI developers.

In this project we want to explore the process of converting MONAI Label trained networks into MONAI bundle format, and demonstrate how the resulting bundles can be applied to datasets in [NCI Imaging Data Commons](https://portal.imaging.datacommons.cancer.gov/).

## Objective

<!-- Describe here WHAT you would like to achieve (what you will have as end result). -->
1. Develop a complete example transforming MONAI Label network to MONAI bundle.
1. Improve existing documentation.
1. Demonstrate how MONAI Label trained network converted to bundle can be applied to a representative sample of data from IDC.


## Approach and Plan

<!-- Describe here HOW you would like to achieve the objectives stated above. -->

1. Use MONAI Label trained model for [segmentation of vertebrae in CT](https://github.com/Project-MONAI/MONAILabel/blob/main/sample-apps/radiology/main.py#L174) as the use case. 
2. Identify MONAI documentation for transforming MONAI Label trained network into MONAI bundle format.
3. Develop MONAI bundle from the network in 1.
4. Select applicable representative subset of data from IDC and apply resulting bundle to a produce segmentations, save segmentations as DICOM SEG, confirm visualization with OHIF.
5. Document the process and any refinements to the existing instructions.

## Progress and Next Steps

<!-- Update this section as you make progress, describing of what you have ACTUALLY DONE. If there are specific steps that you could not complete then you can describe them here, too. -->

1. Identified MONAI Label network location; discussed the project with Stephen, identified relevant expertise on MONAI side; planning to have coordination meeting with Roya.
1. ...
1. ...

# Illustrations

<!-- Add pictures and links to videos that demonstrate what has been accomplished.
![Description of picture](Example2.jpg)
![Some more images](Example2.jpg)
-->

# Background and References

- [NCI Imaging Data Commons](ttps://portal.imaging.datacommons.cancer.gov/)
- [MONAI bundle docs](https://github.com/Project-MONAI/tutorials/blob/main/bundle/get_started.md)