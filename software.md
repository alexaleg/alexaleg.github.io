---
layout: page
permalink: /software/
title: "Software"
softwares:
    - title:   "CLUE"
      desc:    "This is a python library that provides an implementation of several different methods to compute linearl lumpings for dynamical systems. This is a work in progress."
      url:     "https://github.com/alexaleg/CLUE"
    - title:   "Optimal operation of small LNG cycles"
      desc:    "This is a MATLAB implementation of a simulation of a small LNG refrigeration cycle. It uses an equations based approach in which the thermodynamics, equipment models, and energy consumption are optimized simultaneously." 
      url:     "https://github.com/alexaleg/OptimRefCycles"
---
{% assign thumbnail="left" %}

{% for soft in page.softwares %}
[**{{soft.title}}**]({% if soft.internal %}{{soft.url | prepend: site.baseurl}}{% else %}{{soft.url}}{% endif %})<br />
{% if soft.desc %} **Description:** {{soft.desc}}
{% endif %}
{% endfor %}


