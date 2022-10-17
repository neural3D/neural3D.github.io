---
title: "People"
permalink: /people/
layout: single
classes: wide
---

## Main Principal Investigator

{% for person in site.people %}
  {% if person.project_position == "principal" %}
  <h3><a href="{{ person.link }}">{{ person.name }}</a> </h3>
  <p>{{ person.position }} ({{ person.university }})</p>
  {% endif %}
{% endfor %}

## Project Leads
{% for person in site.people %}
  {% if person.project_position == "lead" %}
  <h3><a href="{{ person.link }}">{{ person.name }}</a> </h3>
  <p>{{ person.position }} ({{ person.university }})</p>
  {% endif %}
{% endfor %}

## Project Staff
{% for person in site.people %}
  {% if person.project_position == "staff" %}
  <h3><a href="{{ person.link }}">{{ person.name }}</a> </h3>
  <p>{{ person.position }} ({{ person.university }})</p>
  {% endif %}
{% endfor %}

## Associated Researchers
Not funded by project funds, but active collaboration in ongoing research.

{% for person in site.people %}
  {% if person.project_position == "associate" %}
  <h3><a href="{{ person.link }}">{{ person.name }}</a> </h3>
  <p>{{ person.position }} ({{ person.university }})</p>
  {% endif %}
{% endfor %}