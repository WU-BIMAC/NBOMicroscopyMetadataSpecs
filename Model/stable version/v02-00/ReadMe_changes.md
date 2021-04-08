Microscopy Metadata Specifications - v02-00
-------------------------------------------
These specifications are being developed as a community effort initially led by the 4D Nucleome ([**4DN**](https://www.4dnucleome.org/)) Imaging Working Group (IWG) and the Bioimaging North America (BINA) Quality-Control and Data Management Working Group ([**QC-DM-WG**](https://www.bioimagingna.org/qc-dm-wg)) to extend the OME Data Model.

The next version of the Specifications are being developed as part of a **community outreach effort** that is currently underway in collaboration with the Quality Assessment and Reproducibility for Instruments & Images in Light Microscopy ([**QUAREP-LiMi**](https://quarep.org/))

The proposed prefix for this namespace is **NBO** for 4d**N** **B**ina **O**me

This version of the model is a major overhaul with several important revisions that were introduced as a result of several months of evaluation, feedback collection and correction of v01.07 by the members of the BINA Quality Control and Data Management Working Group.

******************
Summary of Changes
******************

## Introduced the sub-division of the initially proposed of the 4DN Extension of the OME model into three separate extensions:

1 - Core and Basic
2 - Advanced and Confocal
3 - Calibration and Performance

## Simplified the Tier system from 5 to 3 tier levels.

* Introduced Acquisition Software and Software Modules.

* Introduced multiple new hardware components including:

- Apertures (Iris Aperture, Shutter, Phase Ring, PinHole, Diffraction Grating, etc.,)
- Optical Assemblies (Microscope Tube, Condenser etc.,)
- Optics Holders (Filter Wheel, Filter Slider, etc.,)
- Confocal Scanners (Spinning Disk, Raster Scanner, etc.,)
- Acousto-Optical Devices (AOBS, AOTF, etc.,)
- Electro-Optical Devices (Liquid Crystal Tunable Filter, Deformable Mirror, etc.,)

* Introduced several improvements in the image acquisition settings model:

- Sample and Sample related elements (Sample Holder, Cover Glass, etc.,)
- Fluorophore and Immersion Liquid
- Several new Settings elements (MicroscopeTableSettings, PrismSettings, ShutterSettings, etc.,)
