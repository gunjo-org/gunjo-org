---
layout: default
permalink: /
---
# {{ site.title }}
### 新着情報
{% for post in site.posts limit:3 %}
{{ post.date | date: site.date_format }} [{{ post.title }}]({{ post.url }})
{% endfor %}

[<i class="fa-bluesky"></i>](https://bsky.app/profile/{{ site.did }})
[<i class="fa-github"></i>](https://github.com/morpho-social)
