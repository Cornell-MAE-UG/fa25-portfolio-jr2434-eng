---
layout: default
title: Junayed Ridwan - Portfolio
permalink: /projects/
---

<div class="gallery-container">
<div class="project-gallery">
    {% assign visible_projects = site.projects | where_exp: "project", "project.gallery != false" %}
    {% for project in visible_projects %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
          <p>{{ project.title}}</p>
        </a>
      </div>
    {% endfor %}
</div>
</div>