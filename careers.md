---
layout: default
title: Careers
---

<h1>Careers</h1>

<ul>
  {% for career in site.careers %}
    <li>
      <h2>{{ career.name }}</h2>
      <h3>{{ career.position }}</h3>
      <p>{{ career.content | markdownify }}</p>
    </li>
  {% endfor %}
</ul>
