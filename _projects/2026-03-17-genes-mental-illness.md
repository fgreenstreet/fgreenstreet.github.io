---
title: 'Can our genes predict where mental illness affects the brain?'
date: 2026-03-17 00:00:00
description:
project: genes-mental-illness
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
