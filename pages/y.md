---
layout: page
title: why
permalink: /y/
---

{% assign sorted = site.pages | sort: "title" %}
  {% for p in sorted %}
    {% if p.title and p.layout %}
    - [{{ p.title }}]({{ p.url }})
    {% endif %}
  {% endfor %}