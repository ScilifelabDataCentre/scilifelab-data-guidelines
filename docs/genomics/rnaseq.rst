.. |data_type| replace:: RNA sequencing

#################
|data_type|
#################
.. include:: ../template/intro.rst

.. include:: ../template/generation.rst

* `NGI <https://ngisweden.scilifelab.se/>`_ (National Genomics Infrastructure) 
  offers an infrastructure equipped with a comprehensive range of technology 
  platforms for next generation sequencing (NGS) and genotyping.

Data analysis
=============
Facilities which offer data analysis services for RNA-seq datasets:
Standard analyses (pipelines):
***********************************
* `NGI nf-core RNA-seq pipeline <https://github.com/nf-core/rnaseq/>`_

Project-specific analyses:
***********************************
`NBIS support <https://nbis.se/support>`_ (National Bioinformatics 
  Infrastructure Sweden) national research infrastructure offers bioinformatic 
  support in various forms for a wide range of areas including NGS, proteomics, 
  metabolomics and biostatistics.

.. include:: ../template/analysis_compute.rst

.. include:: ../template/storage.rst

Data sharing
=============
In the era of `FAIR </docs/general/fair_principles>`_ (Findable, Accessible, 
Interoperable and Reusable) and `Open science 
<https://www.vr.se/english/mandates/open-science/open-access-to-research-data.html>`_, 
datasets should be made available to the public. 

Repositories for RNA sequencing data (non-human)
**************************************************************
* European Nucleotide Archive (`ENA <https://www.ebi.ac.uk/ena>`_) for raw read 
  data
* `ArrayExpress <https://www.ebi.ac.uk/arrayexpress/>`_ for experiment 
  descriptions and processed expression data

Samples are linked between databases to make sure each part of the dataset is 
findable. Submitted data can be kept private until the associated research 
article is published (embargo). 

`ENA <https://www.ebi.ac.uk/ena>`_
------------------------------------------
The ENA hosts an instance of the Sequence Read Archive (SRA), the same 
archive that exists on NCBI. SRA accepts raw sequence data from any 
sequencing platform, generated in any research project. 

There are several ways to `submit <https://www.ebi.ac.uk/ena/submit>`_ 
data to ENA, including extensive documentation on `programmatic submissions 
<https://ena-docs.readthedocs.io/en/latest/programmatic.html>`_.

`ArrayExpress <https://www.ebi.ac.uk/arrayexpress/>`_
-------------------------------------------------------
ArrayExpress is tighty integrated with `ENA <https://www.ebi.ac.uk/ena>`_ 
and similar to NCBI's Gene Expression Omnibus database it can be used to 
archive experimental designs and analysis files based on the raw sequence 
reads. 

ArrayExpress has its own `submission portal 
<https://www.ebi.ac.uk/arrayexpress/submit/overview.html>`_ where information 
is available on what can be submitted and how.

Repositories for RNA sequencing data (human)
**************************************************************
NBIS is building a local federated version of the European Genome-phenome 
Archive (EGA) in Sweden (EGA-SE), allowing for the publication of sensitive 
personal data within a legal framework. Until local EGA is available, the 
dataset should remain in the secure analysis environment (eg at Bianca on 
Uppmax). We suggest to make a metadata-only record in the `SciLifeLab Data 
Repository <https://www.scilifelab.se/community-pages/systems-data/repository/>`_ 
with contact details on how to get access, and for which a DOI (ie a 
persistent identifier) can be issued. The DOI can then be used in the article 
to refer to the dataset. Once the Swedish EGA is operational, and the dataset 
deposited there, the access information can be changed to point at the EGA ID. 
See `https://doi.org/10.17044/NBIS/G000014 
<https://doi.org/10.17044/NBIS/G000014>`_, for an example.

.. include:: ../template/other_repos.rst

.. include:: ../template/metadata.rst

.. include:: ../template/feedback.rst
