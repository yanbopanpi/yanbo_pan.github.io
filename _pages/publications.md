---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---

# Hi, welcome to my research website!
Starting from my sophomore year, I have been involved with research projects in a wide range of astronomical fields, spanning from uncovering the faintest population of galaxies to "weather forecasting" on Hot Jupiters. 

Thanks to my research experience, I have been working on different datasets, like [DELVE](https://datalab.noirlab.edu/delve/), [WOCS](https://www.astro.wisc.edu/research/research-areas/stars-stellar-systems/wocs/), and [JWST Cycle 2 data](https://www.stsci.edu/jwst/phase2-public/3969.pdf). I also learned some useful statistical tools for astrophysics along the way, like [unsupervised clustering](https://scikit-learn.org/stable/modules/clustering.html#clustering) and [rejection / MCMC sampling](https://thejoker.readthedocs.io/en/latest/index.html).

I am interested in continuing my research career in graduate school. I enjoy using statistical tools to solve astrophysical problems. I have been working on ultra-faint dwarf galaxies (UFD), blue straggler stars (BSS), and hot Jupiters to some degree, but I would love to explore more astronomical fields, like black holes, AGN, ISM, etc. 

If you are interested in learning about my research or simply talking about research in general, please don't hesitate to email me (panpi@umich.edu). 


## Alternative evolutionary pathway for stellar population by orbit modeling
### Started 05/2023
  We utilized a custom Monte Carlo (theJoker) sampler, initially created for APOGEE’s sparsely and noisily measured radial velocities, in our examination of the WIYN Open Cluster Survey (WOCS). After utilizing rejection and MCMC sampling, we scrutinized single-lined binary orbits in M67 and NGC 188. Our objective was to evaluate theJoker’s efficacy on binaries with ample radial velocity data (RVD) and investigate the possibility of devising observing plans that would enable us to estimate binary orbital solutions with fewer RVD and better understand the alternative evolutionary tracks for binary stars. 
  Through this research experience, I learned useful statistical methods, like rejection and MCMC sampling. Exposed to time-series data for the first time, I designed a custom pipeline that allows statistical comparison between our results and previous scientific results done by Aaron M. Geller. I also become more familiar with using cloud computing and virtual machines. 
  For our future work, we will fit more binary solutions for WD-MS binaries, while improving the pipeline to better suit observation plans and reduce bias our priors might introduce. 





{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}



