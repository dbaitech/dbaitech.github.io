---
layout: page
title: Cryptographic Algorithms
description: Homomorphic Encryption schemes implemented with Python
img: assets/img/homomorphic_encryption.png
importance: 1
category: Cryptography
related_publications: true
---

The goal of this project was to explore the combination of **LWE-based encryption and ElGamal** to develop a more efficient Private Information Retrieval (PIR) scheme. The project involved implementing both schemes and investigating how their homomorphic properties could be combined within a PIR protocol.

While the proposed combination did not ultimately result in a working efficient scheme, the project provided an opportunity to explore the practical implementation and limitations of these cryptographic techniques.

I created Python implementations of several cryptographic algorithms and protocols:

- SimplePIR {% cite cryptoeprint:2022/949 %}
- ElGamal encryption, including its homomorphic properties
- Private Information Retrieval (PIR) using Secret-key Regev encryption (LWE) and the Kushilevitz–Ostrovsky method, based on *Replication is not needed: single database, computationally-private information retrieval* {% cite Ostrovsky %}

Code available at: 

{% assign repo = site.data.repositories.github_repos[2] %}
{% if repo %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo.liquid repository=repo %}
</div>
{% else %}
  <a href="https://github.com/dbaitech/Cryptographic-Algorithms">Cryptographic Algorithms</a>.
{% endif %}