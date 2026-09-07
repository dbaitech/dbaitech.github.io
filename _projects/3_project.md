---
layout: page
title: Evolutionary Game Theory
description: Distillation and implementation of a paper
img: assets/img/evolution.jpg
importance: 1
category: Computational Biology
related_publications: true
---

Biological populations evolve under pressure from a combination of factors: 
- random genetic mutations
- unpredictable environmental disturbance
- interactions between each other

Natural selection can be abstracted into the idea of there being strategies 'chosen' by evolutionary agents. These strategies consist of the selection of certain genetic mutations that arise in the population over time and they have the underlying goal of maximizing their own fitness in preserving the proportion of stable phenotypes in the population.

In the paper *Stochastic noncooperative and cooperative evolutionary game strategies of a population of biological networks under natural selection* {% cite CHEN201790 %}, this is modelled as both non-cooperative and co-operative evolutionary games. In this project, I focus on the non-cooperative case.

I look at modeling the rate of change of different species in a population which will then be used to demonstrate how effective certain strategies are, meaning how effectively they can counter disturbances and maintain a stable population state with minimal evolutionary effort.

Code and in depth explanation available at: 

{% assign repo = site.data.repositories.github_repos[1] %}
{% if repo %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo.liquid repository=repo %}
</div>
{% else %}
  <a href="https://github.com/dbaitech/evolutionary-game-theory">Evolutionary Game Theory</a>.
{% endif %}