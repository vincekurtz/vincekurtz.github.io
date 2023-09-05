---
layout: page
title: Software
permalink: /software/
description: Open-source software packages I've developed to support my research.
nav: true
nav_order: 3
display_categories: 
horizontal: false
---

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
