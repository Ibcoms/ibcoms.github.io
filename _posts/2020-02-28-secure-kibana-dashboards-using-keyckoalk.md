---
layout: post
title: Secure kibana dashboards using keycloak
#subtitle: Each post also has a subtitle
gh-repo: dnodal0/installcentos
gh-badge: [star, fork, follow]
thumbnail-img: "https://d3uyj2gj5wa63n.cloudfront.net/wp-content/uploads/2018/11/keycloack_spring_multitenant.png"
tags: [kiban,keycloak,elk]
categories: Elastic
comments: true
feature: true
---

Kibana is an open source data visualization plugin for Elasticsearch. It provides visualization capabilities on top of the content indexed on an Elasticsearch cluster. Users can create bar, line, and scatter plots, or pie charts and maps on top of large volumes of data.

But while using kibana, you'll sooner or later face the need to secure it. Kibana itself doesn't support authentication or restricting access to dashboards and we need to use either the official solution from elastic: xpack security, or alternative solutions like search-gard or nginx.

This post, adds another option based on the open source identity and access management from Redhat: keycloak