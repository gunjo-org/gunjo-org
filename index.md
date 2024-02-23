---
layout: default
permalink: /
---
# {{ site.title }}
## - {{ site.tagline }} -
### 新着情報
{% for post in site.posts limit:3 %}
[{{ post.title }}]({{ post.url }})
{% endfor %}

お問合せはこちら: {{ site.email }}

<p class="right">
{{ "now" | date: "%Y年%-m月%-d日" }} 最終更新
</p>

[**Morpho** developed on **GitHub**](https://github.com/morpho-social)