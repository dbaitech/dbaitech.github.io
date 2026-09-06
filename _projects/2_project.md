---
layout: page
title: CS Academy - Bioinformatics
description: Using Python to analyze DNA
img: assets/img/dna.png
importance: 1
category: Computational Biology
related_publications: false
---

I created and taught this project at the <a href="https://web.cs.toronto.edu/news-events/news/tag/CS+Academy">University of Toronto's CS Academy</a>, an annual weeklong research immersion course for high school students hosted by the Department of Computer Science.

Feel free to check out the <a href="https://github.com/dbaitech/cs_academy_bioinformatics/tree/main/lessons">lessons</a> I made and learn about how to analyze DNA using <b>genomic signatures</b> and <b>sequence alignment</b>!

You can also implement the DNA analysis toolkit in Python through these <a href="https://github.com/dbaitech/cs_academy_bioinformatics/tree/main/notebooks/colab_notebooks">Colab Notebooks</a>.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/genomic_signature.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sequence_alignment.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Full repository available at: 

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo.liquid repository=site.data.repositories.github_repos[4] %}
</div>
{% else %}
  <a href="https://github.com/dbaitech/cs_academy_bioinformatics">CS Academy Bioinformatics</a>.
{% endif %}