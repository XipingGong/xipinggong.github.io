---
layout: archive
permalink: /research/
author_profile: true
title: ""
---

Overview
======

My research interest is generally using and developing advanced computational methods
(_e.g._, electronic structure calculations, molecular dynamcis, and statistic models)
to address some fundamental problems in the chemistry, biology, materials, and food science.


-----------------------

{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}
