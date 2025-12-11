---
layout: page
title: Home
permalink: /
---

<section class="hero">
  <h1>SPRING Doctoral Network</h1>
  <p>
    Preparing the next generation of resilience experts for future
    large-scale critical infrastructures through a Europe-wide doctoral training network.
  </p>
  <p class="hero-meta">
    Marie Skłodowska-Curie Actions (MSCA) Doctoral Network – Grant Agreement No. 101227080
  </p>
  <p>
    <a href="{{ '/doctoral-projects/' | relative_url }}" class="button">
      View doctoral projects (DC1–DC15)
    </a>
  </p>
</section>

<section class="highlights">
  <h2>What is SPRING?</h2>
  <p>
    SPRING brings together universities, research institutes and industry partners to train 15
    Doctoral Candidates (DCs) in the modelling, design and operation of resilient, cyber-secure
    large-scale critical infrastructures.
  </p>
</section>

<section class="latest-news">
  <h2>Latest News</h2>
  <ul class="news-list">
    {% for post in site.posts limit:3 %}
      <li>
        <span class="news-date">{{ post.date | date: "%d %b %Y" }}</span>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% else %}
      <li>No news posts yet. Add one in the <code>_posts</code> folder.</li>
    {% endfor %}
  </ul>
</section>
