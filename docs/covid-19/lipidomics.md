# Recommendations for Lipidomics

Lipidomics revealed an altered lipid composition in infected cells and serum lipid levels in patients with preexisting conditions. Lipid rafts (lipid microdomains) play a critical role in viral infections facilitating virus entry, replication, assembly and budding. Lipid rafts are enriched in glycosphingolipids, sphingomyelin and cholesterol. It is likely that SARS-CoV-2 enters the cell via angiotensin-converting enzyme-2 (ACE2) that depends on the integrity of lipid rafts in the infected cell membrane. 

## General Recommendations for Researchers
Lipidomics analysis should follow the guidelines of the [Lipidomic Standards Initiative](https://lipidomics-standards-initiative.org/guidelines)

## Repositories
The largest repository for lipidomics data is [Metabolights](https://www.ebi.ac.uk/metabolights/) 

## Data and metadata standards

* Metadata should follow recommendations from the [CIMR standard](http://msi-workgroups.sourceforge.net/bio-metadata/) by the Metabolomics Standards Initiative. It should be made available as tab or comma separated files (.tsv or .csv).

* Data can be stored in LC-MS file,  in tab (.tsv) or comma (.csv) separated formats.

### Data analysis
* Most of the analysis is usually performed using the software delivered by the suppliers of the instrumentation. In line with generic software recommendations it should be made sure that the process and parameters are well described, and that the output is converted to a standard format.

* [Workflow for Metabolomics (W4M)](https://workflow4metabolomics.org/) is a collaborative portal dedicated to metabolomics data
processing, analysis and annotation for Metabolomics community.

* Data processing using [R software](https://www.r-project.org/) and associated packages from [Bioconductor](https://www.bioconductor.org/) ([xcms](https://www.bioconductor.org/packages/release/bioc/html/xcms.html), [camera](https://www.bioconductor.org/packages/release/bioc/html/CAMERA.html), [mixOmics](https://bioconductor.org/packages/release/bioc/html/mixOmics.html))  is a flexible and reproducible way for lipidomic data analysis.
### Compound identification
* After data processing, potential biomarkers should be annotated. This could be done either by manual ([Lipid Maps tools](http://www.lipidmaps.org/tools/ms/))  or automated identification against templates ([Library templates for compounds identification](http://prime.psc.riken.jp/compms/msdial/main.html#MSP)) with the help of software such as [LipidBlast](https://fiehnlab.ucdavis.edu/projects/LipidBlast), [MSPepSearch](https://chemdata.nist.gov/dokuwiki/doku.php?id=peptidew:mspepsearch) or [MS-DIAL](http://prime.psc.riken.jp/compms/msdial/main.html).

* Lipids classification and nomenclature should follow the [LIPID MAPS guidelines](https://www.lipidmaps.org/resources/tutorials/lipid_cns.html)
