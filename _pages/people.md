---
title: "People"
permalink: /people/
layout: single
classes: wide
---

{% for person in site.people %}
  <h3><a href="{{ person.link }}">{{ person.name }}</a> </h3>
  <p>{{ person.position }} ({{ person.university }})</p>
{% endfor %}