---
title: Publications
subtitle: Selected papers and preprints
permalink: /publications/
---

<ul>
{% assign pubs = site.publications | sort: "year" | reverse %}
{% for pub in pubs %}
  <li style="margin-bottom:10px;">
    <strong>{{ pub.title }}</strong><br/>
    <span class="small">{{ pub.authors }} ({{ pub.year }}). {{ pub.venue }}.</span>
    {% if pub.doi %} <a href="{{ pub.doi }}">DOI</a>{% endif %}
    {% if pub.pdf %} · <a href="{{ pub.pdf }}">PDF</a>{% endif %}
  </li>
{% endfor %}
</ul>
