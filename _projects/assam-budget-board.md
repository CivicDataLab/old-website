---
layout: page
title: Assam Budget Board
---

<h1>Assam Budget Board</h1>

{% for prj in site.projects %}
  <h2>{{ prj.name }} - {{ prj.position }}</h2>
  <p>{{ prj.content | markdownify }}</p>
{% endfor %}