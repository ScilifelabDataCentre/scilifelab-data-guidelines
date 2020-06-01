# Recommendations for Host Genomics Data
Host genomics data is often coupled to human subjects. This comes with many ethical and legal obligations, such as apply for an ethics approval and report the data processing to your [Data protection officer](/docs/general/data_protection_officer). See the page on [Sensitive personal data](/docs/general/sensitive_data) for more information.

## General Recommendations
* Data sharing of not only summary statistics (or significant data) but also raw data (individual-level data) will foster a build-up of larger datasets. This will eventually allow identifying the determinants of phenotype more accurately.
* Especially for raw sequencing data make sure to include QC results and details of the sequencing platform used.
* Common terminologies for reporting statistical tests (e.g with [StatO](http://stato-ontology.org/)) enable reuse and reproducibility.
* Researchers interested in human leukocyte antigen (HLA) genomics are referred to the [HLA COVID-19 consortium](http://hlacovid19.org/)

## Repositories
Several different types of host genomics data are being collected for COVID-19 research. Some suitable repositories for these are:

* **Gene expression**: A curated list can be found in FAIRsharing some specific examples are listed below. 

  *  **Transcriptomics of human subjects** (i.e. requiring authorized access): NBIS is building a local federated version of the European Genome-phenome Archive (EGA) in Sweden (EGA-SE), allowing for the publication of sensitive personal data within a legal framework. Until local EGA is available, the dataset should remain in the secure analysis environment (eg at Bianca on Uppmax). We suggest to make a metadata-only record in the [SciLifeLab Data Repository](https://scilifelab.figshare.com/) with contact details on how to get access, and for which a DOI (ie a persistent identifier) can be issued. The DOI can then be used in the article to refer to the dataset. Once the Swedish EGA is operational, and the dataset deposited there, the access information can be changed to point at the EGA ID. See [https://doi.org/10.17044/NBIS/G000014](https://doi.org/10.17044/NBIS/G000014), for an example.

  * **Transcriptomics (cell lines/animals)**: [ArrayExpress](https://www.ebi.ac.uk/arrayexpress/). The [submission portal](https://www.ebi.ac.uk/arrayexpress/submit/overview.html) gives information on what can be submitted and how. Underlying reads will  automatically be deposited to 
  European Nucleotide Archive [ENA](https://www.ebi.ac.uk/ena). 
  * **Microarray-based gene expression data**: [ArrayExpress](https://www.ebi.ac.uk/arrayexpress/). The [submission portal](https://www.ebi.ac.uk/arrayexpress/submit/overview.html) gives information on what can be submitted and how. Data on the originating sample will automatically be deposited to [BioSamples](https://www.ebi.ac.uk/biosamples/).

* **Genome-wide association studies (GWAS)**: [GWAS Catalog](https://www.ebi.ac.uk/gwas/); [GWAS Central](https://doi.org/10.25504/FAIRsharing.vkr57k); for human data requiring restricted access please see section on *Transcriptomics of human subjects* above.
* **Adaptive Immune Receptor Repertoire sequencing (AIRR-seq)**: Samples the diversity of the immunoglobulins/antibodies and T cell receptors present in a host. The respective gene loci undergo random and irreversible rearrangement during lymphocyte development, therefore this data is fundamentally distinct from conventional genome sequencing. 

   It is recommended that data be deposited using [AIRR Community](http://www.airr-community.org/) compliant processes and standards, in either of the following repositories:

   *  AIRR-seq specific repositories that are part of the [AIRR Data Commons](https://docs.airr-community.org/en/latest/api/adc.html), for example the [iReceptor Public Archive](https://fairsharing.org/FAIRsharing.ekdqe5)  or [VDJServer](https://vdjserver.org/)
   *  INSDC repositories via NCBI SRA/Genbank, following the AIRR Community recommended [NCBI
submission processes](https://docs.airr-community.org/en/latest/standards/data_submission.html#data-submission)

## Data and metadata standards
### Gene expression
#### Transcriptomics:
* Preferred minimal metadata standard: [MINSEQE](http://www.fged.org/projects/minseqe/)
* Preferred file formats (sequencing-based):
  * Raw sequences: [.fastq](https://www.open-bio.org/2009/12/17/nar-fastq-format/) (compression can be added with gzip)
  * Mapped sequences: [.sam](https://github.com/samtools/samtools) (compression with [.bam](http://genome.ucsc.edu/goldenPath/help/bam.html) or [.cram](https://www.sanger.ac.uk/science/tools/cram))
  * Transcripts per million (TPM): [.csv](https://tools.ietf.org/html/rfc4180)
* Also see [FAIRsharing using the query ‘transcriptomics’](https://fairsharing.org/standards/?q=transcriptomics)
#### Microarray-based gene expression data:
* Preferred minimal metadata standard: [MIAME](http://www.fged.org/projects/miame/)
* Preferred file formats: tab-delimited text eg [MAGE-TAB](http://fged.org/projects/mage-tab/) and [ISA-TAB](https://isa-tools.org/), and raw data file formats from commercial microarray platforms ([Annotare accepted formats](https://www.ebi.ac.uk/fg/annotare/help/accepted_raw_ma_file_formats.html))

### Genome-wide association studies (GWAS):
* Preferred minimal metadata standard: [MIxS](https://gensc.org/mixs/)
* Preferred file formats 
  *  for binary files: [.bim](https://www.cog-genomics.org/plink2/formats#bim), [.fam](https://www.cog-genomics.org/plink2/formats#fam) and [.bed](https://www.cog-genomics.org/plink2/formats#bed)
  *  for text-format files: [.ped](https://www.cog-genomics.org/plink2/formats#ped) and [.map](https://www.cog-genomics.org/plink2/formats#map)

### Adaptive Immune Receptor Repertoire sequencing (AIRR-seq).
* Preferred minimal metadata standards: [MiAIRR](https://docs.airr-community.org/en/latest/miairr/introduction_miairr.html)
* Preferred file formats: [AIRR repertoire metadata](https://docs.airr-community.org/en/latest/datarep/metadata.html#file-format-specification) (formatted as .json or .yaml), [AIRR rearrangements](https://docs.airr-community.org/en/latest/datarep/format.html#formatspecification) (formatted as .tsv)

