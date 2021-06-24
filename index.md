---
layout: base
title: "Ibcoms | Devops & Cloud Consulting"
css:
  - /assets/css/index.css
ext-css:
  - //fonts.googleapis.com/css?family=Roboto:400,700
js:
  - /assets/js/index.js
ext-js:
  - //cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js
---

<div id="header" markdown="1">
# Ibcoms {#title}
<div id="header-inner" markdown="1">

## Consulting {#subtitle}

#### Expert DevOps et Cloud [David AKIF](https://www.ibcoms.com/) {#sub-subtitle}
</div>

<a href="/contact" class="actionbtn">
<span class="far fa-envelope" aria-hidden="true"></span>
Contactez-nous
</a>
{: .actionbtn-out :}
<div id="particles-js"></div>
</div>

<div id="main-sections">

<div id="clients-out" class="page-section">
  <div id="clients">
    <div class="section-title">Ils nous font confiance</div>
    <div id="clients-subtitle">Nos clients partagent les mêmes exigences d'efficacité, de réactivité et de qualité.</div>
    <div id="client-logos">
      {% for client in site.data.clients %}
        <a class="client-img" href="{{ client.url }}" title="{{ client.name }}">
          <img alt="{{ client.name }}" src="/assets/img/logos/{{ client.img }}" />
        </a>
      {% endfor %}
    </div>
  </div>
</div>

<!--- Latest blog -->
<!---
<div id="services-out" class="page-section">
  <div id="services">
    <div id="services-list">
    </div>
  </div>
</div>
-->
<!--- A propos -->
<div class="cut-buffer aboutus-buffer"></div>
<div id="aboutus-out" class="page-section">
  <div id="aboutus">
    <div class="section-title">A propos d'Ibcoms</div>
    <div id="aboutus-text">
    Fondée en 2019 par David AKIF <b>Ibcoms</b> est une société française de conseil et d'ingénierie informatique située au cœur de la ville de Rueil-Malmaison.
    <br/>Nous mettons en avant notre savoir-faire autour du <b>DevOps</b> et du <b>Cloud.</b><br/>
    <b>Ibcoms</b> rassemble une équipe d'Experts qui partage leurs connaissances et leurs passion.
    <br/><br/><b></b>
    </div>
  </div>
</div>
<!--- -->
<div id="cta-out" class="page-section">
  <div id="cta">
    <div class="section-title">Cloud Consulting</div><br/>
    <div class="section-sub-title">DevOps, Cloud privé/public, Docker/Kubernetes</div>
  <br/>
  </div>
</div>

<!--- Clients -->
<div class="cut-buffer portfolio-buffer"></div>

<div id="portfolio-out" class="page-section grey-section">
  <div id="portfolio">
    <div class="section-title">
      Outils DevOps les plus utilisés
    </div>
    <div id="shinyapps-big">
      {% for app in site.data.portfolio %}
	    <div class="shinyapp">
          <a class="applink" href="{{ app.url }}">
            <img class="appimg" src="/assets/img/screenshots/{{ app.img }}" />
            <div class="apptitle">{{ app.title }}</div>
            <div class="appdesc">{{ app.description }}</div>
          </a>
        </div>
	  {% endfor %}
    </div>
  </div>
</div>
<div id="portfolio-out" class="page-section grey-section">
  <div id="portfolio">
    <div class="section-title">
      Derniers articles
    </div>
    <div id="shinyapps-big">
      {% for app in site.posts limit:6 %}
	    <div class="shinyapp">
          <a class="applink" href="{{ app.url }}">
            <img class="appimg" src="{{ app.thumbnail-img | absolute_url }}" alt="Post thumbnail">
            <div class="apptitle">{{ app.title }}</div>
            <div class="appdesc">{{ app.desc }}</div>
          </a>
        </div>
	  {% endfor %}
    </div>
  </div>
</div>
  </div>