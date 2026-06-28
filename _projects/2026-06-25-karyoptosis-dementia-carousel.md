---
title: 'New mechanism found for neuronal death in Alzheimer''s and frontotemporal dementia'
date: 2026-06-25 00:00:00
description:
project: karyoptosis-dementia-carousel
featured_image: '01.webp'
article_url: 'https://www.kcl.ac.uk/news/new-mechanism-found-for-neuronal-death-inalzheimers-and-frontotemporal-dementia'
client: "King's College London"
graphics:
  - '/images/comms-projects/karyoptosis-dementia-carousel/01.webp'
  - '/images/comms-projects/karyoptosis-dementia-carousel/02.webp'
  - '/images/comms-projects/karyoptosis-dementia-carousel/03.webp'
  - '/images/comms-projects/karyoptosis-dementia-carousel/04.webp'
  - '/images/comms-projects/karyoptosis-dementia-carousel/06.webp'
  - '/images/comms-projects/karyoptosis-dementia-carousel/07.webp'
  - '/images/comms-projects/karyoptosis-dementia-carousel/08.webp'
  - '/images/comms-projects/karyoptosis-dementia-carousel/09.webp'
  - '/images/comms-projects/karyoptosis-dementia-carousel/10.webp'
---

Visuals and article by Francesca Greenstreet for King's College London.

[Read the article →](https://www.kcl.ac.uk/news/new-mechanism-found-for-neuronal-death-inalzheimers-and-frontotemporal-dementia)


<div class="gallery" data-columns="2">
	{% assign project_images = site.static_files | where_exp: "file", "file.path contains page.project" | sort_natural: "name" %}
	{% for image in project_images %}
	<img loading="lazy" src="{{ image.path }}">
	{% endfor %}
</div>
