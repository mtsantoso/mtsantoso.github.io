---
layout: page
title: design
permalink: /design/
nav: true
nav_order: 4
---

<div class="projects">
  <div class="row row-cols-1 row-cols-md-2">
    {% assign design_projects = site.projects | where: "category", "design" | sort: "importance" %}
    {% for project in design_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>