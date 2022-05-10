---
layout: page
permalink: /courses/
title: teaching
description: Materials for courses you taught. Replace this text with your description.
nav: false
horizontal: true
order: 40
---

For now, this page is assumed to be a static description of your courses. You can convert it to a collection similar to `_projects/` so that you can have a dedicated page for each course.

Organize your courses by years, topics, or universities, however you like!

<div class="projects">
  {% if site.enable_course_categories and page.display_categories %}
  <!-- Display categorized courses -->
    {% for category in page.display_categories %}
      <h2 class="category">{{ category }}</h2>
      {% assign categorized_courses = site.courses | where: "category", category %}
      {% assign sorted_courses = categorized_courses | sort: "start"  | reverse %}
      <!-- Generate cards for each course -->
      {% if page.horizontal %}
        <div class="container">
          <div class="row row-cols-2">
          {% for project in sorted_courses %}
            {% include projects_horizontal.html %}
          {% endfor %}
          </div>
        </div>
      {% else %}
        <div class="grid">
          {% for project in sorted_courses %}
            {% include projects.html %}
          {% endfor %}
        </div>
      {% endif %}
    {% endfor %}

  {% else %}
  <!-- Display courses without categories -->
    {% assign sorted_courses = site.courses | sort: "start" | reverse %}
    <!-- Generate cards for each course -->
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-1">
        {% for project in sorted_courses %}
          {% include projects_horizontal.html %}
        {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="grid">
        {% for project in sorted_courses %}
          {% include projects.html %}
        {% endfor %}
      </div>
    {% endif %}

  {% endif %}

</div>
