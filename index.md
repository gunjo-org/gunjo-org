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
<a href="{{ post.url }}">{{ post.title | truncate: 20 }}</a>
<br />
{% endfor %}
</fieldset>
<br />
<small>
お問い合わせはこちら: {{ site.email }}
</small>
<br />
<div id="cal-heatmap"></div>
<script>
const cal = new CalHeatmap();
cal.paint({});
render(<div id="cal-heatmap"></div>);
</script>
