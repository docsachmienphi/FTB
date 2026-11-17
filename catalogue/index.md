---
layout: default
title: Stories by Topic
description: "Browse From The Beginning stories by topic: company history, founder stories, and invention history."
permalink: /topics/
redirect_from:
  - /catalogue/
---

# Stories by Topic

Every story we tell is one of three kinds: the history of a company, the story of its founder, or the history of an invention. Most stories are two at once, a company and the person who began it. Choose the kind you love most, and begin where it began.

<div class="grid">
{% assign n = site.categories["Company-History"] | size %}
<div class="story" onclick="location.href='/company-history/'">
<div class="cover cover-thumb"><img src="/assets/images/coca/coca-pemberton-lab.jpg" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Topic &middot; {% if n == 1 %}1 story{% else %}{{ n }} stories{% endif %}</div><h3>Company History</h3><p>How famous companies were built, from the very first day: Coca-Cola, Nike, Amazon, Toyota, KFC and many more.</p></div>
</div>
{% assign n = site.categories["Founder-Stories"] | size %}
<div class="story" onclick="location.href='/founder-stories/'">
<div class="cover cover-thumb"><img src="/assets/images/elon/elon-hero.jpg" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Topic &middot; {% if n == 1 %}1 story{% else %}{{ n }} stories{% endif %}</div><h3>Founder Stories</h3><p>The founders and dreamers behind the brands: Elon Musk, Jensen Huang, Harland Sanders and many more.</p></div>
</div>
{% assign n = site.categories["Invention-History"] | size %}
<div class="story" onclick="location.href='/invention-history/'">
<div class="cover cover-thumb"><img src="/assets/images/boot/boot-lineup.jpg" alt="" loading="lazy"></div>
<div class="story-body"><div class="meta">Topic &middot; {% if n == 1 %}1 story{% else %}{{ n }} stories{% endif %}</div><h3>Invention History</h3><p>How famous things were invented, and the hands that made them real. More invention stories are coming.</p></div>
</div>
</div>

Or simply browse [all the stories](/stories/) in one long list.

<script type="application/ld+json">
{"@context":"https://schema.org","@type":"ItemList","name":"From The Beginning Stories by Topic","itemListElement":[{"@type":"ListItem","position":1,"name":"Company History","url":"https://fromthebeginning.xyz/company-history/"},{"@type":"ListItem","position":2,"name":"Founder Stories","url":"https://fromthebeginning.xyz/founder-stories/"},{"@type":"ListItem","position":3,"name":"Invention History","url":"https://fromthebeginning.xyz/invention-history/"}]}
</script>
