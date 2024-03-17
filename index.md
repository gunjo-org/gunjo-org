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
var currentTime = new Date();
var year = currentTime.getFullYear()
var cal = new CalHeatMap();
cal.init({
    itemSelector: "#cal-heatmap",
    domain: "month",
    data: "/assets/cal.json",
    start: new Date(year, 0),
    cellSize: 9,
    range: 13,
    previousSelector: "#cal-heatmap-PreviousDomain-selector",
    nextSelector: "#cal-heatmap-NextDomain-selector",
    legend: [2, 4, 6, 8],
});
</script>
