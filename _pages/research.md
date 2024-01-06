---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# Hi, welcome to my research website! 👋
Starting from my sophomore year, I have been involved with research projects in a wide range of astronomical fields, spanning from uncovering the faintest population of galaxies to "weather forecasting" on Hot Jupiters. 

Thanks to my research experience, I have been working on different datasets, like [DELVE](https://datalab.noirlab.edu/delve/), [WOCS](https://www.astro.wisc.edu/research/research-areas/stars-stellar-systems/wocs/), and [JWST Cycle 2 data](https://www.stsci.edu/jwst/phase2-public/3969.pdf). I also learned some useful statistical tools for astrophysics along the way, like [unsupervised clustering](https://scikit-learn.org/stable/modules/clustering.html#clustering) and [rejection / MCMC sampling](https://thejoker.readthedocs.io/en/latest/index.html).

I am interested in continuing my research career in graduate school. I enjoy using statistical tools to solve astrophysical problems. I have been working on ultra-faint dwarf galaxies (UFD), blue straggler stars (BSS), and hot Jupiters to some degree, but I would love to explore more astronomical fields, like black holes, AGN, ISM, etc. 

If you are interested in learning about my research or simply talking about research in general, please don't hesitate to email me (panpi@umich.edu). 



## Alternative evolutionary pathway for stellar population by orbit modeling ⭐
### Started 05/2023
![BSS_HR](https://yanbopanpi.github.io/yanbo_pan.github.io//images/BSS_HR.png){: .align-right width="400px"}
We utilized a custom Monte Carlo (theJoker) sampler, initially created for APOGEE’s sparsely and noisily measured radial velocities, in our examination of the WIYN Open Cluster Survey (WOCS). After utilizing rejection and MCMC sampling, we scrutinized single-lined binary orbits in M67 and NGC 188. Our objective was to evaluate theJoker’s efficacy on binaries with ample radial velocity data (RVD) and investigate the possibility of devising observing plans that would enable us to estimate binary orbital solutions with fewer RVD and better understand the alternative evolutionary tracks for binary stars. 
  
Through this research experience, I learned useful statistical methods, like rejection and MCMC sampling. Exposed to time-series data for the first time, I designed a custom pipeline that allows statistical comparison between our results and previous scientific results done by [Aaron M. Geller](https://arxiv.org/abs/2101.07883). I also become more familiar with using cloud computing and virtual machines. 
  
For our future work, we will fit more binary solutions for WD-MS binaries, while improving the pipeline to better suit observation plans and reduce bias our priors might introduce. 

![binary_demo](https://yanbopanpi.github.io/yanbo_pan.github.io//images/binary_demo.jpg)
*image credit: Aaron Geller*


## Ultra-faint dwarf satellite search 🌌
### Started 01/2023
![AndXXIX](https://yanbopanpi.github.io/yanbo_pan.github.io//images/AndXXIX.png){: .align-right width="320px"}
By analyzing the stellar spatial distribution, we try to search for potential ultra-faint dwarf (UFD) galaxies of M31 by examining stellar overdensities within the DELVE survey. We attempt to search for overdensities for horizontal branch (HB) and red giant branch stars (RGB) using Density-Based Spatial Clustering of Applications with Noise (DBSCAN). We first focused on Pegasus IV dwarf galaxy and its stellar population as a guide for designing our overdensity search pipeline. With the detected overdensities on the color-magnitude diagram, we also explore the stellar overdensities regarding their spatial distribution. 
  
After devising the pipeline with DBSCAN, we also tried using HDBSCAN and OPTICS to test which unsupervised machine learning method yielded the best result for the UFD search. Finally, OPTICS is chosen since it recovers several UFDs of M31 with the least number of false positives. During this project, we also explore the star-galaxy separation criteria in the DELVE survey. The tip of the red giant branch selection criteria is modified based on the star-galaxy separation magnitude limit. 
  
Through this experience, I learned about unsupervised machine learning algorithms by dealing with large survey data. I also have a taste of astrostatistics and design my own SQL query throughout this project. 

To further this project, I hope to introduce other types of stars (MS, BSS) into the selection criteria. Also, data from larger areas of the sky will be explored for those “missing satellites”. 

![delve](https://yanbopanpi.github.io/yanbo_pan.github.io//images/delve_dr2_footprint.png)
*image credit: DELVE Collaboration*


## Hot Jupiter multi-dimensional atmospheric modeling 🪐
### Started 01/2024
This is the project I am going to start in this 2024 winter semester. I do not have any immediate results yet, but I can share my research plan. 

We recently observed the hot Jupiter WASP-52b with JWST as part of a Cycle 2 Program aiming to measure differences between the east and west sides of the planet. We will be analyzing the chemical composition, temperature, and cloud properties on each side of the planet. 

The science goals of this project are:
1. Measure the chemical composition of WASP-52b’s atmosphere using a Bayesian atmospheric retrieval code.
2. Identify whether a 2D atmospheric model is preferred over a 1D model, and if so, quantify differences between the morning and evening terminators (west and east). 
3. Investigate and correct for the influence of unocculted starspots on WASP-52b’s JWST transmission spectrum.


![JWST](https://yanbopanpi.github.io/yanbo_pan.github.io//images/JWST.jpg){: .align-left width="300px"}
*image credit: NASA/JPL-Caltech*
  
Results coming soon ...



{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}



