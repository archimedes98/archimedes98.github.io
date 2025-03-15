---
layout: page
title: Home
id: home
permalink: /
---

<img width="40%" src="{{ site.baseurl }}/assets/cover.jpg"/>


{% for i in (3..4) reversed %}

  <h1>{{ i }} семестр</h1>
  <ul>
    {% for note in site.notes %}
      {% assign ipad = i | prepend: '000' | slice: -2, 2 | prepend: '/' | append: '/' %}
      {% if note.category == 'subject' and note.path contains ipad %}
      <li>
        <a class="internal-link" href="{{ note.url }}">
          {{ note.title }}
        </a>
      </li>
      {% endif %}
    {% endfor %}
  </ul>
{% endfor %}

{% comment %}

<!--
<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>
-->

{% endcomment %}
<style>
  .wrapper {
    max-width: 46em;
  }
</style>
