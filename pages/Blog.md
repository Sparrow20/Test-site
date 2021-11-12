---
layout: page
title: Blog
permalink: /blog/
---

<div class="posts">
    {% assign sorted = site.post| sort: 'date' | reverse %}
    {% for post in sorted%}
        <article>
            <h1><a href="/site{{ post.url }}">{{ post.title }}</a></h1>
            Published on {{ post.date | date_to_string }}
            {{ post.excerpt }}
        </article>
    {% endfor %}
</div>