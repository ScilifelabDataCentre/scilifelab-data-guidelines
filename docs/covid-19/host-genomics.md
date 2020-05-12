# Recommendations for Host Genomics Data
Host genomics data is often coupled to human subjects. This comes with many ethical and legal obligations, such as apply for an ethics approval and report the data processing to your [Data protection officer](/docs/general/data_protection_officer). See the page on [Sensitive personal data](/docs/general/sensitive_data) for more information.

## General Recommendations
* Data sharing of not only summary statistics (or significant data) but also raw data (individual-level data) will foster a build-up of larger datasets. This will eventually allow identifying the determinants of phenotype more accurately.
* Especially for raw sequencing data make sure to include QC results and details of the sequencing platform used.
* Common terminologies for reporting statistical tests (e.g with [StatO](https://doi.org/10.25504/FAIRsharing.na5xp)) enable reuse and reproducibility.
* Researchers interested in HLA genomics are referred to the [HLA COVID-19 consortium](http://hlacovid19.org/)

## Repositories
Several different types of host genomics data are being collected for COVID-19 research. Some suitable repositories for these are:

* **Gene expression**: A curated list can be found in FAIRsharing (FAIRsharing 2020d) some specific examples are listed below. To achieve load balancing, it is in general recommended to choose the respective regional repository for data deposition. Note that INSDC resources synchronize most for their data sets daily (ex: EGA/JGA/dbGaP, ArrayExpress/GEA/GEO).

  *  **Transcriptomics of human subjects** (i.e. requiring authorized access): NBIS is building a local federated version of the European Genome-phenome Archive (EGA) in Sweden (EGA-SE), allowing for the publication of sensitive personal data within a legal framework. Until local EGA is available, the dataset should remain in the secure analysis environment (eg at Bianca on Uppmax). We suggest to make a metadata-only record in the [SciLifeLab Data Repository](https://scilifelab.figshare.com/) with contact details on how to get access, and for which a DOI (ie a persistent identifier) can be issued. The DOI can then be used in the article to refer to the dataset. Once the Swedish EGA is operational, and the dataset deposited there, the access information can be changed to point at the EGA ID. See [https://doi.org/10.17044/NBIS/G000014](https://doi.org/10.17044/NBIS/G000014), for an example.

  * **Transcriptomics (cell lines/animals)**: European Nucleotide Archive [ENA](https://www.ebi.ac.uk/ena). There are several ways to [submit](https://www.ebi.ac.uk/ena/submit) data to ENA, including extensive documentation on [programmatic submissions](https://ena-docs.readthedocs.io/en/latest/programmatic.html).
  * **Gene expression arrays**: [ArrayExpress](https://www.ebi.ac.uk/arrayexpress/). The [submission portal](https://www.ebi.ac.uk/arrayexpress/submit/overview.html) gives information on what can be submitted and how.

<!--- * **Genome-wide association studies (GWAS)**: [GWAS Catalog](https://doi.org/10.25504/FAIRsharing.blUMRx); EGA; [GWAS Central](https://doi.org/10.25504/FAIRsharing.vkr57k)
* **Adaptive Immune Receptor Repertoire sequencing (AIRR-seq)**: samples the diversity of the immunoglobulins/antibodies and T cell receptors present in a host. The respective gene loci undergo random and irreversible rearrangement during lymphocyte development, therefore this data is fundamentally distinct from conventional genome sequencing. AIRR-seq data and annotations can be submitted to dedicated repositories: [iReceptor Public Archive](https://fairsharing.org/search/?q=AIRR) or [VDJServer](https://fairsharing.org/FAIRsharing.nzdq0f). It is also possible to submit these data to general purpose repositories (SRA, Genbank), for this process there are detailed instructions ([AIRR Community 2020](https://docs.airr-community.org/en/latest/api/adc_api.html)). -->

## Data and metadata standards
### Gene expression
#### Transcriptomics:
* Preferred minimal metadata standard: [MINSEQE](https://doi.org/10.25504/FAIRsharing.a55z32)
* Preferred file formats (sequencing-based):
  * Raw sequences: .fastq (compression can be added with gzip)
  * Mapped sequences: [.sam](https://doi.org/10.25504/FAIRsharing.r2ts5t) (compression with [.bam](https://doi.org/10.25504/FAIRsharing.hza1ec) or .cram)
  * Transcript count: TPM .csv
* Also see [FAIRsharing using the query ‘transcriptomics’](https://fairsharing.org/standards/?q=transcriptomics)
#### Microarrays:
* Preferred minimal metadata standard: [MIAME](https://doi.org/10.25504/FAIRsharing.32b10v)
* Preferred file formats tab-delimited text, raw data file formats from
commercial microarray platforms (Affymetrix, Illumina etc)

<!--- ### Genome-wide association studies (GWAS):
* Preferred minimal metadata standard: [MIxS](https://doi.org/10.25504/FAIRsharing.9aa0zp)
* Preferred file formats: for binary files: .bim .fam and [.bed](https://doi.org/10.25504/FAIRsharing.mwmbpq); for text-format files .ped and .map

### Adaptive Immune Receptor Repertoire sequencing (AIRR-seq).
* Preferred minimal metadata standards: [MiAIRR](https://docs.airr-community.org/en/latest/miairr/introduction_miairr.html)
* Preferred file formats: [AIRR repertoire metadata](https://docs.airr-community.org/en/latest/datarep/metadata.html#file-format-specification) (formatted as .JSON or .YAML), [AIRR rearrangements](https://docs.airr-community.org/en/latest/datarep/format.html#formatspecification) (formatted as .TSV)
* Also see [FAIRsharing using the query ‘AIRR’](https://fairsharing.org/search/?q=AIRR) -->

