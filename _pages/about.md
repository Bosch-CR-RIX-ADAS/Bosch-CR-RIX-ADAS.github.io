---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

We are researchers in ADAS field from Bosch Coporate Research, with expert competences on perception, planning, E2E and VLA.
Welcome to our homeland and enjoy!

---

## News

{% for post in site.news reversed limit:5 %}
  {% include archive-single.html %}
{% endfor %}

## Publications

{% for post in site.publications reversed limit:5 %}
  {% include archive-single.html %}
{% endfor %}