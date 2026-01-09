---
title: BAIC Lab
subtitle: Behavior & AI Collaboration — research at the intersection of people and intelligent systems.
---

<div class="grid">
  <div class="card">
    <h3>Research</h3>
    <p class="small">Explore our projects, methods, and current directions.</p>
    <p><a href="/projects/">View projects →</a></p>
  </div>
  <div class="card">
    <h3>Publications</h3>
    <p class="small">Papers, preprints, and selected outputs.</p>
    <p><a href="/publications/">Browse publications →</a></p>
  </div>
  <div class="card">
    <h3>Join the lab</h3>
    <p class="small">Open positions and how to get involved.</p>
    <p><a href="/contact/">Contact us →</a></p>
  </div>
</div>

## Latest news
<ul>
{% for post in site.posts limit:3 %}
  <li><a href="{{ post.url }}">{{ post.title }}</a> <span class="small">— {{ post.date | date: "%b %d, %Y" }}</span></li>
{% endfor %}
</ul>
