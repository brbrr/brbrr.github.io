---
layout: post
title: "Speechless trip"
description: "Как я угорел один в Европе"
category:
tags: []
---

<p>{{ layout.theme }}</p>

<p>{{ page.layout.theme }}</p>

<p>{{ page.title }}</p>



{% for node in site.pages %}
  {% if node.title != null %}
      {% if page.url == node.url %}
      <li class="active"><a href="{{ BASE_PATH }}{{node.url}}" class="active">{{node.title}}</a></li>
      {% else %}
      <li><a href="{{ BASE_PATH }}{{node.url}}">{{node.title}}</a></li>
      {% endif %}
    {% endif %}
{% endfor %}
