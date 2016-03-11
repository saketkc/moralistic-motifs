# moralistic-motifs
Review of motif finders with a focus on phylogenetic footprinting

## Motif Representation/Modeling variation
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

    >I describe a straightforward generalization of the PWM model, that considers frequencies of dinucleotides instead of      individual nucleotides. Unlike previous efforts, this method considers all dinucleotides within an extended binding    
    region, and does not make an attempt to determine a priori the significance of particular dinucleotide correlations.       describe how to use a “dinucleotide weight matrix” (DWM) to predict binding sites, dealing in particular with the          complication that its entries are not independent probabilities. Benchmarks show, for many factors, a dramatic             improvement over PWMs in precision of predicting known targets. In most cases, significant further improvement arises      by extending the commonly defined “core motifs” by about 10bp on either side
  
3. Variable Width permitting representation/methods 
  1. [Prediction of nuclear hormone receptor response elements](http://press.endocrine.org/doi/full/10.1210/me.2004-0101)
      
      >New bioinformatics methods for the analysis of regulatory sequences are required to address the complex properties         associated with known regulatory elements targeted by the receptors because the standard methods for binding site          prediction fail to reflect the diverse target site configurations. We have constructed a flexible Hidden Markov            Model framework capable of predicting NHR binding sites. The model allows for variable spacing and orientation of          half-sites. 

  2. [Discovery of novel tumor suppressor p53 response elements using information theory](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2441790/pdf/gkn189.pdf)
      
      >An accurate method for locating genes under tumor suppressor p53 control that is based on a wellestablished               mathematical theory and built using naturally occurring, experimentally proven p53 sites is essential in                   understanding the complete p53 network. We used a molecular information theory approach to create a flexible model         for p53 binding.
      By searching around transcription start sites in human chromosomes 1 and 2, we predicted 16
      novel p53 binding sites and experimentally demonstrated that 15 of the 16 (94%) sites were bound by
      p53.

  3. [The p53HMM algorithm: using profile hidden markov models to detect p53-responsive genes](http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-10-111)
  
      >A computational method (called p53HMM) is presented that utilizes Profile Hidden Markov Models (PHMMs) to estimate        the relative binding affinities of putative p53 response elements (REs), both p53 single-sites and cluster-sites.          These models incorporate a novel "Corresponded Baum-Welch" training algorithm that provides increased predictive           power by exploiting the redundancy of information found in the repeated, palindromic p53-binding motif. The                predictive accuracy of these new models are compared against other predictive models, including position specific          score matrices (PSSMs, or weight matrices). We also present a new dynamic acceptance threshold, dependent upon a           putative binding site's distance from the Transcription Start Site (TSS) and its estimated binding affinity. This new       criteria for classifying putative p53-binding sites increases predictive accuracy by reducing the false positive           rate.

4.  Linear Model: [A linear model for transcription factor binding affinity prediction in protein binding microarrays](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0020059)

      >We present a linear model for predicting the binding affinity of a protein toward DNA sequences based on PBM data.        Our model represents the measured intensity of an individual probe as a sum of the binding affinity contributions of       the probe's subsequences. These subsequences characterize a DNA binding motif and can be used to predict the               intensity of protein binding against arbitrary DNA sequences

5. Linear Regression: [An Interaction-Dependent Model for Transcription Factor Binding](http://www-stat.wharton.upenn.edu/~stjensen/papers/shanejensen.interact06.pdf)  

      >The a priori expectation is that the presence or
      absence of the estimated motif in a promoter should be a good indicator of the
      binding of the TF to that promoter. This association between the presence of the
      transcription factor motif and its binding is however weak in a majority of cases
      where the whole genome ChIP experiments have been performed. One possible
      reason for this is that the DNA binding of a particular transcription factor
      depends not only on its own motif, but also on synergistic or antagonistic action
      of neighboring motifs for other transcription factors. We believe that modeling
      this interaction-dependent binding with linear regression can better explain the
      observed binding data. 
  
6. Biophysical [Inferring binding energies from selected binding](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000590)
  
    >We employ a biophysical model that accounts for the non-linear relationship between binding energy and the statistics     of selected binding sites. The model includes the chemical potential of the transcription factor, non-specific binding     affinity of the protein for DNA, as well as sequence-specific parameters that may include non-independent contributions     of bases to the interaction. 

## Reviews

1. [Evaluation of methods for modeling transcription factor sequence specificity - Weirauch and Hughes](http://www.nature.com/nbt/journal/v31/n2/pdf/nbt.2486.pdf) 
    
    >Here we applied 26 such approaches to in vitro protein binding microarray data for 66 mouse TFs belonging to various      families. For nine TFs, we also scored the resulting motif models on in vivo data, and found that the best in              vitro–derived motifs performed similarly to motifs derived from the in vivo data.

2. [The Next Generation of Transcription Factor Binding Site Prediction - Matthelier and Wasserman (2013)](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003214) 
  
    >We present a new graphical representation of the motifs that convey properties of position
    interdependence. TFFMs have been assessed on ChIP-seq data sets coming from the ENCODE project, revealing that
    they can perform better than both PWMs and the dinucleotide weight matrix extension in discriminating ChIP-seq from
    background sequences

3. [Assessment of Algorithms for Inferring Positional Weight Matrix Motifs of Transcription Factor Binding Sites Using Protein Binding Microarray Data - Orenstein and Shamir (2012)](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0046145) 

    >We present a systematic comparison of four methods developed specifically for reconstructing a binding site motif         represented as a positional weight matrix from PBM data.

4. [Motif discovery and transcription factor binding sites before and after the next-generation sequencing era - Zambelli and Pavesi (2012)](http://bib.oxfordjournals.org/content/14/2/225.full.pdf)
  
    >ChIP, applied to transcription factors and coupled with genome tiling arrays (ChIP on Chip) or next-generation sequencing technologies (ChIP-Seq) has opened new avenues in research, as well as posed new challenges to bioinformaticians developing algorithms and methods for motif discovery.

4. [Regulatory Motif Analysis - Moses and Sinha (2009)](http://link.springer.com/chapter/10.1007%2F978-0-387-92738-1_7)
    > Comprehensive review 

5. [Assessment of composite motif discovery methods - Kreppler and Drablos(2008)](http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-9-123)
  
    >Traditionally, most of these methods have addressed the problem of single motif discovery – discovering binding motifs     for individual transcription factors. In higher organisms, however, transcription factors usually act in combination       with nearby bound factors to induce specific regulatory behaviours. Hence, recent focus has shifted from single motifs     to the discovery of sets of motifs bound by multiple cooperating transcription factors, so called composite motifs or      cis-regulatory modules. Given the large number and diversity of methods available, independent assessment of methods       becomes important. Although there have been several benchmark studies of single motif discovery, no similar studies        have previously been conducted concerning composite motif discovery.

6. [A survey of motif discovery methods in an integrated framework - Sandve and Drablos (2006)](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1479319/)
  
    >Several recent methods try to integrate additional sources of information, including microarray experiments (gene         expression and ChlP-chip). There is also a growing awareness that regulatory elements work in combination, and that        this combinatorial behavior must be modeled for successful motif discovery. However, the multitude of methods and          approaches makes it difficult to get a good understanding of the current status of the field.

7. [Improved benchmarks for computational motif discovery - Sandve and Drablos (2007)](http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-8-193) 
  
    >An important step in annotation of sequenced genomes is the identification of transcription factor binding sites. More     than a hundred different computational methods have been proposed, and it is difficult to make an informed choice.         Therefore, robust assessment of motif discovery methods becomes important, both for validation of existing tools and       for identification of promising directions for future research.

8. [Locating mammalian transcription factor binding sites: A survey of computational and experimental techniques - Elnitski, Farnham, Jones (2006)](http://genome.cshlp.org/content/16/12/1455.full.pdf) 
  
    >This review summarizes approaches for in silico, in vitro, and in vivo identification of transcription factor
    binding sites. A variety of techniques useful for localized- and high-throughput analyses are discussed here, with
    emphasis on aspects of data generation and verification.

9. [Assessing computational tools for the discovery of transcription factor binding sites - Tompa and Zhu (2005)](http://www.nature.com/nbt/journal/v23/n1/pdf/nbt1053.pdf) 
    
    >The prediction of regulatory elements is a problem where computational methods offer great hope. Over the past few        years, numerous tools have become available for this task. The purpose of the current assessment is twofold: to provide     some guidance to users regarding the accuracy of currently available tools in various settings, and to provide a           benchmark of data sets for assessing future tools.

10. [Limitations and potentials of current motif discovery algorithms - Hu and Kihara (2005)](http://nar.oxfordjournals.org/content/33/15/4899.full.pdf)
    
    >Here, we designed a comprehensive set of performance measures and benchmarked five modern sequence-based motif            discovery algorithms using large datasets generated from Escherichia coli RegulonDB. 

11. [Modeling the specificity of protein-dna interactions - Stormo (2000)](http://link.springer.com/article/10.1007%2Fs40484-013-0012-4#/page-1)


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
