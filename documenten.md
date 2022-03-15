---
layout: default
title: Documenten en verwijzingen
description: Relevante documenten en links, onder andere vanuit het voorgaande programma "publieke controle op algoritmes".
---
{% for doc in site.data.documenten %}
## {{ doc.title }}
{{ doc.description }}
{% endfor %}