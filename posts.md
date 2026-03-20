---
layout: page
title: Blog
permalink: /blog/
---

{% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}
{% for year in posts_by_year %}
<h2 class="posts-year">{{ year.name }}</h2>
<ul class="posts-list">
  {% for post in year.items %}
  <li class="posts-list-item">
    <time class="posts-list-date" datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d" }}</time>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>
{% endfor %}

{% if site.posts.size == 0 %}
<p>No posts yet.</p>
{% endif %}
