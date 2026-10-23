---
layout: about
title: About
permalink: /
subtitle: PhD student in mathematics · <a href="https://www.univ-lyon1.fr/">Université Claude Bernard Lyon 1</a>
profile:
  align: right
  image: Anastasios-Fotiadis.webp
  image_circular: false
  more_info: >
    <p>Lyon, France</p>
selected_papers: false
social: false
announcements:
  enabled: false
latest_posts:
  enabled: false
---

I am a mathematician working in **differential geometry**. My research interests include Poisson geometry, singular foliations, higher structures, and interactions with infinite-dimensional geometry.

Since October 2024, I have been a PhD student at [Université Claude Bernard Lyon 1](https://www.univ-lyon1.fr/). My advisor is [Leonid Ryvkin](https://ryvkin.eu/).

<div class="current-focus" markdown="1">
<span class="section-label">Currently thinking about</span>

Linearization of dg-manifolds and Lie ∞-algebroids around singular points and submanifolds.

[More about my research →]({{ '/research/' | relative_url }})
</div>

<section class="home-section biography" aria-labelledby="short-bio">
  <h2 id="short-bio">Short bio</h2>
  <div class="education-list">
    {% for item in site.data.education %}
    <div class="education-row">
      <span class="entry-date">{{ item.period }}</span>
      <div>
        <div class="entry-title">{{ item.degree }}</div>
        <div class="entry-detail">{% if item.institution_url %}<a href="{{ item.institution_url }}">{{ item.institution }}</a>{% else %}{{ item.institution }}{% endif %}</div>
      </div>
    </div>
    {% endfor %}
  </div>
  <p class="section-more"><a href="{{ '/cv/' | relative_url }}">Full academic CV →</a></p>
</section>

<section class="home-section" aria-labelledby="recent-talks">
  <div class="section-heading"><h2 id="recent-talks">Recent talks</h2><a href="{{ '/talks/' | relative_url }}">View all →</a></div>
  {% for item in site.data.talks limit:2 %}
  <div class="talk-row compact">
    <span class="entry-date">{{ item.date }}</span>
    <div><a class="entry-title" href="{{ item.url }}">{{ item.title }}</a><div class="entry-detail">{{ item.venue }}</div></div>
  </div>
  {% endfor %}
</section>

<section class="home-section contact-section" aria-labelledby="contact">
  <h2 id="contact">Contact</h2>
  <p>The best way to reach me is by email.</p>
  <p class="contact-address">familyname @ math dot univ-lyon1 dot fr</p>
  <p class="contact-links"><a href="https://github.com/anastasis-dev97"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a><span aria-hidden="true">·</span><a href="https://www.univ-lyon1.fr/">Université Lyon 1 ↗</a></p>
</section>
