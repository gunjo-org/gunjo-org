---
layout: default
permalink: /
---
## {{ site.title }}
{{ site.description }}
<fieldset>
<legend>
### 新着情報
</legend>
{% for post in site.posts limit:5 %}
[{{ post.title }}]({{ post.url }})
{% endfor %}
</fieldset>
<small>
お問い合わせはこちら: {{ site.email }}
</small>
