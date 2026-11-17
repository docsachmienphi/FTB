---
layout: default
title: Story Topics
description: "Browse From The Beginning stories by topic: drinks and food, sportswear and shoes, cars, tech and shopping, and the founders themselves."
permalink: /topics/
redirect_from:
  - /catalogue/
---

# Browse Stories by Topic

Every story we tell, sorted by topic. Some topics hold the brands you see every day. One topic holds the people behind them. Pick a topic that makes you curious, and begin where it began.

<div class="grid">
{% assign p = site.posts | where: "slug", "history-of-kfc" | first %}
<div class="story" onclick="location.href='/topics/drinks-and-food/'">
<div class="cover cover-thumb"><img src="{{ p.cover_thumb }}" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Topic &middot; {{ site.data.catalogue["drinks-food"] | size }} stories</div><h3>Drinks & Food</h3><p>Coca-Cola, Pepsi, KFC, Starbucks and more: the tastes the whole world knows, from the very first day.</p></div>
</div>
{% assign p = site.posts | where: "slug", "history-of-nike" | first %}
<div class="story" onclick="location.href='/topics/sportswear/'">
<div class="cover cover-thumb"><img src="{{ p.cover_thumb }}" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Shelf &middot; {{ site.data.catalogue["sportswear"] | size }} stories</div><h3>Sportswear & Shoes</h3><p>Nike, Adidas, Puma and the football boot: the shoes the world runs in, and the brothers who split them in two.</p></div>
</div>
{% assign p = site.posts | where: "slug", "history-of-jensen-huang" | first %}
<div class="story" onclick="location.href='/topics/cars-tech-shopping/'">
<div class="cover cover-thumb"><img src="{{ p.cover_thumb }}" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Shelf &middot; {{ site.data.catalogue["cars-tech"] | size }} stories</div><h3>Cars, Tech & Shopping</h3><p>Toyota, Amazon, Walmart and NVIDIA: the machines and marketplaces that changed modern life.</p></div>
</div>
{% assign p = site.posts | where: "slug", "history-of-elon-musk" | first %}
<div class="story" onclick="location.href='/topics/people/'">
<div class="cover cover-thumb"><img src="{{ p.cover_thumb }}" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Shelf &middot; {{ site.data.catalogue["people"] | size }} stories</div><h3>People - The Founders</h3><p>Elon Musk, Jensen Huang and more: the founders and dreamers behind the brands. This topic keeps growing.</p></div>
</div>
</div>

Or simply browse [all the stories](/stories/) in one long list.

<script type="application/ld+json">
{"@context":"https://schema.org","@type":"ItemList","name":"From The Beginning Story Topics","itemListElement":[{"@type":"ListItem","position":1,"name":"Drinks & Food","url":"https://fromthebeginning.xyz/topics/drinks-and-food/"},{"@type":"ListItem","position":2,"name":"Sportswear & Shoes","url":"https://fromthebeginning.xyz/topics/sportswear/"},{"@type":"ListItem","position":3,"name":"Cars, Tech & Shopping","url":"https://fromthebeginning.xyz/topics/cars-tech-shopping/"},{"@type":"ListItem","position":4,"name":"People - The Founders","url":"https://fromthebeginning.xyz/topics/people/"}]}
</script>
