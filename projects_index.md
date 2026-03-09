---
layout: page
title: Projects
permalink: /projects/
---

<div>
  <ul>
    {% assign categories = site.projects | where: "is_category", true %}
  {% for category in categories %}
    <li><a href="{{ category.url }}">{{ category.title }}</a></li>
  {% endfor %}
  </ul>
</div>

