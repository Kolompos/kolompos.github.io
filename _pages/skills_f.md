---
layout: page
permalink: /skills/field/
title: Skills by field
description: An ordered set of my skills categorized by field of profession.
nav: false
display_categories: [mechanics, electronics, embedded, desktop, misc]
horizontal: false
---

<!-- pages/skills_f.md -->
<div class="skills">
{%- if site.enable_skill_categories and page.display_categories %}
  <!-- Display categorized skills -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_skills = site.skills | where: "category", category -%}
  {%- assign sorted_skills = categorized_skills | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_skills -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_skills -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}
{%- endif -%}
</div>
