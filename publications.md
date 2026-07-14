---
title: Publications
subtitle: Articles, working papers, and selected research outputs.
permalink: /publications/
math: true
---

Edit publication entries in `_data/publications.yml`. You can include links to PDFs,
code, slides, datasets, or journal pages.

{% for publication in site.data.publications %}
  {% include publication.html publication=publication %}
{% endfor %}
