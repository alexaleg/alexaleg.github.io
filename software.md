---
layout: page
permalink: /software/
title: "Software"
softwares:
    - title:   "CLUE"
      desc:  "Python implementation of my current work as a PhD."
      url:     "https://github.com/alexaleg/CLUE"
    - title:   "Optimal operation of small LNG cycles"
      desc:  "This repository corresponds to the MATLAB simulation codes for modelling and optimizing the Mini - LNG System proposed by Nekså, 2010. A previous mdoel of this system was developed by Leguizamon, 2016. This works expands and improves the previous formulation." 
      url:     "https://github.com/alexaleg/OptimRefCycles"
---
{% assign thumbnail="left" %}

{% for soft in page.softwares %}
[**{{soft.title}}**]({% if soft.internal %}{{soft.url | prepend: site.baseurl}}{% else %}{{soft.url}}{% endif %})<br />
{% if soft.desc %} **Description:** {{soft.desc}}
{% endif %}
{% endfor %}


