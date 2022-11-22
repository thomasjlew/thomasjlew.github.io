---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---


<!-- The list below is updated infrequently; you can find all my publications on [Google Scholar](https://scholar.google.com/citations?user=qdnDZkYAAAAJ). -->

## Preprints
{% for post in site.preprints reversed %}
  {% include archive-single-paper.html %}
{% endfor %}

## Publications
{% for post in site.publications reversed %}
  {% include archive-single-paper.html %}
{% endfor %}

{% include base_path %}

<!-- {% for post in site.publications reversed %}
  {% include archive-single-paper.html %}
{% endfor %} -->
