---
layout: default
title: People & Founder Stories
description: "From The Beginning stories about the founders themselves: Elon Musk, Jensen Huang, and the people behind the brands. More founder stories are coming."
permalink: /catalogue/people/
---

# People - The Founders

Behind every beginning, there is a person. This shelf is for the founders themselves: the dishwasher who became a CEO, the young man who crossed an ocean with almost nothing, and the dreamers who kept going when it would have been easier to stop. We are telling more and more of these stories, and this shelf will keep growing.

{% assign slugs = site.data.catalogue["people"] %}
<div class="grid">
{% for post in site.posts %}{% if slugs contains post.slug %}
<div class="story" onclick="location.href='{{ post.url }}'">
{% if post.cover_thumb %}<div class="cover cover-thumb"><img src="{{ post.cover_thumb }}" alt="" loading="lazy"></div>{% else %}<div class="cover {{ post.cover_class | default: 'c-default' }}{% if post.cover_image %} has-img{% endif %}">{% if post.cover_image %}<img class="cover-img" src="{{ post.cover_image }}" alt="" loading="lazy">{% endif %}<div class="years">{{ post.cover_years }}</div><div class="brand">{{ post.cover_brand | default: post.title }}</div>{% if post.cover_fate %}<div class="fate">{{ post.cover_fate }}</div>{% endif %}</div>{% endif %}
<div class="story-body"><div class="meta">{{ post.categories | first | replace: '-', ' ' }}</div><h3>{{ post.title }}</h3><p>{{ post.description }}</p></div>
</div>
{% endif %}{% endfor %}
</div>

Looking for another shelf? Browse the [Story Catalogue](/catalogue/) or [all stories](/stories/).
