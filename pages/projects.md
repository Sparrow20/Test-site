---
layout: page
title: Projects
permalink: /projects/
---


{% for projects in site.projects %}
  <div class="projects">
    <h2><a href= "/site{{ projects.url }}">{{ projects.title }} </a></h2>
    {{ projects.content }}
  </div>
{% endfor %}