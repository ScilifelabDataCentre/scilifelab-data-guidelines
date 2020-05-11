# Data documentation - metadata 
Good documentation in research projects, describing how the datasets were created, how they are structured, and what they mean, is essential for making your data understandable. Metadata provides such 'data about data' , and may include information on the methodology used to collect the data, analytical and procedural information, definitions of variables, units of measurement, any assumptions made, the format and file type of the data and software used to collect and/or process the data.

## Metadata standards
Researchers are strongly encouraged to use community metadata standards where these are in place, consult e.g. [FAIRsharing.org](https://fairsharing.org/standards/?q=&selected_facets=status:Ready&selected_facets=expanded_onto_disciplines_exact:Life%20Science). Data repositories may also provide guidance about appropriate metadata standards and requirements e.g. [ENA sample checklists](https://www.ebi.ac.uk/ena/submit/checklists). It is highly recommended to, already from the beginning of the project, structure e.g. sample metadata in a way that enables sequence data submission  without having to reformat the metadata.

Below are examples of standards for Life Science community, adapted from Table 4 in *Griffin PC, Khadake J, LeMay KS et al. Best practice data life cycle approaches for the life sciences. F1000Research 2018, 6:1618.* doi: [10.12688/f1000research.12344.2](10.12688/f1000research.12344.2)

* [MINSEQE](http://fged.org/site_media/pdf/MINSEQE_1.0.pdf)
Minimum Information about a high- throughput SEQuencing Experiment. Developed by the Functional Genomics Data Society. Used in the NCBI Sequence Read Archive, ArrayExpress.


* [MIxS - MIGS/MIMS](http://wiki.gensc.org/index.php?title=MIGS/MIMS)  

Minimum Information about a (Meta)Genome Sequence. The  MIMS extension includes key environmental metadata. Developed by the Genomic Standards Consortium. Numerous adopters including NCBI/EBI/DDBJ databases.


* [MIMARKS](http://wiki.gensc.org/index.php?title=MIMARKS)  

Minimum Information about a MARKer gene Sequence. This is an extension of MIGS/MIMS for environmental sequences. Developed by the Genomic Standards Consortium. Numerous adopters including NCBI/EBI/DDBJ databases.


* [MIMIx](http://www.psidev.info/mimix)  

Minimum Information about a Molecular Interaction eXperiment. Developed by the Proteomics Standards Initiative. Adopted by the IMEx Consortium databases.
	

* [MIAPE](http://www.psidev.info/miape)  

Minimum Information About a Proteomics Experiment. Developed by the Proteomics Standards Initiative. Adopted by PRIDE, World-2DPAGE and ProteomeXchange databases.
	

* [Metabolomics Standards Initiative (MSI) standards](http://www.metabolomics-msi.org/)  

Minimal reporting structures that represent different parts of the metabolomics workflow. Developed by the Metabolomics Standards Initiative (MSI) and the Coordination of Standards in Metabolomics (COSMOS) consortium.


* [MIRIAM](http://co.mbine.org/standards/miriam)  

Minimal Information Required In the Annotation of Models. For annotation and curation of computational models in biology. Initiated by the BioModels.net effort. Adopted by the EBI BioModels database and others.


* [MIAPPE](http://cropnet.pl/phenotypes/wp-content/uploads/2016/04/MIAPPE.pdf)  

Minimum Information About a Plant Phenotyping Experiment. Covers study, environment, experimental design, sample management, biosource, treatment and phenotype. Adopted by the Plant Phenomics and Genomics Research Data Repository and the Genetic and Genomic Information System (GnpIS).


* [MDM](http://www.ebi.ac.uk/ena/submit/pathogen-data)  

Minimal Data for Mapping for sample and experimental metadata for pathogen genome-scale sequence data. Developed by the Global Microbial Identifier Initiative and EBI. Complies with EBI ENA database submission requirements.


* [FAANG sample metadata specification](https://github.com/FAANG/faang-metadata/blob/master/docs/faang_sample_metadata.md)  

Metadata specification for biological samples derived from animals (animals, tissue samples, cells or other biological materials). Complies with EBI database requirements and BioSamples database formats. Developed and used by the Functional Annotation of Animal Genomes Consortium.


* [FAANG experimental metadata specification](https://github.com/FAANG/faang-metadata/blob/master/docs/faang_experiment_metadata.md)  

Metadata specification for sequencing and array experiments on animal samples. Developed and used by the Functional Annotation of Animal Genomes Consortium.

## Ontologies

For a suggested list of ontologies appropriate for Life Science community please see [FAIRsharing.org](https://fairsharing.org/standards/?q=&selected_facets=status:Ready&selected_facets=expanded_onto_disciplines_exact:%20Life%20Science&selected_facets=type_exact:terminology%20artifact), filter on e.g. Domain.

Below are ontology resources, adapted from Table 2 in *Griffin PC, Khadake J, LeMay KS et al. Best practice data life cycle approaches for the life sciences. F1000Research 2018, 6:1618.* doi: [10.12688/f1000research.12344.2](10.12688/f1000research.12344.2)

* [Ontology Lookup Service](http://www.ebi.ac.uk/ols/) - 
Discover different ontologies and their contents.

* [OBO Foundry](http://obofoundry.org/) - Table of open biomedical ontologies with information
on development status, license and content.

* [Zooma](http://www.ebi.ac.uk/spot/zooma/) - Assign ontology terms using curated mapping.

* [Webulous](https://www.ebi.ac.uk/efo/webulous/) - 
Create new ontology terms easily.

* [Ontobee](http://www.ontobee.org) - A linked data server that facilitates ontology data
sharing, visualization, and use.

## Data dictionary

Capture any additional documentation needed to enable reuse of the data in Readme text files and [Data Dictionaries](https://help.osf.io/hc/en-us/articles/360019739054-How-to-Make-a-Data-Dictionary) that describe what all the variable names and values in your data really mean.
