---
layout: page
title: Theorycraft
description: Bridging the Games Research-Practice Gap through Theory Translation
img: assets/img/projects/TheoryCraft.jpg
importance: 1
category: research
researchers: [elme@itu.dk, fefe@itu.dk, daben@itu.dk, ropi@itu.dk, javo@itu.dk]
---

<h3>Translating theory into practice for game designers</h3>

Games research rarely meets the needs of design practice. The EU-funded [THEORYCRAFT](https://cordis.europa.eu/project/id/101043198) project aims to bridge the gap between research and design practice. It will study the way game design practitioners use theory to demonstrate how theory needs to be transformed to bridge research and design practice. In addition, it will generate theories of poorly understood games phenomena based on theories in psychology, and deliver translational resources that express theories in ways that are helpful and practical for game design. Lastly, the project will assess how useful these theories are in closing the gap between research and design practice.


<h4>Objective</h4>

How can theory inform design practice? This question is among the grand challenges in both Human-Computer Interaction (HCI) and games research. Despite numerous efforts to bridge the research-practice gap, the two poles seem irreconcilable. Instead of a robust and generalizable knowledge base to tackle foundational problems around technology use, cumulative knowledge building is impeded by weak empirical studies and rampant theoretical misconceptions. Instead of providing practitioners with useful theory-based insights, research results often remain too abstract and not sufficiently actionable to be adopted into design practice.

THEORYCRAFT tackles this conundrum by means of theory translation, demonstrating how theory needs to be transformed and specified to bridge research and design practice. We approach theory translation from four angles: 1) We investigate how game design practitioners make use of theory to identify avenues for productive theory translation. 2) We translate theoretical propositions from psychology to build explanatory theories of ill-understood games phenomena. 3) We develop translational resources that convey theoretical propositions in a manner that is useful and actionable for game design. 4) We evaluate the translated theories in terms of their utility to bridge research and design practice. Individually, each angle will result in important advances in HCI and games research. Collectively, THEORYCRAFT will produce a breakthrough in transparent and systematic theory translation, which will radically transform how knowledge is built, represented and disseminated – steering HCI and games research towards greater scientific integrity, practical relevance, and impact.

<img src="LOGO_ERC-FLAG_EU.png" alt="Flag of the European Union and the Logo f the European Research Council" style="width:25%;height:25%">


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


