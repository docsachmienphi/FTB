---
layout: default
title: Sportswear & Shoes Stories
description: "From The Beginning stories about how famous sportswear brands began: Nike, Adidas, Puma, and the history of the football boot."
permalink: /topics/sportswear/
redirect_from:
  - /catalogue/sportswear/
---

# Sportswear & Shoes

Every famous shoe began in a small room. Two brothers making shoes in their mother's laundry room, until one argument split them into two rival companies across a river. A young runner selling shoes from the trunk of his car. And a simple leather boot that, over five hundred years, became a boot of only 99 grams. These are the stories of the shoes the world runs in.

{% assign slugs = site.data.catalogue["sportswear"] %}
<div class="grid">
{% for post in site.posts %}{% if slugs contains post.slug %}
<div class="story" onclick="location.href='{{ post.url }}'">
{% if post.cover_thumb %}<div class="cover cover-thumb"><img src="{{ post.cover_thumb }}" alt="" loading="lazy"></div>{% else %}<div class="cover {{ post.cover_class | default: 'c-default' }}{% if post.cover_image %} has-img{% endif %}">{% if post.cover_image %}<img class="cover-img" src="{{ post.cover_image }}" alt="" loading="lazy">{% endif %}<div class="years">{{ post.cover_years }}</div><div class="brand">{{ post.cover_brand | default: post.title }}</div>{% if post.cover_fate %}<div class="fate">{{ post.cover_fate }}</div>{% endif %}</div>{% endif %}
<div class="story-body"><div class="meta">{{ post.categories | first | replace: '-', ' ' }}</div><h3>{{ post.title }}</h3><p>{{ post.description }}</p></div>
</div>
{% endif %}{% endfor %}
</div>

Looking for another topic? Browse [all topics](/topics/) or [all stories](/stories/).
