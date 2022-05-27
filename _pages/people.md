---
layout: page
title: people
permalink: /people/
# description: Human-Centered Data Science @ IT University of Copenhagen.
nav: true
order: 15

#profile:
#  align: right
#  image: 081021 SK_1-crop_more.jpg
#  address: >
#    <p>4D22</p>
#    <p>Rued Langgaards Vej 7</p>
#    <p>DK-2300 Copenhagen S, Denmark</p>

news: false  # includes a list of news items
people: true  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

{% if page.people %}
  {% include people.html %}
{% endif %}
