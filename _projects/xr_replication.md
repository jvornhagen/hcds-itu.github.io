---
layout: page
title: Replication crisis in Extended Reality
description: Exploring the extent of replicability in XR
img: assets/img/template/12.jpg
importance: 1
category: research
researchers: [olgl@itu.dk, asmo@itu.dk]
---

Extended reality (XR) research continues to produce breakthroughs in interaction techniques, discover remarkable behavioral effects of acting with virtual bodies and environments, and demonstrate its ability to move traditional laboratory experiments  online. In consequence, XR research has a growing relevance for many scientific communities with vast empirical and practical implications.
 
As in other sciences, questions about replicability and robustness of empirical findings are increasingly being raised. Despite XR as a technological medium is exceptionally well suited for cross-lab replications, initiatives that are being implemented in other behavioral sciences, such as open source, open data, preregistration, multi-site studies, adversarial collaboration, and many others, are rarely used in XR research.
 
Some of the most well known findings from XR research draws on inspiration from psychology, such as avatar embodiment, social biases, and therapy. As psychology as a science has been particularly criticized for lack of successful replications (Open Science Collaboration, Science, 2015), it further emphasizes the need for systematic investigations of scientific practices in XR research. 
 
This project will therefore explore the extent of the replicability crisis in XR research. The project will establish the applicability of initiatives, that have improved scientific practice in other research areas, for XR research. As a result, the project will lead an international open science initiative to make both previous and future XR research more robust.

The project is a joint project with [Department of Computer Science at University of Copenhagen](http://diku.dk), funded by the [Pioneer Centre for AI](https://www.aicentre.dk/), DNRF grant number P1.

<div class="row">
    {% for researcher in researchers %}
        {% assign person = site.people | find: "email", researcher %}
        {% include person.html %}
    {% endfor %}
</div>
<div class="caption">
    Researchers involved in the project
</div>


