---
layout: page
permalink: /grants/
title: Grants
description:
nav: true
nav_order: 2
---

## Recent Grant Support

<ul>
  {% for grant in site.data.grants %}
    <li>{{ grant }}</li>
  {% endfor %}
</ul>
