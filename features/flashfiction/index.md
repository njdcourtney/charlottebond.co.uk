---
layout: default
title: Flash Fiction
---

For 2018 I'm publishing a piece of flash fiction on the first Friday of every month. All the pieces are on my blog, but here they are all collected in one place.

<ul>
{% for post in site.categories.flashfiction %}
<li><a href="{{ post.url }}">{{ post.title }}</a> Posted on {{ post.date | date: '%B %-d, %Y' }}</li>
{% endfor %}
</ul>