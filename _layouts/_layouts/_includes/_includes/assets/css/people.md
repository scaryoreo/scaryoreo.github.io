---
title: People
subtitle: Current members and alumni
permalink: /people/
---

## Current
<div class="grid">
{% assign current = site.people | where: "status", "current" | sort: "order" %}
{% for p in current %}
  <div class="card">
    <h3><a href="{{ p.url }}">{{ p.name }}</a></h3>
    <div class="small">{{ p.role }}</div>
    <div class="small">{{ p.interests }}</div>
  </div>
{% endfor %}
</div>

## Alumni
<div class="grid" style="margin-top:14px;">
{% assign alumni = site.people | where: "status", "alumni" | sort: "order" %}
{% for p in alumni %}
  <div class="card">
    <h3><a href="{{ p.url }}">{{ p.name }}</a></h3>
    <div class="small">{{ p.role }}</div>
    <div class="small">{{ p.now }}</div>
  </div>
{% endfor %}
</div>
