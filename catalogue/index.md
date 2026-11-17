---
layout: default
title: Story Catalogue
description: "The From The Beginning story catalogue: every story on its shelf - drinks and food, sportswear and shoes, cars, tech and shopping, and the founders themselves."
permalink: /catalogue/
---

# The Story Catalogue

Every story we tell, placed on its shelf. Some shelves hold the brands you see every day. One shelf holds the people behind them. Pick a shelf that makes you curious, and begin where it began.

<div class="grid">
{% assign p = site.posts | where: "slug", "history-of-kfc" | first %}
<div class="story" onclick="location.href='/catalogue/drinks-and-food/'">
<div class="cover cover-thumb"><img src="{{ p.cover_thumb }}" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Shelf &middot; {{ site.data.catalogue["drinks-food"] | size }} stories</div><h3>Drinks & Food</h3><p>Coca-Cola, Pepsi, KFC, Starbucks and more: the tastes the whole world knows, from the very first day.</p></div>
</div>
{% assign p = site.posts | where: "slug", "history-of-nike" | first %}
<div class="story" onclick="location.href='/catalogue/sportswear/'">
<div class="cover cover-thumb"><img src="{{ p.cover_thumb }}" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Shelf &middot; {{ site.data.catalogue["sportswear"] | size }} stories</div><h3>Sportswear & Shoes</h3><p>Nike, Adidas, Puma and the football boot: the shoes the world runs in, and the brothers who split them in two.</p></div>
</div>
{% assign p = site.posts | where: "slug", "history-of-jensen-huang" | first %}
<div class="story" onclick="location.href='/catalogue/cars-tech-shopping/'">
<div class="cover cover-thumb"><img src="{{ p.cover_thumb }}" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Shelf &middot; {{ site.data.catalogue["cars-tech"] | size }} stories</div><h3>Cars, Tech & Shopping</h3><p>Toyota, Amazon, Walmart and NVIDIA: the machines and marketplaces that changed modern life.</p></div>
</div>
{% assign p = site.posts | where: "slug", "history-of-elon-musk" | first %}
<div class="story" onclick="location.href='/catalogue/people/'">
<div class="cover cover-thumb"><img src="{{ p.cover_thumb }}" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Shelf &middot; {{ site.data.catalogue["people"] | size }} stories</div><h3>People - The Founders</h3><p>Elon Musk, Jensen Huang and more: the founders and dreamers behind the brands. This shelf keeps growing.</p></div>
</div>
</div>

Or simply browse [all the stories](/stories/) in one long list.

<script type="application/ld+json">
{"@context":"https://schema.org","@type":"ItemList","name":"From The Beginning Story Catalogue","itemListElement":[{"@type":"ListItem","position":1,"name":"Drinks & Food","url":"https://fromthebeginning.xyz/catalogue/drinks-and-food/"},{"@type":"ListItem","position":2,"name":"Sportswear & Shoes","url":"https://fromthebeginning.xyz/catalogue/sportswear/"},{"@type":"ListItem","position":3,"name":"Cars, Tech & Shopping","url":"https://fromthebeginning.xyz/catalogue/cars-tech-shopping/"},{"@type":"ListItem","position":4,"name":"People - The Founders","url":"https://fromthebeginning.xyz/catalogue/people/"}]}
</script>
