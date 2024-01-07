---
layout: page
title: "BlendMR: A Computational Method to Create Ambient Mixed Reality Interfaces"
related_publications: 
---

{% assign entry = bibliography --query @*[title={{page.title}}] %}

<div class = "publication-authors"> 
{{entry.author}}</div>

{%- if entry.award != blank -%}
    <div class = "publication-award"> <i class="fa-solid fa-trophy"></i> {{entry.award}}</div>
{%- endif -%}

<a class = "publication-venue" href={{entry.conference_link}}>{{entry.conference}}</a>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path=entry.fig1 title="figure 1" class="img-fluid " %}
    </div>
</div>


<div class = "publication-header"> Abstract</div>
{{entry.abstract}}
<div class = "publication-header"> Paper </div>
<a class = "publication-materials" href = {{entry.pdf}}>View paper PDF</a>
<br>
<a class = "publication-materials" href = {{entry.url}}>View in ACM Digital Library</a>


<div class = "publication-header"> Video</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/3vQCdW7UCN8?si=rwHOWEL9Ss1Jfp4r" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>
</div>