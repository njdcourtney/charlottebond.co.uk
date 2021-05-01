---
layout: default
title: Prince Questions
---

2019 is the year of the prince! 

Throughout 2018, I asked friends and contacts what they thought made a good princess. You can find the answers to those questions [here]({% link features/princessquestions/index.md %}) 

This year, I will be asking authors from a variety of genres as well as a host of others from editors to academics, what they think makes a definitive prince.

<ul>
{% for post in site.categories.princequestions %}
<li><a href="{{ post.url }}">{{ post.title }}</a> Posted on {{ post.date | date: '%B %-d, %Y' }}</li>
{% endfor %}
</ul>