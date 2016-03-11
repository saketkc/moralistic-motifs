# moralistic-motifs
Review of motif finders with a focus on phylogenetic footprinting

## Motif Representation
1. Dinucleotide Dependencies(using PBM) [Improved models for transcription factor binding site identification using nonindependent interactions](http://www.genetics.org/content/genetics/early/2012/04/11/genetics.112.138685.full.pdf)

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
2. Dinucleotide Weight Matrices(DWM) [Dinucleotide weight matrices for predicting transcription
factor binding sites: generalizing the position weight matrix](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0009722) 

  > I describe a straightforward generalization of the PWM model, that considers frequencies of dinucleotides instead of individual nucleotides. Unlike previous efforts, this method considers all dinucleotides within an extended binding region, and does not make an attempt to determine a priori the significance of particular dinucleotide correlations. I describe how to use a “dinucleotide weight matrix” (DWM) to predict binding sites, dealing in particular with the complication that its entries are not independent probabilities. Benchmarks show, for many factors, a dramatic improvement over PWMs in precision of predicting known targets. In most cases, significant further improvement arises by extending the commonly defined “core motifs” by about 10bp on either side
  
3. Variable Width permitting representation/methods 
  1. [Prediction of nuclear hormone receptor response elements](http://press.endocrine.org/doi/full/10.1210/me.2004-0101)
  
      >New bioinformatics methods for the analysis of regulatory sequences are required to address the complex properties         associated with known regulatory elements targeted by the receptors because the standard methods for binding site           prediction fail to reflect the diverse target site configurations. We have constructed a flexible Hidden Markov Model       framework capable of predicting NHR binding sites. The model allows for variable spacing and orientation of      half-sites. 
  2. [Discovery of novel tumor suppressor p53 response elements using information theory](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2441790/pdf/gkn189.pdf)
      
      >An accurate method for locating genes under tumor suppressor p53 control that is based on a wellestablished mathematical theory and built using naturally occurring, experimentally proven p53 sites is essential in understanding the complete p53 network. We used a molecular information theory approach to create a flexible model for p53 binding.
By searching around transcription start sites in human chromosomes 1 and 2, we predicted 16
novel p53 binding sites and experimentally demonstrated that 15 of the 16 (94%) sites were bound by
p53.

  3. [The p53HMM algorithm: using profile hidden markov models to detect p53-responsive genes](http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-10-111)
  
    >A computational method (called p53HMM) is presented that utilizes Profile Hidden Markov Models (PHMMs) to estimate the relative binding affinities of putative p53 response elements (REs), both p53 single-sites and cluster-sites. These models incorporate a novel "Corresponded Baum-Welch" training algorithm that provides increased predictive power by exploiting the redundancy of information found in the repeated, palindromic p53-binding motif. The predictive accuracy of these new models are compared against other predictive models, including position specific score matrices (PSSMs, or weight matrices). We also present a new dynamic acceptance threshold, dependent upon a putative binding site's distance from the Transcription Start Site (TSS) and its estimated binding affinity. This new criteria for classifying putative p53-binding sites increases predictive accuracy by reducing the false positive rate.


## Reviews

1. [Evaluation of methods for modeling transcription factor sequence specificity - Weirauch and Hughes](http://www.nature.com/nbt/journal/v31/n2/pdf/nbt.2486.pdf) 
    > . Here we applied 26 such approaches to in vitro protein binding microarray data for 66 mouse TFs belonging to various families. For nine TFs, we also scored the resulting motif models on in vivo data, and found that the best in vitro–derived motifs performed similarly to motifs derived from the in vivo data.

2. [The Next Generation of Transcription Factor Binding Site Prediction
](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003214) - 2013 
  > We present a new graphical representation of the motifs that convey properties of position
  interdependence. TFFMs have been assessed on ChIP-seq data sets coming from the ENCODE project, revealing that
  they can perform better than both PWMs and the dinucleotide weight matrix extension in discriminating ChIP-seq from
  background sequences

3. [Modeling the specificity of protein-dna interactions - Stormo](http://link.springer.com/article/10.1007%2Fs40484-013-0012-4#/page-1)

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
  
- Deep Learning
  1. [Predicting the sequence specificities of DNA- and RNA-binding proteins by deep learning - ](http://www.nature.com/nbt/journal/v33/n8/pdf/nbt.3300.pdf)
  
- Beyond PWMs
  1. [Improved models for transcription factor binding site identification using non-independent interactions - Zhao and Stormo](http://www.genetics.org/content/191/3/781.full.pdf)
