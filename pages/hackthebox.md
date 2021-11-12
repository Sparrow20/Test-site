---
layout: page
title: Hack The Box Write-ups 
permalink: /hackthebox/
---

<div class="hackthebox">
    {% assign sorted = site.hackthebox| sort: 'date' | reverse %}
    {% for hackthebox in sorted%}
        <article>
            <h1><a href="/site{{ hackthebox.url }}">{{ hackthebox.title }}</a></h1>
            Published on {{ hackthebox.date | date_to_string }}
            {{ hackthebox.excerpt }}
        </article>
    {% endfor %}
</div>