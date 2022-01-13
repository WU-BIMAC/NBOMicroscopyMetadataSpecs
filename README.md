<img align="right" src="https://github.com/WU-BIMAC/MicroMetaApp.github.io/blob/master/images/Nature%20Methods_COVER.png">

The **4D<ins>N</ins>-<ins>B</ins>INA-<ins>O</ins>ME (NBO) Microscopy Metadata Specifications** was developed as part of a **global community initiative** including the **[4D Nucleome Imaging Working Group](https://www.4dnucleome.org/)**, **[BINA Quality Control and Data Management Working Group](https://www.bioimagingna.org/qc-dm-wg)** and **[QUAREP-LiMi](https://quarep.org/)**. 
 
> **News!** The works of this **global community effort** resulted in multiple publications featured on a recent **Nature Methods FOCUS ISSUE** dedicated to **[Reporting and reproducibility in microscopy](https://www.nature.com/collections/djiciihhjh)**. 

> **News!** Specifically, for a thorought description of the 4DN-BINA-OME (NBO) Microscopy Metadata Specifications consult our recent **[Nature Methods](https://doi.org/10.1038/s41592-021-01315-z)** and **[BioRxiv.org](https://doi.org/10.1101/2021.05.31.446382)** publications!

> **Learn More!** If you are a newby and you want to learn more about the importannce of metadata and quality control to ensure full reproducibility, quality and scientific value in light microscopy, please take a look at our recently posted overview manuscript entitled **"A perspective on Microscopy Metadata: data provenance and quality control"**, which is available on [ArXiv.org](https://arxiv.org/abs/1910.11370).

**Development is continuing!** Please contribute to the new V02-10 draft of the model. Click [**here**](Model/in%20progress/v02-10) for a shortcut to the model directory. To create an issue, click on "Issues" above, the "New Issue" button, and select whether you are submitting a proposed new feature/element or want to propose a change to elements of the current proposal.

# 4D Nucleome + Bioimaging North America Microscopy Metadata Tiered Specifications extending the OME Data Model

Adequate record keeping is essential for most experiments as it is necessary in order to evaluate results, share data and allow experiments to be repeated. Keeping notes on microscopy experiments should be relatively unchallenging in this regard, as the microscope is a machine equipped with a limited number of known parts and settings.

Metadata automatically recorded by microscopes from different companies vary widely and pose a substantial challenge for microscope users to create a good faith record of their work. Similarly, the complexity and aim of experiments using microscopes varies leading to different reporting requirements from the simple description of a sample to the need to document the complexities of sub-diffraction resolution imaging in living cells and beyond.

In 2005 the Open Microscopy Environment (OME) initiative defined the OME data model "to serve as an informatics framework for imaging in biological microscopy experiments, including representation of acquisition parameters, annotations and image analysis results." (verbatim from: [Goldberg et al., 2005](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2005-6-5-r47)).
The OME model forms the basis of the [BioFormats library](https://www.openmicroscopy.org/bio-formats/) and is implemented in the [OME-TIFF](https://docs.openmicroscopy.org/ome-model/6.0.0/index.html#ome-tiff) file format and in the [OMERO](https://www.openmicroscopy.org/omero/scientists/) image data repository.

Despite the this very successful efforts, there remains a substantial gap between the OME data model and its wide adoption by the wide bio-imaging community as a bona fide Microscopy Data and Metadata Standard, dictating the set of metadata descriptors to be recorded or published with imaging datasets.

Here we present the 4DN-BINA Microscopy Metadata (Figure 1) guidelines, which is a tiered system of guidelines (Figure 3) that was developed by the [4D Nucleome (4DN) initiative](https://www.4dnucleome.org/) Imaging Standards Working Group and by the [BINA Quality Control and Data Management Working Group](https://www.bioimagingna.org/qc-dm-wg) for documenting the provenance and the quality of microscopy image data. In particular the proposal describes metadata standards for capturing: 

1. MICROSCOPE HARDWARE Specifications
2. IMAGE ACQUISITION Settings
3. OPTICAL, EXCITATION POWER and WAVELENGTH, MECHANICAL and DETECTOR CALIBRATION Procedures

<p align="center">
  <img src="https://github.com/WU-BIMAC/NBOMicroscopyMetadataSpecs/blob/master/Graphics/Figure-1_v03_MM+model elements.png" title="Figure 1: Image Metadata versus Microscopy Metadata">
</p>

**Figure 1: Imaging Experiment Workflows and Microscopy Metadata**

# Proposed Suite of 4DN-BINA Extensions of the OME Data-Model
To facilitate future adaptation and expansion of the guidelines, the proposed 4DN-BINA-OME model is organized on the basis of the core vs. extension ontology concepts. As such the proposal posits the following four components (see Figures 2 and 3):

1. A proposed revision of the OME Core Model
2. A 4DN-BINA-OME Basic extension
3. A 4DN-BINA-OME Advanced + Confocal extension
4. A 4DN-BINA-OME Calibration extension

<p align="center">
  <img src="https://github.com/WU-BIMAC/NBOMicroscopyMetadataSpecs/blob/master/Graphics/4DN-BINA-OME%20CORE%2BCALIBRATION%2BBASIC%2BADV%2BCONF%20EXTENSION_Instrument_v04.png" title="Figure 2A: OME Image Core ontology vs. 4DN-BINA-OME Extensions">
</p>

<p align="center">
  <img src="https://github.com/WU-BIMAC/NBOMicroscopyMetadataSpecs/blob/master/Graphics/4DN-BINA-OME%20CORE%2BCALIBRATION%2BBASIC%2BADV%2BCONF%20EXTENSION_Image_v05.png" title="Figure 2B: OME Image Core ontology vs. 4DN-BINA-OME Extensions">
</p>

**Figure 2: OME Image Core ontology vs. 4DN-BINA-OME Extensions**

In addition to extending the [OME data model](https://docs.openmicroscopy.org/ome-model/5.6.1/developers/model-overview.html) and maintaining full-compatibility with it, the main advance provided by the 4DN-BINA-OME guidelines is to posit the subdivision of imaging experiments among a set of five Tiers representing increasing imaging and analytical complexity levels. As a consequence, these guidelines not only provide an OME-based comprehensive list of metadata key-value pairs that should be recorded, but also details which subset of the full list should be recorded depending on the specific Tier the experiment belongs to. In so doing the guidelines lie the foundation for the birth of a microscopy data standard that could serve the same purpose the Encode guidelines serve in the genomic community.

In order to foster the wide usability of the guidelines, the proposal aim at providing detailed explanations of why these values matter. Finally, in order to aide their adoption by software developers, the guidelines are expressed in the Extensible Markup Language (XML) Schema Definition ([XSD](https://www.w3.org/XML/Schema)) format that can be utilized to generate code for both traditional databases and other software utilizing the data model.

# Tier System Proposal

<p align="center">
  <img src="https://github.com/WU-BIMAC/NBOMicroscopyMetadataSpecs/blob/master/Graphics/Figure-3_v06_REVISED.png" title="Figure 3: Tier System">
</p>

**Figure 3: Tier System**

# Repository content and documentation
The proposed Microscopy Metadata guidelines are available as follows:

1. An .xsd file providing the XML-schema for the proposed OME extension.
2. A .graphml providing an rendering of the INSTRUMENT Specifications and IMAGE ACQUISITION Settings sections of the model using the Entity-Relationship (ER) formalism. In order to open the file you can use the [yED application](https://www.yworks.com/products/yed).
3. A PDF version of the same ER schema.
4. A .xsl worksheet providing a comprehensive list of metadata key-value pairs that should be recorded for each tier, which can be found [here -->](https://docs.google.com/spreadsheets/d/16IQl-K8UIStsdlkNzJTA7LzMCan9qyS3KKcmEJ5wu28/edit?usp=sharing)
