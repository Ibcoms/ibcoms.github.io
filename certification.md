---
layout: base
title: "Nos certifications"
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
    <div class="section-title">Nos certifications et qualifications</div>
    <div id="clients-subtitle">La reconnaissance de notre savoir-faire</div>
    <div id="client-logos">
      {% for cert in site.data.certifications %}
        <a class="cert-img" href="{{ cert.url }}" title="{{ cert.name }}">
          <img alt="{{ cert.name }}" src="/assets/img/logos/{{ cert.img }}" />
        </a>
      {% endfor %}
    </div>
  </div>
</div>