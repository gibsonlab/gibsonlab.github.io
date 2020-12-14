---
layout: default
title: About
permalink: /about/
---

The Gibson Lab is part of the [Division of Computational Pathology](https://comp-path.bwh.harvard.edu/) at [Brigham and Women's Hospital](https://www.brighamhealth.org/) and [Harvard Medical School](https://hms.harvard.edu/). We are physically located in the  [Hale Building for Transformative Medicine (BTM) in 8002](https://www.google.com/maps/place/Building+for+Transformative+Medicine+at+Brigham+and+Women's+Hospital/@42.3353661,-71.1087175,15z/data=!4m5!3m4!1s0x0:0x35376a566e389c7d!8m2!3d42.3353661!4d-71.1087175) in Boston with space also at the [MIT Stata Center (32-G570)](https://www.google.com/maps/place/Stata+Center,+32+Vassar+St,+Cambridge,+MA+02139/@42.3616095,-71.0928242,17z/data=!3m1!4b1!4m5!3m4!1s0x89e370a95d3025a9:0xb1de557289ff6bbe!8m2!3d42.3616095!4d-71.0906355)  in Cambridge.

In our research we leverage tools from machine learning and control to understand biological systems.  Control theoretic concepts are integrated both in the design of our optimization schemes and statistical machine learning models, as well as in the design of our *in vitro* and *in vivo* experiments. Current and future projects include
* Statistical learning applied to microbial dynamics (Bayesian nonparametrics, layered latent state-space models)
* Theoretical foundations at the intersection of machine learning and control
* Genetically engineering and controlling a microbial consortia
* Host-Microbiome interactions
* Time-series "omics" (metagenomics, transcriptomics, and metabolomics)


## Sample from our theoretical learning research

Gradient based optimization schemes are at the core of both adaptive control and optimization in ML (connections between the two are reported [here](/papers/gaudio19cdc.pdf)). We leverage techniques used in adaptive control to improve the stability properties of momentum based gradient algorithms resulting in **provably stable** accelerated algorithms. Our algorithms are a log factor slower than Nesterov but with **stability guarantees**, see our [Higher Order Tuner](https://arxiv.org/abs/2005.01529) in Figure 1. Having *a priori* stability guarantees will be critical for certifying and deploying real-time and safety critical ML algorithms in medical applications.
<p><figure class="image" style="
    float: center;
    width: 450px;
    margin: auto;
    display: block;
    max-width: 100%;
    max-height: 100%;">
<img src='/image/highordertuner3.svg' alt="higher order tuner" style="
    width: 450px;
    display: block;
    margin: auto;" />
    <figcaption> Figure 1: Higher order tuner demonstrating the ability to maintain stability during model training. At step 500 there is an abrupt change in the magnitude of the training data <button name="button" onclick="window.location.href='https://arxiv.org/abs/2005.01529'"><i class="far fa-file-pdf"></i> paper</button></figcaption>
</figure></p>

## Sample from our experimental research

Our main experimental system for studying the microbiome is [gnotobiotic](https://en.wikipedia.org/wiki/Gnotobiosis) mice. We are particularly interested in developing bacterio-therapies, and to develop those therapies we need to have an experimental system that allows us to probe the dynamics of complex microbial communities *in vivo*. We colonize [germ-free](https://en.wikipedia.org/wiki/Germ-free_animal) mice with defined microbial communities as well as human fecal samples (creating "humanized" mice). To obtain rich dynamic profiles we perturb the microbial environment by changing the diet of the animals, presenting colonization challenges from other bacteria, delivering antibiotics, and by introducing bacteriophages. One of our experiments looking to understand the direct and indirect role of phage predation on the microbiome is shown in Figure 2 (accompanying [paper](/papers/hsu19hostmicrobe.pdf)).

<p><figure class="image" style="
    width: 650px;
    float: center;
    margin: auto;
    max-width: 100%;
    max-height: 100%;">
<img src='/image/mouse_time.png' alt="mouse time series" style="width: 650px;
    display: block;
    margin: auto;" />
    <figcaption> Figure 2: Gnotobiotic model of phage predation in the murine gut <button name="button" onclick="window.location.href='/papers/hsu19hostmicrobe.pdf'"><i class="far fa-file-pdf"></i> paper</button></figcaption>
</figure></p>

## Samples from our modeling research

To answer our biological questions surrounding the microbiome we build statistical models that propagate measurement and latent state uncertainty throughout the model. One example of this is our Robust and Scalable Model of Microbiome Dynamics (Figure 3). This model is a Bayesian nonparametric model of microbial dynamics based on what we term interaction modules, or learned clusters of latent variables with redundant interaction structure. This allows our model of dynamics to scale to hundreds of microbial taxa. Another example of our modeling work is the method Chronostrain (Figure 4). Chronostrain is a sequencing quality, host, and time aware strain tracking algorithm.

<div style="display: inline-block;">
<figure class="image" style="
    float: left;
    width: 49%;
    max-width: 100%;
    max-height: 100%;">
<a href="/posters/gibson18icml.pdf"><img src='/posters/vec_gibson.svg' alt="mouse time series" style="width: 100%;
    display: block;
    margin: auto;
    float: auto;" /></a>
    <figcaption> Figure 3: Robust and Scalable Model of Microbiome Dynamics
    <button name="button" onclick="window.location.href='http://proceedings.mlr.press/v80/gibson18a.html'"><i class="far fa-file-pdf"></i> paper</button>
    <button name="button" onclick="window.location.href='/posters/gibson18icml.pdf'"><i class="far fa-file-pdf"></i> poster</button>
    </figcaption>
</figure><figure class="image" style="
    float: right;
    width: 49%;
    max-width: 100%;
    max-height: 100%;">
<a href="/posters/kim20mlcb.pdf"><img src='/image/kim20mlcb.png' alt="mouse time series" style="width: 100%;
    display: block;
    margin: auto;
    float: auto;" /></a>
    <figcaption> Figure 4: Chronostrain: Sequence quality and time aware strain tracking with shotgun metagenomic data
    <button name="button" onclick="window.location.href='/posters/kim20mlcb.pdf'"><i class="far fa-file-pdf"></i> poster</button>
    </figcaption>
</figure>
</div>

## Collaborators

### Labs
- [Berger Lab - MIT](http://people.csail.mit.edu/bab/)
- [Walt Lab - BWH, HMS, Wyss Institute](https://waltlab.bwh.harvard.edu/)
- [Gerber Lab - BWH, HMS](https://gerber.bwh.harvard.edu/)
- [Wang Lab - Columbia](http://wanglab.c2b2.columbia.edu/)
- [Active Adaptive Control Lab - MIT (Annaswamy)](http://aaclab.mit.edu/)
- [Hultgren Lab - WUSTL](https://hultgrenlab.wustl.edu/)
- [Bacterial Genomics Group - Broad Institute (Earl)](https://www.broadinstitute.org/bios/ashlee-earl)

### Joint funded projects
- **[The rules of microbiota colonization of the mammalian gut](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2025515&HistoricalAwards=false):**
A $2.9 Million NSF project with Co-PIs Georg Gerber and Harris Wang with Travis Gibson as a Co-Investigator - "This project has three main thrusts: 1) Learn microbial community-level rules that quantitatively predict population dynamics of mouse gut colonization and assess these rules across differing ranges of microbial diversity and composition, 2) Elucidate microbial gene-level mechanisms that predict mouse gut colonization dynamics, and 3) Profile microbial spatiotemporal organization and dynamics during gut colonization at the species and gene level to predict microbial community dynamics."
[![The rules of microbiota colonization of the mammalian gut](/image/nsfmtm.svg){: style="
    display: block;
    margin: auto;
    width: 650px;
    max-width: 100%;
    max-height: 100%;""}](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2025515&HistoricalAwards=false)
