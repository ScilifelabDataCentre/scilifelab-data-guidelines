.. |data_type| replace:: Whole-genome sequencing (human)

#################
|data_type|
#################
.. include:: ../template/intro.rst

.. include:: ../template/generation.rst

* `NGI <https://ngisweden.scilifelab.se/>`_ (National Genomics Infrastructure) 
  offers an infrastructure equipped with a comprehensive range of technology 
  platforms for next generation sequencing (NGS) and genotyping.

.. include:: ../template/analysis.rst

.. 
  include:: ../template/analysis_compute.rst

Computational resources
**************************
`SNIC <https://www.snic.se/>`_ (Swedish National Infrastructure for Computing) national research infrastructure makes available large scale high performance computing resources. The SNIC-SENS Bianca system is designed to be used for processing sensitive human data. See the instructions for `applying for a Bianca project <https://www.uppmax.uu.se/support/getting-started/applying-for-sens-project/>`_.

* Note that in case you work at a different institute than Uppsala University, you need a data processing agreement between your institute and UPPMAX/Uppsala University for using the Bianca system - see `instructions at UPPMAX <https://www.uppmax.uu.se/support/faq/general-miscellaneous-faq/sensitive+data+questions/>`_.

Data storage and archiving
==========================
After the project is finished, the data needs to be stored in a backed-up fashion 
at least for 10 years, and for as long as the data is of scientific value. After 
this time, some of the data should be archived and some can be disposed. It is 
best to contact your :doc:`university </docs/general/research_data_office>` for 
information about the procedures for this. 

Data sharing
=============
In the era of `FAIR </docs/general/fair_principles>`_ (Findable, Accessible, 
Interoperable and Reusable) and `Open science 
<https://www.vr.se/english/mandates/open-science/open-access-to-research-data.html>`_, 
datasets should be made available to the public. 

Repositories for Whole-genome sequencing data (human)
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
See `https://doi.org/10.17044/scilifelab.12292778 
<https://doi.org/10.17044/scilifelab.12292778>`_, for an example.

.. include:: ../template/metadata.rst

.. include:: ../template/feedback.rst
