---
layout: default
---
<article>
<h1>{{ page.title | escape }}</h1>
<small>{{ page.date | date: "%Y年%-m月%-d日" }} 投稿</small>
{{ content }}
</article>

{% include pagination.md %}
