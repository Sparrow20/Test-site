---
layout: page
title: Write-Ups
permalink: /write-ups/
---

<div class="writeups">
    {% assign sorted = site.writeups| sort: 'date' | reverse %}
    {% for writeups in sorted%}
        <article>
            <h1><a href="/site{{ writeups.url }}">{{ writeups.title }}</a></h1>
            Published on {{ writeups.date | date_to_string }}
            {{ writeups.excerpt }}
        </article>
    {% endfor %}
</div>