---
layout: page
title: Blog
permalink: /blog/
---

{% if paginator.posts %}
  {% for post in paginator.posts %}
### [{{ post.title }}]({{ post.url }})

{{ post.excerpt }}

  {% endfor %}
{% else %}
  {% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})

{{ post.excerpt }}

  {% endfor %}
{% endif %}
