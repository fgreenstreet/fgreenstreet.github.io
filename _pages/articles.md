---
title: Articles
subtitle: A collection of science news articles written by Francesca Greenstreet.
description: A collection of science news articles written by Francesca Greenstreet.
permalink: /articles
---

{% for project in site.projects reversed %}
{% if project.article_url %}
<p style="margin-bottom: 1.5em;">
<a href="{{ project.article_url }}" target="_blank"><strong>{{ project.title }}</strong></a><br>
<span style="opacity: 0.6; font-size: 0.9em;">{{ project.date | date: "%B %Y" }}</span>
{% if project.client %}<span style="display: inline-block; background: #f0f0f0; padding: 2px 8px; border-radius: 3px; font-size: 0.8em; margin-left: 8px;">{{ project.client }}</span>{% endif %}
</p>
{% endif %}
{% endfor %}
