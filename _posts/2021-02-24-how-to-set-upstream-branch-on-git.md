---
layout: post
title: How To Set Upstream Branch on Git
subtitle: DevOps, Git, and Agile updates from the Ibcoms team
gh-repo: dnodal0/installcentos
gh-badge: [star, follow]
thumbnail-img: "https://devconnected.com/wp-content/uploads/2019/10/featured-15.png"
tags: [branch,upstream,git]
comments: true
feature: true
---
Dans ce blog, vous apprendrez tout sur la configuration d'un amont pour un référentiel git, une branche et l'utilisation de la commande –set-upstream-to

You will also learn about different scenarios where git upstream is used and how to apply it in your git development workflow.

Have you wondered how to keep the forked repo in sync with the main repo? It’s done by adding the main repo as the upstream. It is explained in the below sections.
{% highlight javascript linenos %}
git remote add upstream https://github.com/devopscube/vagrant-examples.git
{% endhighlight %}
