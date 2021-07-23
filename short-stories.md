---
layout: default
title: Short Stories
---

{% assign sorted-posts = site.short-stories | reverse %}
{% for story in sorted-posts %}

### {{story.title}}

{{ story.content | markdownify }}

{% endfor %}
