# Recommendations for Host Genomics Data
Host genomics data is often coupled to human subjects. This comes with many ethical and legal obligations, such as apply for an ethics approval and report the data processing to your [Data protection officer](/docs/general/data_protection_officer). See the page on [Sensitive personal data](/docs/general/sensitive_data) for more information.

## General Recommendations
* Data sharing of not only summary statistics (or significant data) but also raw data (individual-level data) will foster a build-up of larger datasets. This will eventually allow identifying the determinants of phenotype more accurately.
* Especially for raw sequencing data make sure to include QC results and details of the sequencing platform used.
* Common terminologies for reporting statistical tests (e.g with [StatO](https://doi.org/10.25504/FAIRsharing.na5xp)) enable reuse and reproducibility.

## Repositories
Several different types of host genomics data are being collected for COVID-19 research. Some suitable repositories for these are:
* Gene expression: A curated list can be found in FAIRsharing (FAIRsharing 2020d) some specific examples are listed below. To achieve load balancing, it is in general recommended to choose the respective regional repository for data deposition. Note that INSDC resources synchronize most for their data sets daily (ex: EGA/JGA/dbGaP, ArrayExpress/GEA/GEO).
  *  Transcriptomics of human subjects (i.e., requiring authorized access):
■ European Genome-Phenome Archive (EGA) (FAIRsharing 2015d) (if the
data must be stored locally, EGA is working on a software package that
can be installed locally and connects to the central metadata archive for
findability)

  * Transcriptomics (cell lines/animals):
■ ENA (FAIRsharing 2015e), for submission documentation see (ENA-Docs 2020)

  * Gene expression arrays:
■ EBI ArrayExpress (FAIRsharing Team 2015a)

* Genome-wide association studies (GWAS): GWAS Catalog; EGA; GWAS Central
* Adaptive Immune Receptor Repertoire sequencing (AIRR-seq)1 data and annotations can be submitted to dedicated repositories: iReceptor Public Archive (FAIRsharing 2020e) or VDJServer (FAIRsharing 2018b). It is also possible to submit these data to general purpose repositories (SRA, Genbank), for this process there are detailed instructions (AIRR Community 2020).
## Data and metadata standards
1. Gene expression
1.1. Transcriptomics.
1.1.1. Preferred minimal metadata standard MINSEQE
1.1.2. Preferred file formats (sequencing-based):
1.1.2.1. Raw sequences: fastq (compression can be added with gzip)
1.1.2.2. Mapped sequences: .sam (compression with .bam or .cram)
1.1.2.3. Transcript count: TPM .csv
1.1.3. Also see FAIRsharing using the query ‘transcriptomics’
1.2. Microarrays:
1.2.1. Preferred minimal metadata standard: MIAME.
1.2.2. Preferred file formats tab-delimited text, raw data file formats from
commercial microarray platforms (Affymetrix, Illumina etc)
1 Adaptive Immune Receptor Repertoire sequencing (AIRR-seq) samples the diversity of the
immunoglobulins/antibodies and T cell receptors present in a host. The respective gene loci undergo
random and irreversible rearrangement during lymphocyte development, therefore this data is
fundamentally distinct from conventional genome sequencing.
RDA-COVID19 Working Group
RDA COVID-19; recommendations and guidelines, 3rd release 8 May 2020 45
2. Genome-wide association studies (GWAS):
2.1. Preferred minimal metadata standard: MIxS
2.2. Preferred file formats: for binary files: .bim .fam and .bed; for text-format files
.ped and .map.
3. Adaptive Immune Receptor Repertoire sequencing (AIRR-seq).
3.1. Preferred minimal metadata standards: MiAIRR
3.2. Preferred file formats:
3.2.1. AIRR repertoire metadata (formatted as .JSON or .YAML), AIRR
rearrangements (formatted as .TSV)
3.3. Also see FAIRsharing using the query ‘AIRR’.
