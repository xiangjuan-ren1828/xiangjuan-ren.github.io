---
layout: default
title: Projects
permalink: /projects/
---

# Projects

Below are some of my projects. Each project is a markdown file under the _projects/ directory.

<ul>
{% for project in site.projects %}
  <li>
    <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
    {% if project.excerpt %} — {{ project.excerpt }}{% endif %}
  </li>
{% endfor %}
</ul>