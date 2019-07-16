---
layout: default
title: Arquivo
---


{% for post in site.categories.Personal %}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
