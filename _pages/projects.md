---
layout: page
title: art
permalink: /art/
description: As an undergrad, I did art and design at University of Michigan. Here are some of my projects from back in the days.
nav: true
nav_order: 4
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">

  <!-- <h2 class="category">{{ category }}</h2> -->
  {%- assign categorized_projects = site.projects | sort: "year"-%}
  {%- assign sorted_projects = categorized_projects| sort: "importance" %}
  <!-- Generate cards for each project -->
  
    <div class="grid" >
      {%- for project in site.projects -%}
        {% include projects.html %}
      {%- endfor %}
    </div>


</div>
