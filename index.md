---
title: Grimoire and Lore from Destiny
---

{% assign grimoire = site.grimoire | sort: 'order' %}
{% for item in grimoire %}
  <h2>{{ item.title }}</h2>

  {% if rental.content %}
    {{ rental.content }}
  {% endif %}
{% endfor %}
