---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# Welcome to my research website! 👋
Starting from my sophomore year, I have been involved with research projects in a variety of astronomical fields, spanning from mining the faintest population of galaxies to the atmosphere characterization on Hot Jupiters. 

Thanks to my research experience, I have been working on various datasets, like [DELVE](https://datalab.noirlab.edu/delve/), [WOCS](https://www.astro.wisc.edu/research/research-areas/stars-stellar-systems/wocs/), and [JWST Cycle 2 data](https://www.stsci.edu/jwst/phase2-public/3969.pdf). I also learned some useful statistical tools for astrophysics along the way, like [unsupervised clustering](https://scikit-learn.org/stable/modules/clustering.html#clustering), [rejection/MCMC sampling](https://thejoker.readthedocs.io/en/latest/index.html), and [atmospheric retrievals with nested sampling](https://poseidon-retrievals.readthedocs.io/en/latest/index.html#).

I am interested in continuing my research career in graduate school. I enjoy using modern statistical tools to solve astrophysical problems. I have been working on ultra-faint dwarf galaxies (UFD), blue straggler stars (BSS), and hot Jupiters to some degree, but I would love to explore more astronomical fields, like black holes, AGN, ISM, quasars, etc. 

If you are interested in learning about my research or simply talking about science in general, please don't hesitate to email me (panpi@umich.edu). 



## Hot Jupiter multi-dimensional atmospheric modeling 🪐
### Advisor: [Ryan MacDonald](https://distantworlds.space/)
### 01/2024 - Present

We recently observed the hot Jupiter WASP-52b with JWST as part of a Cycle 2 Program aiming to measure differences between the east and west sides of the planet. We will be analyzing the chemical composition, temperature, and cloud properties on each side of the planet. 

The science goals of this project are:
1. Measure the chemical composition of WASP-52b’s atmosphere using a Bayesian atmospheric retrieval code. (**ongoing**)
2. Identify whether a 2D atmospheric model is preferred over a 1D model, and if so, quantify differences between the morning and evening terminators (west and east). (**future**)
3. Investigate and correct for the influence of unocculted starspots on WASP-52b’s JWST transmission spectrum. (**ongoing**)

Stellar inhomogeneities (unocculted starspots or faculae) are believed to influence exoplanet transmission spectroscopy. Therefore, modeling and retrieving stellar features is crucial for understanding the exoplanet’s atmospheric properties. In this study, we apply atmospheric retrievals on the optical to infrared (0.6–2.7 μm) transmission spectrum of the hot Jupiter WASP-52b observed with JWST NIRISS/SOSS instruments. Our objective is to measure its atmospheric chemical composition and study the influence of unocculted stellar features on the transmission spectrum using POSEIDON (a Bayesian atmospheric retrieval algorithm). Since WASP-52b presents significant stellar features and starspot crossing events during the transit, we introduce unocculted starspot or facula (fraction, temperature, and surface gravity as free parameters) in the retrieval process. We will present our retrieval result on atmospheric composition and stellar feature estimates. This work allows us to establish constraints on WASP-52b’s planetary atmosphere and the stellar feature of its host star. _Result plots coming soon_.

<!---
Please check the awesome [exoplanet travel bureau](https://exoplanets.nasa.gov/alien-worlds/exoplanet-travel-bureau/) graphics 
![JWST](https://yanbopanpi.github.io/yanbo_pan.github.io//images/JWST.jpg){: .align-left width="300px"}\
*image credit: NASA/JPL-Caltech*  
!--->




## Alternative evolutionary pathway for stellar population by orbit modeling ⭐
### Advisor: [Robert Mathieu](https://www.astro.wisc.edu/?uw_staff=mathieu-robert)
### Started 05/2023 - Present
### [Astrobites](https://astrobites.org/2024/07/03/ur-blue-stars-that-should-not-exist/)
![BSS_HR](https://yanbopanpi.github.io/yanbo_pan.github.io//images/BSS_HR.png){: .align-right width="400px"}
<!--- old abstract commented out
We utilized a custom Monte Carlo (theJoker) sampler, initially created for APOGEE’s sparsely and noisily measured radial velocities, in our examination of the WIYN Open Cluster Survey (WOCS). After utilizing rejection and MCMC sampling, we scrutinized single-lined binary orbits in M67 and NGC 188. Our objective was to evaluate theJoker’s efficacy on binaries with ample radial velocity data (RVD) and investigate the possibility of devising observing plans that would enable us to estimate binary orbital solutions with fewer RVD and better understand the alternative evolutionary tracks for binary stars. % >new abstract below
!--->

Blue Straggler Stars (BSS) are believed to have originated from binary star interactions. Therefore, modeling binary orbits is crucial for understanding their formation and evolution. In this study, we applied The Joker (a Monte Carlo rejection sampler) to model binary orbits in the WIYN Open Cluster Survey (WOCS). Our objective was to evaluate The Joker’s efficacy on binaries with ample radial-velocity data (RVD). Exploring the potential usage of The Joker, designed for sparsely measured radial velocities, we applied it to known single-lined binary orbits in M67 and NGC 188. With 70+ binary systems, we compared our Joker orbital parameters among binaries having a diverse array of period-eccentricity combinations (Geller et al. 2021). We found that 5-7 RVD start to meaningfully constrain orbital parameters, and 8-10 RVD are required for unimodal period solutions with eccentricities converging to previous studies’ solutions. Additionally, we explored the possibility of devising observing plans having limited prior measurements with The Joker predicting possible periastron approach times to constrain eccentricity. This work enables us to estimate binary orbital solutions with fewer RVD and to enhance our understanding of the alternative evolutionary tracks of binary systems.
  
Through this research experience, I learned about rejection and MCMC sampling. Exposed to time-series radial-velocity data for the first time, I designed a custom pipeline that allows statistical comparison between our results and previous scientific results done by [Aaron M. Geller](https://arxiv.org/abs/2101.07883). I also become more familiar with using cloud computing and virtual machines. 
  
For our future work, we will fit more binary solutions for WD-MS binaries, while improving the pipeline to better suit observation plans and reduce bias our priors might introduce. This study is also used to design future observation plans to break the degeneracies between possible orbits. 

![binary_demo](https://yanbopanpi.github.io/yanbo_pan.github.io//images/binary_demo.jpg)
*image credit: Aaron Geller*


## Ultra-faint dwarf satellite search 🌌
### Advisor: [Eric Bell](https://sites.lsa.umich.edu/ericbell/)
### 01/2023 - 05/2024
![star_galaxy](https://yanbopanpi.github.io/yanbo_pan.github.io//images/star_galaxy_classification.png){: .align-right width="450px"}
<!---
By analyzing the stellar spatial distribution, we try to search for potential ultra-faint dwarf (UFD) galaxies of M31 by examining stellar overdensities within the DELVE survey. We attempt to search for overdensities for horizontal branch (HB) and red giant branch stars (RGB) using Density-Based Spatial Clustering of Applications with Noise (DBSCAN). We first focused on Pegasus IV dwarf galaxy and its stellar population as a guide for designing our overdensity search pipeline. With the detected overdensities on the color-magnitude diagram, we also explore the stellar overdensities regarding their spatial distribution. 
!--->
Ultra-faint dwarf (UFD) satellite galaxies are believed to have the oldest, most dark-matter-dominated, and least chemically evolved stellar populations. Therefore, UFDs serve as effective cosmological probes for the early stage of the Universe. In this study, we applied unsupervised machine learning (DBSCAN & OPTICS) to search for potential UFDs by analyzing spatial overdensities of the tip of red giant branch (TRGB) stars in the DELVE survey. 

![AndXXIX](https://yanbopanpi.github.io/yanbo_pan.github.io//images/AndXXIX.png){: .align-left width="250px"}
<!---
After devising the pipeline with DBSCAN, we also tried using HDBSCAN and OPTICS to test which unsupervised machine learning method yielded the best result for the UFD search. Finally, OPTICS is chosen since it recovers several UFDs of M31 with the least number of false positives. During this project, we also explore the star-galaxy separation criteria in the DELVE survey. The tip of the red giant branch selection criteria is modified based on the star-galaxy separation magnitude limit. 
!--->
Our objective is to complement the current catalog of UFDs in the local volume while exploring the potential of using modern statistical density searching tools in UFD studies. We have focused on searching for M31 UFDs and recovered all 10 M31 satellite galaxies in the DELVE DR2 coverage. This work provides tools to identify UFDs in large sky surveys, which helps to test the cosmological constraints of the Lambda Cold Dark Matter (ΛCDM ) model.


Through this experience, I learned about unsupervised machine learning algorithms by dealing with large survey data. I also have a taste of astrostatistics and designed my own SQL query throughout this project. 

To further this project, I hope to introduce other types of stars (MS, BSS) into the selection criteria. Also, data from larger areas of the sky will be explored for those “missing satellites”. 

![delve](https://yanbopanpi.github.io/yanbo_pan.github.io//images/delve_dr2_footprint.png)
*image credit: DELVE Collaboration*


## Kinematics of ultra-faint dwarf galaxies 🌌
### Advisor: [Marla Geha](http://www.astro.yale.edu/mgeha/)
### 05/2024 - Present

Results coming soon

  




{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}



