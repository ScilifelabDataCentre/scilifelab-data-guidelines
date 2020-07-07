# Recommendations for Virus Genomics Data
## Repositories
We suggest that raw virus sequence data as well as assembled and annotated genomes are submitted to [ENA](https://www.ebi.ac.uk/ena). 
* There are several ways to [submit](https://www.ebi.ac.uk/ena/submit) data to ENA, including [SARS-CoV-2 submission](https://ena-browser-docs.readthedocs.io/en/latest/help_and_guides/sars-cov-2-submissions.html) and extensive documentation on [programmatic submissions](https://ena-docs.readthedocs.io/en/latest/programmatic.html).
* Before submission of raw sequence data (e.g. shotgun sequencing) it is necessary to remove contaminating human reads. This can be done using e.g. [Metagen-FastQC](https://github.com/Finn-Lab/Metagen-FastQC), or ask for assistance at [virus-dataflow@ebi.ac.uk](mailto:virus-dataflow@ebi.ac.uk).

## Data and metadata standards
A list of relevant data and metadata standards can be found in [FAIRsharing](https://fairsharing.org/search/?q=genomics&content=standards), some specific examples are below.

### Data standards
We suggest that data is preferentially stored in the following formats, in order to maximize the interoperability with each other and with standard analysis pipelines:  
  * **Raw sequences:** [.fastq](https://support.illumina.com/bulletins/2016/04/fastq-files-explained.html), optionally add compression with gzip 
  * **Genome contigs:** [.fastq](https://support.illumina.com/bulletins/2016/04/fastq-files-explained.html) if uncertainties of the assembler can be captured, otherwise use [.fasta](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=BlastHelp); optionally add compression with gzip
  * **De novo aligned sequences:** [.afa](https://www.cgl.ucsf.edu/chimera/docs/ContributedSoftware/multalignviewer/afasta.html)
* **Gene Structure:** [.gtf](https://mblab.wustl.edu/GTF22.html)
* **Gene Features:** [.gff](https://github.com/The-Sequence-Ontology/Specifications/blob/master/gff3.md)
* **Sequences mapped to a genome:** [.sam](https://github.com/samtools/samtools) or the compressed formats [.bam](http://samtools.github.io/hts-specs/) or [.cram](https://www.ga4gh.org/cram/). Please ensure that the used reference sequence is also publically available and that the @SQ header is present and unambiguously describes the used reference sequence.
* **Variant calling:** [.vcf](http://samtools.github.io/hts-specs/). Please ensure that the used reference sequence is also publically available and that it is unambiguously referenced in the header of the .vcf file, e.g. using the URL field of the ##contig field.
* **Browser:** [.bed](http://genome.ucsc.edu/FAQ/FAQformat#format1)

### Metadata standards
Consider annotating virus genomes using the [ENA virus pathogen reporting standard checklist](https://www.ebi.ac.uk/ena/data/view/ERC000033), which is a minimal information standard under development right now and the more general [Viral Genome Annotation System](http://cefg.uestc.cn/vgas/) (VGAS) ([Zhang et al. 2019](https://doi.org/10.3389/fmicb.2019.00184)).

##### Phylogenetic analysis
For submitting data and metadata relating to phylogenetic relationships (including topology, branch lengths, and support values) consider using widely accepted formats such as [Newick](http://evolution.genetics.washington.edu/phylip/newicktree.html), [NEXUS](https://academic.oup.com/sysbio/article/46/4/590/1629695) and [PhyloXML](http://www.phyloxml.org/). The [Minimum Information About a Phylogenetic Analysis](https://github.com/evoinfo/miapa) checklist provides a reference list of useful tree annotations. 
