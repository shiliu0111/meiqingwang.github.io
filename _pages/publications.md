---
layout: page
permalink: /publications/
title: Publications
description: † Equal Contribution, * Corresponding Author(s).
nav: true
nav_order: 2
---

<!-- Bibsearch Feature -->
{% include bib_search.liquid %}

<!-- Journal Articles -->
## Journal Articles
<div class="publications">
  {% bibliography --query @article %}
</div>

<!-- Conference Proceedings -->
## Conference Proceedings
<div class="publications">
  {% bibliography --query @inproceedings %}
</div>
