---
title: Artikel
layout: page
language: de
permalink: /de/blog
---

{% assign posts = site.posts | where: "language", page.language | sort: "date" | reverse %}
<ul>
{% for post in posts %}
<li><a href="{{ post.url | absolute_url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
