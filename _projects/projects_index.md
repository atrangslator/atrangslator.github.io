---
layout: page
title: Projects
permalink: /projects/
---

{% assign grouped = site.projects | group_by: "categories" %}
{% for group in grouped %}
  <h2>{{ group.name }}</h2>
  <ul>
    {% for project in group.items %}
      <li><a href="{{ project.url }}">{{ project.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
