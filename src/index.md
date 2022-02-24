---
title: My first page Nurul Atiah
layout: base.njk
---

{% include "postlist.njk" %}

{% for fact in facts | randomItem %}{% endfor %}

## Blog Posts

{% for post in collections.posts %}
{{ post.data.title }}
{% endfor %} 

## Cat of the Day

<img src="{{ catpic }}" />