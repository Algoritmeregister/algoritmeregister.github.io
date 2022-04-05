---
layout: default
title: Algoritmeregister in het kort
description: 
---
## Ontstaan: Publieke Controle op Algoritmen

Het consortium "publieke controle op algoritmes" is in 2020 gestart om te kijken op welke manier overheden transparanter kunnen zijn over de inzet van algoritmes in hun organisatie. Eind 2021 zijn daaruit voortgekomen ([bekijk de documenten online](algoritmeregister.org/documenten)):

- een Handreiking Governance, voor het verantwoord inzetten van algoritmische toepassingen;
- een Handreiking Bezwaarprocedure, voor het inrichten van een toegankelijke bezwaarprocedure voor algoritmisch genomen besluiten; en
- Inkoopvoorwaarden, contractbepalingen in aanvulling op de GIBIT voor het rechtvaardig gebruik van algoritmische toepassingen.

Daarnaast werd software design bureau Tiltshift aangehaakt om te helpen invulling te geven aan het idee van een "algoritmeregister". Tijdens de ontwerpsessies kwam naar voren dat de wensen en ideeën breed uiteen liepen: van een code database met daarin de programmacode van alle algoritmes die ingezet worden, tot inzicht in specifieke besluiten en de rol van een algoritme daarin, tot een "algoritmeinspectie" die (al dan niet vooraf) adviseert of toetst of de inzet van een bepaald algoritme ethisch verantwoord is, tot een "algoritme 101", uitlegfilmpjes voor de gebruikte algoritmes voor politici en beleidsmakers.

Uiteindelijk is gekozen voor een concept dat wat dichter bij huis ligt en een basis kan vormen ook voor één of meerdere van bovenstaande concepten: een registratie-applicatie waarin de organisatie voor iedere inzet van een (impactvol) algoritme bijhoudt waarom er in dat specifieke geval gekozen is om een algoritmische toepassing in te zetten, wat daarbij de risico's zijn en waar de verantwoordelijkheden liggen.

Ondertussen zijn er afgelopen jaar ook andere ontwikkelingen geweest: zowel vanuit de Europese Unie als vanuit de Tweede Kamer wordt aangestuurd op het verplicht bijhouden van een algoritmeregister door (publieke) organisaties. Ook zijn is er een scala aan "impact assesments" gepubliceerd vanuit diverse kennisinstituten voor de inzet van AI door overheden.

Het doel van het project algoritmeregister is om deze verschillende ontwikkelingen bij elkaar te brengen in één gezamenlijke context en vanuit daar instrumenten te realiseren die organisaties in de praktijk ondersteunen bij het verantwoorden en verantwoord inzetten van algoritmes in de overheid.

## Uit het filmpje

_"De overheid gebruikt algoritmes. Dit gebeurt ook in jouw organisatie. Bijvoorbeeld bij het onderhouden van de buitenruimte, het voorkomen van fraude, of het verbeteren van de verkeersveiligheid._

_We zetten algoritmes in om processen te verbeteren. Maar dat gaat niet altijd meteen goed._

_Als overheid ben je verplicht om verantwoord en transparant te handelen. Kan jij eigenlijk verantwoorden hou jouw organisatie algoritmes gebruikt? Daar kan de toolkit bij helpen: zo geeft het algoritmeregister inzicht in de wijze waarop algoritmes worden ingezet; het algoritmekader biedt overzicht van de geldende wet- en regelgeving, en hoe jouw organisatie verantwoording kan afleggen. De inkoopvoorwaarden zorgen ervoor dat ook leveranciers daaraan voldoen. Maakt een burger bezwaar op een besluit waar een algoritme ingezet is? Het "stappenplan bezwaar" legt uit hoe je de juiste informatie verzamelt om het bezwaar eerlijk te beoordelen._

_Ga aan de slag met de toolkit! Ga naar publiekecontrole.com __[redactie: deze is momenteel niet beschikbaar]__ voor meer informatie."_

## Uit de architectuurdocumentatie

### Kaders

- Overheid wil transparant zijn. Transparantie van besluitvorming en openbaarheid van __[redactie: de inzet van]__ algoritmen dragen daaraan bij.
- Overheid wil voldoen aan wet en regelgeving.
- Algoritmeregister draagt indirect bij aan transparantie van besluitvorming want geen inzicht in individuele besluiten. __[redactie: maar juist op de procesinrichting?]__

### Principes

- AR is open (informatie)
- AR gebruikt open format (standaard)
- AR is complient
- __[redactie: AR is onderdeel van common ground (open source)? open, tenzij?]__

### Richtlijnen

- AR gebruikt JSON
- AR API is beschreven __[redactie: creative commons?]__
- AR informatiemodel is open __[redactie: creative commons?]__
- AR voldoet aan WCAG __[redactie: versie 2.1?]__ voor Digitoegankelijkheid

### Principes __[redactie: principes deel 2?]__

- Begrijpelijk geschreven: begrijpelijke taal
- Grondslag beschreven: besluit om het in te zetten
- Minimale set informatie: standaard velden __[redactie: waaronder werking en data?]__
- Werking en data __[redactie: zie boven]__

### Hoofdlijn

