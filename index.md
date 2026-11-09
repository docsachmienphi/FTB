---
layout: default
title: From The Beginning - How Companies Were Built
description: "The entire history of famous companies and founders, told slowly in simple English. Coca-Cola, Nike, Adidas, Amazon and more."
---

<div class="hero hero-banner">
<div class="kicker">Stories of how things began</div>
<h1>Every great company started small.</h1>
<p>Warm stories about how companies were built, how founders began with almost nothing, and how small ideas grew to change the world. Told slowly, in simple and clear English.</p>
<p><a class="btn" href="https://www.youtube.com/@FromTheBeginning9" target="_blank" rel="noopener">Watch on YouTube</a> <a class="btn btn-ghost" href="/stories/">Read the Stories</a></p>
<div class="timeline">
<div class="dot">1886<br>Coca-Cola</div>
<div class="dot">1898<br>Pepsi</div>
<div class="dot">1937<br>Toyota</div>
<div class="dot">1949<br>Adidas</div>
<div class="dot">1964<br>Nike</div>
<div class="dot">1994<br>Amazon</div>
</div>
</div>

## Latest Stories

Read a short version of each story, then watch the full story on YouTube.

<div class="grid">
{% for post in site.posts limit:9 %}
<div class="story" onclick="location.href='{{ post.url }}'">
<div class="cover {{ post.cover_class | default: 'c-default' }}"><div class="years">{{ post.cover_years }}</div><div class="brand">{{ post.cover_brand | default: post.title }}</div>{% if post.cover_fate %}<div class="fate">{{ post.cover_fate }}</div>{% endif %}</div>
<div class="story-body"><div class="meta">{{ post.categories | first | replace: '-', ' ' }}</div><h3>{{ post.title }}</h3><p>{{ post.description }}</p></div>
</div>
{% endfor %}
</div>

## Why From The Beginning?

Every big company was once a small idea in a kitchen, a garage, or a backyard. A sick pharmacist stirring syrup. Two brothers making shoes. A man selling books from his garage.

On this website you can read a short version of each story, learn the most surprising facts, and then watch the full story on YouTube.

## Popular Topics

- Company History: Coca-Cola, Nike, Adidas, Amazon, Toyota, Pepsi
- Founder Stories: the people behind the brands, and what they wanted
- Great Inventions: how famous things were invented
