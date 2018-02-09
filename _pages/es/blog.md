---
title: Artículos
layout: page
language: es
permalink: /es/blog
---

{% assign posts = site.posts | where: "language", page.language | sort: "date" | reverse %}
<ul class="posts-list">
{% for post in posts %}
<li>{% include post-excerpt.html %}</li>
{% endfor %}
</ul>
