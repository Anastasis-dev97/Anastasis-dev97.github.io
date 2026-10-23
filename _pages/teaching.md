---
layout: page
title: teaching
permalink: /teaching/
nav: true
nav_order: 3
description: Tutorials and exercise sessions in mathematics.
---

{% for item in site.data.teaching %}
<article class="teaching-entry">
  <span class="section-label">{{ item.period }}</span>
  <h2>{{ item.title }}</h2>
  <p class="teaching-institution">{{ item.institution }}</p>
  <p>{{ item.role }}</p>
  {% if item.coordinator %}<p class="entry-detail">Course coordinator: <a href="{{ item.coordinator_url }}">{{ item.coordinator }}</a>.</p>{% endif %}
</article>
{% endfor %}

<p class="section-more">For questions about my teaching, please <a href="{{ '/#contact' | relative_url }}">contact me</a>.</p>
