---
layout: default
title: The Source
number: 003
---

# The Source

MY WONDEFUL SOURCES
<!-- <iframe width="420" height="315" src="https://www.youtube.com/watch?v=EmSrQCDsMv4&t=1282s&ab_channel=BillRaymond" frameborder="0" ></iframe> -->



{% assign pages = site.pages | where_exp: "item", "item.title" | where_exp: "item", "item.title != 'Search'" %}

{% assign collections = site.mindoc_images %}

{% assign pagesAndPosts = pages | concat: collections %}

{% for pageAndPost in pagesAndPosts %}
    {% for text in pagesAndPosts %}
    {{ text.url | jsonify }}
    {% endfor %}
{% endfor %}