Algoritme wordt gebruikt in een proces vanuit een grondslag (wet, regeling) en werkt op een set data (bewerkt informatie). De uitkomst van het algoritme is input voor een besluit. Dat besluit kun je aanvechten door middel van bezwaar of beroep. Tegen het besluit om het algoritme in te zetten kun je ook in bezwaar of beroep. Het is op dit moment niet wettelijk geregeld dat zo'n besluit er moet zijn (doorgaans de uitvoerder die besluit algoritme in te zetten, grondslag is verantwoordelijkheid van bestuurder).

Rollen en actoren: belanghebbende, volksvertegenwoordiger, uitvoerder, algoritmehouder __[redactie: wat is dit precies?]__.

## Algoritmeregister, een decentrale (common ground) tool

In het algoritmeregister worden registraties aangemaakt voor iedere inzet van een (impactvolle) algoritmische toepassing. Daarbij wordt beschreven welke rol het algoritme in het proces speelt en op hoofdlijnen wat en hoe het algoritme dat doet. Daarnaast worden verwijzingen opgenomen naar de (open source) code (+beschrijving) voor exacte functioneren en (open) data (+beschrijving) voor exacte trainingsdata (buiten het algoritmeregister).

Vastleggen van individuele besluiten (log) is geen onderdeel van het algoritmeregister. Daarvoor zou wellicht een andere toepassing kunnen komen, die dan verwijst naar de registratie in het algoritmeregister.

Het algoritmeregister moet de mogelijkheid bieden om de informatie over algoritmen op andere plaatsen te gebruiken, bijvoorbeeld naar de corporate website. Voor de hand ligt dit te realiseren door middel van een (gestandaardiseerde) API.

### As A Service

Mogelijk kan Algoritmeregister _"as a Service"_ aangeboden worden aan organisaties, zodat ze de software niet ieder onafhankelijk hoeven te installeren en updaten.

## Algoritmecatalogus, een centrale voorziening voor zoeken en inzien

Landelijke voorziening biedt overzicht van alle registraties in alle (aangemelde) decentrale algoritmeregisters met de mogelijkheid om  hierin te zoeken en te filteren (op organisatie, type algoritme, risico-indicatie, ...), en mogelijk ook dingen als abonneren op mutaties en voeren van discussies. Dit betreft de minimale set aan informatie vastgelegd in de landelijke standaard (vanuit consortium vastgesteld), een superset van de Europese standaard, zodat alle vereiste informatie vanuit EU uit de nationale catalogus kan worden opgehaald/aangeleverd. De lokale informatie in het algoritmeregister kan uitgebreider zijn, maar bevat ten minste de informatie vereist voor landelijke publicatie (door middel van (gestandaardiseerde) publicatie naar bijvoorbeeld data.overheid.nl of een andere landelijke faciliteit (nationale algoritmecatalogus).)

## Uit de woordenlijst

Een __algoritmische toepassing__ is software (een computerprogramma of "app") waarmee op geautomatiseerde wijze voorspellingen worden gedaan, besluiten worden genomen en/of adviezen worden gegeven door gebruik te maken van data-analyse, statistiek en/of zelflerende logica.

Algoritmische toepassingen worden ingezet bijvoorbeeld om de doorstroom van verkeer te regelen, om geluidsoverlast te voorspellen, of om fraudeurs op te sporen.

### Grip op inzet van algoritmische toepassingen

Een __algoritmeregister__ is een decentrale applicatie voor het maken, bijhouden en publiek beschikbaar stellen van registraties van de inzet van  algoritmische toepassingen door een (overheids)organisatie.

Met een algoritmeregister houden organisaties zicht op de algoritmes die ze gebruiken. Per inzet van een algoritmische toepassing slaan ze daarin informatie op over bijvoorbeeld doel, impact, menselijke maat, risico's, eigenaarschap en brondata.


### Centraal overzicht

BZK organiseert een centrale __catalogus__ waarin registraties uit de verschillende decentrale algoritmeregisters op één plek te doorzoeken en in te zien zijn.

### Open Standaard

Hoe meer organisaties in dezelfde structuur werken, hoe makkelijker het wordt om hierin te navigeren (en van elkaar te leren). Daarom wordt er door een breed consortium van overheden bottom-up gewerkt aan een open standaard voor de registratie van de inzet van algoritmische toepassingen door overheden, de _algoritmeregister standaard_ (EN: _Algorithmic Transparency Standard_). Zo weten leveranciers van algoritmeregister software welke informatie hun software moet bevatten en op welke manier die beschikbaar moet worden gesteld.

### Open Source

Een aantal van de betrokken overheden is voornemens om de algoritmeregister software zelf _open source_ te ontwikkelen. Dat wil wel zeggen dat de vraag is wie deze ontwikkeling gaat instigeren; dat kan door middel van het afnemen van een product van een leverancier (onder voorwaarde dat het een open source product is dat wordt doorontwikkeld), of door het organiseren van een ontwikkeltraject (waarbij dan alsnog moet worden geregeld dat er een hostingpartij is).

## Meer informatie

Voor meer informatie kunt u kijken op [www.algoritmeregister.org](https://www.algoritmeregister.org)
