---
permalink: /
title: "About Our"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div class="feature__wrapper">
  <div class="feature__item feature__item--left">
    <div class="archive__item-teaser">
      <img src="{{ '/images/logos/CR_RIX3_logo.png' | prepend: base_path }}" alt="Lab photo">
    </div>
    <div class="feature__item-body">
      <p>We are researchers in ADAS field from Bosch Coporate Research, with expert competences on perception, planning, E2E and VLA. Welcome to our homeland and enjoy!</p>
    </div>
  </div>
</div>
<div style="clear:both"></div>

## Publications

{% assign selected_publications = site.publications | where: "select", true | reverse %}
{% for post in selected_publications limit:5 %}
  {% include archive-single.html %}
{% endfor %}

---

## Partners & Affiliates

{% include base_path %}
<div class="logo-grid">
  {% assign logos = site.static_files | where_exp:"f","f.path contains '/images/school_logos/'" %}
  {% for logo in logos %}
    <div class="logo-grid__item">
      <img src="{{ logo.path | prepend: base_path }}" alt="logo">
    </div>
  {% endfor %}
</div>