---
layout: page
title: Try Hack Me Write-ups 
permalink: /tryhackme/
---

<div class="tryhackme">
    {% assign sorted = site.tryhackme| sort: 'date' | reverse %}
    {% for tryhackme in sorted%}
        <article>
            <h1><a href="/site{{ tryhackme.url }}">{{ tryhackme.title }}</a></h1>
            Published on {{ tryhackme.date | date_to_string }}
            {{ tryhackme.excerpt }}
        </article>
    {% endfor %}
</div>