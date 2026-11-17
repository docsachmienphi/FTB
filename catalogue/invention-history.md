---
layout: default
title: Invention History
description: "From The Beginning invention history stories: how famous things were invented, beginning with the five-hundred-year story of the football boot. More invention stories are coming."
permalink: /topics/invention-history/
---

# Invention History

Some beginnings are not a company or a person, but a thing. An idea that someone made real, which then quietly changed how the whole world lives. Our invention stories follow those things from their first day. This is our youngest topic, and it begins with a story of five hundred years: how a simple leather boot became the football boot of only 99 grams. More invention stories are coming.

{% assign posts = site.categories["Invention-History"] %}
<div class="grid">
{% for post in posts %}
<div class="story" onclick="location.href='{{ post.url }}'">
{% if post.cover_thumb %}<div class="cover cover-thumb"><img src="{{ post.cover_thumb }}" alt="" loading="lazy"></div>{% else %}<div class="cover {{ post.cover_class | default: 'c-default' }}{% if post.cover_image %} has-img{% endif %}">{% if post.cover_image %}<img class="cover-img" src="{{ post.cover_image }}" alt="" loading="lazy">{% endif %}<div class="years">{{ post.cover_years }}</div><div class="brand">{{ post.cover_brand | default: post.title }}</div>{% if post.cover_fate %}<div class="fate">{{ post.cover_fate }}</div>{% endif %}</div>{% endif %}
<div class="story-body"><div class="meta">{{ post.categories | first | replace: '-', ' ' }}</div><h3>{{ post.title }}</h3><p>{{ post.description }}</p></div>
</div>
{% endfor %}
</div>

Looking for another topic? Browse [Stories by Topic](/topics/) or [all stories](/stories/).
