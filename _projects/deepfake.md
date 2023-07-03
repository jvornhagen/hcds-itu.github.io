---
layout: page
title: DEEPFAKE
description: Investigating Persuasiveness of Deepfake vidoes
img: assets/img/template/12.jpg
importance: 1
category: research
researchers: [davw@itu.dk, lucr@itu.dk, soekn@itu.dk, asmo@itu.dk]
published: false
---

This project will investigate the threat to online information integrity posed by the emergence of recent advances to synthetically generated disinformation (so-called deepfakes). To that end, the project will investigate the cognitive effects of exposure to deepfake-videos presented as evidence in the context of a deceptive social media posts, by comparing exposure to social media posts including less sophisticated deceptive media. By analyzing the effects of deepfake stimuli in a realistic context, this project will shed light on the extend of the threat posed by this emerging technology and inform future decision makers with insights about the cognitive factors that shape users’ perception of disinformation when contextualized across media formats.

This project is funded by [Meta Research](https://research.facebook.com/), through the [Foundational Integrity Research programme](https://research.facebook.com/research-awards/2022-foundational-integrity-research-request-for-proposals/#award-recipients).

<h3> People </h3>
<div class="row">
    {% for researcher in page.researchers %}
        {% assign person = site.people | find: "email", researcher %}
        {% include person.html %}
    {% endfor %}
</div>
<div class="caption">
    Researchers involved in the project
</div>


