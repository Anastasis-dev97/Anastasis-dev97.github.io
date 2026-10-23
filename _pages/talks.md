---
layout: page
title: talks
permalink: /talks/
nav: true
nav_order: 2
description: Talks, conferences, workshops, and seminar organization.
---

<nav class="section-links" aria-label="On this page"><a href="#talks">Talks</a><a href="#conferences">Conferences & workshops</a><a href="#organization">Organization</a></nav>

<section aria-labelledby="talks">
  <h2 id="talks">talks</h2>
  {% assign talk_groups = site.data.talks | group_by: 'year' %}
  {% for group in talk_groups %}
  <h3 class="year-heading">{{ group.name }}</h3>
  {% for item in group.items %}
  <article class="talk-row">
    <div class="entry-date">{{ item.date }}</div>
    <div>
      <h4 class="entry-title">{{ item.title }}</h4>
      <p class="entry-detail">{% if item.url %}<a href="{{ item.url }}">{{ item.venue }}</a>{% else %}{{ item.venue }}{% endif %}</p>
    </div>
  </article>
  {% endfor %}
  {% endfor %}
</section>

<section class="content-section" aria-labelledby="conferences">
  <h2 id="conferences">conferences & workshops</h2>
  {% assign conference_groups = site.data.conferences | group_by: 'year' %}
  {% for group in conference_groups %}
  <h3 class="year-heading">{{ group.name }}</h3>
  {% for item in group.items %}
  <article class="talk-row">
    <div class="entry-date">{{ item.date }}</div>
    <div>
      <h4 class="entry-title"><a href="{{ item.url }}">{{ item.title }}</a></h4>
      <p class="entry-detail">{{ item.venue }}</p>
    </div>
  </article>
  {% endfor %}
  {% endfor %}
</section>

<section class="content-section" aria-labelledby="organization">
  <h2 id="organization">organization</h2>
  <p>During my time as a master's student in Thessaloniki, I was co-organizer of the <a href="https://sites.google.com/view/studentseminar-mathauth-en/home">Graduate students' seminar</a>.</p>
</section>
