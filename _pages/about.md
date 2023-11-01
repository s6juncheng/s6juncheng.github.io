---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


I am currently a senior research scientist at [DeepMind](https://deepmind.com/). I work on deciphering the human genome with machine learning. My previous work involved modeling RNA splicing and degradation, as well as predicting variant effect for coding and non-coding variants. I did my PhD at the Technical University of Munich (TUM) with [Julien Gagneur](https://www.in.tum.de/gagneurlab/home/) on computational biology. 
Please refer to my [Google Scholar](https://scholar.google.de/citations?user=nfCxSdcAAAAJ&hl=en) 
for a complete list of my publications.

Email: s6juncheng [at] gmail [dot] com

---

## Publications

### Genetic variant interpretation

+ **Cheng, J.**, Novati, G., Pan, J., Bycroft, C., Žemgulytė, A., Applebaum, T., Pritzel, A., Wong, L.H., Zielinski, M., Sargeant, T., Schneider, R.G., Andrew, S., Jumper, J., Hassabis, D., **Kohli, P.**, **Avsec, Ž.**, 2023. Accurate proteome-wide missense variant effect prediction with AlphaMissense. *Science*, 381(6664).

+ **Cheng, J.**, Celik, M.H., Kundaje, A. and Gagneur, J.,
  <a href="https://genomebiology.biomedcentral.com/articles/10.1186/s13059-021-02273-7">MTSplice predicts effects of genetic variants on tissue-specific splicing</a>.
  *Genome Biology*, 2021.

+ **Cheng J**, Nguyen TY, Cygan KJ, Çelik MH, Fairbrother WG, Gagneur J.
  <a href="https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1653-z">MMSplice: modular modeling improves the predictions of genetic variant effects on splicing</a>.
  *Genome Biology*. 2019 Dec;20(1):1-5.

+ Mount SM, Avsec Ž, Carmel L, Casadio R, Çelik MH, Chen K, **Cheng J**, Cohen NE, Fairbrother WG, Fenesh T, Gagneur J.
  <a href="https://onlinelibrary.wiley.com/share/I8PPEAAFMKUADZWSXCBP?target=10.1002/humu.23869">Assessing predictions of the impact of variants on splicing in CAGI5</a>.
  *Human Mutation*. 2019 Sep;40(9):1215-24.

+ **Cheng J**, Çelik MH, Nguyen TY, Avsec Ž, Gagneur J.
  <a href="https://onlinelibrary.wiley.com/share/ZCUVMNIB2GTQQC5E4SVB?target=10.1002/humu.23788">CAGI 5 splicing challenge: Improved exon skipping and intron retention predictions with MMSplice</a>.
  *Human Mutation*. 2019 Sep;40(9):1243-51.


### Biological Discoveries

+ **Cheng J**, Maier KC, Avsec Ž, Rus P, Gagneur J.
  <a href="https://rnajournal.cshlp.org/content/23/11/1648">Cis-regulatory elements explain most of the mRNA stability variation across genes in yeast</a>.
  *RNA*. 2017 Nov 1;23(11):1648-59.

+ **Cheng J**, Metge F, Dieterich C.
  <a href="https://doi.org/10.1093/bioinformatics/btv656">Specific identification and quantification of circular RNAs from sequencing data</a>.
  *Bioinformatics*. 2016 Apr 1;32(7):1094-6.


+ Weigelt CM, Sehgal R, Tain LS, **Cheng J**, Eßer J, Pahl A, Dieterich C, Grönke S, Partridge L.
  <a href="https://www.sciencedirect.com/science/article/pii/S1097276520303968">An Insulin-Sensitive Circular RNA that Regulates Lifespan in Drosophila</a>.
  *Molecular Cell*, 2020 Jul 16;79(2):268-79.


### Computational Immunology

+ **Jun Cheng**, Kaïdre Bendjama, Karola Rittner, Brandon Malone
  <a href="https://doi.org/10.1093/bioinformatics/btab422">BERTMHC: Improves MHC-peptide class II interaction prediction with transformer and multiple instance learning</a>.
  *Bioinformatics*, 2021.

+ Malone B, Simovski B, Moline C, **Cheng J**, Gheorghe M, Fontenelle H, Vardaxis I, Tennoe S, Malmberg JA, Stratford R, Clancy T.
  <a href="https://www.nature.com/articles/s41598-020-78758-5">Artificial intelligence predicts the immunogenic landscape of SARS-CoV-2: toward universal blueprints for vaccine designs</a>.
  *Scientific Reports*. 2020
  

### Bioinformatics & Machine learning

+ Avsec Ž, Kreuzhuber R, Israeli J, Xu N, **Cheng J**, Shrikumar A, Banerjee A, Kim DS, Beier T, Urban L, Kundaje A.
  <a href="https://www.nature.com/articles/s41587-019-0140-0">The Kipoi repository accelerates community exchange and reuse of predictive models for genomics</a>.
  *Nature Biotechnology*. 2019 Jun;37(6):592-600.

+ Avsec Ž, Barekatain M, **Cheng J**, Gagneur J.
  <a href="https://doi.org/10.1093/bioinformatics/btx727">Modeling positional effects of regulatory sequences with spline transformations increases prediction accuracy of deep neural networks</a>.
  *Bioinformatics*. 2018 Apr 15;34(8):1261-9.

----

## Software
Here is a list of open source software that I developed or had major contribution to.
These tools are typically implementation of machine learning models originated from research projects.

---
### [MMSplice & MTSplice](https://github.com/gagneurlab/MMSplice_MTSplice)

Predict variant effect on splicing. MMSplice is the winning model of the [CAGI5 splicing challenge](https://genomeinterpretation.org/content/vex-seq).
MMSplice is also integrated in the popular general purpose variant effect predictor [CADD](https://cadd.gs.washington.edu/news).
MTSplice enhances MMSplice by predicting tissue-specific variant effect.
Currently, Muhammed Hasan Çelik and I are maintaining the tool.


### [ggpval](https://github.com/s6juncheng/ggpval)

A R package to add statistical test and *P*-value annotations to ``ggpplot2``.
Currently, the user community and myself are maintaining the tool.

### [BERTMHC](https://github.com/s6juncheng/BERTMHC)
A python package to re-train and predict with BERTMHC model, a transformer model to predict binding and presentation of peptides by MHC class II.

### [DCC](https://github.com/dieterich-lab/DCC)

A python package to detect circRNAs from next-generation sequence data.
Currently, the Dieterich lab is maintaining the tool.

--------

I contributed the following projects:

### [kipoi](https://kipoi.org)
Kipoi (pronounce: kípi; from the Greek κήποι: gardens) is an API and a repository of ready-to-use trained models for genomics.
It currently contains 2133 different models, covering canonical predictive tasks in transcriptional and post-transcriptional gene regulation. 
