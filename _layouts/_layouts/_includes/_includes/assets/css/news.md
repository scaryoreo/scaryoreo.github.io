---
title: News
subtitle: Updates from the lab
permalink: /news/
---

<ul>
{% for post in site.posts %}
  <li><a href="{{ post.url }}">{{ post.title }}</a> <span class="small">— {{ post.date | date: "%b %d, %Y" }}</span></li>
{% endfor %}
</ul>
