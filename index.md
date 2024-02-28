---
layout: default
permalink: /
---
## {{ site.title }}
{{ site.description }}
<fieldset>
<legend>
<h3>新着情報</h3>
</legend>
{% for post in site.posts limit:5 %}
<a href="{{ post.url }}">{{ post.title }}</a>
<br />
{% endfor %}
</fieldset>
<br />
<small>
お問い合わせはこちら: {{ site.email }}
</small>
