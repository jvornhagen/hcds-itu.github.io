---
layout: about
title: about
permalink: /
description: Human-Centered Data Science @ IT University of Copenhagen.
order: 10

#profile:
#  align: right
#  image: 081021 SK_1-crop_more.jpg
#  address: >
#    <p>4D22</p>
#    <p>Rued Langgaards Vej 7</p>
#    <p>DK-2300 Copenhagen S, Denmark</p>

news: false  # includes a list of news items
people: false  # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

The Human-Centered Data Science research group (HCDS) focuses on the human factors in the conception, use, and understanding of data. Positioned in the intersection of data science, social science, HCI, and CSCW we are interested in understanding and exploring human practices enabled by technology. We combine both quantitative and qualitative methods, and work with computational methods such as statistics, machine learning, network analysis together with qualitative methods such as ethnography, interviews, and observations.

Our research aims to contribute to often overlooked human-centered dimensions of data science such as individual differences, domain-expertise, design implications, and societal impact. Within HCDS, we work across several topics, including digital media platforms, information visualization, crowd sourcing, affective computing, behavioral modeling, and societal challenges related to digital infrastructure more broadly.

<div class="news">
  <h1>news</h1>
  {% if site.news  %}
    <div class="table-responsive">
      <table class="table table-sm table-borderless">
      {% assign news = site.news | reverse %}
      {% for item in news limit: site.news_limit %}
        <tr>
          <th scope="row">{{ item.date | date: "%b %-d, %Y" }}</th>
          <td>
            {% if item.inline %}
              {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
            {% else %}
              <a class="news-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
            {% endif %}
          </td>
        </tr>
      {% endfor %}
      </table>
    </div>
  {% else %}
    <p>No news so far...</p>
  {% endif %}
</div>

<div class="People">
  <h1>People</h1>
  {% if site.people  %}
    <div class="container" style="width:75%">
      <!-- {% assign people = site.people | where: "group", "Faculty" | sort: "started" %} -->
      {% assign people = site.people | where: "status", "Current" %}
      {% for person in people limit: site.people_limit %}
        {% assign remainder = forloop.index | modulo: 4 %}
        {% if forloop.first == true %}
          <div class="row">
        {% elsif remainder == 4 %}
          </div>
          <div class="row">
        {% endif %}

        {% include person.html %}

        {% if forloop.last %}
          </div>
        {% endif %}
      {% endfor %}
    </div>

    <!-- <div class="table-responsive">
      <table class="table table-sm table-borderless">
      {% assign people = site.people | reverse %}
      {% for item in people limit: site.people_limit %}
        <tr>
          <th scope="row">{{ item.name }}</th>
          <td>
            {% if item.inline %}
              {{ item.title | remove: '<p>' | remove: '</p>' | emojify }}
            {% else %}
              <a class="people-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
            {% endif %}
          </td>
        </tr>
      {% endfor %}
      </table>
    </div> -->
  {% else %}
    <p>No people so far...</p>
  {% endif %}
</div>
<script type="text/javascript">
// randomize order within each row
var rows = document.getElementsByClassName('row')
for(var i = 0; i < rows.length; i++) {
  var row = rows[i]
  for (var j = row.children.length; j >= 0; j--) {
    row.appendChild(row.children[Math.random() * j | 0]);
  }
}
</script>




