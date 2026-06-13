---
title: 'A long-term and scalable system to record from neural organoids'
date: 2026-03-27 00:00:00
description:
project: pavlinek-organoids
featured_image: '1.webp'
article_url: 'https://www.kcl.ac.uk/news/a-long-term-and-scalable-system-to-record-from-neural-organoids'
client: "King's College London"
---

Visuals and article by Francesca Greenstreet for King's College London.

[Read the article →](https://www.kcl.ac.uk/news/a-long-term-and-scalable-system-to-record-from-neural-organoids)


<div class="gallery" data-columns="2">
	{% assign project_images = site.static_files | where_exp: "file", "file.path contains page.project" | sort_natural: "name" %}
	{% for image in project_images %}
	<img loading="lazy" src="{{ image.path }}">
	{% endfor %}
</div>
