---
layout: default
title: Documenten en verwijzingen
description: Relevante documenten en links, onder andere vanuit het voorgaande programma "publieke controle op algoritmes".
splash: true
cta-button:
    url: /bijeenkomsten
    text: Kom naar de bijeenkomsten
---
{% assign docs = site.data.documenten | sort: "title" %}
{% for doc in docs %}
[{{ doc.title }}](#{{ doc.title | downcase | replace: "*", "" | replace: "(", "" | replace: ")", "" | replace: " ", "-" }})
{% endfor %}

{% for doc in docs %}
## {{ doc.title }}
{{ doc.description }}
[terug omhoog](#)
{% endfor %}
