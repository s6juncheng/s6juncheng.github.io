---
permalink: /research/
title: "Research"
author_profile: true
redirect_from: 
  - /md/
  - /research.html
---

{% include base_path %}

Recent years have seen revolutionary progress in high throughput biology and machine learning, yet much is to be done to combine the progress in these two fields. 
My research focuses on the development and application of machine learning methods on large-scale biological data for more precise understanding of human disease.
The methods can be used, for example, to diagnose genetic diseases, to predict cancer driver mutation, to stratify cancer patients, and to design effective vaccines. 
I’m passionate about drawing insights from complex biological data and developing methods with high impact applications. 
I’m also interested in pushing the state-of-the-art in machine learning.

## Variant Effect Prediction with Machine Learning Models
A human genome encodes information about gene expression regulation, which is essential to an individual's well-being. 
However, our current understanding of genetic determinants of gene expression regulation is still limited. 
Consequently, we do not know the disease impact of most genetic variants, nor can we interpret most of the variants associated with diseases. 
A challenging task in human genetics is to precisely locate disease causing mutations among thousands of genetic variants found in any individual.

A part of my research is to train machine learning models taking genetic variants as input to predict their functional and disease impact.
My previous research in this area focused on RNA splicing and RNA degradation. 
We trained a neural network model from large-scale perturbation assays and genome annotation data to predict variant effects on splicing. 
The model, MMSplice, can precisely predict splicing level change subject to variants (Figure 1) ([Cheng et al., 2019](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1653-z)). 
MMSplice is the winning model for the [CAGI5 public splicing challenge](https://genomeinterpretation.org/content/vex-seq) and 
has been integrated to the popular variant effect predictor [CADD](https://cadd.gs.washington.edu/news). 

![](/images/ISM.png)
<sub>**Figure 1** In-silico mutagenesis analysis of example MMSplice predictions. Red color indicates variant increase Ψ while blue color 
indicates variant decrease Ψ. Alphabet letter height indicates effect magnitude. Gray bars are gene structure schema, 
thick ones are exons while thin ones are introns.</sub>

The limitation of MMSplice and other methods on variant interpretation for splicing is the lack of tissue specificity. 
To overcome this limitation, we developed MTSplice which combines MMSplice and a tissue-specific splicing level prediction model to predict tissue-specific variant effects ([Cheng et al., 2020](https://www.biorxiv.org/content/10.1101/2020.06.07.138453v1)).
We show that MTSplice can capture tissue-specific disease signals related to Autism Spectrum Disorder when comparing the predicted functional scores in the proband group and the unaffected sibling control group (Figure 2).

![](/images/ASD.png)
<sub>**Figure 2** Brain-specific mutational burden on splicing in ASD. (A). Tissue-agnostic variant effect prediction with MMSplice. 
Splice-region de novo mutations (n=3,884) of the proband group (gray) have significantly lower predicted logit(Ψ) according to MMSplice 
compared to those of the unaffected sibling group (orange). The effect size is larger for variants in LoF-intolerant genes (n=1,081). 
Shown are the means and standard 95% confidence intervals. P-values from one-sided Wilcoxon test. (B). Tissue-specific variant-effect prediction with MTSplice. 
Distribution of effect size (difference of average logit(Ψ) for proband versus control siblings de novo mutations) for brain tissues (right boxes) and other 
tissues (left boxes), and for all de novo mutations (left panel) or de novo mutations in LoF-intolerant genes (right panel) with MTSplice. 
The predicted effect sizes are more pronounced for brain tissues.</sub>



## Immunogenicity Prediction for Vaccine Design
Genetic mutations in cancer cells are the source of neoantigens, which can be used to design vaccines. 
Because neoantigen are truly tumor specific, they are ideal targets for cancer immunotherapies. 
Besides predicting the functional and disease impact of mutations, I’m also interested in integrating variant effect predictors with immunogenicity predicting models to design therapeutic vaccines.

Adaptive immunity is triggered by a series of processes involving antigen processing, presentation and recognition. 
Each of the steps is highly selective and specific (Figure 3). Machine learning models have long been applied to model different immune 
response steps and are widely used for vaccine design. However, the performance in many cases are very limited. 
I'm interested in developing improved models for 1) peptide-MHC interaction prediction, 2) pMHC-TCR binding prediction, 3) neoantigen discovery from new sources.

![](/images/immue.png)
<sub>**Figure 3** Antigen presentation. MHC molecules present antigens on the cell surface to T-cells to activate immune response. </sub>

Under this scope, I developed BERTMHC ([Cheng et al., 2020](https://www.biorxiv.org/content/10.1101/2020.11.24.396101v1)), 
a model to predict the binding and presentation of peptides by MHC class II. The paper shows that unsupervised pretraining, 
which is common in nature language processing, and our new probability re-weighted multiple instance learning algorithm improved previous
state-of-the-art for this task.

## Improved Understanding of Biological Systems 
Beyond developing new methods to achieve prediction tasks, I’m also interested in applying computational methods to improve our understanding of fundamental 
biology systems. Such projects will be in collaboration with experimental biologists to generate data and validate hypotheses. 

One example is a study about mRNA stability ([Cheng et al., 2017](https://rnajournal.cshlp.org/content/23/11/1648)). 
Understanding the regulation of mRNA stability in the cell is crucial. For instance, at least two Covid19 vaccines are based on mRNA technologies
([BioNTech](https://biontech.de/covid-19) and [Moderna](https://www.modernatx.com/modernas-work-potential-vaccine-against-covid-19)), 
it is crucial to have mRNAs that translate efficiently and stable in the cell. 
In this study I systematically searched for sequence determinants of mRNA stability with a linear mixed-effects model. 
We also show that codon usage, which is known to highly affect translation efficiency, also being the major determinant of mRNA stability.
To the end, we are able to predict mRNA stability with R^2=0.59 solely from its sequence. 

In another study, I identified a circRNA (circSfl) with a computational method developed by myself ([Cheng et al., 2016](https://doi.org/10.1093/bioinformatics/btv656)). In collaboration with colleagues at MPI for Biology of Ageing, 
we showed that overexpression of circSfl can extend the lifespan of fruit flies ([Weigelt et al., 2020](https://www.sciencedirect.com/science/article/pii/S1097276520303968)). 
This is important since many ageing mechanisms are very conserved in humans.

## Single-cell multiomics data integration
In biomedical experiments, an increasing variety of “omics” data from patients are generated, such as transcriptomics, proteomics, ATAC-seq, etc. 
A challenging task is how to integrate the different data modalities and represent them meaningfully in a data manifold that is optimal for 
downstream applications. I explore this topic with the latest development in generative models.


## Others
Other than the above topics, I'm also interested in:

 1) Graph representation learning
 
 2) Biological sequence representation learning
 
 3) RNA binding protein binding site prediction 
 
 4) Data efficient machine learning methods
 
 5) Efficient approximate inference applied to biological problems.