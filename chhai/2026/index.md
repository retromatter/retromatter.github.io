---
layout: chhai
title: print-ready
---

<ul>
  {% for file in site.static_files %}
    {% if file.path contains '/chhai/2026/' and file.extname == '.pdf' %}
      <li>
        <a href="{{ file.path | relative_url }}" target="_blank">
          {{ file.basename | replace: "-", " " | capitalize }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>