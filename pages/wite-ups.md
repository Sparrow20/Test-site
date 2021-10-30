---
layout: page
title: Write-Ups
permalink: /write-ups/
---

{% for writeup in site.writeups %}
  <div class="writeup">
    <h2><a href= "{{ writeup.url }}">{{ writeup.title }} </a></h2>
    {{ writeup.content }}
  </div>
{% endfor %}