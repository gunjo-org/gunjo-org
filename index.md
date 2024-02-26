---
layout: default
permalink: /
---
## {{ site.title }}
{{ site.description }}

### 新着情報
{% for post in site.posts limit:5 %}
{% unless site.posts %}
[{{ post.title }}]({{ post.url }})
{% endunless %}
{% endfor %}

<small>
お問い合わせはこちら: {{ site.email }}
</small>
