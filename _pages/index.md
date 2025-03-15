---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

Надо заполнить

**Предметы**

<ul>
    <li>
        04
        <ul>
            <li>
              <a class="internal-link" href="{% link _notes/04/PH.md %}">
                  Философия
              </a>
            </li>
            <li>
              <a class="internal-link" href="{% link _notes/04/OS.md %}"> 
                  Операционные системы
              </a>
              
              <!--<a class="internal-link" href="{{ site.baseurl }}{{ Электротехника }}">Электротехника</a>-->
            </li>
        </ul>
    </li>

    <li>
        03
        <ul>
            <li>
              <a class="internal-link" href="{% link _notes/03/ET.md %}">
                  Электротехника
              </a>
            </li>
            <li>
              <a class="internal-link" href="{% link _notes/03/ML.md %}"> 
                  Математическая логика и теория алгоритмов 
              </a>
              
              <!--<a class="internal-link" href="{{ site.baseurl }}{{ Электротехника }}">Электротехника</a>-->
            </li>
        </ul>
    </li>
</ul>

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

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
