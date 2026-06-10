---
title: Videos
subtitle: Video interviews with scientists
description: Video interviews conducted by Francesca Greenstreet.
permalink: /videos
layout: default
---

<section class="portfolio">
<div class="content-wrap portfolio-wrap">
{% for project in site.projects reversed %}
{% if project.linkedin_embed_id %}
<div class="portfolio-item portfolio-item--video">
<div class="portfolio-item__embed">
<iframe src="https://www.linkedin.com/embed/feed/update/urn:li:{{ project.linkedin_embed_id }}?collapsed=1" height="800" width="100%" frameborder="0" allowfullscreen="" title="{{ project.title }}"></iframe>
</div>
</div>
{% elsif project.video_url and project.featured_image %}
<div class="portfolio-item">
<a class="portfolio-item__link" href="{{ project.video_url }}">
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
