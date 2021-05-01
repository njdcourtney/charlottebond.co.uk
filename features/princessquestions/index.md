---
layout: default
title: Princess Questions
---

2018 is the year of the princess! 

Throughout the year, I will be asking authors from a variety of genres as well as a host of others from editors to academics, what they think makes a definitive princess.

<ul>
{% for post in site.categories.princessquestions %}
<li><a href="{{ post.url }}">{{ post.title }}</a> Posted on {{ post.date | date: '%B %-d, %Y' }}</li>
{% endfor %}
</ul>