---
layout: single
permalink: /
author_profile: true
title: ""
redirect_from:
  - /about/
  - /about.html
---

<span style="color:blue">Welcome to my personal homepage</span>
==============
----------------------

I am currently a Ph.D. student in the
[Professor Jianhan Chen's lab](https://people.chem.umass.edu/jchenlab/main.html)
at the Department of Chemistry, UMass Amherst.
My ongoing project is developing the implicit solvent models
to accelerate the conformational sampling of disordered proteins.

<span style="color:blue">Recent News</span>
==============
----------------------

<div class="grid__wrapper">
  {% for post in site.news limit: 4 %}
     {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

