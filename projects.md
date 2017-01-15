---
layout: page
title: My side projects
permalink: /projects/
menu: true
project: false
---

<ul class="post-list project-list">
  {% for page in site.pages %}
    {% if page.project %}
      <li>
          <a class="page-link" href="{{ page.url | prepend: site.baseurl }}">
            <img class="shadow project-banner-image" src="/images/{{ page.header_image }}" alt="{{ page.title }}" title="{{ page.title }}" data-rjs="2" />
          </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
