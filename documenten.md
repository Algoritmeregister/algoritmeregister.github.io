---
layout: default
title: Documenten
description: Relevante documenten die onder andere vanuit het programma "publieke controle op algoritmes" zijn opgeleverd.
---
{% for doc in site.data.documenten %}
## {{ doc.title }}
{{ doc.description }}
{% endfor %}