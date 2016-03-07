# moralistic-motifs
Review of motif finders with a focus on phylogenetic footprinting

## Motif Representation
1. [Improved models for transcription factor binding site identification using nonindependent interactions](http://www.genetics.org/content/genetics/early/2012/04/11/genetics.112.138685.full.pdf)

  >The specificity of most TFs is currently modeled using
  position weight matrices (PWMs) that assume the positions within a binding site
  contribute independently to binding affinity for any site. Extensive, highthroughput
  quantitative binding assays let us examine, for the first time, the
  independence assumption for many TFs.  We introduce a binding energy model (BEM) that can include
  energy parameters for non-independent contributions to binding affinity. We
  show that in most cases where a PWM is not sufficient, a BEM that includes
  energy parameters for adjacent di-nucleotide contributions models the specificity
  very well. Having more accurate models of specificity greatly improves the
  interpretation of in vivo TF localization data, such as from ChIP-seq experiments. 
2. 

## Reviews

1. [The Next Generation of Transcription Factor Binding Site Prediction
](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003214) - 2013 
  > We present a new graphical representation of the motifs that convey properties of position
  interdependence. TFFMs have been assessed on ChIP-seq data sets coming from the ENCODE project, revealing that
  they can perform better than both PWMs and the dinucleotide weight matrix extension in discriminating ChIP-seq from
  background sequences

2. [Modeling the specificity of protein-dna interactions - Stormo](http://link.springer.com/article/10.1007%2Fs40484-013-0012-4#/page-1)

## Methods for TFBS prediction

- Phylogenetic Footprinting
  1. [Discovery of functional elements in 12 Drosophila genomes using evolutionary signatures - Stark, Kellis et al.](http://www.nature.com/nature/journal/v450/n7167/pdf/nature06340.pdf)

- Experimentally mapped TSS data to focus on promoter proximal regions
  1. [Improved detection of motifs with preferential location in promoters - Bernard and Brunaud](http://www.nrcresearchpress.com.sci-hub.io/doi/abs/10.1139/g10-042?url_ver=Z39.88-2003&rfr_id=ori%3Arid%3Acrossref.org&rfr_dat=cr_pub%3Dpubmed&) NOTE: The link is `sci-hub.io`, not available to USC otherwise
  
- Histone Modification or DNA Accessiblity information
  1. [Sequence and chromatin determinants of cell-type-specific transcription factor binding - Arvey, Leslie](http://genome.cshlp.org/content/22/9/1723.full.pdf)

- Density of local motifs
  1. [oPOSSUM: identification of over-represented transcription factor binding sites
in co-expressed genes - Sui, Walsh](http://nar.oxfordjournals.org/content/33/10/3154.full-text-lowres.pdf)
  2. [oPOSSUM: integrated tools for analysis of regulatory motif over-representation- Ho Sui, Wasserman](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1933229/pdf/gkm427.pdf) 
