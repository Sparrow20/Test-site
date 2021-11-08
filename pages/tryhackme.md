---
layout: page
title: Try Hack Me Write-ups 
permalink: /tryhackme/
---

{% for tryhackme in site.tryhackme %}
  <div class="tryhackme">
    <h2><a href= "/site{{ tryhackme.url }}">{{ tryhackme.title }} </a></h2>
    {{ tryhackme.content }}
  </div>
{% endfor %}