# Recommendations for Virus Genomics Data
## Repositories
We suggest that raw virus sequence data as well as assembled and annotated genomes are submitted to [ENA](https://www.ebi.ac.uk/ena). 
* There are several ways to [submit](https://www.ebi.ac.uk/ena/submit) data to ENA, including [SARS-CoV-2 submission](https://ena-browser-docs.readthedocs.io/en/latest/help_and_guides/sars-cov-2-submissions.html) and extensive documentation on [programmatic submissions](https://ena-docs.readthedocs.io/en/latest/programmatic.html).
* Before submission of raw sequence data (e.g. shotgun sequencing) it is necessary to remove contaminating human reads.

## Data and metadata standards
A list of relevant data and metadata standards can be found in [FAIRsharing](https://fairsharing.org/search/?q=genomics&content=standards), some specific examples are below.

### Data standards
We suggest that data is preferentially stored in the following formats, in order to maximize the interoperability with each other and with standard analysis pipelines:  
  * **Raw sequences:** [.fastq](https://doi.org/10.25504/FAIRsharing.r2ts5t) optionally add compression with gzip 
  * **Genome contigs:** [.fastq](https://doi.org/10.25504/FAIRsharing.r2ts5t) if uncertainties of the assembler can be captured, [.fasta](https://doi.org/10.25504/FAIRsharing.rz4vfg) otherwise; optionally add compression with gzip
  * **De novo aligned sequences:** .afa
* **Gene Structure:** [.gtf](https://doi.org/10.25504/FAIRsharing.sggb1n)
* **Gene Features:** [.gff](https://doi.org/10.25504/FAIRsharing.dnk0f6)
* **Sequences mapped to a genome:** [.sam](https://doi.org/10.25504/FAIRsharing.hza1ec) or the compressed formats [.bam](https://doi.org/10.25504/FAIRsharing.hza1ec) or .cram. Please ensure that the used reference sequence is also publically available and that the @SQ header is present and unambiguously describes the used reference sequence.
* **Variant calling:** [.vcf](https://doi.org/10.25504/FAIRsharing.cfzz0h). Please ensure that the used reference sequence is also publically available and that it is unambiguously referenced in the header of the .vcf file, e.g. using the URL field of the ##contig field.
* **Browser:** [.bed](https://doi.org/10.25504/FAIRsharing.mwmbpq)

### Metadata standards
Consider annotating virus genomes using the [ENA virus pathogen reporting standard checklist](https://www.ebi.ac.uk/ena/data/view/ERC000033), which is a minimal information standard under development right now and the more general Viral Genome Annotation System (VGAS) ([Zhang et al. 2019](https://doi.org/10.3389/fmicb.2019.00184)).

##### Phylogenetic analysis
For submitting data and metadata relating to phylogenetic relationships (including topology, branch lengths, and support values) consider using widely accepted formats such as Newick, NEXUS and PhyloXML ([Stoltzfus et al. 2012](httpf://doi.org/10.1186/1756-0500-5-574)). The [Minimum Information About a Phylogenetic Analysis](https://github.com/evoinfo/miapa)  checklist provides a reference list of useful tree annotations. 
