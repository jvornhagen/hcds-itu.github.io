---
layout: page
title: large high-resolution displays
description: Much of my research deals with visualizations on large displays. With large displays, it is possible to show one large visualization, or alternatively, many smaller visualization views.
img: assets/img/topics/large-high-resolution-displays-square.png
importance: 2
---

Much of my research deals with visualizations on large displays. With large displays, it is possible to show one large visualization, or alternatively, many smaller visualization views. The figure illustrates the option of showing many smaller visualization views. I see this choice as principal, and as the most important consideration to keep in mind, when designing visualizations for large displays.

Displaying one large visualization gives room to subdivide the space into what we can consider as separate views. This option enables the designer to use spatial encoding to communicate the relations between individual views.

Displaying many smaller visualization views, designers can let users arrange these to make sense of data. This option leaves the task of communicating views’ relations to the designer, primarily using alternatives to spatial encoding.

This is a simple but crucial point of my thesis work {% cite knudsen2015how %}.

Clearly, while these two options delimit the potential extremes of visualization views’ size, it is also possible to use them in combination. For example, by showing small views as overlays on top of a large visualization that fills an entire display.

In my work, I study both of these options. However, my focus has mainly been on using many small visualization views. This changes the manifestation of abundant display space. Here, abundant display space turns view-considerations into metaview considerations (i.e., considerations about or beyond the view), and changes the focus to letting users create new visualizations effectively and showing meta-visualizations of their relations. I discuss this in a paper co-authored with Sheelagh Carpendale, where we also introduce the notion of view relations {% cite knudsen2016view %}.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/1.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/3.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/5.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal it's glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/6.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% responsive_image path: assets/img/11.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

References
----------

<div class="publications">
  {% bibliography --cited %}
</div>
