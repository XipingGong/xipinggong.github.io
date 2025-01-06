---
layout: archive
permalink: /news/
author_profile: true
title: ""
---

News
====
The following news tracks all exciting moments.

-------------------------


{% include base_path %}

{% for post in site.news reversed %}
  <article>
    <h2>{{ post.title }}</h2>
    <p><strong>Published:</strong> {{ post.date | date: "%B %d, %Y" }}</p>
    <div>
      {{ post.content | markdownify }}
    </div>
  </article>
  <hr>
{% endfor %}


{%- comment -%}
{% include base_path %}

{% for post in site.news reversed %}
  {% include archive-single.html %}
{% endfor %}
{%- endcomment -%}
