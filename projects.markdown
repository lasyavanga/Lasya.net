---
layout: page
title: Projects
permalink: /projects/
---

{% for project in site.data.projects %}

<div class="projects">
<p class="project-date">{{project.date}}</p>
<h4>{{project.title}}</h4>
<p>{{project.description}}</p>

{% for link in project.links %}

<ul>
<li><a href="{{link.link}}">{{link.name}}</a></li>
</ul>
{% endfor %}

</div>
{% endfor %}
