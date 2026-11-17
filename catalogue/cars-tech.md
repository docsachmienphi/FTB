---
layout: default
title: Cars, Tech & Shopping Stories
description: "From The Beginning stories about how famous car, technology and shopping companies began: Toyota, Amazon, Walmart, NVIDIA, Elon Musk and Jensen Huang."
permalink: /topics/cars-tech-shopping/
redirect_from:
  - /catalogue/cars-tech-shopping/
---

# Cars, Tech & Shopping

Some beginnings change how the whole world moves, thinks, and shops. A loom maker whose son dreamed of cars. Books packed one box at a time in a garage, until the garage became the world's biggest store. A small-town shop that outgrew every rival, and computer chips first drawn on a napkin in a diner booth. These are the stories of the machines and marketplaces of modern life.

{% assign slugs = site.data.catalogue["cars-tech"] %}
<div class="grid">
{% for post in site.posts %}{% if slugs contains post.slug %}
<div class="story" onclick="location.href='{{ post.url }}'">
{% if post.cover_thumb %}<div class="cover cover-thumb"><img src="{{ post.cover_thumb }}" alt="" loading="lazy"></div>{% else %}<div class="cover {{ post.cover_class | default: 'c-default' }}{% if post.cover_image %} has-img{% endif %}">{% if post.cover_image %}<img class="cover-img" src="{{ post.cover_image }}" alt="" loading="lazy">{% endif %}<div class="years">{{ post.cover_years }}</div><div class="brand">{{ post.cover_brand | default: post.title }}</div>{% if post.cover_fate %}<div class="fate">{{ post.cover_fate }}</div>{% endif %}</div>{% endif %}
<div class="story-body"><div class="meta">{{ post.categories | first | replace: '-', ' ' }}</div><h3>{{ post.title }}</h3><p>{{ post.description }}</p></div>
</div>
{% endif %}{% endfor %}
</div>

Looking for another topic? Browse [all topics](/topics/) or [all stories](/stories/).
