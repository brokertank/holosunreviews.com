---
layout: archive
title: "Reviews"
permalink: /reviews/
author_profile: false
---

{% for post in site.categories.reviews %}
  <article class="archive-item">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
  </article>
{% endfor %}