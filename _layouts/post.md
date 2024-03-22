---
layout: default
---
<article>
<h2>{{ page.title | escape }}</h2>
<small>{{ page.date | date: "%Y年%-m月%-d日" }} 投稿</small>
{{ content }}
</article>

{% include pagination.md %}

<small>&copy;&nbsp;{{ 'now' | date: "%Y" }}&nbsp;{{ site.title }}</small>
