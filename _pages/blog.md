---
title: "最新文章"
layout: archive
permalink: /blog/
author_profile: true
---

## 我的專案作品

{% for item in site.portfolio reversed %}
  <div class="archive-item">
    <h3><a href="{{ item.url }}">{{ item.title }}</a></h3>
    <p class="archive-date">{{ item.date | date: "%Y年%m月%d日" }}</p>
    {% if item.excerpt %}
      <p>{{ item.excerpt }}</p>
    {% endif %}
  </div>
{% endfor %}

---

## 部落格文章

{% for post in site.posts limit: 10 %}
  <div class="archive-item">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p class="archive-date">{{ post.date | date: "%Y年%m月%d日" }}</p>
    {% if post.excerpt %}
      <p>{{ post.excerpt }}</p>
    {% endif %}
  </div>
{% endfor %}
