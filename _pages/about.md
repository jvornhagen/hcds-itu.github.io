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

news: true  # includes a list of news items
people: false  # includes a list of news items
select_papers: true # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

The Human-Centered Data Science research group (HCDS) focuses on the human factors in the conception, use, and understanding of data. Positioned in the intersection of data science, social science, HCI, and CSCW we are interested in understanding and exploring human practices enabled by technology. We combine both quantitative and qualitative methods, and work with computational methods such as statistics, machine learning, network analysis together with qualitative methods such as ethnography, interviews, and observations.

Our research aims to contribute to often overlooked human-centered dimensions of data science such as individual differences, domain-expertise, design implications, and societal impact. Within HCDS we work across several topics, including digital media platforms, information visualization, crowd sourcing, affective computing, behavioral modeling, and societal challenges related to digital infrastructure more broadly.


<div id="people" class="People">
  <h1>People</h1>
  {% if site.people  %}
    <div class="container">
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
  var myList = document.querySelector('#people');
  for (var i = myList.children.length; i >= 0; i--) {
      myList.appendChild(myList.children[Math.random() * i | 0]);
  }
</script>


<!-- # People

**Luca Rossi**  
*Associate Professor*  
lucr@itu.dk

{% responsive_image path: assets/img/profile-photos/luca.jpg class: "img-fluid rounded z-depth-1" alt: "Photo of Luca Rossi" %}

Luca Rossi’s research connects media and communication studies with computational approaches. He explores how digital technologies and social media impact complex social processes such as participation, activism, politics and, more recently, information propagation.

**Søren Knudsen**  
*Assistant Professor*  
soekn@itu.dk

{% responsive_image path: assets/img/profile-photos/soren.jpg class: "img-fluid rounded z-depth-1" alt: "Photo of Søren Knudsen" %}

Søren Knudsen’s research focuses on information visualization and human-computer interaction. He is interested in supporting people in understanding, making sense of, and discussing data in face-to-face and online contexts, for example supported by large or multiple displays and social media.

**Aske Mottelson**  
*Assistant Professor*  
asmo@itu.dk

{% responsive_image path: assets/img/profile-photos/aske.png class: "img-fluid rounded z-depth-1" alt: "Photo of  Aske Mottelson" %}

Aske Mottelson’s research is in the intersection between psychology and data science. Aske conducts experiments and employs methods from statistical analysis and behavioral modeling to expand our understanding of humans through the use of technology. Aske is currently interested in (among other things) affective computing, sensing techniques, and virtual reality.

## Alumni

**Öykü Yilmaz**  
*Master student*  
oeyi@itu.dk

{% responsive_image path: assets/img/profile-photos/oyku.png class: "img-fluid rounded z-depth-1" alt: "Photo of Öykü Yilmaz" %}

Öykü Yilmaz is a MSc Student in Software Design. She is designing a prototype to improve the self-awareness of Twitter users by visualizing the consequences of their actions when sharing or retweeting a post. The project build on mixed methods and aims both at measuring the actual users’ understanding of the consequences of their network behavior as well as testing several visualization strategies to improve it.
-->
