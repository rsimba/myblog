---
layout: page
title: Arquivos
---

{% for post in site.categories.Arquivos %}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
