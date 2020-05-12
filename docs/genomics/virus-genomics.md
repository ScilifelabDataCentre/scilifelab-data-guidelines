# Recommendations for Virus Genomics Data
We suggest that raw virus sequence data as well as assembled and annotated genomes are submitted to ENA. Before submission of raw sequence data (e.g.,
 shotgun sequencing) it is necessary to remove contaminating human reads.

There are several specialized COVID-19 portals, https://www.covid19dataportal.se/ https://www.covid19dataportal.org/

## Data and metadata standards
A list of relevant data and metadata standards can be found in FAIRsharing (FAIRsharing 2020c), some specific examples are below.

### Data standards
We suggest that data is preferentially stored in the following formats, in order to maximize the interoperability with each other and with standard analysis pipelines:  
  * **Raw sequences:** .fastq (FAIRsharing 2015g); optionally add compression with gzip 
  * **Genome contigs:** .fastq if uncertainties of the assembler can be captured, .fasta (FAIRsharing 2015f) otherwise; optionally add compression with gzip
  * **De novo aligned sequences:** .afa
* **Gene Structure:** .gtf (FAIRsharing 2015h)
* **Gene Features:** .gff (FAIRsharing 2015i)
* **Sequences mapped to a genome:** .sam (FAIRsharing 2015m) or the compressed formats .bam (FAIRsharing 2015a) or .cram. Please ensure that the used reference sequence is also publically available and that the @SQ header is present and unambiguously describes the used reference sequence.
* **Variant calling:** .vcf (FAIRsharing 2015o). Please ensure that the used reference sequence is also publically available and that it is unambiguously referenced in the header of the .vcf file, e.g., using the URL field of the ##contig field.
* **Browser:** .bed (FAIRsharing 2015b)

### Metadata standards
Consider annotating virus genomes using the ENA virus pathogen reporting standard checklist (European Nucleotide Archive 2020), which is a minimal information standard under development right now and the more general Viral Genome Annotation System (VGAS) (Zhang et al. 2019).

##### Phylogenetic analysis
For submitting data and metadata relating to phylogenetic relationships (including topology, branch lengths, and support values) consider using widely accepted formats such as Newick, NEXUS and PhyloXML (Stoltzfus et al. 2012). The Minimum Information About a Phylogenetic Analysis (Lapp 2017) checklist provides a reference list of useful tree annotations. 
