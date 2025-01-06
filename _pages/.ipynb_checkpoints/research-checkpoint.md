---
layout: archive
permalink: /research/
author_profile: true
title: ""
---

Overview
======

My research interest is generally using and developing advanced computational methods
to address some fundamental problems in various scientific disciplines, 
including the chemistry, biology, materials, and food science.

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
