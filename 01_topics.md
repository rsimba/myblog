---
layout: page
title: Tópicos
---

{% for post in site.categories.topicos %}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
