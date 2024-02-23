---
layout: default
permalink: /
---
# {{ site.title }}
### 新着情報
{% for post in site.posts limit:3 %}
[{{ post.title }}]({{ post.url }})
{% endfor %}
[&raquo; 続きを読み込む](/posts/)

[**Morpho** developed on **GitHub**](https://github.com/morpho-social)
