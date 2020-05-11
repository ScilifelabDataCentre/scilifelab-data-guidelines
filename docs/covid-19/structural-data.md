# Recommendations for Structural data
## Repositories
Several different types of structural data are being collected for Covid-19 research. Some suitable repositories for these are:
* Structural data on proteins acquired using any experimental technique should be deposited in the wwPDB: Worldwide Protein Data Bank; a collaborating cluster of three regional centers at Europe EBI PDBe (PDBe-KB) and The Electron Microscopy Data Bank EMDB.

* A public information sharing portal and data repository for the drug discovery community, initiated by the Global Health Drug Discovery Institute of China (GHDDI) is the GHDDI Info Sharing Portal and includes the following: a) compound libraries including the ReFRAME compound library (the world’s largest collection of its kind, containing over 12,000 known drugs), a diversity-based synthetic compound library, a natural product library, a traditional Chinese medicine extract library, b) Drug Discovery Cloud Computing System on Alibaba Cloud, c) Data mining and integration of historical drug discovery efforts against coronavirus (e.g. SARS/MERS) using AI and big data, d) Molecular chemical modeling and simulation data using computational tools.

## Locating existing data 
A community data repository and curation service for Structure, Models, Therapeutics, Simulations related computations for research into the SARS-CoV-2 / COVID-19 / ”Coronavirus” pandemic is maintained by The (Molecular Sciences Software Institute (MolSSI))(https://molssi.org/) and [BioExcel](https://bioexcel.eu/) and [can be found here](https://covid.bioexcel.eu/).

## Data and metadata standards
**X-ray diffraction**
1.1. There are no widely accepted standards for X-ray raw data files. Generally these are stored and archived in the Vendor’s native formats. Metadata is stored in CBF/imgCIF format (See: catalogue of metadata resources for crystallographic applications) 
1.2. Processed structural information is submitted to structural databases in the .pdf or .mmCIF format.

**Electron microscopy**

2.1. Data archiving and validation standards for cryo-EM maps and models are coordinated internationally by EMDataResource (EMDR).
2.2. Every cryo-EM structure (map, experimental metadata, and optionally coordinate model) is deposited and processed through the wwPDB OneDep system
(deposit.wwpdb.org), following the same annotation and validation workflow also used for X-ray crystallography and NMR structures. EMDB holds all workflow
metadata while PDB holds a subset of the metadata.
2.3. Most electron microscopy data is stored in either raw data formats (binary, bitmap images, tiff, etc.) or proprietary formats developed by vendors (dm3, emispec, etc.).
2.4. Processed structural information is submitted to structural resources as PDBx/mmCIF.
2.5. Experimental metadata include information about the sample, specimen
preparation, imaging, image processing, symmetry, reconstruction method,
resolution and resolution method, as well as a description of the modeling/fitting procedures used and are described in EMDR, see also Lawson et al 2020.

**NMR**

3.1. There are no widely accepted standards for NMR raw data files. Generally these are stored and archived in single FID/SER files.
3.2. One effort for the standardization of NMR parameters extracted from 1D and 2D spectra of organic compounds to the proposed chemical structure is the NMReDATA format.
3.3. There is no universally accepted format, especially for crucial FID-associated metadata. The NMR-STAR is the archival format used by the Biological Nuclear Magnetic Resonance data Bank (BMRB), the international repository of biomolecular NMR data and an archive of the Worldwide Protein Data Bank (wwPDB 2018).
3.4. The nmrML format specification (XML Schema Definition (XSD) and an
accompanying controlled vocabulary called nmrCV) is an open mark up language an ontology for NMR data.

**Neutron scattering**

4.1. The nuclear data evaluations have been separately released from different countries. ENDF/B-VI of Cross-Section Evaluation Working Group (CSEWG) and JEFF of OECD/NEA have been widely utilized in the nuclear community. The latest versions of the two nuclear reaction data libraries arer JEFF-3.3 in 2017 (Cabellos) and ENDF/B-VIII.0 in 2018 (Brown et al., 2018) with a significant upgrade in data for a number of nuclides (Carlson et al., 2018).
4.2. Neutron scattering data are stored in the internationally-adopted ENDF-6 format maintained by CSEWG.

**Molecular Dynamics (MD) simulations of SARS-CoV-2 proteins**

5.1. Raw trajectory files containing all the coordinates, velocities, forces and energies of the simulation are stored as binary files: .trr, .dcd, .xtc and .netCDF; See also a description of metadata standards to be considered.
5.2. Refined structural models from experimental structural data.

**Computer-aided drug design data**
6.1. Virtual screening results are stored in chemical data formats such as .mol/.sdf, .mol2, .pdb, SMILES, InChi.
