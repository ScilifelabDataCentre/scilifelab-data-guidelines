# Recommendations for Structural data
## Repositories
Several different types of structural data are being collected for Covid-19 research. Some suitable repositories for these are:

* Structural data on proteins acquired using using any experimental technique (x-ray crystallography, nuclear magnetic resonance)  should be deposited in the [wwPDB: Worldwide Protein Data Bank](http://www.wwpdb.org/) via EBI [PDBe](https://www.ebi.ac.uk/pdbe/).


## Locating existing data 
The [COVID-19 Molecular Structure and Therapeutics Hub](https://covid.bioexcel.eu/) community data repository and curation service for structure, models, therapeutics, simulations and related computations for research into the COVID-19 pandemic is maintained by [The Molecular Sciences Software Institute (MolSSI)](https://molssi.org/) and [BioExcel](https://bioexcel.eu/).

## Data and metadata standards
**X-ray diffraction**
* There are no widely accepted standards for X-ray raw data files. Generally these are stored and archived in the Vendor’s native formats. Metadata is stored in [CBF/imgCIF](https://www.iucr.org/resources/cif) format (see also [Catalogue of Metadata Mesources for Crystallographic Applications](https://www.iucr.org/resources/data/dddwg/metadata-catalogue)). 
* Processed structural information is submitted to structural databases in the [PDBx/mmCIF](http://mmcif.pdb.org/) format.

**Electron microscopy**
* Data archiving and validation standards for cryo-EM maps and models are coordinated internationally by [EMDataResource](http://emdataresource.org/) (EMDR).
* Cryo-EM structures (map, experimental metadata, and optionally coordinate model) are deposited and processed through the [wwPDB OneDep system](https://deposit-2.wwpdb.org/), following the same annotation and validation workflow also used for X-ray crystallography and nuclear magnetic resonance (NMR) structures. EMDB holds all workflow metadata while PDB holds a subset of the metadata.
* Most electron microscopy data is stored in either raw data formats (binary, bitmap images, tiff, etc.) or proprietary formats developed by vendors (dm3, emispec, etc.).
* Processed structural information is submitted to structural resources as [PDBx/mmCIF](http://mmcif.pdb.org/).
* Experimental metadata are described in [EMDR](http://emdataresource.org/index.html), see also [Lawson et al 2020](https://aca.scitation.org/doi/10.1063/1.5138589)

**NMR**
* There are no widely accepted standards for NMR raw data files. Generally these are stored and archived in single FID/SER files.
* One effort for the standardization of NMR parameters extracted from 1D and 2D spectra of organic compounds to the proposed chemical structure is the [NMReDATA initiative](http://nmredata.org/) format.
* There is no universally accepted format, especially for crucial FID-associated metadata. [NMR-STAR](http://www.bmrb.wisc.edu/formats.shtml) and its [NMR-STAR Dictionary](https://github.com/uwbmrb/nmr-star-dictionary) is the archival format used by the [Biological Nuclear Magnetic Resonance data Bank](http://www.bmrb.wisc.edu/) (BMRB), the international repository of biomolecular NMR data and an archive of the [Worldwide Protein Data Bank](http://www.wwpdb.org/) (wwPDB).
* The [nmrML format specification](http://nmrml.org/) (XML Schema Definition (XSD) and an accompanying controlled vocabulary called nmrCV) are an open mark up language and ontology for NMR data.
* Processed structural information is submitted in the [PDBx/mmCIF](http://mmcif.pdb.org/) format.

**Neutron scattering**
* ENDF/B-VI of Cross-Section Evaluation Working Group ([CSEWG](https://www.nndc.bnl.gov/csewg/)) and JEFF of OECD/NEA have been widely utilized in the nuclear community. The latest versions of the two nuclear reaction data libraries are [JEFF-3.3](https://www.oecd-nea.org/dbdata/jeff/) and ENDF/B-VIII.0 ([Brown et al., 2018](https://www.sciencedirect.com/science/article/pii/S0969804319301484#bib3)) with a significant upgrade in data for a number of nuclides ([Carlson et al., 2018](https://www.sciencedirect.com/science/article/pii/S0969804319301484#bib6)).
* Neutron scattering data are stored in the internationally-adopted [ENDF-6](https://www.oecd-nea.org/dbdata/data/manual-endf/endf102.pdf) format maintained by [CSEWG](https://www.nndc.bnl.gov/csewg/).
* Processed structural information is submitted in the [PDBx/mmCIF](http://mmcif.pdb.org/) format.

**Molecular Dynamics (MD) simulations**
* Raw trajectory files containing all the coordinates, velocities, forces and energies of the simulation are stored as binary files: .trr, .dcd, .xtc and [.netCDF](https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_data_model.html)
* Refined structural models from experimental structural data using MD simulations are stored in
[.pdb](https://www.rcsb.org/pdb/static.do?p=file_formats/index.jsp#pdb) format 

**Computer-aided drug design data**
* Virtual screening results are stored in 3D chemical data formats such as [.pdb](http://www.wwpdb.org/documentation/file-format)
* Structural formulas either in [SMILES](https://nepis.epa.gov/Exe/ZyPDF.cgi?Dockey=2000CAUR.PDF) or [ IUPAC
International Chemical Identifier](https://iupac.org/who-we-are/divisions/division-details/inchi/) (InChi), and identified through InChIKey, a non-proprietary identifier for chemical substances ([Heller et al., 2015](https://doi.org/10.1186/s13321-015-0068-4)).
