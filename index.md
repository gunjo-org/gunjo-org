---
layout: default
permalink: /
---

# {{ site.title }}
### 新着情報
{% for post in site.posts limit:3 %}
[{{ post.title }}]({{ post.url }})
{% endfor %}

<p class="right">
<a href="/articles/">&raquo; 続きを読み込む</a>
</p>

[**Morpho** developed on **GitHub**](https://github.com/morpho-social)