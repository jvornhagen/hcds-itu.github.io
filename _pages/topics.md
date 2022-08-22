---
layout: page
title: topics
permalink: /topics/
description:
nav: false
horizontal: false
order: 25
---
<div class="projects">
  {% assign sorted_topics = site.topics | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
    <div class="container">
      <div class="row row-cols-2">
      {% for project in sorted_topics %}
        {% include projects_horizontal.html %}
      {% endfor %}
      </div>
    </div>
  {% else %}
    <div class="grid">
      {% for project in sorted_topics %}
        {% include projects.html %}
      {% endfor %}
    </div>
  {% endif %}
</div>
