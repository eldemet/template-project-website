---
layout: page
title: Latest News
permalink: /news/
---

This page contains all news and updates from the SPRING Doctoral Network.

<ul class="news-list">
  {% for post in site.posts %}
    <li>
      <span class="news-date">{{ post.date | date: "%d %b %Y" }}</span>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      {% if post.author %}
        <span class="news-author"> · {{ post.author }}</span>
      {% endif %}
    </li>
  {% else %}
    <li>No news posts yet. Check back soon for updates.</li>
  {% endfor %}
</ul>
