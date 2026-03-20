---
layout: page
title: Projects
permalink: /projects/
---

{% if site.projects.size > 0 %}
<ul class="projects-list">
  {% for project in site.projects %}
  <li class="projects-list-item">
    <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
    {% if project.description %}<p>{{ project.description }}</p>{% endif %}
  </li>
  {% endfor %}
</ul>
{% else %}
<p style="color: var(--text-light);">Projects coming soon.</p>
{% endif %}
