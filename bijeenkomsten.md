---
layout: default
title: Bijeenkomsten
description: In samenwerking met Code for NL en de Foundation for Public Code organiseren we open bijeenkomsten over het algoritmeregister en algoritmische transparantie in bredere zin.
---
## Bijeenkomsten

Iedere laatste **maandag** van de maand is er een Kopgroepgroep bijeenkomst: deze zijn open voor algoritmeverantwoordelijken en -geïnteresseerden uit andere organisaties die willen meekijken en meeleren.

Iedere laatste **donderdag** van de maand is er een open meetup over algoritmische transparantie in bredere zin, voor developers en designers, onderzoekers, betrokken ambtenaren en andere geïnteresseerden.

<ul>
{% for bijeenkomst in site.data.bijeenkomsten %}
<li>
    <b>{{ bijeenkomst.wanneer }}</b>
    <h2>{{ bijeenkomst.titel }}</h2>
    <span class="label">{{ bijeenkomst.type }}</span>
    <p>{{ bijeenkomst.omschrijving }}</p>
</li>
{% endfor; %}
</ul>

<h2 class="my5">Aanmelden</h2>

Aanmelden kan via de Code for NL meetup pagina.

<a href="https://www.meetup.com/Code-For-NL/" class="btn display-inline-block mb4">www.meetup.com/Code-For-NL/</a>
