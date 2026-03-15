---
layout: archive
permalink: /research/
author_profile: true
title: ""
---


<span style="color:blue">Computational Modeling and Simulations</span>
======

My research is dedicated to leveraging computational methods to address complex challenges across various scientific disciplines. By utilizing advanced modeling techniques, simulations, and data-driven approaches, I aim to uncover insights that are otherwise difficult to obtain through traditional experimental methods. Through these efforts, I strive to make significant contributions to the advancement of knowledge and the development of innovative solutions for real-world problems.

-----------------------

{% assign grouped_posts = site.research | group_by: "category" %}

{% for group in grouped_posts %}
  <h2>{{ group.name }}</h2> <!-- Displays the category name -->
  <ul>
    {% for post in group.items %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
