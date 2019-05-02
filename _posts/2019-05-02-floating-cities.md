---
layout: post
title: "The Floating Cities of Venus"
category: art
tags: [writing, art, scifi]
---
{% assign theart = site.art | where: 'title', 'The Floating Cities of Venus' %}
{% for art in theart %}
    ![{{ art.title }}]({{ art.image_path }} "{{ art.title }}")
    {{ art.description }}
{% endfor %}