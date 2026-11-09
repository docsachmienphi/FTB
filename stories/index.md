---
layout: default
title: All Stories
description: "All From The Beginning stories: the entire history of famous companies, founders and inventions."
permalink: /stories/
---

# All Stories

Company history, founder stories, and great inventions, from the very beginning.

<div class="grid">
{% for post in site.posts %}
<div class="story" onclick="location.href='{{ post.url }}'">
<div class="cover {{ post.cover_class | default: 'c-default' }}{% if post.cover_image %} has-img{% endif %}">{% if post.cover_image %}<img class="cover-img" src="{{ post.cover_image }}" alt="" loading="lazy">{% endif %}<div class="years">{{ post.cover_years }}</div><div class="brand">{{ post.cover_brand | default: post.title }}</div>{% if post.cover_fate %}<div class="fate">{{ post.cover_fate }}</div>{% endif %}</div>
<div class="story-body"><div class="meta">{{ post.categories | first | replace: '-', ' ' }}</div><h3>{{ post.title }}</h3><p>{{ post.description }}</p></div>
</div>
{% endfor %}
</div>
