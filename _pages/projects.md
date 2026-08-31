---
layout: page
title: Software
permalink: /projects/
nav: true
nav_order: 1
horizontal: false
---

Since I started coding during my PhD I wrote multiple pieces of codes. Some more useful than others and some better written than others. It is only during my postdoc time that I started to think that since 95% of my time in research is passed coding I might as well learn how to write it correctly and how to release them in the wild. And so I did! I learnt how to use github, how to write documentation, tests, how to package something etc...Some have also been published in journals!

Here is the list of Software I have worked on. They are more or less in reversed chronological order. 

PS: I have two github account [astrom-tom](https://github.com/astrom-tom) which I do not use anymore (and I am completely locked out of it) and the one I use daily [Romain-Thomas-Shef](https://github.com/Romain-Thomas-Shef).

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
