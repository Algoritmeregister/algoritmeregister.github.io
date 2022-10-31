---
layout: default
title: Werkdefinities Algoritmeregister
description: Wat is een algoritme? Wat bedoelen we met hoog risico? Op deze pagina houden we de werkdefinities bij voor de belangrijkste termen binnen Algoritmeregister.
splash: true
cta-button:
    url: /werkgroep
    text: Meer informatie
---
<div id="data"></div>
<script>
    var _data;
    var url = "https://standaard.algoritmeregister.org/data/glossary.json";
    fetch(url).then(response => response.json()).then(data => render(data));

    function render(data) {
        var rootDiv = document.createElement("div");
        rootDiv.setAttribute("id", "data");
        for(var i in data) {
            var prop = data[i];
            var p = document.createElement("p");
            var b = document.createElement("b");
            b.appendChild(document.createTextNode(
                `${prop.name} `));
            p.appendChild(b);
            var span = document.createElement("span");
            span.style.background = "#aaa";
            span.style.color = "#fff";
            span.style.borderRadius = "4px";
            span.style.padding = "0 4px";
            span.style.fontSize = "0.8em";
            span.style.fontFamily = "monospace";
            span.appendChild(document.createTextNode(
                `${i}`));
            p.appendChild(span);
            p.appendChild(document.createTextNode(
                `: ${prop.description}`));
            rootDiv.appendChild(p);
        }
        document.getElementById("data").replaceWith(rootDiv);
    }
</script>
