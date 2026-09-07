---
layout: page
title: Family Tree Template
description: A Next.js project
img: assets/img/family_tree_1.png
importance: 1
category: Web Dev
related_publications: false
---

*Still in development* 

I'm developing a Next.js family tree template using the <a href="https://balkan.app/FamilyTreeJS">Balkan Family Tree library</a>. Designed with a clean aesthetic, it gives each family member a dedicated detail page that opens when selected.

Family data can be loaded directly from a JSON file or connected to a PostgreSQL database. The database structure uses modular tables to separate individuals from their relationships, which the application dynamically combines for rendering.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/family_tree_1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/family_tree_2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Code available at: 

{% assign repo = site.data.repositories.github_repos[5] %}
{% if repo %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo.liquid repository=repo %}
</div>
{% else %}
  <a href="https://github.com/dbaitech/family-tree">Family Tree</a>.
{% endif %}