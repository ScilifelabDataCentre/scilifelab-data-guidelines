# Recommendations for Proteomics
Proteomics studies are used to find biomarkers for disease and susceptibility. 

## Repositories
For a curated list of relevant repositories see [FAIRsharing using the query ’proteomics’](https://fairsharing.org/search/?q=proteomics&content=biodbcore&name=&taxonomies=&organisations=&shortname=&description=&supportlinks=&licenses=&countries=&maintainers=&expanded_onto_domains=&expanded_onto_disciplines=&user_defined_tags=&record_id=&miriam_id=&search_state=hidden). The [ProteomeXchange Consortium](https://doi.org/10.25504/FAIRsharing.92dt9d) enables searches across the following deposition databases, following common standards.
 
* For shotgun proteomics use [PRIDE](https://www.ebi.ac.uk/pride/)
* For targeted proteomics use [Panorama](https://panoramaweb.org/project/home/begin.view) or [PASSEL](http://www.peptideatlas.org/passel/)
* For repossessed results use [PeptideAtlas](http://www.peptideatlas.org/) or [MassIVE](https://massive.ucsd.edu/)

## Data and metadata standards
For a curated list of relevant standards see [FAIRsharing using the query ’proteomics’](https://fairsharing.org/search/?q=proteomics&content=standard&name=&taxonomies=&organisations=&shortname=&description=&supportlinks=&licenses=&countries=&maintainers=&expanded_onto_domains=&expanded_onto_disciplines=&user_defined_tags=&record_id=&miriam_id=&search_state=hidden).

* Use the minimal information model specified in [MIAPE](http://www.psidev.info/miape) by the HUPO Proteomics Standards
Initiative ([HUPO PSI](https://doi.org/10.1038/nbt1329)), and fill the model using the controlled vocabularies specified by the Proteomics Standards Initiative, [PSI CVs](http://www.psidev.info/groups/mass-spectrometry#controlled)
* Recommended formats: 
  * For gel electrophoresis [gelML](http://www.psidev.info/gelml/1.0)
  * For transition lists [TraML](http://www.psidev.info/traml)
  * For raw spectrometer output [mzML](http://www.psidev.info/mzml)
  * For reporting [mzTab](http://www.psidev.info/mztab)
  * For protein quantisation data [mzQuantML](http://www.psidev.info/mzquantml)
  * For protein identification data [mzIdentML](http://www.psidev.info/mzidentml)
  * For metadata [ISA-TAB](https://isa-tools.org/) with conversion to PRIDE format
