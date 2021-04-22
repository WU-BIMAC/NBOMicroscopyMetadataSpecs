Microscopy Metadata Specifications - v02-00
-------------------------------------------
These specifications are being developed as a community effort initially led by the 4D Nucleome ([**4DN**](https://www.4dnucleome.org/)) Imaging Working Group (IWG) and the Bioimaging North America (BINA) Quality-Control and Data Management Working Group ([**QC-DM-WG**](https://www.bioimagingna.org/qc-dm-wg)) to extend the OME Data Model.

The proposed prefix for this namespace is **NBO** for 4d**N** **B**ina **O**me

Version v2.00 the current stable version of the model and it represents  a major overhaul with significant revisions that were introduced as a result of several months of evaluation, feedback collection and correction of v01.07 by the members of the BINA [**QC-DM-WG**](https://www.bioimagingna.org/qc-dm-wg).

******************
Summary of Changes
******************

1. Introduced the sub-division of the initially proposed of the 4DN Extension of the OME model into three separate extensions:
    - Core and Basic
    - Advanced and Confocal
    - Calibration and Performance

2. Simplified the Tier system from 5 to 3 tier levels.

3. Introduced Acquisition Software and Software Modules.

4. Introduced multiple new hardware components including:
    - Apertures (Iris Aperture, Shutter, Phase Ring, PinHole, Diffraction Grating, etc.,)
    - Optical Assemblies (Microscope Tube, Condenser etc.,)
    - Optics Holders (Filter Wheel, Filter Slider, etc.,)
    - Confocal Scanners (Spinning Disk, Raster Scanner, etc.,)
    - Acousto-Optical Devices (AOBS, AOTF, etc.,)
    - Electro-Optical Devices (Liquid Crystal Tunable Filter, Deformable Mirror, etc.,)

5. Introduced several improvements in the image acquisition settings model:
    - Sample and Sample related elements (Sample Holder, Cover Glass, etc.,)
    - Fluorophore and Immersion Liquid
    - Several new Settings elements (MicroscopeTableSettings, PrismSettings, ShutterSettings, etc.,)
