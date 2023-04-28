---
title: "Publications"
permalink: /publications/
layout: archive
classes: wide
---


<ul class="taxonomy__index">
  {% assign postsInYear = site.publications | group_by_exp: 'publication', 'publication.date | date: "%Y"' %}
  {% for year in postsInYear %}
    <li>
      <a href="#{{ year.name }}">
        <strong>{{ year.name }}</strong> <span class="taxonomy__count">{{ year.items | size }}</span>
      </a>
    </li>
  {% endfor %}
</ul>

{% assign entries_layout = page.entries_layout | default: 'list' %}
{% assign postsByYear = site.publications | group_by_exp: 'publication', 'publication.date | date: "%Y"' %}
{% for year in postsByYear %}
  <section id="{{ year.name }}" class="taxonomy__section">
    <h2 class="archive__subtitle">{{ year.name }}</h2>
    <div class="entries-{{ entries_layout }}">
      {% for post in year.items %}
          <h3><a href="{{ post.link }}">{{ post.title }}</a> </h3>
          <p>
            {{ post.authors }}<br>
            <i>{{ post.publication }}</i>
          </p>
      {% endfor %}
    </div>
    <a href="#page-title" class="back-to-top">{{ site.data.ui-text[site.locale].back_to_top | default: 'Back to Top' }} &uarr;</a>
  </section>
{% endfor %}