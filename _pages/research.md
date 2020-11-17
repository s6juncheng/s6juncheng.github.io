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
I trained a neural network model from large-scale perturbation assays and genome annotation data to predict variant effects on splicing. 
The model, MMSplice, can precisely predict splicing level change subject to variants (Figure 1) (Cheng et al., 2019, Genome Biology). 
MMSplice is the winning model for the [CAGI5 public splicing challenge](https://genomeinterpretation.org/content/vex-seq) and 
has been integrated to the popular variant effect predictor [CADD](https://cadd.gs.washington.edu/news). 

![](/images/ISM.png)
*Figure 1*

The limitation of MMSplice and other methods on variant interpretation for splicing is the lack of tissue specificity. 
To overcome this limitation, we developed MTSplice which combines MMSplice and a tissue-specific splicing level prediction model to predict tissue-specific variant effects.
We show that MTSplice can capture tissue-specific disease signals related to Autism Spectrum Disorder when comparing the predicted functional scores in the proband group and the unaffected sibling control group (Figure 2).

![](/images/ASD.png)
*Figure 2*


## Immunogenicity prediction for vaccine design
Genetic mutations in cancer cells are the source of neoantigens, which can be used to design vaccines. 
Because neoantigen are truly tumor specific, they are ideal targets for cancer immunotherapies. 
Besides predicting the functional and disease impact of mutations, I’m also interested in integrating variant effect predictors with immunogenicity predicting models to design therapeutic vaccines.

Adaptive immunity is triggered by a series of processes involving antigen processing, presentation and recognition. 
Each of the steps is highly selective and specific.  Machine learning models have long been applied to model different immune 
response steps and are widely used for vaccine design. However, the performance in many cases are very limited. 
I'm interested in developing improved models for 1) peptide-MHC interaction prediction, 2) pMHC-TCR binding prediction, 3) neoantigen discovery from new sources.

## Improved understanding of biological systems 
Beyond developing new methods to achieve prediction tasks, I’m also interested in applying computational methods to improve our understanding of fundamental 
biology systems. Such projects will be in collaboration with experimental biologists to generate data and validate hypotheses. 

We identified a circRNA (circSfl) with a computational method developed by myself. In collaboration with colleagues at MPI for Biology of Ageing, 
we showed that overexpression of circSfl can extend the lifespan of fruit flies (Weigelt et al., 2020). 
In another study in collaboration with colleagues at MPI for Biophysical Chemistry, 
we found and validated a 3’UTR motif ATATTC that destabilizes mRNA transcripts (Cheng et al., 2017). 
The same study also found codon usage explains most of the mRNA half-life variability across genes.

## Others
Other than the above topics, I'm also interested in 1) developing cis-trans models for RNA-protein binding, 2) single-cell multiomics data integration, 3) data efficient machine learning methods.