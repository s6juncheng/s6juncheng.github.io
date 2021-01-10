---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

I'm a researcher interested in machine learning for biomedicine. I'm currently a research scientist at NEC labs. 
I did my PhD at the Technical University of Munich (TUM) with [Julien Gagneur](https://www.in.tum.de/gagneurlab/home/) on computational biology. 
I was also a visiting student with [Anshul Kundaje](https://sites.google.com/site/anshulkundaje/Home) at Stanford. I did a research internship at Amazon on contextual bandits for personalized recommendations.
As a master student, I worked with [Christoph Dieterich](http://dieterichlab.org/) on circRNAs in Ageing at the Max Planck Institute for Biology of Ageing and [Maria von Korff Schmising](https://www.mpipz.mpg.de/von_korff) on circadian clock of flowering time control at the Max Planck Institute for Plant Breeding Research.

For more detailed introduction about my research please refer to my [Research](https://s6juncheng.github.io/research/) and [Publications](https://s6juncheng.github.io/publications/).
I also make my research accessible through open-source [Software](https://s6juncheng.github.io/software/).

Email: s6juncheng [at] gmail [dot] com

## News

* 2021-01-06: [MTSplice](https://www.biorxiv.org/content/10.1101/2020.06.07.138453v1) is accepted at Genome Biology!
    - MTSplice extend [MMSplice](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1653-z) to predict **tissue-specific** variant effect on splicing.
    - We show the largest improvement of MTSplice in brain tissues.
    - MTSplice captures brain-specific disease signals related to autism that are missed by tissue-agnostic models.

* 2020-12-23: Our paper about designing universal vaccines for Covid is now published on [Scientific Reports](https://www.nature.com/articles/s41598-020-78758-5).  
    - We profiled the entire SARS-CoV-2 proteome for their antigen presentation and immunogenicity potential and identified “epitope hotspot” immunogenic regions.
    - We identified an optimal constellation of epitope hotspots that could provide maximum coverage in the global population.
    
* 2020-11-24: [BERTMHC](https://www.biorxiv.org/content/10.1101/2020.11.24.396101v1) is online!
    - BERTMHC is a deep learning model to predict MHC class II antigen presentation. Antigen presentation is a key step in immune response. 
    Better antigen presentation model has broad applications in vaccine design. 
    - We show that a BERT architecture trained on protein sequences with self-supervised learning is able to improve the prediction of peptide MHC binding.
    - We propose an iteratively re-weighted multiple instance learning algorithm to predict antigen presentation by MHC class II molecules. 
    The algorithm effectively trains on data where a single peptide is presented by a bag of MHC molecules mixed with true and false presenters.
    - In real applications of vaccine design for patients, we would like to maximize the probability of antigen presentation given a bag of MHC molecules from patients, 
    our method fit well with this application.
    