---
layout: base
title: "Nos clients"
css:
  - /assets/css/index.css
ext-css:
  - //fonts.googleapis.com/css?family=Roboto:400,700
js:
  - /assets/js/index.js
ext-js:
  - //cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js
cover-img: "/assets/img"
---
<div id="header" markdown="1">
</div>
<div id="clients-out" class="page-section cut1">
  <div id="clients">
    <div class="section-title">Ils nous font confiance</div>
    <div id="clients-subtitle">Nos clients sont de grand groupes</div>
    <div id="client-logos">
      {% for client in site.data.clients %}
        <a class="client-img" href="{{ client.url }}" title="{{ client.name }}">
          <img alt="{{ client.name }}" src="/assets/img/logos/{{ client.img }}" />
        </a>
      {% endfor %}
    </div>
  </div>
</div>