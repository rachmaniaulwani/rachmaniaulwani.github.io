---
layout: page
title: projects
permalink: /projects/
description: A collection of my work and hobbies.
nav: true
nav_order: 2
display_categories: [UBC Course, Fun]  # These must match exactly
horizontal: false
---
<div class="projects">
  {% if site.enable_project_categories and page.display_categories %}
    {% for category in page.display_categories %}
      <h2 class="category">{{ category }}</h2>
      {% include projects_by_category.liquid %}
    {% endfor %}
  {% else %}
    {% include projects.liquid %}
  {% endif %}
</div>
