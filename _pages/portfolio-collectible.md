---
permalink: /portfolio-summary/collectible/
title: "Collectible Portfolio Summary"
layout: archive
author_profile: false
---

Track and analyze collectible investments including LEGO sets, trading cards, and other valuable items.

## Portfolio Entries

{% assign collectibles_posts = site.categories.collectibles %}
{% if collectibles_posts.size > 0 %}
  {% for post in collectibles_posts reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
  *No collectibles entries yet.*
{% endif %}
