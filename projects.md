---
layout: page
title: My side projects
permalink: /projects/
menu: true
project: false
---

<ul class="post-list">
  {% for page in site.pages %}
    {% if page.project %}
      <li>
          <a class="page-link" href="{{ page.url | prepend: site.baseurl }}">
            <img class="shadow" src="/images/{{ page.header_image }}" alt="{{ page.title }}" title="{{ page.title }}" />
          </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
