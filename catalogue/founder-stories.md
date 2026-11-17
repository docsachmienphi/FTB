---
layout: default
title: Founder Stories
description: "From The Beginning founder stories: the people behind the brands - Elon Musk, Jensen Huang, Harland Sanders, Sam Walton and more."
permalink: /founder-stories/
redirect_from:
  - /topics/founder-stories/
  - /catalogue/people/
  - /topics/people/
---

# Founder Stories

Behind every beginning, there is a person. A dishwasher who became a CEO. A pharmacist who died before his drink conquered the world. A man who lost his restaurant at sixty-five and started again. These are the stories of the founders themselves, the dreamers who kept going when it would have been easier to stop. We are telling more and more of these stories.

{% assign posts = site.categories["Founder-Stories"] %}
<div class="grid">
{% for post in posts %}
<div class="story" onclick="location.href='{{ post.url }}'">
{% if post.cover_thumb %}<div class="cover cover-thumb"><img src="{{ post.cover_thumb }}" alt="" loading="lazy"></div>{% else %}<div class="cover {{ post.cover_class | default: 'c-default' }}{% if post.cover_image %} has-img{% endif %}">{% if post.cover_image %}<img class="cover-img" src="{{ post.cover_image }}" alt="" loading="lazy">{% endif %}<div class="years">{{ post.cover_years }}</div><div class="brand">{{ post.cover_brand | default: post.title }}</div>{% if post.cover_fate %}<div class="fate">{{ post.cover_fate }}</div>{% endif %}</div>{% endif %}
<div class="story-body"><div class="meta">{{ post.categories | first | replace: '-', ' ' }}</div><h3>{{ post.title }}</h3><p>{{ post.description }}</p></div>
</div>
{% endfor %}
</div>

Looking for another topic? Browse [Stories by Topic](/topics/) or [all stories](/stories/).
