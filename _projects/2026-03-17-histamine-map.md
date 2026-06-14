---
title: 'Brain histamine map connects genes to brain function and mental health'
date: 2026-05-12 00:00:00
description:
project: histamine-map
featured_image: '01.webp'
article_url: 'https://www.kcl.ac.uk/news/brain-histamine-map-connects-genes-to-brain-function-and-mental-health'
client: "King's College London"
---

Visuals and article by Francesca Greenstreet for King's College London.

[Read the article →](https://www.kcl.ac.uk/news/brain-histamine-map-connects-genes-to-brain-function-and-mental-health)


<div class="gallery" data-columns="2">
	{% assign project_images = site.static_files | where_exp: "file", "file.path contains page.project" | sort_natural: "name" %}
	{% for image in project_images %}
	<img loading="lazy" src="{{ image.path }}">
	{% endfor %}
</div>
