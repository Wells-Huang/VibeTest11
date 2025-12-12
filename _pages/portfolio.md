---
title: "專案作品"
layout: archive
permalink: /portfolio/
author_profile: true
---

{% for item in site.portfolio reversed %}
  <div class="archive-item">
    <h3><a href="{{ item.url }}">{{ item.title }}</a></h3>
    <p class="archive-date">{{ item.date | date: "%Y年%m月%d日" }}</p>
    {% if item.excerpt %}
      <p>{{ item.excerpt }}</p>
    {% endif %}
    {% if item.header.teaser %}
      <img src="{{ item.header.teaser }}" alt="{{ item.title }}" style="max-width: 100%; height: auto;">
    {% endif %}
  </div>
  <hr>
{% endfor %}
