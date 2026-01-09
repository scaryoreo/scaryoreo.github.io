---
title: Projects
subtitle: Ongoing and recent research
permalink: /projects/
---

<div class="grid">
{% assign projs = site.projects | sort: "order" %}
{% for pr in projs %}
  <div class="card">
    <h3><a href="{{ pr.url }}">{{ pr.title }}</a></h3>
    <div class="small">{{ pr.summary }}</div>
    {% if pr.tags %}
      <div style="margin-top:10px;">
      {% for t in pr.tags %}<span class="badge">{{ t }}</span>{% endfor %}
      </div>
    {% endif %}
  </div>
{% endfor %}
</div>
