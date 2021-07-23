---
layout: default
title: Novels and Novellas
---

{% assign loopindex = 0 %}

{% assign sorted-posts = site.books | reverse %}
{% for story in sorted-posts %}

    {% assign loopindex = loopindex | plus: 1 %}
    {% assign rowfinder = loopindex | modulo: 2 %}

---

    {% if story.cover %}
        {% if rowfinder == 1 %}
{% include img-float-right.html img=story.cover alt=story.title link=story.cover %}
        {% else %}
{% include img-float-left.html img=story.cover alt=story.title link=story.cover %}
        {% endif %}
    {% endif %}

### {{story.title}}
{: .text-center}

{{ story.content }}

{% include clearfix.html %}
    
{% endfor %}



