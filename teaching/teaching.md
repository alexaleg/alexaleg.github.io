---
layout: page
permalink: /teaching/
title: Teaching
curs:
    
pasts:
    - title:   "Design definition and implementation of a programming language"
      note:  "Project supervision"
      year:    "2023-I, 2024-I"
      uni:     "Aalborg University"
      url:     "https://moduler.aau.dk/course/2022-2023/DSNDATB410"
    - title:   "Data analysis and modelling"
      note:    "Project supervision"
      year:    "2022-II, 2023-II"
      uni:     "Aalborg University"
      url:     "https://moduler.aau.dk/course/2022-2023/DSNDATB521"
    - title:   "Cálculo Diferencial"
      <>note:  "In Spanish"
      year:    "2021-II"
      uni:     "Universidad Nacional de Colombia Sede Bogotá"
      url:     "/teaching/2021icd/" 
    - title:   "Ecuaciones Diferenciales"
      <>note:  "In Spanish"
      year:    "2020-II"
      uni:     "Universidad Nacional de Colombia Sede Bogotá"
      url:     "/teaching/2020iiecdif/" 
    - title:   "Ecuaciones Diferenciales"
      <>note:  "In Spanish"
      year:    "2020-I"
      uni:     "Universidad Nacional de Colombia Sede Bogotá"
      url:     https://sites.google.com/unal.edu.co/ecdif-2020i/
    - title:   "Química I"
      <>note:  ""
      year:    "2017-I to 2019-I"
      uni:     "Universidad Central"
      url:
    - title:   "Fisicoquímica I"
      <>note:  ""
      year:    "2017-I"
      uni:     "Universidad Central"
      url:

---

Some resources for students ([here](/teaching/resources)):
## Current
{% assign thumbnail="left" %}

{% for cur in page.curs %}
[**{{cur.title}}**]({% if cur.internal %}{{cur.url | prepend: site.baseurl}}{% else %}{{cur.url}}{% endif %})<br />
{{cur.uni}}<br />
*{{cur.year}}*
{% if cur.note %} *({{cur.note}})*
{% endif %}
{% endfor %}

## Past 
{% for past in page.pasts %}
[**{{past.title}}**]({% if past.internal %}{{past.url | prepend: site.baseurl}}{% else %}{{past.url}}{% endif %})<br />
{{past.uni}}<br />
*{{past.year}}*
{% if past.note %} *({{past.note}})*
{% endif %}
{% endfor %}
