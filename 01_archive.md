---
layout: default
title: Arquivo
---


<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
  
        * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})

    {% endfor %}
  </div>
{% endfor %}
</div>
