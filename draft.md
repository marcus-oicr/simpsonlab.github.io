---
layout: default
title: Draft
---

## Draft Blog Posts

{% for post in site.posts %}
  {% if post.draft %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
  {% endif %}
{% endfor %}