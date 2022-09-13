---
layout: default
title: Standaard voor Algoritmische Transparantie
description: Wat willen we voor informatie bijhouden over de inzet van algoritmische applicaties? Het consortium "publieke controle op algoritmes" heeft hiervoor een versie 0.2 standaard opgesteld. Deze willen we nu met alle overheden in de praktijk verder doorontwikkelen. In een parallel wetstraject wordt - ook in overleg met overheden - bezien welke informatie verplicht zal worden.
splash: true
cta-button:
    url: https://standaard.algoritmeregister.org
    text: Meer informatie
---
<div id="data"></div>
<script>
    var _data;
    var url = "https://standaard.algoritmeregister.org/schemas/registration-v0.2.nl.schema.json";
    fetch(url).then(response => response.json()).then(data => render(data));

    function render(data) {
        console.log(data);
        var rootDiv = document.createElement("div");
        rootDiv.setAttribute("id", "data");
        for(var i in data.properties) {
            var prop = data.properties[i];
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
