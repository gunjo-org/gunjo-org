---
layout: default
permalink: /
---
## {{ site.title }}
{{ site.description }}

### 新着情報
{% for post in site.posts limit:5 %}
[{{ post.title }}]({{ post.url }})
{% endfor %}

<small>
お問い合わせはこちら: {{ site.email }}
</small>
