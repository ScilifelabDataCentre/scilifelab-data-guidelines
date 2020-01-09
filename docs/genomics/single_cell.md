# Single-cell genomics
The data life cycle is typically divided into design, generation, analysis, storage & archiving, and sharing. Below you will find information about infrastructure resources available during these phases.

 ![](/docs/images/data_life_cycle_circle_logos.png)

## Data design
During this phase you plan for wich data is needed to answer your research question. High quality science is often only possible if the resource facilities you intend to use gets involved already in the planning phase of a project. Consultation and advice regarding data management planning, data generation and data analysis are offered by [NBIS](https://nbis.se/) and [SciLifeLab](https://www.scilifelab.se/). 

It is wise to write a data management plan, using either a tool provided by your university or [DS wizard](http://dsw.scilifelab.se/).

Also, some resources have specific application periods and thus needs to be contacted well in advance. If your project includes sensitive human data, note that there are ethical and legal issues that you have to consider, such as apply for an ethics approval and report the data processing to your [Data protection officer](/docs/general/data_protection_officer). See the page on [Sensitive personal data](/docs/general/sensitive_data) for more information.

## Data generation
Facilities which offer data generation services for single-cell genomics:

* [NGI](https://ngisweden.scilifelab.se/) (National Genomics Infrastructure) offers an infrastructure equipped with a comprehensive range of technology platforms for next generation sequencing (NGS) and genotyping.

* [Eukaryotic Single-Cell Genomics (ESCG)](http://escg.se/) offers streamlined single cell RNA sequencing, as well as whole genome DNA amplification

* [Microbial Single Cell Genomics](https://www.scilifelab.se/facilities/single-cell/)

Consider to upload the raw data to a repository already when receiving them, under an embargo. This way you always have an off-site backup with the added benefit of making the [Data sharing](#data-sharing) phase more efficient.

## Data analysis
Facilities which offer data analysis services for single-cell datasets:

* [NBIS](https://nbis.se/support/ "NBIS support") (National Bioinformatics Infrastructure Sweden) is a national research infrastructure that offers bioinformatic support in various forms for a wide range of areas including NGS, proteomics, metabolomics and biostatistics.

### Computational resources:
[SNIC](https://www.snic.se/ "SNIC homepage") (Swedish National Infrastructure for Computing) is a national research infrastructure that makes available large scale high performance computing resources. [Apply](https://www.snic.se/allocations/compute/ "SNIC compute") for Small, Medium, Large or Sensitive data allocation, depending on size and type of project.

## Data storage and archiving
After the project is finished, the data needs to be stored in a backed-up fashion at least for 10 years, and for as long as the data is of scientific value. After this time, some of the data should be archived and some can be disposed. It is best to contact your [university](/docs/general/research_data_office) for information about the procedures for this. 

[SNIC](https://www.snic.se/allocations/storage/ "SNIC storage") offers storage for small and medium-sized datasets. In the future also large-sized storage will be offered.

## Data sharing
In the era of [FAIR](https://www.force11.org/group/fairgroup/fairprinciples) (Findable, Accessible, Interoperable and Reusable) and [Open science](https://www.vr.se/english/mandates/open-science/open-access-to-research-data.html), datasets should be made available to the public. 

### Repositories appropriate for single-cell (non human) datasets

* European Nucleotide Archive ([ENA](https://www.ebi.ac.uk/ena)) for raw read data
* [ArrayExpress](https://www.ebi.ac.uk/arrayexpress/) for experiment descriptions and processed expression data

Samples are linked between databases to make sure each part of the dataset is findable. Submitted data can be kept private until the associated research article is published (embargo). 

##### [ENA](https://www.ebi.ac.uk/ena)

The ENA hosts an instance of the Sequence Read Archive (SRA), the same archive that exists on NCBI. SRA accepts raw sequence data from any sequencing platform, generated in any research project.  

**Submission**

There are several ways to [submit](https://www.ebi.ac.uk/ena/submit) data to ENA, including extensive documentation on [programmatic submissions](https://ena-docs.readthedocs.io/en/latest/programmatic.html).

##### [ArrayExpress](https://www.ebi.ac.uk/arrayexpress/)

ArrayExpress is tighty integrated with [ENA](https://www.ebi.ac.uk/ena) and similar to NCBI's Gene Expression Omnibus database it can be used to archive experimental designs and analysis files based on the raw sequence reads. 

**Submission**

ArrayExpress has its own [submission portal](https://www.ebi.ac.uk/arrayexpress/submit/overview.html) where information is available on what can be submitted and how.

#### Other repositories
For other domain-specific repositories, see e.g. [ELIXIR Core resources](https://elixir-europe.org/platforms/data/core-data-resources), or [FAIRsharing](https://fairsharing.org/databases/) (the latter can also assist in finding metadata standards suitable for describing your datasets). For datasets that do not fit into domain-specifik repositories, there are general repositories such as [Figshare](https://figshare.com/) and [Zenodo](https://zenodo.org/).

## Feedback
Any comments or questions? Please don't hesitate to send an email to [data-management@scilifelab.se](mailto:data-management@scilifelab.se)