---
layout: archive
title: "Researches"
permalink: /publications/
author_profile: true
---

## Hi, welcome to my research website!
Starting from my sophomore year, I have been involved with research projects in a wide range of astronomical fields, spanning from uncovering the faintest population of galaxies to "weather forecasting" on Hot Jupiters. You can find detailed project descriptions in the following tabs. 

Thanks to my research experience, I have been working on different datasets, like [DELVE](https://datalab.noirlab.edu/delve/), [WOCS](https://www.astro.wisc.edu/research/research-areas/stars-stellar-systems/wocs/), and [JWST Cycle 2 data](https://www.stsci.edu/jwst/phase2-public/3969.pdf). I also learned useful statistical tools along the way, like [unsupervised clustering](https://scikit-learn.org/stable/modules/clustering.html#clustering) and [rejection / MCMC sampling](https://thejoker.readthedocs.io/en/latest/index.html).

If you are interested in learning about my research, please don't hesitate to [email me](panpi@umich.edu). 

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}



