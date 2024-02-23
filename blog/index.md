---
layout: default
title: 新着情報
permalink: /blog/
pagination: 
  enabled: true
---
<ul>
  {% for post in paginator.posts %}
  <li>
    <time>
      {% assign date_format = site.date_format %}
      {{ post.date | date: date_format }}
    </time>
    <h2>
      <a class="link" href="{{ post.url }}">{{ post.title | escape }}</a>
    </h2>
    <p>
      {{ post.content | strip_html | escape | truncate: 80 }}
    </p>
  </li>
  {% endfor %}
</ul>
{% if paginator.total_pages > 1 %}
<div>
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}">&laquo;</a>
  {% else %}
    <span>&laquo;</span>
  {% endif %}
  {% for page in (1..paginator.total_pages) %}
    {% if page == paginator.page %}
      <span>{{ page }}</span>
    {% elsif page == 1 %}
      <a href="/posts/">{{ page }}</a>
    {% else %}
      <a href="{{ site.paginate_path | replace: ':num', page }}">{{ page }}</a>
    {% endif %}
  {% endfor %}
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}">&raquo;</a>
  {% else %}
    <span>&raquo;</span>
  {% endif %}
</div>
{% endif %}
