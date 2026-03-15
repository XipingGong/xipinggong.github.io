---
layout: archive
permalink: /news/
author_profile: true
title: ""
---

<span style="color:blue">Recent News</span>
====
{% assign sorted_news = site.news | sort: 'date' | reverse %}
{% for post in sorted_news limit:10  %}
  <li>
    <a href="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.date | date: "%m/%d/%Y" }} - {{ post.title }}</a>
  </li>
{% endfor %}


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
