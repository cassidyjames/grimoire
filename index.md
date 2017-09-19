---
title: Grimoire and Lore from Destiny
---

{% assign grimoire = site.grimoire | sort: 'order' %}
{% for item in grimoire %}
  ## {{ item.title }}

  {% if rental.content %}
    {{ rental.content }}
  {% endif %}
{% endfor %}
