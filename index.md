---
layout: home
author_profile: true
---

## 最新文章

### 我的專案作品

{% for item in site.portfolio limit: 5 %}
#### [{{ item.title }}]({{ item.url }})
*{{ item.date | date: "%Y年%m月%d日" }}*

{{ item.excerpt }}

{% if item.header.teaser %}
![{{ item.title }}]({{ item.header.teaser }})
{% endif %}

---

{% endfor %}

### 最新部落格

{% for post in site.posts limit: 5 %}
#### [{{ post.title }}]({{ post.url }})
*{{ post.date | date: "%Y年%m月%d日" }}*

{{ post.excerpt }}

---

{% endfor %}
