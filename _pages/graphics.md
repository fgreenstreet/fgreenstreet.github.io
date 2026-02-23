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
{% if project.graphics %}
<div class="portfolio-item">
<a class="portfolio-item__link" href="{{ project.url | relative_url }}">
<div class="portfolio-item__image">
<img src="{{ project.featured_image | relative_url }}" alt="{{ project.title }}">
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
