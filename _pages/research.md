---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# Welcome to My Research Website! 👋

During my undergraduate career, I have participated in research projects, spanning from characterizing the atmospheres of Hot Jupiters to mining and analyzing some of the faintest galaxies. Thanks to these experiences, I have worked with diverse datasets, such as [DELVE](https://datalab.noirlab.edu/delve/), [WOCS](https://www.astro.wisc.edu/research/research-areas/stars-stellar-systems/wocs/), and [JWST transit data](https://www.stsci.edu/jwst/phase2-public/3969.pdf). Along the way, I also learned some useful statistical tools for astrophysics, like:
- [Unsupervised clustering](https://scikit-learn.org/stable/modules/clustering.html#clustering)
- [Rejection sampling](https://thejoker.readthedocs.io/en/latest/index.html)
- [Atmospheric retrievals with nested sampling](https://poseidon-retrievals.readthedocs.io/en/latest/index.html#)

I am interested in continuing my research journey in graduate school. I enjoy using modern statistical tools to answer astrophysical problems. My current work spans ultra-faint dwarf galaxies (UFDs), blue straggler stars (BSSs), and Hot Jupiters. However, I would love to explore more astronomical fields, like gravitational lensing, ISM, and beyond. 

If you are interested in learning about my research or simply chatting about science in general, please don't hesitate to email me at **panpi@umich.edu**.  I’d love to connect!


## Hot Jupiter multi-dimensional atmospheric modeling 🪐
### Advisor: [Ryan MacDonald](https://distantworlds.space/)
### 01/2024 - Present
We observed the hot Jupiter WASP-52b with JWST as part of a Cycle 2 Program aiming to measure differences between the east and west limbs of the planet. We analyzed the chemical composition, temperature, and cloud properties on each side of the planet. The science goals of this project are:
1. Measure the chemical composition of WASP-52b’s atmosphere using a Bayesian atmospheric retrieval code. (**ongoing**)
2. Identify whether a 2D atmospheric model is preferred over a 1D model, and if so, quantify differences between the morning and evening terminators (west and east). (**ongoing**)
3. Investigate and correct for the influence of unocculted starspots on WASP-52b’s JWST transmission spectrum. (**ongoing**)

Unocculted stellar contamination (starspots or faculae) can strongly influence exoplanet transmission spectroscopy. Therefore, incorporating these stellar active regions into atmospheric retrieval algorithms is crucial for reliably inferring exoplanet atmosphere properties. We recently observed a hot Jupiter orbiting a highly active star, WASP-52b, with JWST to directly test methods to disentangle stellar inhomogeneities from planetary atmospheric features. I will present the full optical to near-infrared (0.6-5.2 μm) transmission spectrum of WASP-52b from two JWST transits, one with NIRISS/SOSS and one with NIRSpec G395H. Since our WASP-52b transmission spectra are strongly sculpted by both occulted starspot crossing events during the transit and unocculted active regions, we incorporate starspots and faculae into our retrieval analysis. I will present our detailed constraints on the chemical inventory and aerosol properties of WASP-52b’s atmosphere, demonstrating strategies to overcome stellar contamination of transmission spectra. _We are close to understand WASP-52's stellar features and results are coming soon_.


## Kinematics of ultra-faint dwarf galaxies 🌌
### Advisor: [Marla Geha](http://www.astro.yale.edu/mgeha/)
### 05/2024 - 08/2024
Ultra-faint dwarf (UFD) satellite galaxies are believed to have the oldest, most dark-matter dominated, and least chemically evolved stellar populations (Simon 2019). Therefore, UFDs serve as effective cosmological probes for the early Universe and are pristine laboratories for dark matter physics. In this study, we analyze resolved stars of two Milky Way satellite galaxies, Pegasus 3 and Pegasus 4, to provide more precise and accurate measurements of their velocity dispersion, dynamical masses, and mass to light ratios compared to previous studies (Cerny et al. 2023a; Kim et al. 2016). We first select member stars within these two galaxies using radial velocity, proper motion, equivalent width, and color & magnitude measurements. With these selected member stars’ radial velocity measurements, we apply a customized MCMC procedure to fit for their systematic velocity and velocity dispersion, which gives us their dynamical mass estimates (Walker et al. 2006; Wolf et al. 2010; Foreman-Mackey et al. 2013). We reconfirm and conclude these two systems are dark matter dominated dwarf galaxies by comparing them with other similarly faint stellar systems. This work offers us more accurate dynamical mass estimates of Peg 3 & 4 with more spectroscopically selected member stars.




## Alternative evolutionary pathway for stellar population by orbit modeling ⭐
### Advisor: [Robert Mathieu](https://www.astro.wisc.edu/?uw_staff=mathieu-robert)
### Started 05/2023 - 06/2024
### [Astrobites](https://astrobites.org/2024/07/03/ur-blue-stars-that-should-not-exist/)
![BSS_HR](https://yanbopanpi.github.io/yanbo_pan.github.io//images/BSS_HR.png){: style="width: 50%; max-width: 450px; height: auto; float: right;"}
Blue Straggler Stars (BSS) are believed to have originated from binary star interactions. Therefore, modeling binary orbits is crucial for understanding their formation and evolution. In this study, we applied The Joker (a Monte Carlo rejection sampler) to model binary orbits in the WIYN Open Cluster Survey (WOCS). Our objective was to evaluate The Joker’s efficacy on binaries with ample radial-velocity data (RVD). Exploring the potential usage of The Joker, designed for sparsely measured radial velocities, we applied it to known single-lined binary orbits in M67 and NGC 188. With 70+ binary systems, we compared our Joker orbital parameters among binaries having a diverse array of period-eccentricity combinations (Geller et al. 2021). We found that 5-7 RVD start to meaningfully constrain orbital parameters, and 8-10 RVD are required for unimodal period solutions with eccentricities converging to previous studies’ solutions. Additionally, we explored the possibility of devising observing plans having limited prior measurements with The Joker predicting possible periastron approach times to constrain eccentricity. This work enables us to estimate binary orbital solutions with fewer RVD and to enhance our understanding of the alternative evolutionary tracks of binary systems.

For our future work, we will fit more binary solutions for WD-MS binaries, while improving the pipeline to better suit observation plans and reduce bias our priors might introduce. This study is also used to design future observation plans to break the degeneracies between possible orbits. 
<!---
Through this research experience, I learned about rejection and MCMC sampling. Exposed to time-series radial-velocity data for the first time, I designed a custom pipeline that allows statistical comparison between our results and previous scientific results done by [Aaron M. Geller](https://arxiv.org/abs/2101.07883). I also become more familiar with using cloud computing and virtual machines. 
!--->
![binary_demo](https://yanbopanpi.github.io/yanbo_pan.github.io//images/binary_demo.jpg){: style="width: 50%; max-width: 450px; height: auto; float: left;"}
*image credit: Aaron Geller*


<br>

## Mining Ultra-Faint Galaxies in the Local Group 🌌
### Advisor: [Eric Bell](https://sites.lsa.umich.edu/ericbell/)
### 01/2023 - 05/2024
![star_galaxy](https://yanbopanpi.github.io/yanbo_pan.github.io//images/star_galaxy_classification.png){: style="width: 50%; max-width: 450px; height: auto; float: right;"}
<!---
By analyzing the stellar spatial distribution, we try to search for potential ultra-faint dwarf (UFD) galaxies of M31 by examining stellar overdensities within the DELVE survey. We attempt to search for overdensities for horizontal branch (HB) and red giant branch stars (RGB) using Density-Based Spatial Clustering of Applications with Noise (DBSCAN). We first focused on Pegasus IV dwarf galaxy and its stellar population as a guide for designing our overdensity search pipeline. With the detected overdensities on the color-magnitude diagram, we also explore the stellar overdensities regarding their spatial distribution. 
!--->
Ultra-faint dwarf (UFD) satellite galaxies are believed to have the oldest, most dark-matter-dominated, and least chemically evolved stellar populations. Therefore, UFDs serve as effective cosmological probes for the early stage of the Universe. In this study, we applied unsupervised machine learning (DBSCAN & OPTICS) to search for potential UFDs by analyzing spatial overdensities of the tip of red giant branch (TRGB) stars in the DELVE survey. 

![AndXXIX](https://yanbopanpi.github.io/yanbo_pan.github.io//images/AndXXIX.png){: style="width: 50%; max-width: 450px; height: auto; float: left;"}
<!---
After devising the pipeline with DBSCAN, we also tried using HDBSCAN and OPTICS to test which unsupervised machine learning method yielded the best result for the UFD search. Finally, OPTICS is chosen since it recovers several UFDs of M31 with the least number of false positives. During this project, we also explore the star-galaxy separation criteria in the DELVE survey. The tip of the red giant branch selection criteria is modified based on the star-galaxy separation magnitude limit. 
!--->
Our objective is to complement the current catalog of UFDs in the local volume while exploring the potential of using modern statistical density searching tools in UFD studies. We have focused on searching for M31 UFDs and recovered all 10 M31 satellite galaxies in the DELVE DR2 coverage. This work provides tools to identify UFDs in large sky surveys, which helps to test the cosmological constraints of the Lambda Cold Dark Matter (ΛCDM) model.

<!---
Through this experience, I learned about unsupervised machine learning algorithms by dealing with large survey data. I also have a taste of astrostatistics and designed my own SQL query throughout this project. 
!--->

To further this project, I hope to introduce other types of stars (MS, BSS) into the selection criteria. Also, data from larger areas of the sky will be explored for those “missing satellites”. 

![delve](https://yanbopanpi.github.io/yanbo_pan.github.io//images/delve_dr2_footprint.png)
*image credit: DELVE Collaboration*



  




{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}



