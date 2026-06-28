---
title: 'Parkinson''s hallucinations linked to altered brain region communications'
date: 2026-06-10 00:00:00
description:
project: parkinsons-hallucinations
featured_image: '1.webp'
client: "King's College London"
---

Visuals by Francesca Greenstreet for King's College London.


<div class="gallery" data-columns="2">
	{% assign project_images = site.static_files | where_exp: "file", "file.path contains page.project" | sort_natural: "name" %}
	{% for image in project_images %}
	<img loading="lazy" src="{{ image.path }}">
	{% endfor %}
</div>
