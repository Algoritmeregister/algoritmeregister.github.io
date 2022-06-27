---
layout: default
title: Bijeenkomsten
description: Maandelijks zijn er open bijeenkomsten voor algoritmeverantwoordelijken en geïnteresseerden uit andere organisaties die willen meekijken en meeleren.
splash:
    image: true
    link:
        url: https://kennisnetwerkdata.pleio.nl/groups/view/e724a355-a0e8-41ed-b436-adad74da1913/registratie-van-algoritmen-en-sensoren
        text: Praat mee op Pleio
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

Wil je uitnodigingen ontvangen voor de bijeenkomsten? Meld je aan met een e-mail naar:

<a href="mailto:info@algoritmeregister.org" class="btn display-inline-block mb4">info@algoritmeregister.org</a>

<!-- 
Aanmelden kan via de Code for NL meetup pagina.

<a href="https://www.meetup.com/Code-For-NL/" class="btn display-inline-block mb4">www.meetup.com/Code-For-NL/</a>
-->
