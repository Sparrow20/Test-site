---
layout: page
title: Projects
permalink: /projects/
---

<div class="projects">
    {% assign sorted = site.projects| sort: 'date' | reverse %}
    {% for projects in sorted%}
        <article>
            <h1><a href="/site{{ projects.url }}">{{ projects.title }}</a></h1>
            Published on {{ projects.date | date_to_string }}
            {{ projects.excerpt }}
        </article>
    {% endfor %}
</div>