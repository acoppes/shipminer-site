---
layout:       page
title:        
permalink:    /drafts/
meta_robots:  noindex
---

<p>These are draft posts for previewing.</p>

<div class="posts">
  {% assign sorted = site.drafts | sort: 'date' | reverse %}
  {% for draft in sorted %}
  {%- if draft.hide == null or draft.hide == false -%}
    <div class="post py2">
      <p class="post-meta h5">{{ draft.date | date: site.date_format }}</p>
      <a href="{{site.baseurl}}{{ draft.url }}" class="post-link"><h3 class="post-title">{{ draft.title }}</h3></a>
      {% if draft.categories.size > 0 %}
        <span class="post-meta small">
          {% for category in draft.categories %}
            <a href="{{ category }}" class="category">{{ category }}</a>
          {% endfor %}
        </span>
      {% endif %}
      {%- if site.show_excerpts -%}
        {{ draft.excerpt }}
      {%- endif -%}
    </div>
  {%- endif -%}
  {% endfor %}
</div>