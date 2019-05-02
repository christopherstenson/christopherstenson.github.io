---
layout: post
title: "The Floating Cities of Venus"
category: art
tags: [writing, art, scifi]
---

{% assign theart = site.art | where: 'title', 'The Floating Cities of Venus' %}
{% for art in theart %}
    <img src="{{ art.image_path }}" title="{{ art.title }}" alt="{{ art.title }}"\>
    {{ art.description }}
{% endfor %}