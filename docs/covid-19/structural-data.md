# Recommendations for Structural data
## Repositories
Several different types of structural data are being collected for Covid-19 research. Some suitable repositories for these are:
* Structural data on proteins acquired using x-ray crystallography and nuclear magnetic resonance techniques should be deposited in the [wwPDB: Worldwide Protein Data Bank](https://doi.org/10.25504/FAIRsharing.mckkb4) via Europe EBI [PDBe (PDBe-KB)](https://doi.org/10.25504/FAIRsharing.26ek1v).

* Structural data on proteins acquired using electron microscopy and tomography techniques should be deposited in the Electron Microscopy
Public Image Archive [EMPIAR](https://www.ebi.ac.uk/pdbe/emdb/empiar/).


* A public information sharing portal and data repository for the drug discovery community, initiated by the Global Health Drug Discovery Institute of China (GHDDI) is the [GHDDI Info Sharing Portal](https://ghddi-ailab.github.io/Targeting2019-nCoV/) and includes the following: a) compound libraries including the [ReFRAME](https://reframedb.org/) compound library (the world’s largest collection of its kind, containing over 12,000 known drugs), a diversity-based synthetic compound library, a natural product library, a traditional Chinese medicine extract library, b) [Drug Discovery Cloud Computing System on Alibaba Cloud](https://www.alibabacloud.com/solutions/lifesciences-ehpc), c) Data mining and integration of historical drug discovery efforts against coronavirus (e.g. SARS/MERS) using AI and big data, d) Molecular chemical modeling and simulation data using computational tools.

## Locating existing data 
A community data repository and curation service for Structure, Models, Therapeutics, Simulations related computations for research into the SARS-CoV-2 / COVID-19 / ”Coronavirus” pandemic is maintained by [The Molecular Sciences Software Institute (MolSSI)](https://molssi.org/) and [BioExcel](https://bioexcel.eu/) and [can be found here](https://covid.bioexcel.eu/).

## Data and metadata standards
**X-ray diffraction**
* There are no widely accepted standards for X-ray raw data files. Generally these are stored and archived in the Vendor’s native formats. Metadata is stored in CBF/[imgCIF](https://doi.org/10.25504/FAIRsharing.zr52g5) format (see: [catalogue of metadata resources for crystallographic applications](https://www.iucr.org/resources/data/dddwg/metadata-catalogue)). 
* Processed structural information is submitted to structural databases in the .pdf or [.mmCIF](https://doi.org/10.25504/FAIRsharing.fd28en) format.

**Electron microscopy**
* Data archiving and validation standards for cryo-EM maps and models are coordinated internationally by [EMDataResource](http://emdataresource.org/) (EMDR).
* Every cryo-EM structure (map, experimental metadata, and optionally coordinate model) is deposited and processed through the wwPDB OneDep system (deposit.wwpdb.org), following the same annotation and validation workflow also used for X-ray crystallography and NMR structures. EMDB holds all workflow metadata while PDB holds a subset of the metadata.
* Most electron microscopy data is stored in either raw data formats (binary, bitmap images, tiff, etc.) or proprietary formats developed by vendors (dm3, emispec, etc.).
* Processed structural information is submitted to structural resources as [PDBx/mmCIF](https://doi.org/10.25504/FAIRsharing.fd28en).
* Experimental metadata include information about the sample, specimen
preparation, imaging, image processing, symmetry, reconstruction method,
resolution and resolution method, as well as a description of the modeling/fitting procedures used and are described in [EMDR](http://emdataresource.org/index.html), see also [Lawson et al 2020](https://aca.scitation.org/doi/10.1063/1.5138589).

**NMR**
* There are no widely accepted standards for NMR raw data files. Generally these are stored and archived in single FID/SER files.
* One effort for the standardization of NMR parameters extracted from 1D and 2D spectra of organic compounds to the proposed chemical structure is the [NMReDATA](http://nmredata.org/) format.
* There is no universally accepted format, especially for crucial FID-associated metadata. The [NMR-STAR](http://www.bmrb.wisc.edu/dictionary/3.1html_frame/frame_index.html) is the archival format used by the Biological Nuclear Magnetic Resonance data Bank (BMRB), the international repository of biomolecular NMR data and an archive of the Worldwide Protein Data Bank (wwPDB [2018](https://link.springer.com/article/10.1007/s10858-018-0220-3#ref-CR23)).
* The [nmrML format specification](http://nmrml.org/) (XML Schema Definition (XSD) and an accompanying controlled vocabulary called nmrCV) is an open mark up language and ontology for NMR data.

**Neutron scattering**
* The nuclear data evaluations have been separately released from different countries. ENDF/B-VI of Cross-Section Evaluation Working Group (CSEWG) and JEFF of OECD/NEA have been widely utilized in the nuclear community. The latest versions of the two nuclear reaction data libraries are JEFF-3.3 in 2017 ([Cabellos et al., 2017](https://www.sciencedirect.com/science/article/pii/S0969804319301484#bib4)) and ENDF/B-VIII.0 in 2018 ([Brown et al., 2018](https://www.sciencedirect.com/science/article/pii/S0969804319301484#bib3)) with a significant upgrade in data for a number of nuclides ([Carlson et al., 2018](https://www.sciencedirect.com/science/article/pii/S0969804319301484#bib6)).
* Neutron scattering data are stored in the internationally-adopted [ENDF-6](https://www.oecd-nea.org/dbdata/data/manual-endf/endf102.pdf) format maintained by [CSEWG](https://www.nndc.bnl.gov/csewg/).

**Molecular Dynamics (MD) simulations of SARS-CoV-2 proteins**
* Raw trajectory files containing all the coordinates, velocities, forces and energies of the simulation are stored as binary files: .trr, .dcd, .xtc and [.netCDF](https://fairsharing.org/bsg-s001210/); See also a [description of metadata standards](https://mmb.irbbarcelona.org/BigNASim/htmlib/help/pdf/d7.3_-_white_paper_on_standards_for_data_handling.pdf) to be considered.
* Refined structural models from experimental structural data.

**Computer-aided drug design data**
* Virtual screening results are stored in chemical data formats such as .mol/.sdf, .mol2, .pdb, SMILES, InChi.
