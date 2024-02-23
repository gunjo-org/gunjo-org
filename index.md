---
layout: default
permalink: /
---
# {{ site.title }}
### 新着情報
{% for post in site.posts limit:3 %}
{{ post.date | date: site.date_format }} [{{ post.title }}]({{ post.url }})
{% endfor %}
[**Morpho** developed on **GitHub**](https://github.com/morpho-social)
