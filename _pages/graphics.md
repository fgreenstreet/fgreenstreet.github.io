---
title: Graphics
subtitle: Visual science communication
description: Science graphics and illustrations created by Francesca Greenstreet.
permalink: /graphics
layout: default
---

<section class="portfolio">
<div class="content-wrap portfolio-wrap">
{% for project in site.projects reversed %}
{% if project.graphics or project.project %}
{% if project.project %}
{% assign project_featured_image = "/images/comms-projects/" | append: project.project | append: "/" | append: project.featured_image %}
{% else %}
{% assign project_featured_image = project.featured_image %}
{% endif %}
<div class="portfolio-item">
<a class="portfolio-item__link" href="{{ project.url | relative_url }}">
<div class="portfolio-item__image">
<img src="{{ project_featured_image | relative_url }}" alt="{{ project.title }}" loading="lazy">
</div>
<div class="portfolio-item__content">
<div class="portfolio-item__info">
<h2 class="portfolio-item__title">{{ project.title }}</h2>
<p class="portfolio-item__subtitle">{{ project.subtitle }}</p>
</div>
</div>
</a>
</div>
{% endif %}
{% endfor %}
</div>
</section>
