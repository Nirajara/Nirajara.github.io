---
layout: page
permalink: /archery/
title: Archery
nav: false
display_categories: [archery1, archery2]
nav_order: 5
---

Hi there! I shoot Barebow for the <a href="https://dev.uclaclubarchery.com/">UCLA archery team</a>! I joined (having basically never shot before) in September 2021 and I've had a lot of fun practicing and competing! 

Here's some of the latest competitions I've shot in!

<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category"></h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  <div class="container">
    <div class="row row-cols-0">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  <div class="container">
    <div class="row row-cols-0">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
{%- endif -%}
</div>
