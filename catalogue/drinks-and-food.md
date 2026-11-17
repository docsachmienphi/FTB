---
layout: default
title: Drinks & Food Stories
description: "From The Beginning stories about how famous drinks and food brands began: Coca-Cola, Pepsi, KFC, Starbucks, Heinz, Red Bull and Hershey."
permalink: /catalogue/drinks-and-food/
---

# Drinks & Food

The tastes the whole world knows began as one person's small experiment. A pharmacist stirring syrup in a backyard. A drink mixed at a small-town pharmacy counter. Fried chicken cooked at a gas station, and an energy drink from Thailand that nobody believed in. These are the stories of the drinks and foods on every table today, followed back to the first day.

{% assign slugs = site.data.catalogue["drinks-food"] %}
<div class="grid">
{% for post in site.posts %}{% if slugs contains post.slug %}
<div class="story" onclick="location.href='{{ post.url }}'">
{% if post.cover_thumb %}<div class="cover cover-thumb"><img src="{{ post.cover_thumb }}" alt="" loading="lazy"></div>{% else %}<div class="cover {{ post.cover_class | default: 'c-default' }}{% if post.cover_image %} has-img{% endif %}">{% if post.cover_image %}<img class="cover-img" src="{{ post.cover_image }}" alt="" loading="lazy">{% endif %}<div class="years">{{ post.cover_years }}</div><div class="brand">{{ post.cover_brand | default: post.title }}</div>{% if post.cover_fate %}<div class="fate">{{ post.cover_fate }}</div>{% endif %}</div>{% endif %}
<div class="story-body"><div class="meta">{{ post.categories | first | replace: '-', ' ' }}</div><h3>{{ post.title }}</h3><p>{{ post.description }}</p></div>
</div>
{% endif %}{% endfor %}
</div>

Looking for another shelf? Browse the [Story Catalogue](/catalogue/) or [all stories](/stories/).
