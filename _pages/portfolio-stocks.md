---
permalink: /portfolio-summary/stocks/
title: "Stock Portfolio Summary"
layout: archive
author_profile: false
---

Track and analyze equity investments including individual stocks, ETFs, and index funds.

## Portfolio Entries

{% assign stocks_posts = site.categories.stocks %}
{% if stocks_posts.size > 0 %}
  {% for post in stocks_posts reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
  *No stocks entries yet.*
{% endif %}
