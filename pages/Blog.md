---
layout: page
title: Blog
permalink: /blog/
---

<div class="posts">
    {% for post in site.post%}
        <article>
            <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
            Published on {{ post.date | date_to_string }}
            {{ post.excerpt }}
        </article>
    {% endfor %}
</div>