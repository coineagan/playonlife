---
title: posts
layout: root
permalink: /
---

{% for article in site.articles reversed %}
  <li>
    <time datetime="{{ article.date | date: '%B %-d, %Y' }}">
      {{ article.date | date: '%B %-d, %Y' }}
    </time>
    <a href="{{ article.url }}">{{ article.title }}</a>
  </li>
{% endfor %}

