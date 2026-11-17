---
layout: default
title: Company History
description: "From The Beginning company history stories: how famous companies were built, from the very first day - Coca-Cola, Nike, Adidas, Amazon, Toyota and more."
image: /assets/images/topics/company-history-cover.jpg
permalink: /company-history/
redirect_from:
  - /topics/company-history/
  - /catalogue/drinks-and-food/
  - /catalogue/sportswear/
  - /catalogue/cars-tech-shopping/
  - /topics/drinks-and-food/
  - /topics/sportswear/
  - /topics/cars-tech-shopping/
---

# Company History

Every famous company was once nothing. No big office. No famous name. Just a small idea, in a small place, and a long road ahead. Here are the stories of how those companies were built, told from the very first day: the first product, the first failure, the first small win, and the moment everything changed.

{% assign posts = site.categories["Company-History"] %}
<div class="grid">
{% for post in posts %}
<div class="story" onclick="location.href='{{ post.url }}'">
{% if post.cover_thumb %}<div class="cover cover-thumb"><img src="{{ post.cover_thumb }}" alt="" loading="lazy"></div>{% else %}<div class="cover {{ post.cover_class | default: 'c-default' }}{% if post.cover_image %} has-img{% endif %}">{% if post.cover_image %}<img class="cover-img" src="{{ post.cover_image }}" alt="" loading="lazy">{% endif %}<div class="years">{{ post.cover_years }}</div><div class="brand">{{ post.cover_brand | default: post.title }}</div>{% if post.cover_fate %}<div class="fate">{{ post.cover_fate }}</div>{% endif %}</div>{% endif %}
<div class="story-body"><div class="meta">{{ post.categories | first | replace: '-', ' ' }}</div><h3>{{ post.title }}</h3><p>{{ post.description }}</p></div>
</div>
{% endfor %}
</div>

Looking for another topic? Browse [Stories by Topic](/topics/) or [all stories](/stories/).
