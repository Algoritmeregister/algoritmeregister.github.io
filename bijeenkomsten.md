---
layout: default
title: Bijeenkomsten
description: Maandelijks zijn er open bijeenkomsten voor algoritmeverantwoordelijken en geïnteresseerden uit andere organisaties die willen meekijken en meeleren.
splash: true
orgs: true
---
<ul>
{% for bijeenkomst in site.data.bijeenkomsten %}
<li>
    <b>{{ bijeenkomst.wanneer }}</b>
    <h2>{{ bijeenkomst.titel }}</h2>
    <span class="label">{{ bijeenkomst.type }}</span>
    <p>{{ bijeenkomst.omschrijving }}</p>
</li>
{% endfor %}
</ul>

<h2 class="my5">Aanmelden</h2>

Aanmelden kan via de Code for NL meetup pagina.

<a href="https://www.meetup.com/Code-For-NL/" class="btn display-inline-block mb4">www.meetup.com/Code-For-NL/</a>
