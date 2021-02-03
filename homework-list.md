---
layout: page
title:  Homework
permalink: /topics-list/
---

{% for hw in site.homework %}
  <p>
    <a target="_parent" href="..{{ hw.url }}">
      {{ hw.title }}
    </a>
  </p>
{% endfor %}

